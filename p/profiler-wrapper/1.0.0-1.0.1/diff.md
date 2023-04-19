# Comparing `tmp/profiler_wrapper-1.0.0.tar.gz` & `tmp/profiler_wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profiler_wrapper-1.0.0.tar", last modified: Wed Apr 19 19:27:58 2023, max compression
+gzip compressed data, was "profiler_wrapper-1.0.1.tar", last modified: Wed Apr 19 19:37:08 2023, max compression
```

## Comparing `profiler_wrapper-1.0.0.tar` & `profiler_wrapper-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-04-19 19:27:58.944302 profiler_wrapper-1.0.0/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)    33254 2023-04-19 19:00:10.000000 profiler_wrapper-1.0.0/LICENSE.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)     1784 2023-04-19 19:27:58.944302 profiler_wrapper-1.0.0/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)     1116 2023-04-19 19:18:18.000000 profiler_wrapper-1.0.0/README.md
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-04-19 19:27:58.944302 profiler_wrapper-1.0.0/profiler_wrapper.egg-info/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)     1784 2023-04-19 19:27:58.000000 profiler_wrapper-1.0.0/profiler_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      205 2023-04-19 19:27:58.000000 profiler_wrapper-1.0.0/profiler_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-04-19 19:27:58.000000 profiler_wrapper-1.0.0/profiler_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-04-19 19:27:58.000000 profiler_wrapper-1.0.0/profiler_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 profiler_wrapper-1.0.0/pyproject.toml
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-04-19 19:27:58.944302 profiler_wrapper-1.0.0/setup.cfg
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      886 2023-04-19 19:27:46.000000 profiler_wrapper-1.0.0/setup.py
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-04-19 19:37:08.231990 profiler_wrapper-1.0.1/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)    33254 2023-04-19 19:00:10.000000 profiler_wrapper-1.0.1/LICENSE.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)     1730 2023-04-19 19:37:08.231990 profiler_wrapper-1.0.1/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)     1062 2023-04-19 19:29:26.000000 profiler_wrapper-1.0.1/README.md
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-04-19 19:37:08.231990 profiler_wrapper-1.0.1/profiler_wrapper.egg-info/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)     1730 2023-04-19 19:37:08.000000 profiler_wrapper-1.0.1/profiler_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      212 2023-04-19 19:37:08.000000 profiler_wrapper-1.0.1/profiler_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-04-19 19:37:08.000000 profiler_wrapper-1.0.1/profiler_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)        4 2023-04-19 19:37:08.000000 profiler_wrapper-1.0.1/profiler_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 profiler_wrapper-1.0.1/pyproject.toml
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      618 2023-04-19 19:35:24.000000 profiler_wrapper-1.0.1/run.py
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-04-19 19:37:08.231990 profiler_wrapper-1.0.1/setup.cfg
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      886 2023-04-19 19:36:59.000000 profiler_wrapper-1.0.1/setup.py
```

### Comparing `profiler_wrapper-1.0.0/LICENSE.txt` & `profiler_wrapper-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `profiler_wrapper-1.0.0/PKG-INFO` & `profiler_wrapper-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiler_wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper script for easier use of the built-in profiler
 Home-page: https://github.com/superstes/python3-profile-wrapper
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/python3-profile-wrapper
 Project-URL: Bug Tracker, https://github.com/superstes/python3-profile-wrapper/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,25 +19,19 @@
 This package provides a wrapper function for easier usage of the built-in profiler.
 
 It only uses builtin modules.
 
 ## Install
 
 ```bash
-python3 -m pip install profiler_wrapper
+python3 -m pip install profiler-wrapper
 ```
 
 See: [PyPI](https://pypi.org/project/profiler_wrapper/)
 
-## Install
-
-```bash
-pip install profiler_wrapper
-```
-
 ## Usage
 
 ```python3
 from profiler_wrapper import profile
 
 def function_to_profile(switch: bool, data: dict, msg: str):
     ...
```

### Comparing `profiler_wrapper-1.0.0/README.md` & `profiler_wrapper-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,19 @@
 This package provides a wrapper function for easier usage of the built-in profiler.
 
 It only uses builtin modules.
 
 ## Install
 
 ```bash
-python3 -m pip install profiler_wrapper
+python3 -m pip install profiler-wrapper
 ```
 
 See: [PyPI](https://pypi.org/project/profiler_wrapper/)
 
-## Install
-
-```bash
-pip install profiler_wrapper
-```
-
 ## Usage
 
 ```python3
 from profiler_wrapper import profile
 
 def function_to_profile(switch: bool, data: dict, msg: str):
     ...
```

### Comparing `profiler_wrapper-1.0.0/profiler_wrapper.egg-info/PKG-INFO` & `profiler_wrapper-1.0.1/profiler_wrapper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiler-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper script for easier use of the built-in profiler
 Home-page: https://github.com/superstes/python3-profile-wrapper
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/python3-profile-wrapper
 Project-URL: Bug Tracker, https://github.com/superstes/python3-profile-wrapper/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,25 +19,19 @@
 This package provides a wrapper function for easier usage of the built-in profiler.
 
 It only uses builtin modules.
 
 ## Install
 
 ```bash
-python3 -m pip install profiler_wrapper
+python3 -m pip install profiler-wrapper
 ```
 
 See: [PyPI](https://pypi.org/project/profiler_wrapper/)
 
-## Install
-
-```bash
-pip install profiler_wrapper
-```
-
 ## Usage
 
 ```python3
 from profiler_wrapper import profile
 
 def function_to_profile(switch: bool, data: dict, msg: str):
     ...
```

### Comparing `profiler_wrapper-1.0.0/setup.py` & `profiler_wrapper-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as info:
     long_description = info.read()
 
 setuptools.setup(
     name='profiler_wrapper',
-    version='1.0.0',
+    version='1.0.1',
     author='René Rath',
     author_email='contact@superstes.eu',
     description='Wrapper script for easier use of the built-in profiler',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/superstes/python3-profile-wrapper',
     project_urls={
```

