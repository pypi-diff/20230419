# Comparing `tmp/privateai_client-1.0.3.tar.gz` & `tmp/privateai_client-1.0.4.tar.gz`

## Comparing `privateai_client-1.0.3.tar` & `privateai_client-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.3/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/README.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/objects.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/pai_client.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/components/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/components/pai_requests.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/components/pai_responses.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/components/pai_uris.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 privateai_client-1.0.3/src/paiclient/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0    32957 2020-02-02 00:00:00.000000 privateai_client-1.0.3/tests/test_request_objects.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 privateai_client-1.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.0.3/LICENSE
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 privateai_client-1.0.3/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 privateai_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 privateai_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.4/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    32957 2020-02-02 00:00:00.000000 privateai_client-1.0.4/tests/test_request_objects.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 privateai_client-1.0.4/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 privateai_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 privateai_client-1.0.4/PKG-INFO
```

### Comparing `privateai_client-1.0.3/.pytest_cache/v/cache/nodeids` & `privateai_client-1.0.4/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/objects.py` & `privateai_client-1.0.4/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/pai_client.py` & `privateai_client-1.0.4/src/privateai_client/pai_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/components/pai_requests.py` & `privateai_client-1.0.4/src/privateai_client/components/pai_requests.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/components/pai_responses.py` & `privateai_client-1.0.4/src/privateai_client/components/pai_responses.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/components/pai_uris.py` & `privateai_client-1.0.4/src/privateai_client/components/pai_uris.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/src/paiclient/components/request_objects.py` & `privateai_client-1.0.4/src/privateai_client/components/request_objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/tests/test_request_objects.py` & `privateai_client-1.0.4/tests/test_request_objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/LICENSE` & `privateai_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/README.md` & `privateai_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.3/pyproject.toml` & `privateai_client-1.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "privateai_client"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Adam Guiducci", email="adam.guiducci@private-ai.com" },
 ]
 description = "A thin client for communicating with the Private Ai de-identication api."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `privateai_client-1.0.3/PKG-INFO` & `privateai_client-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: privateai_client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A thin client for communicating with the Private Ai de-identication api.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

