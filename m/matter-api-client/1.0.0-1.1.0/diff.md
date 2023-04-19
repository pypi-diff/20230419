# Comparing `tmp/matter_api_client-1.0.0-py3-none-any.whl.zip` & `tmp/matter_api_client-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6701 bytes, number of entries: 12
+Zip file size: 6704 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_api_client/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_api_client/__init__.py
 -rw-r--r--  2.0 unx       92 b- defN 20-Feb-02 00:00 matter_api_client/config.py
 -rw-r--r--  2.0 unx      893 b- defN 20-Feb-02 00:00 matter_api_client/decorators.py
 -rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 matter_api_client/exceptions.py
 -rw-r--r--  2.0 unx     2113 b- defN 20-Feb-02 00:00 matter_api_client/http_client.py
 -rw-r--r--  2.0 unx     2491 b- defN 20-Feb-02 00:00 matter_api_client/http_client_async.py
 -rw-r--r--  2.0 unx      222 b- defN 20-Feb-02 00:00 matter_api_client/response.py
-?rw-r--r--  2.0 unx     4943 b- defN 20-Feb-02 00:00 matter_api_client-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_api_client-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_api_client-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1039 b- defN 20-Feb-02 00:00 matter_api_client-1.0.0.dist-info/RECORD
-12 files, 13316 bytes uncompressed, 4931 bytes compressed:  63.0%
+?rw-r--r--  2.0 unx     4944 b- defN 20-Feb-02 00:00 matter_api_client-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_api_client-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_api_client-1.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1039 b- defN 20-Feb-02 00:00 matter_api_client-1.1.0.dist-info/RECORD
+12 files, 13317 bytes uncompressed, 4934 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: matter_api_client/http_client_async.py
 Comment: 
 
 Filename: matter_api_client/response.py
 Comment: 
 
-Filename: matter_api_client-1.0.0.dist-info/METADATA
+Filename: matter_api_client-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_api_client-1.0.0.dist-info/WHEEL
+Filename: matter_api_client-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_api_client-1.0.0.dist-info/licenses/LICENSE
+Filename: matter_api_client-1.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_api_client-1.0.0.dist-info/RECORD
+Filename: matter_api_client-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_api_client/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

## Comparing `matter_api_client-1.0.0.dist-info/METADATA` & `matter_api_client-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-api-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Matter's API Client Library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-api-client#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-api-client/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-api-client
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: aiohttp==3.8.4
-Requires-Dist: matter-exceptions==1.0.1
-Requires-Dist: orjson==3.8.8
+Requires-Dist: matter-exceptions>=1.1.0
+Requires-Dist: orjson==3.8.10
 Requires-Dist: requests==2.28.2
 Description-Content-Type: text/markdown
 
 # matter-api-client
 
 **Table of Contents**
```

## Comparing `matter_api_client-1.0.0.dist-info/licenses/LICENSE` & `matter_api_client-1.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

