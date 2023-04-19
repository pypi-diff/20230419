# Comparing `tmp/dagster-wandb-0.18.7.tar.gz` & `tmp/dagster-wandb-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.18.7.tar", last modified: Thu Apr 13 15:12:36 2023, max compression
+gzip compressed data, was "dagster-wandb-0.19.0.tar", last modified: Wed Apr 19 19:14:08 2023, max compression
```

## Comparing `dagster-wandb-0.18.7.tar` & `dagster-wandb-0.19.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:36.441506 dagster-wandb-0.18.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      679 2023-04-13 15:12:36.441506 dagster-wandb-0.18.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:36.441506 dagster-wandb-0.18.7/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33673 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:36.441506 dagster-wandb-0.18.7/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2157 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/types.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:12:36.441506 dagster-wandb-0.18.7/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      679 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 15:12:36.000000 dagster-wandb-0.18.7/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-13 15:12:36.445506 dagster-wandb-0.18.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1360 2023-04-13 15:03:07.000000 dagster-wandb-0.18.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33673 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/types.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-19 19:14:08.000000 dagster-wandb-0.19.0/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-04-19 19:14:08.691882 dagster-wandb-0.19.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-04-19 19:01:30.000000 dagster-wandb-0.19.0/setup.py
```

### Comparing `dagster-wandb-0.18.7/LICENSE` & `dagster-wandb-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/PKG-INFO` & `dagster-wandb-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.18.7
+Version: 0.19.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.18.7/dagster_wandb/__init__.py` & `dagster-wandb-0.19.0/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb/io_manager.py` & `dagster-wandb-0.19.0/dagster_wandb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb/launch/configs.py` & `dagster-wandb-0.19.0/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb/launch/ops.py` & `dagster-wandb-0.19.0/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb/resources.py` & `dagster-wandb-0.19.0/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb/types.py` & `dagster-wandb-0.19.0/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.19.0/dagster_wandb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.18.7
+Version: 0.19.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.18.7/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.19.0/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.18.7/setup.py` & `dagster-wandb-0.19.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     install_requires=[
-        "dagster==1.2.7",
+        "dagster==1.3.0",
         "wandb>=0.13.5",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

