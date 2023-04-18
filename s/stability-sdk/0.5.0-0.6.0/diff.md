# Comparing `tmp/stability-sdk-0.5.0.tar.gz` & `tmp/stability-sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.5.0.tar", last modified: Fri Apr 14 04:22:17 2023, max compression
+gzip compressed data, was "stability-sdk-0.6.0.tar", last modified: Tue Apr 18 22:23:33 2023, max compression
```

## Comparing `stability-sdk-0.5.0.tar` & `stability-sdk-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.206665 stability-sdk-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.206665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.731961 stability-sdk-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-18 22:23:10.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.731961 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 22:23:12.000000 stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.735961 stability-sdk-0.6.0/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-18 22:23:33.000000 stability-sdk-0.6.0/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-18 22:23:33.000000 stability-sdk-0.6.0/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:23:33.000000 stability-sdk-0.6.0/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 22:23:33.000000 stability-sdk-0.6.0/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 22:23:33.000000 stability-sdk-0.6.0/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:23:33.739961 stability-sdk-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-18 22:23:08.000000 stability-sdk-0.6.0/tests/test_utils.py
```

### Comparing `stability-sdk-0.5.0/LICENSE` & `stability-sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/PKG-INFO` & `stability-sdk-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.5.0/README.md` & `stability-sdk-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/setup.py` & `stability-sdk-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from setuptools import setup, find_namespace_packages
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.5.0',
+    version='0.6.0',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
 
     description='Python SDK for interacting with stability.ai APIs',
     long_description=README,
     long_description_content_type="text/markdown",
 
     install_requires=[
         'Pillow',
-        'grpcio==1.48.1',
-        'grpcio-tools==1.48.1',
+        'grpcio==1.53.0',
+        'grpcio-tools==1.53.0',
         'python-dotenv',
-        'protobuf==3.19.5'
+        'protobuf==4.21.12'
     ],
     extras_require={
         'dev': [
             'pytest',
             'grpcio-testing'
     ]},
     packages=find_namespace_packages(
```

### Comparing `stability-sdk-0.5.0/src/stability_sdk/__main__.py` & `stability-sdk-0.6.0/src/stability_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/client.py` & `stability-sdk-0.6.0/src/stability_sdk/client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.6.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk/utils.py` & `stability-sdk-0.6.0/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.6.0/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.5.0/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.6.0/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/tests/test_client.py` & `stability-sdk-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.5.0/tests/test_utils.py` & `stability-sdk-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

