# Comparing `tmp/cwsearch_utils-0.1.5-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5057 bytes, number of entries: 7
+Zip file size: 5056 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
--rw-rw-r--  2.0 unx     7258 b- defN 23-Apr-18 21:39 cwsearch_utils/aggregate.py
+-rw-rw-r--  2.0 unx     7268 b- defN 23-Apr-19 03:49 cwsearch_utils/aggregate.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Apr-18 00:21 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-18 21:40 cwsearch_utils-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 21:40 cwsearch_utils-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-18 21:40 cwsearch_utils-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-18 21:40 cwsearch_utils-0.1.5.dist-info/RECORD
-7 files, 13293 bytes uncompressed, 4021 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-19 03:49 cwsearch_utils-0.1.6.dist-info/RECORD
+7 files, 13303 bytes uncompressed, 4020 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.1.5.dist-info/METADATA
+Filename: cwsearch_utils-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.1.5.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.1.5.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.1.5.dist-info/RECORD
+Filename: cwsearch_utils-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/aggregate.py

```diff
@@ -112,15 +112,15 @@
             print(f"tag specified={tag}, but could not get resources. Ignoring tag..")
             get_files_list_one_group(s3client, bucket, prefix, None, None, rv)
     else:
         get_files_list_one_group(s3client, bucket, prefix, None, None, rv)
     rv.sort(reverse=True, key=my_filelisting_sort_fnx)
     return rv
 
-def process_file(client, bucket, key, ner_entities, infinstor_time_spec):
+def process_file(client, bucket, key, ner_entities, infinstor_time_spec, tag):
     try:
         dnm = os.path.join('/tmp', key[key.rindex('/') + 1:])
         print(f"Downloading object {key} to local file {dnm}")
         client.download_file(bucket, key, dnm)
         dct = infinstor_lock.load_from_db(dnm, tag)
         union(ner_entities, dct, infinstor_time_spec)
         os.remove(dnm)
@@ -146,15 +146,15 @@
         print(f"{fl[2]} : sz={fl[1]} : {fl[0]}", flush=True)
 
     # next, read each file and fill ner_entities
     ner_entities = {}
     total_sz = 0
     for one_entry in files:
         print(f"Processing file {one_entry[0]} last_modified {one_entry[2]}")
-        if process_file(s3client, bucket, one_entry[0], ner_entities, infinstor_time_spec):
+        if process_file(s3client, bucket, one_entry[0], ner_entities, infinstor_time_spec, tag):
             total_sz = total_sz + one_entry[1]
         if total_sz > (512 * 1024 * 1024):
             print(f"Stopping after processing files of size {total_sz}")
             break
         else:
             print(f"Continuing after processing {total_sz} bytes")
         tnow = datetime.datetime.utcnow()
```

## Comparing `cwsearch_utils-0.1.5.dist-info/METADATA` & `cwsearch_utils-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.1.5.dist-info/RECORD` & `cwsearch_utils-0.1.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cwsearch_utils/aggregate.py,sha256=VbI09-A7ISYXzgw9ykyucblhuR6Xv40yYa3Csb2_b54,7258
+cwsearch_utils/aggregate.py,sha256=Cd1PwG359nGUS7S94EtAqGTM64apKjwQbdRIW5hIBLY,7268
 cwsearch_utils/infinstor_lock.py,sha256=kxY_afhPD8K50s1C-bxzs0DX3I28HLsayM-fn8H0Sw8,4780
-cwsearch_utils-0.1.5.dist-info/METADATA,sha256=FFsAceDs69MQ9eceXzXb9dBd8--cl3lLQZqS4-HWixk,570
-cwsearch_utils-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.1.5.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.1.5.dist-info/RECORD,,
+cwsearch_utils-0.1.6.dist-info/METADATA,sha256=x71HYeRQMnUx9AL7e1-Ham0iB4w12ti0yE9BTcxBOX4,570
+cwsearch_utils-0.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.1.6.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.1.6.dist-info/RECORD,,
```

