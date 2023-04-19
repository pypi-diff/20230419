# Comparing `tmp/BraAndKet-0.8.1.tar.gz` & `tmp/BraAndKet-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BraAndKet-0.8.1.tar", last modified: Thu Mar  9 07:41:04 2023, max compression
+gzip compressed data, was "BraAndKet-0.8.2.tar", last modified: Wed Apr 19 10:48:23 2023, max compression
```

## Comparing `BraAndKet-0.8.1.tar` & `BraAndKet-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.477518 BraAndKet-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-09 07:41:04.477518 BraAndKet-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 07:41:04.477518 BraAndKet-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/BraAndKet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-09 07:41:04.000000 BraAndKet-0.8.1/src/BraAndKet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-09 07:41:04.000000 BraAndKet-0.8.1/src/BraAndKet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 07:41:04.000000 BraAndKet-0.8.1/src/BraAndKet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-09 07:41:04.000000 BraAndKet-0.8.1/src/BraAndKet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-09 07:41:04.000000 BraAndKet-0.8.1/src/BraAndKet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/braandket/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/braandket/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/backend/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/backend/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/backend/tensorflow_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/braandket/model/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.473518 BraAndKet-0.8.1/src/braandket/space/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/space/hilbert_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/space/num_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/space/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.477518 BraAndKet-0.8.1/src/braandket/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/tensor/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/tensor/special.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/tensor/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:41:04.477518 BraAndKet-0.8.1/src/braandket/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-09 07:40:49.000000 BraAndKet-0.8.1/src/braandket/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.736989 BraAndKet-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/BraAndKet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/tensorflow_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/hilbert_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/num_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/utils/utils.py
```

### Comparing `BraAndKet-0.8.1/LICENSE` & `BraAndKet-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/PKG-INFO` & `BraAndKet-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.1
+Version: 0.8.2
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 License-File: LICENSE
 
 # BraAndKet
 
 [![License](https://img.shields.io/github/license/ZhengKeli/BraAndKet)](https://github.com/ZhengKeli/BraAndKet/blob/master/LICENSE)
```

### Comparing `BraAndKet-0.8.1/README.md` & `BraAndKet-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/pyproject.toml` & `BraAndKet-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "BraAndKet"
-version = "0.8.1"
+version = "0.8.2"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 description = "BraAndKet is a library for numeral calculations of discrete quantum systems."
 readme = "README.md"
 
 urls.repository = "https://github.com/ZhengKeli/BraAndKet"
 authors = [{ name = "Zheng Keli", email = "zhengkeli2009@126.com" }]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = ["numpy"]
 optional-dependencies.tf = ["tensorflow"]
 
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 packages.find.where = ["src"]
```

### Comparing `BraAndKet-0.8.1/src/BraAndKet.egg-info/PKG-INFO` & `BraAndKet-0.8.2/src/BraAndKet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.1
+Version: 0.8.2
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 License-File: LICENSE
 
 # BraAndKet
 
 [![License](https://img.shields.io/github/license/ZhengKeli/BraAndKet)](https://github.com/ZhengKeli/BraAndKet/blob/master/LICENSE)
```

### Comparing `BraAndKet-0.8.1/src/BraAndKet.egg-info/SOURCES.txt` & `BraAndKet-0.8.2/src/BraAndKet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/backend/backend.py` & `BraAndKet-0.8.2/src/braandket/backend/backend.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/backend/default.py` & `BraAndKet-0.8.2/src/braandket/backend/default.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/backend/numpy_backend.py` & `BraAndKet-0.8.2/src/braandket/backend/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/backend/tensorflow_backend.py` & `BraAndKet-0.8.2/src/braandket/backend/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/model/model.py` & `BraAndKet-0.8.2/src/braandket/model/model.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/space/hilbert_space.py` & `BraAndKet-0.8.2/src/braandket/space/hilbert_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/space/num_space.py` & `BraAndKet-0.8.2/src/braandket/space/num_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/space/space.py` & `BraAndKet-0.8.2/src/braandket/space/space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/tensor/operations.py` & `BraAndKet-0.8.2/src/braandket/tensor/operations.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/tensor/special.py` & `BraAndKet-0.8.2/src/braandket/tensor/special.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/tensor/tensor.py` & `BraAndKet-0.8.2/src/braandket/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.1/src/braandket/utils/utils.py` & `BraAndKet-0.8.2/src/braandket/utils/utils.py`

 * *Files identical despite different names*

