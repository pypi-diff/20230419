# Comparing `tmp/cloudlab_client-0.1.79.tar.gz` & `tmp/cloudlab_client-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlab_client-0.1.79.tar", max compression
+gzip compressed data, was "cloudlab_client-0.1.83.tar", max compression
```

## Comparing `cloudlab_client-0.1.79.tar` & `cloudlab_client-0.1.83.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1022 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/README.md
--rw-r--r--   0        0        0        0 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/__init__.py
--rw-r--r--   0        0        0     8305 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/client.py
--rw-r--r--   0        0        0     1635 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/test_client.py
--rw-r--r--   0        0        0      451 2023-04-10 22:35:34.075517 cloudlab_client-0.1.79/pyproject.toml
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cloudlab_client-0.1.79/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-19 19:52:48.752319 cloudlab_client-0.1.83/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:52:48.752319 cloudlab_client-0.1.83/cloudlab_client/__init__.py
+-rw-r--r--   0        0        0     8351 2023-04-19 19:52:48.752319 cloudlab_client-0.1.83/cloudlab_client/client.py
+-rw-r--r--   0        0        0     1635 2023-04-19 19:52:48.752319 cloudlab_client-0.1.83/cloudlab_client/test_client.py
+-rw-r--r--   0        0        0      451 2023-04-19 19:53:10.812472 cloudlab_client-0.1.83/pyproject.toml
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cloudlab_client-0.1.83/PKG-INFO
```

### Comparing `cloudlab_client-0.1.79/README.md` & `cloudlab_client-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `cloudlab_client-0.1.79/cloudlab_client/client.py` & `cloudlab_client-0.1.83/cloudlab_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     def __init__(self, name: str, json_body: str) -> None:
         self.name = name
         self.uuid = json_body["uuid"]
         dateformat = "%Y-%m-%dT%H:%M:%SZ"
         self.created = datetime.strptime(json_body["created"], dateformat)
         if "started" in json_body and json_body["started"]:
             self.started = datetime.strptime(json_body["started"], dateformat)
+        else:
+            self.started = None
         self.expires = datetime.strptime(json_body["expires"], dateformat)
         self._raw = json_body
         assert_nonempty_args(self, ["name", "uuid"])
 
 @inject_generic_repr
 
 class CloudlabAPIException(Exception):
```

### Comparing `cloudlab_client-0.1.79/cloudlab_client/test_client.py` & `cloudlab_client-0.1.83/cloudlab_client/test_client.py`

 * *Files identical despite different names*

### Comparing `cloudlab_client-0.1.79/PKG-INFO` & `cloudlab_client-0.1.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlab-client
-Version: 0.1.79
+Version: 0.1.83
 Summary: Client for the cloudlab academic cloud environment.
 Author: Yannis Zarkadas
 Author-email: yanniszark@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

