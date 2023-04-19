# Comparing `tmp/peakina-0.9.4.tar.gz` & `tmp/peakina-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakina-0.9.4.tar", max compression
+gzip compressed data, was "peakina-0.9.5.tar", max compression
```

## Comparing `peakina-0.9.4.tar` & `peakina-0.9.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1510 2023-04-03 15:38:42.924878 peakina-0.9.4/LICENSE
--rw-r--r--   0        0        0     3490 2023-04-03 15:38:42.924878 peakina-0.9.4/README.md
--rw-r--r--   0        0        0      462 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/__init__.py
--rw-r--r--   0        0        0     6598 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/cache.py
--rw-r--r--   0        0        0     1041 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/datapool.py
--rw-r--r--   0        0        0     6778 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/datasource.py
--rw-r--r--   0        0        0     6949 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/helpers.py
--rw-r--r--   0        0        0      344 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/__init__.py
--rw-r--r--   0        0        0     4253 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/fetcher.py
--rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/ftp_fetcher.py
--rw-r--r--   0        0        0     8033 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/ftp_utils.py
--rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/http/__init__.py
--rw-r--r--   0        0        0     1369 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/http/http_fetcher.py
--rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/local/__init__.py
--rw-r--r--   0        0        0      378 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/local/file_fetcher.py
--rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/__init__.py
--rw-r--r--   0        0        0     1206 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/s3_fetcher.py
--rw-r--r--   0        0        0     4478 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/s3_utils.py
--rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/py.typed
--rw-r--r--   0        0        0      361 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/readers/__init__.py
--rw-r--r--   0        0        0     4107 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/csv.py
--rw-r--r--   0        0        0     1477 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/excel.py
--rw-r--r--   0        0        0      491 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/geodata.py
--rw-r--r--   0        0        0     1626 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/json.py
--rw-r--r--   0        0        0     1435 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/xml.py
--rw-r--r--   0        0        0     2598 2023-04-03 15:38:42.928877 peakina-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 peakina-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-19 09:52:27.643959 peakina-0.9.5/LICENSE
+-rw-r--r--   0        0        0     3490 2023-04-19 09:52:27.643959 peakina-0.9.5/README.md
+-rw-r--r--   0        0        0      462 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/__init__.py
+-rw-r--r--   0        0        0     6598 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/cache.py
+-rw-r--r--   0        0        0     1041 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/datapool.py
+-rw-r--r--   0        0        0     6778 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/datasource.py
+-rw-r--r--   0        0        0     6949 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/helpers.py
+-rw-r--r--   0        0        0      344 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/__init__.py
+-rw-r--r--   0        0        0     4253 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/ftp/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/ftp/ftp_fetcher.py
+-rw-r--r--   0        0        0     8033 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/ftp/ftp_utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/http/__init__.py
+-rw-r--r--   0        0        0     1369 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/http/http_fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/local/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/local/file_fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/s3/__init__.py
+-rw-r--r--   0        0        0     1206 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/s3/s3_fetcher.py
+-rw-r--r--   0        0        0     4649 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/io/s3/s3_utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/py.typed
+-rw-r--r--   0        0        0      361 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/__init__.py
+-rw-r--r--   0        0        0     4107 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/csv.py
+-rw-r--r--   0        0        0     1477 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/excel.py
+-rw-r--r--   0        0        0      491 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/geodata.py
+-rw-r--r--   0        0        0     1626 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/json.py
+-rw-r--r--   0        0        0     1435 2023-04-19 09:52:27.643959 peakina-0.9.5/peakina/readers/xml.py
+-rw-r--r--   0        0        0     2598 2023-04-19 09:52:27.647959 peakina-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 peakina-0.9.5/PKG-INFO
```

### Comparing `peakina-0.9.4/LICENSE` & `peakina-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/README.md` & `peakina-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/cache.py` & `peakina-0.9.5/peakina/cache.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/datapool.py` & `peakina-0.9.5/peakina/datapool.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/datasource.py` & `peakina-0.9.5/peakina/datasource.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/helpers.py` & `peakina-0.9.5/peakina/helpers.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/fetcher.py` & `peakina-0.9.5/peakina/io/fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/ftp/ftp_fetcher.py` & `peakina-0.9.5/peakina/io/ftp/ftp_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/ftp/ftp_utils.py` & `peakina-0.9.5/peakina/io/ftp/ftp_utils.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/http/http_fetcher.py` & `peakina-0.9.5/peakina/io/http/http_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/s3/s3_fetcher.py` & `peakina-0.9.5/peakina/io/s3/s3_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/io/s3/s3_utils.py` & `peakina-0.9.5/peakina/io/s3/s3_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,21 +49,25 @@
     if file:
         assert objectname, "s3 objectname can't be empty"
 
     return access_key, secret, urlchunks.hostname, objectname
 
 
 def _s3_open_file_with_retries(fs: s3fs.S3FileSystem, path: str, retries: int) -> Any:
-    for _ in range(retries):
+    nb_tries = 0
+    while nb_tries < retries:
         try:
-            logger.info(f"opening {path}")
+            logger.info(f"Opening {path}")
             file = fs.open(path)
             return file
         except Exception as ex:
-            logger.warning(f"could not open {path}: {ex}")
+            nb_tries += 1
+            if nb_tries >= retries:
+                raise Exception(f"Could not open {path} ({nb_tries} tries): {ex}") from ex
+            logger.warning(f"Could not open {path}: {ex}")
             # if the file has just been uploaded, then it might not be visible immediatly
             # but the fail to open has been cached by s3fs
             # so, we invalidate the cache
             fs.invalidate_cache(path)
             # and we give some time to S3 to settle the file status
             sleep(1)
```

### Comparing `peakina-0.9.4/peakina/readers/csv.py` & `peakina-0.9.5/peakina/readers/csv.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/readers/excel.py` & `peakina-0.9.5/peakina/readers/excel.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/readers/json.py` & `peakina-0.9.5/peakina/readers/json.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/peakina/readers/xml.py` & `peakina-0.9.5/peakina/readers/xml.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.4/pyproject.toml` & `peakina-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peakina"
-version = "0.9.4"
+version = "0.9.5"
 description = "pandas readers on steroids (remote files, glob patterns, cache, etc.)"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 readme = "README.md"
 homepage = "https://github.com/ToucanToco/peakina"
 documentation = "https://toucantoco.github.io/peakina"
 repository = "https://github.com/ToucanToco/peakina"
 license = "BSD-3-Clause"
```

### Comparing `peakina-0.9.4/PKG-INFO` & `peakina-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakina
-Version: 0.9.4
+Version: 0.9.5
 Summary: pandas readers on steroids (remote files, glob patterns, cache, etc.)
 Home-page: https://github.com/ToucanToco/peakina
 License: BSD-3-Clause
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

