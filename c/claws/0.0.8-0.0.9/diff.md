# Comparing `tmp/claws-0.0.8.tar.gz` & `tmp/claws-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claws-0.0.8.tar", last modified: Tue Apr 18 11:37:23 2023, max compression
+gzip compressed data, was "claws-0.0.9.tar", last modified: Wed Apr 19 06:38:22 2023, max compression
```

## Comparing `claws-0.0.8.tar` & `claws-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 claws-0.0.8/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-18 11:37:23.665636 claws-0.0.8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2550 2023-03-31 10:24:28.000000 claws-0.0.8/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1055 2023-04-18 11:37:04.000000 claws-0.0.8/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1026 2023-04-18 11:37:23.665636 claws-0.0.8/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/claws/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-30 09:13:54.000000 claws-0.0.8/src/claws/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10173 2023-04-18 11:35:52.000000 claws-0.0.8/src/claws/aws_utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/src/claws.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      278 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      170 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        6 2023-04-18 11:37:23.000000 claws-0.0.8/src/claws.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-18 11:37:23.665636 claws-0.0.8/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8596 2023-03-30 10:45:09.000000 claws-0.0.8/tests/test_aws_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-19 06:38:22.251607 claws-0.0.9/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 claws-0.0.9/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-19 06:38:22.251607 claws-0.0.9/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2550 2023-03-31 10:24:28.000000 claws-0.0.9/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1080 2023-04-19 06:38:09.000000 claws-0.0.9/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1045 2023-04-19 06:38:22.251607 claws-0.0.9/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-19 06:38:22.251607 claws-0.0.9/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-19 06:38:22.251607 claws-0.0.9/src/claws/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-30 09:13:54.000000 claws-0.0.9/src/claws/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10977 2023-04-19 06:35:00.000000 claws-0.0.9/src/claws/aws_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-19 06:38:22.251607 claws-0.0.9/src/claws.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4386 2023-04-19 06:38:22.000000 claws-0.0.9/src/claws.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      278 2023-04-19 06:38:22.000000 claws-0.0.9/src/claws.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-19 06:38:22.000000 claws-0.0.9/src/claws.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      188 2023-04-19 06:38:22.000000 claws-0.0.9/src/claws.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        6 2023-04-19 06:38:22.000000 claws-0.0.9/src/claws.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-19 06:38:22.251607 claws-0.0.9/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8596 2023-03-30 10:45:09.000000 claws-0.0.9/tests/test_aws_utils.py
```

### Comparing `claws-0.0.8/LICENSE.md` & `claws-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `claws-0.0.8/PKG-INFO` & `claws-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claws
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Crossref Labs AWS tooling system.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `claws-0.0.8/README.md` & `claws-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `claws-0.0.8/pyproject.toml` & `claws-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "claws"
-version = "0.0.8"
+version = "0.0.9"
 description = "The Crossref Labs AWS tooling system."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
@@ -24,15 +24,16 @@
     "aiohttp==3.8.4",
     "yarl==1.8.2",
     "moto==4.1.6",
     "pytest==6.2.5",
     "pytest-asyncio==0.20.3",
     "pytest-localstack==0.6.0",
     "pytest-mock==3.10.0",
-    "coverage==7.2.2,"
+    "coverage==7.2.2,",
+    "smart-open==6.3.0"
 ]
 
 [project.urls]
 homepage = "https://labs.crossref.org"
 documentation = "https://labs.crossref.org"
 repository = "https://gitlab.com/crossref/labs/claws"
 changelog = "https://gitlab.com/crossref/labs/claws/-/blob/main/CHANGELOG.md"
```

### Comparing `claws-0.0.8/setup.cfg` & `claws-0.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = claws
-version = 0.0.8
+version = 0.0.9
 description = The Crossref Labs AWS tooling system.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
@@ -31,14 +31,15 @@
 	yarl==1.8.2
 	moto==4.1.6
 	pytest==6.2.5
 	pytest-asyncio==0.20.3
 	pytest-localstack==0.6.0
 	pytest-mock==3.10.0
 	coverage==7.2.2
+	smart-open==6.3.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `claws-0.0.8/src/claws/aws_utils.py` & `claws-0.0.9/src/claws/aws_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import asyncio
 from functools import wraps
 from typing import Any, Callable
 
 from aiohttp import client
 from yarl import URL
 
+import json
+import logging
+from smart_open import open
+
 
 def deferred_init(func) -> Callable:
     """
     A decorator to indicate that a property should trigger deferred init.
     :param func: the function to wrap.
     :return: a Callable
     """
@@ -365,14 +369,42 @@
         """
         Get a json key from the s3 key
         :param key: the key
         :return: a string
         """
         return key.split("/")[-1].split(".")[0]
 
+    def push_json_to_s3(
+        self,
+        json_obj,
+        bucket,
+        path,
+        verbose=False,
+    ) -> None:
+        """
+        Writes the JSON data to S3
+        :param bucket: the name of the bucket
+        :param path: the path of the object to store
+        :param json_obj: the JSON to write
+        :param verbose: whether to print status messages
+        :return:
+        """
+
+        if verbose:
+            logging.info(f"Writing JSON to S3 bucket {bucket} at path {path}")
+
+        url = f"s3://{bucket}/{path}"
+        with open(
+            url,
+            "w",
+            transport_params={"client": self.s3_client},
+        ) as output:
+            json.dump(json_obj, output, indent=4)
+            output.flush()
+
 
 class S3ObjException(Exception):
     """
     Exception for S3 object errors
     """
 
     pass
```

### Comparing `claws-0.0.8/src/claws.egg-info/PKG-INFO` & `claws-0.0.9/src/claws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claws
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Crossref Labs AWS tooling system.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `claws-0.0.8/tests/test_aws_utils.py` & `claws-0.0.9/tests/test_aws_utils.py`

 * *Files identical despite different names*

