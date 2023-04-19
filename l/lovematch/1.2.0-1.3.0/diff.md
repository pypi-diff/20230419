# Comparing `tmp/lovematch-1.2.0.tar.gz` & `tmp/lovematch-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lovematch-1.2.0.tar", last modified: Wed Apr 19 10:51:51 2023, max compression
+gzip compressed data, was "dist\lovematch-1.3.0.tar", last modified: Wed Apr 19 11:26:59 2023, max compression
```

## Comparing `lovematch-1.2.0.tar` & `lovematch-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:51:51.000000 lovematch-1.2.0/
--rw-rw-rw-   0        0        0      573 2023-04-19 10:51:51.000000 lovematch-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-19 10:21:04.000000 lovematch-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 10:51:51.000000 lovematch-1.2.0/lovematch/
--rw-rw-rw-   0        0        0       72 2023-04-19 10:50:31.000000 lovematch-1.2.0/lovematch/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-04-19 10:49:43.000000 lovematch-1.2.0/lovematch/lovematch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:51:51.000000 lovematch-1.2.0/lovematch.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-19 10:51:50.000000 lovematch-1.2.0/lovematch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-19 10:51:51.000000 lovematch-1.2.0/lovematch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:51:50.000000 lovematch-1.2.0/lovematch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 10:51:50.000000 lovematch-1.2.0/lovematch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 10:51:51.000000 lovematch-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-04-19 10:50:39.000000 lovematch-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:59.000000 lovematch-1.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      596 2023-04-19 11:26:59.000000 lovematch-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-19 11:23:31.000000 lovematch-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:59.000000 lovematch-1.3.0/lovematch/
+-rw-rw-rw-   0        0        0       70 2023-04-19 11:20:34.000000 lovematch-1.3.0/lovematch/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-04-19 10:49:43.000000 lovematch-1.3.0/lovematch/lovematch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:59.000000 lovematch-1.3.0/lovematch.egg-info/
+-rw-rw-rw-   0        0        0      596 2023-04-19 11:26:58.000000 lovematch-1.3.0/lovematch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-19 11:26:58.000000 lovematch-1.3.0/lovematch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:26:58.000000 lovematch-1.3.0/lovematch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 11:26:58.000000 lovematch-1.3.0/lovematch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:26:59.000000 lovematch-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-04-19 11:26:54.000000 lovematch-1.3.0/setup.py
```

### Comparing `lovematch-1.2.0/PKG-INFO` & `lovematch-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python library for calculating love and friendship scores
 Author: Deva
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
```

### Comparing `lovematch-1.2.0/lovematch/lovematch.py` & `lovematch-1.3.0/lovematch/lovematch.py`

 * *Files identical despite different names*

### Comparing `lovematch-1.2.0/lovematch.egg-info/PKG-INFO` & `lovematch-1.3.0/lovematch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python library for calculating love and friendship scores
 Author: Deva
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
```

### Comparing `lovematch-1.2.0/setup.py` & `lovematch-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lovematch',
-    version='1.2.0',
+    version='1.3.0',
     description='A Python library for calculating love and friendship scores',
     author='Deva',
     author_email='your.email@example.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

