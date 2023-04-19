# Comparing `tmp/aliendev_api-0.1.3.tar.gz` & `tmp/aliendev_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_api-0.1.3.tar", max compression
+gzip compressed data, was "aliendev_api-0.1.4.tar", max compression
```

## Comparing `aliendev_api-0.1.3.tar` & `aliendev_api-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 20:02:31.637233 aliendev_api-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-19 20:02:31.637233 aliendev_api-0.1.3/aliendev_api/__init__.py
--rw-r--r--   0        0        0      824 2023-04-19 20:02:31.637233 aliendev_api-0.1.3/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0      479 2023-04-19 20:02:31.637233 aliendev_api-0.1.3/aliendev_api/config/mongo.py
--rw-r--r--   0        0        0     2325 2023-04-19 20:02:31.637233 aliendev_api-0.1.3/aliendev_api/main.py
--rw-r--r--   0        0        0      378 2023-04-19 20:02:50.397352 aliendev_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0      479 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/config/mongo.py
+-rw-r--r--   0        0        0     2325 2023-04-19 20:02:48.193359 aliendev_api-0.1.4/aliendev_api/main.py
+-rw-r--r--   0        0        0      377 2023-04-19 20:03:07.184370 aliendev_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 aliendev_api-0.1.4/PKG-INFO
```

### Comparing `aliendev_api-0.1.3/aliendev_api/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_api-0.1.4/aliendev_api/config/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.3/aliendev_api/main.py` & `aliendev_api-0.1.4/aliendev_api/main.py`

 * *Files identical despite different names*

### Comparing `aliendev_api-0.1.3/PKG-INFO` & `aliendev_api-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliendev-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Nasri Adzlani
 Author-email: nasri@jkt1.ebdesk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

