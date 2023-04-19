# Comparing `tmp/cwsearch_utils-0.1.6-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5056 bytes, number of entries: 7
+Zip file size: 5635 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7268 b- defN 23-Apr-19 03:49 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7900 b- defN 23-Apr-19 17:53 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx      210 b- defN 23-Apr-19 17:07 cwsearch_utils/infinstor_dbutils.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/RECORD
-7 files, 13303 bytes uncompressed, 4020 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-19 17:54 cwsearch_utils-0.1.7.dist-info/RECORD
+8 files, 14236 bytes uncompressed, 4453 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: cwsearch_utils/__init__.py
 Comment: 
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
+Filename: cwsearch_utils/infinstor_dbutils.py
+Comment: 
+
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.6.dist-info/METADATA
+Filename: cwsearch_utils-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.6.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.6.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.6.dist-info/RECORD
+Filename: cwsearch_utils-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -1,31 +1,28 @@
 import os
 import json
 import tempfile
 import datetime
 from arnparse import arnparse
-from . import infinstor_lock
+from cwsearch_utils import infinstor_lock, infinstor_dbutils
+import sqlite3
 
 def my_sort_fnx(a):
     return a[0]
 
 def union(ner_entities, dct, infinstor_time_spec):
     for nm in dct:
         if nm in ner_entities:
             full = ner_entities[nm] + dct[nm]
         else:
             full = dct[nm]
         full.sort(reverse=True, key=my_sort_fnx)
         ner_entities[nm] = full[:100]
 
-def update_cache(infinstor_time_spec, ner_entities, s3client, bucket, prefix):
-    tdir = tempfile.mkdtemp()
-    tfile = os.path.join(tdir, "names.json")
-    with open(tfile, 'w') as ofile:
-        json.dump(ner_entities, ofile, indent=4)
+def update_cache(infinstor_time_spec, tfile, s3client, bucket, prefix):
     object_name = f"{prefix}/index/{infinstor_time_spec}/names.json"
     try:
         response = s3client.upload_file(tfile, bucket, object_name)
     except Exception as ex:
         print(f"Caught {ex} while uploading names entry for timespec {infinstor_time_spec}. Objectname={object_name}")
 
 def my_filelisting_sort_fnx(a):
@@ -112,21 +109,36 @@
             print(f"tag specified={tag}, but could not get resources. Ignoring tag..")
             get_files_list_one_group(s3client, bucket, prefix, None, None, rv)
     else:
         get_files_list_one_group(s3client, bucket, prefix, None, None, rv)
     rv.sort(reverse=True, key=my_filelisting_sort_fnx)
     return rv
 
-def process_file(client, bucket, key, ner_entities, infinstor_time_spec, tag):
+def process_file(client, bucket, key, dstcon, infinstor_time_spec, tag):
     try:
+        dstcur = dstcon.cursor()
+
         dnm = os.path.join('/tmp', key[key.rindex('/') + 1:])
         print(f"Downloading object {key} to local file {dnm}")
         client.download_file(bucket, key, dnm)
-        dct = infinstor_lock.load_from_db(dnm, tag)
-        union(ner_entities, dct, infinstor_time_spec)
+
+        srccon = sqlite3.connect(dnm)
+        srccur = srccon.cursor()
+        if not tag:
+            tag = 'notag'
+        res = srccur.execute(f"SELECT name, timestamp, link, msg FROM links WHERE tag='{tag}'")
+        while True:
+            one_entry = res.fetchone()
+            if not one_entry:
+                break
+            name = one_entry[0]
+            estr = f"INSERT INTO links VALUES ('{one_entry[0]}', '{one_entry[1]}', '{one_entry[2]}', '{one_entry[3]}')"
+            print(f"process_file: executing {estr}")
+            dstcur.execute(f"INSERT INTO links VALUES ('{one_entry[0]}', '{one_entry[1]}', '{one_entry[2]}', '{one_entry[3]}')")
+        dstcon.commit()
         os.remove(dnm)
         return True
     except Exception as e:
         print(f"Caught {e} while downloading {key} from bucket {bucket}. Ignoring and trying next object..")
     return False
 
 def populate_names(bucket, prefix, infinstor_time_spec, log_groups, tag):
@@ -142,29 +154,35 @@
         print(f'Caught {ex} while list_objects_v2 of {bucket} prefix {prefix} time {infinstor_time_spec}', flush=True)
 
     print(f"Reverse Chronological Order Files:")
     for fl in files:
         print(f"{fl[2]} : sz={fl[1]} : {fl[0]}", flush=True)
 
     # next, read each file and fill ner_entities
+    tdir = tempfile.mkdtemp()
+    tfile = os.path.join(tdir, "names.db")
+    con = sqlite3.connect(tfile)
+    infinstor_dbutils.create_table(con)
+
     ner_entities = {}
     total_sz = 0
     for one_entry in files:
         print(f"Processing file {one_entry[0]} last_modified {one_entry[2]}")
-        if process_file(s3client, bucket, one_entry[0], ner_entities, infinstor_time_spec, tag):
+        if process_file(s3client, bucket, one_entry[0], con, infinstor_time_spec, tag):
             total_sz = total_sz + one_entry[1]
         if total_sz > (512 * 1024 * 1024):
             print(f"Stopping after processing files of size {total_sz}")
             break
         else:
             print(f"Continuing after processing {total_sz} bytes")
         tnow = datetime.datetime.utcnow()
         delta = tnow - start_time
         if delta.total_seconds() > 600:
             print(f"Stopping after working for {delta.total_seconds()} seconds")
             break
         else:
             print(f"Continuing after working for {delta.total_seconds()} seconds")
+    con.close()
 
     # finally, write ner_entites to s3
-    update_cache(infinstor_time_spec, ner_entities, s3client, bucket, prefix)
+    update_cache(infinstor_time_spec, tfile, s3client, bucket, prefix)
     return ner_entities
```

## Comparing `cwsearch_utils-0.1.6.dist-info/METADATA` & `cwsearch_utils-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.1.6.dist-info/RECORD` & `cwsearch_utils-0.1.7.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cwsearch_utils/aggregate.py,sha256=Cd1PwG359nGUS7S94EtAqGTM64apKjwQbdRIW5hIBLY,7268
+cwsearch_utils/aggregate.py,sha256=hAjdDpSUhL1ClARsaf3uYTgU0VJKfkKybPsb0QyvYes,7900
+cwsearch_utils/infinstor_dbutils.py,sha256=kC2AgOEON5kIz64TSgGpkdzWuzJUW84rlwosrMRN9cg,210
 cwsearch_utils/infinstor_lock.py,sha256=kxY_afhPD8K50s1C-bxzs0DX3I28HLsayM-fn8H0Sw8,4780
-cwsearch_utils-0.1.6.dist-info/METADATA,sha256=x71HYeRQMnUx9AL7e1-Ham0iB4w12ti0yE9BTcxBOX4,570
-cwsearch_utils-0.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.1.6.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.1.6.dist-info/RECORD,,
+cwsearch_utils-0.1.7.dist-info/METADATA,sha256=a_N9VsRlBujdoXomwWOTKtE8_IhE65qiBRB1yIY3rGA,570
+cwsearch_utils-0.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.1.7.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.1.7.dist-info/RECORD,,
```

