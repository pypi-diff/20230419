# Comparing `tmp/toolshelf-0.2.0.tar.gz` & `tmp/toolshelf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolshelf-0.2.0.tar", last modified: Wed Apr 19 18:47:46 2023, max compression
+gzip compressed data, was "toolshelf-0.2.1.tar", last modified: Wed Apr 19 19:36:21 2023, max compression
```

## Comparing `toolshelf-0.2.0.tar` & `toolshelf-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 18:47:46.813662 toolshelf-0.2.0/
--rw-r--r--   0 ccroberts (105479) staff       (20)      669 2023-04-19 18:47:46.813314 toolshelf-0.2.0/PKG-INFO
--rw-r--r--   0 ccroberts (105479) staff       (20)       38 2023-04-19 18:47:46.813796 toolshelf-0.2.0/setup.cfg
--rw-r--r--   0 ccroberts (105479) staff       (20)      850 2023-04-19 18:33:47.000000 toolshelf-0.2.0/setup.py
-drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 18:47:46.809321 toolshelf-0.2.0/toolshelf/
--rw-r--r--   0 ccroberts (105479) staff       (20)       25 2023-04-19 03:19:38.000000 toolshelf-0.2.0/toolshelf/__init__.py
--rw-r--r--   0 ccroberts (105479) staff       (20)     2499 2023-04-19 17:37:36.000000 toolshelf-0.2.0/toolshelf/toolshelf.py
-drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 18:47:46.812522 toolshelf-0.2.0/toolshelf.egg-info/
--rw-r--r--   0 ccroberts (105479) staff       (20)      669 2023-04-19 18:47:46.000000 toolshelf-0.2.0/toolshelf.egg-info/PKG-INFO
--rw-r--r--   0 ccroberts (105479) staff       (20)      249 2023-04-19 18:47:46.000000 toolshelf-0.2.0/toolshelf.egg-info/SOURCES.txt
--rw-r--r--   0 ccroberts (105479) staff       (20)        1 2023-04-19 18:47:46.000000 toolshelf-0.2.0/toolshelf.egg-info/dependency_links.txt
--rw-r--r--   0 ccroberts (105479) staff       (20)        1 2023-04-19 03:07:22.000000 toolshelf-0.2.0/toolshelf.egg-info/not-zip-safe
--rw-r--r--   0 ccroberts (105479) staff       (20)       54 2023-04-19 18:47:46.000000 toolshelf-0.2.0/toolshelf.egg-info/requires.txt
--rw-r--r--   0 ccroberts (105479) staff       (20)       10 2023-04-19 18:47:46.000000 toolshelf-0.2.0/toolshelf.egg-info/top_level.txt
+drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 19:36:21.273055 toolshelf-0.2.1/
+-rw-r--r--   0 ccroberts (105479) staff       (20)      624 2023-04-19 19:36:21.272585 toolshelf-0.2.1/PKG-INFO
+-rw-r--r--   0 ccroberts (105479) staff       (20)       38 2023-04-19 19:36:21.273213 toolshelf-0.2.1/setup.cfg
+-rw-r--r--   0 ccroberts (105479) staff       (20)      840 2023-04-19 19:36:17.000000 toolshelf-0.2.1/setup.py
+drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 19:36:21.267973 toolshelf-0.2.1/toolshelf/
+-rw-r--r--   0 ccroberts (105479) staff       (20)       25 2023-04-19 03:19:38.000000 toolshelf-0.2.1/toolshelf/__init__.py
+-rw-r--r--   0 ccroberts (105479) staff       (20)     2487 2023-04-19 19:35:25.000000 toolshelf-0.2.1/toolshelf/toolshelf.py
+drwxr-xr-x   0 ccroberts (105479) staff       (20)        0 2023-04-19 19:36:21.271814 toolshelf-0.2.1/toolshelf.egg-info/
+-rw-r--r--   0 ccroberts (105479) staff       (20)      624 2023-04-19 19:36:21.000000 toolshelf-0.2.1/toolshelf.egg-info/PKG-INFO
+-rw-r--r--   0 ccroberts (105479) staff       (20)      249 2023-04-19 19:36:21.000000 toolshelf-0.2.1/toolshelf.egg-info/SOURCES.txt
+-rw-r--r--   0 ccroberts (105479) staff       (20)        1 2023-04-19 19:36:21.000000 toolshelf-0.2.1/toolshelf.egg-info/dependency_links.txt
+-rw-r--r--   0 ccroberts (105479) staff       (20)        1 2023-04-19 03:07:22.000000 toolshelf-0.2.1/toolshelf.egg-info/not-zip-safe
+-rw-r--r--   0 ccroberts (105479) staff       (20)       49 2023-04-19 19:36:21.000000 toolshelf-0.2.1/toolshelf.egg-info/requires.txt
+-rw-r--r--   0 ccroberts (105479) staff       (20)       10 2023-04-19 19:36:21.000000 toolshelf-0.2.1/toolshelf.egg-info/top_level.txt
```

### Comparing `toolshelf-0.2.0/PKG-INFO` & `toolshelf-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: toolshelf
-Version: 0.2.0
+Version: 0.2.1
 Summary: ICESat-2 data analysis tools
 Home-page: https://github.com/chancelorr/toolshelf
 Author: chancelor roberts
 Author-email: ccroberts@ucsd.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved
-
-UNKNOWN
-
```

### Comparing `toolshelf-0.2.0/setup.py` & `toolshelf-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='toolshelf', 
-	version='0.2.0', 
+	version='0.2.1', 
 	description='ICESat-2 data analysis tools',
 	author='chancelor roberts',
 	author_email='ccroberts@ucsd.edu',
 	url='https://github.com/chancelorr/toolshelf',
 	install_requires=[
 		'numpy',
 		'requests',
-		'json',
 		'zipfile',
 		'io',
 		'os',
 		'pprint',
 		're',
 		'time',
 		'h5py'
```

### Comparing `toolshelf-0.2.0/toolshelf/toolshelf.py` & `toolshelf-0.2.1/toolshelf/toolshelf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import requests
-import json
 import zipfile
 import io
 import os
 import pprint
 import re
 import time
 import h5py as h
```

### Comparing `toolshelf-0.2.0/toolshelf.egg-info/PKG-INFO` & `toolshelf-0.2.1/toolshelf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: toolshelf
-Version: 0.2.0
+Version: 0.2.1
 Summary: ICESat-2 data analysis tools
 Home-page: https://github.com/chancelorr/toolshelf
 Author: chancelor roberts
 Author-email: ccroberts@ucsd.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved
-
-UNKNOWN
-
```

