# Comparing `tmp/hsclient-0.3.1.tar.gz` & `tmp/hsclient-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsclient-0.3.1.tar", last modified: Mon Jul 11 14:30:23 2022, max compression
+gzip compressed data, was "hsclient-0.3.3.tar", last modified: Wed Apr 19 20:50:47 2023, max compression
```

## Comparing `hsclient-0.3.1.tar` & `hsclient-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 14:30:23.738378 hsclient-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-07-11 14:30:15.000000 hsclient-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-07-11 14:30:23.738378 hsclient-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-07-11 14:30:15.000000 hsclient-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 14:30:23.734378 hsclient-0.3.1/hsclient/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-11 14:30:15.000000 hsclient-0.3.1/hsclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42466 2022-07-11 14:30:15.000000 hsclient-0.3.1/hsclient/hydroshare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-07-11 14:30:15.000000 hsclient-0.3.1/hsclient/json_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-07-11 14:30:15.000000 hsclient-0.3.1/hsclient/oauth2_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-07-11 14:30:15.000000 hsclient-0.3.1/hsclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 14:30:23.738378 hsclient-0.3.1/hsclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-07-11 14:30:23.000000 hsclient-0.3.1/hsclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-07-11 14:30:23.000000 hsclient-0.3.1/hsclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 14:30:23.000000 hsclient-0.3.1/hsclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-07-11 14:30:23.000000 hsclient-0.3.1/hsclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-11 14:30:23.000000 hsclient-0.3.1/hsclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-11 14:30:23.738378 hsclient-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-07-11 14:30:15.000000 hsclient-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 20:50:37.000000 hsclient-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-19 20:50:47.155613 hsclient-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-19 20:50:37.000000 hsclient-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/hsclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42466 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/hydroshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/json_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/oauth2_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/hsclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-19 20:50:47.155613 hsclient-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-19 20:50:37.000000 hsclient-0.3.3/setup.py
```

### Comparing `hsclient-0.3.1/LICENSE.txt` & `hsclient-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/PKG-INFO` & `hsclient-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 0.3.1
+Version: 0.3.3
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -78,9 +77,7 @@
 # Call the save function to save the metadata edits to HydroShare
 new_resource.save()
 
 # Print the title just added to the resource
 print('Title: ' + new_resource.metadata.title)
 print('Abstract: ' + new_resource.metadata.abstract)
 ```
-
-
```

### Comparing `hsclient-0.3.1/README.md` & `hsclient-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/hsclient/hydroshare.py` & `hsclient-0.3.3/hsclient/hydroshare.py`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/hsclient/json_models.py` & `hsclient-0.3.3/hsclient/json_models.py`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/hsclient/utils.py` & `hsclient-0.3.3/hsclient/utils.py`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/hsclient.egg-info/PKG-INFO` & `hsclient-0.3.3/hsclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 0.3.1
+Version: 0.3.3
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -78,9 +77,7 @@
 # Call the save function to save the metadata edits to HydroShare
 new_resource.save()
 
 # Print the title just added to the resource
 print('Title: ' + new_resource.metadata.title)
 print('Abstract: ' + new_resource.metadata.abstract)
 ```
-
-
```

### Comparing `hsclient-0.3.1/setup.cfg` & `hsclient-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.1/setup.py` & `hsclient-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pathlib
 from setuptools import setup, find_packages
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='hsclient',
-    version='0.3.1',
+    version='0.3.3',
     packages=find_packages(include=['hsclient', 'hsclient.*'],
                            exclude=("tests",)),
     install_requires=[
-        'hsmodels>=0.5.1',
+        'hsmodels>=0.5.5',
         'requests',
         'requests_oauthlib',
         'pandas'
     ],
     url='https://github.com/hydroshare/hsclient',
     license='MIT',
     author='Scott Black',
```

