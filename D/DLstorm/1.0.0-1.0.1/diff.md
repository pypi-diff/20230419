# Comparing `tmp/DLstorm-1.0.0.tar.gz` & `tmp/DLstorm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLstorm-1.0.0.tar", last modified: Wed Apr 19 08:56:51 2023, max compression
+gzip compressed data, was "DLstorm-1.0.1.tar", last modified: Wed Apr 19 09:47:55 2023, max compression
```

## Comparing `DLstorm-1.0.0.tar` & `DLstorm-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:51.834902 DLstorm-1.0.0/
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:51.822903 DLstorm-1.0.0/DLstorm/
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:51.834902 DLstorm-1.0.0/DLstorm/Layers/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      166 2023-04-14 14:20:02.000000 DLstorm-1.0.0/DLstorm/Layers/Base.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     5016 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Layers/BatchNormalization.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     7921 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Layers/Conv.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      652 2023-04-18 09:44:21.000000 DLstorm-1.0.0/DLstorm/Layers/Dropout.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      542 2023-04-14 14:20:02.000000 DLstorm-1.0.0/DLstorm/Layers/Flatten.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1712 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Layers/FullyConnected.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)    13329 2023-04-18 09:44:21.000000 DLstorm-1.0.0/DLstorm/Layers/Helpers.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      889 2023-04-18 09:44:21.000000 DLstorm-1.0.0/DLstorm/Layers/Initializers.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     3588 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Layers/Pooling.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      272 2023-03-21 14:10:09.000000 DLstorm-1.0.0/DLstorm/Layers/ReLU.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      905 2023-03-21 14:47:17.000000 DLstorm-1.0.0/DLstorm/Layers/SoftMax.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      146 2023-04-18 09:44:21.000000 DLstorm-1.0.0/DLstorm/Layers/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     5596 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Model.py
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:51.834902 DLstorm-1.0.0/DLstorm/Optimization/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      397 2023-03-21 15:18:15.000000 DLstorm-1.0.0/DLstorm/Optimization/Loss.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1751 2023-04-19 08:44:04.000000 DLstorm-1.0.0/DLstorm/Optimization/Optimizers.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)       33 2022-10-24 07:00:57.000000 DLstorm-1.0.0/DLstorm/Optimization/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2023-04-19 08:53:41.000000 DLstorm-1.0.0/DLstorm/VERSION
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:49:31.000000 DLstorm-1.0.0/DLstorm/__init__.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1011 2023-04-19 08:13:39.000000 DLstorm-1.0.0/DLstorm/logger.py
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:51.826902 DLstorm-1.0.0/DLstorm.egg-info/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      716 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      749 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/SOURCES.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/dependency_links.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/not-zip-safe
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       68 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/requires.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        8 2023-04-19 08:56:51.000000 DLstorm-1.0.0/DLstorm.egg-info/top_level.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1079 2022-07-17 11:21:32.000000 DLstorm-1.0.0/LICENSE
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      267 2023-04-19 08:54:32.000000 DLstorm-1.0.0/MANIFEST.in
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      716 2023-04-19 08:56:51.834902 DLstorm-1.0.0/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:26.000000 DLstorm-1.0.0/README.md
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      104 2022-07-17 11:21:32.000000 DLstorm-1.0.0/pyproject.toml
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       67 2023-04-14 14:20:02.000000 DLstorm-1.0.0/requirements.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2023-04-19 08:56:51.834902 DLstorm-1.0.0/setup.cfg
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1807 2023-04-19 08:56:15.000000 DLstorm-1.0.0/setup.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 09:47:55.909205 DLstorm-1.0.1/
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 09:47:55.897205 DLstorm-1.0.1/DLstorm/
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 09:47:55.905205 DLstorm-1.0.1/DLstorm/Layers/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      166 2023-04-14 14:20:02.000000 DLstorm-1.0.1/DLstorm/Layers/Base.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     5016 2023-04-19 08:44:04.000000 DLstorm-1.0.1/DLstorm/Layers/BatchNormalization.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     7921 2023-04-19 08:44:04.000000 DLstorm-1.0.1/DLstorm/Layers/Conv.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      652 2023-04-18 09:44:21.000000 DLstorm-1.0.1/DLstorm/Layers/Dropout.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      542 2023-04-14 14:20:02.000000 DLstorm-1.0.1/DLstorm/Layers/Flatten.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1712 2023-04-19 08:44:04.000000 DLstorm-1.0.1/DLstorm/Layers/FullyConnected.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)    13329 2023-04-18 09:44:21.000000 DLstorm-1.0.1/DLstorm/Layers/Helpers.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      889 2023-04-18 09:44:21.000000 DLstorm-1.0.1/DLstorm/Layers/Initializers.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     3588 2023-04-19 08:44:04.000000 DLstorm-1.0.1/DLstorm/Layers/Pooling.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      272 2023-03-21 14:10:09.000000 DLstorm-1.0.1/DLstorm/Layers/ReLU.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      905 2023-03-21 14:47:17.000000 DLstorm-1.0.1/DLstorm/Layers/SoftMax.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      146 2023-04-18 09:44:21.000000 DLstorm-1.0.1/DLstorm/Layers/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     5602 2023-04-19 09:47:27.000000 DLstorm-1.0.1/DLstorm/Model.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 09:47:55.909205 DLstorm-1.0.1/DLstorm/Optimization/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      397 2023-03-21 15:18:15.000000 DLstorm-1.0.1/DLstorm/Optimization/Loss.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1751 2023-04-19 08:44:04.000000 DLstorm-1.0.1/DLstorm/Optimization/Optimizers.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)       33 2022-10-24 07:00:57.000000 DLstorm-1.0.1/DLstorm/Optimization/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2023-04-19 09:47:47.000000 DLstorm-1.0.1/DLstorm/VERSION
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:49:31.000000 DLstorm-1.0.1/DLstorm/__init__.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1011 2023-04-19 08:13:39.000000 DLstorm-1.0.1/DLstorm/logger.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-19 09:47:55.901205 DLstorm-1.0.1/DLstorm.egg-info/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      716 2023-04-19 09:47:55.000000 DLstorm-1.0.1/DLstorm.egg-info/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      749 2023-04-19 09:47:55.000000 DLstorm-1.0.1/DLstorm.egg-info/SOURCES.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-04-19 09:47:55.000000 DLstorm-1.0.1/DLstorm.egg-info/dependency_links.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-04-19 08:56:51.000000 DLstorm-1.0.1/DLstorm.egg-info/not-zip-safe
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       68 2023-04-19 09:47:55.000000 DLstorm-1.0.1/DLstorm.egg-info/requires.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        8 2023-04-19 09:47:55.000000 DLstorm-1.0.1/DLstorm.egg-info/top_level.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1079 2022-07-17 11:21:32.000000 DLstorm-1.0.1/LICENSE
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      267 2023-04-19 08:54:32.000000 DLstorm-1.0.1/MANIFEST.in
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      716 2023-04-19 09:47:55.909205 DLstorm-1.0.1/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2023-04-19 08:56:26.000000 DLstorm-1.0.1/README.md
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      104 2022-07-17 11:21:32.000000 DLstorm-1.0.1/pyproject.toml
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       67 2023-04-14 14:20:02.000000 DLstorm-1.0.1/requirements.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2023-04-19 09:47:55.909205 DLstorm-1.0.1/setup.cfg
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1807 2023-04-19 08:56:15.000000 DLstorm-1.0.1/setup.py
```

### Comparing `DLstorm-1.0.0/DLstorm/Layers/BatchNormalization.py` & `DLstorm-1.0.1/DLstorm/Layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Conv.py` & `DLstorm-1.0.1/DLstorm/Layers/Conv.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Dropout.py` & `DLstorm-1.0.1/DLstorm/Layers/Dropout.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Flatten.py` & `DLstorm-1.0.1/DLstorm/Layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/FullyConnected.py` & `DLstorm-1.0.1/DLstorm/Layers/FullyConnected.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Helpers.py` & `DLstorm-1.0.1/DLstorm/Layers/Helpers.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Initializers.py` & `DLstorm-1.0.1/DLstorm/Layers/Initializers.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/Pooling.py` & `DLstorm-1.0.1/DLstorm/Layers/Pooling.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Layers/SoftMax.py` & `DLstorm-1.0.1/DLstorm/Layers/SoftMax.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/Model.py` & `DLstorm-1.0.1/DLstorm/Model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import copy
-from Layers.Base import BaseLayer
+from DLstorm.Layers.Base import BaseLayer
 from DLstorm.logger import get_file_logger
 
 import numpy as np
 
 _logger = get_file_logger(__name__, 'debug')
 
-
-
 class Model(object):
     def __init__(self, model=None) -> None:
         self.model = []
         self.train_output = {}
         self.eval_output = {}
 
         if isinstance(model, list):
```

### Comparing `DLstorm-1.0.0/DLstorm/Optimization/Optimizers.py` & `DLstorm-1.0.1/DLstorm/Optimization/Optimizers.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm/logger.py` & `DLstorm-1.0.1/DLstorm/logger.py`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/DLstorm.egg-info/PKG-INFO` & `DLstorm-1.0.1/DLstorm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLstorm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deep Learning framework from scratch
 Home-page: https://github.com/HassanRady/DLstorm
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `DLstorm-1.0.0/DLstorm.egg-info/SOURCES.txt` & `DLstorm-1.0.1/DLstorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/LICENSE` & `DLstorm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DLstorm-1.0.0/PKG-INFO` & `DLstorm-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLstorm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deep Learning framework from scratch
 Home-page: https://github.com/HassanRady/DLstorm
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `DLstorm-1.0.0/setup.py` & `DLstorm-1.0.1/setup.py`

 * *Files identical despite different names*

