# Comparing `tmp/lovematch-1.5.0.tar.gz` & `tmp/lovematch-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lovematch-1.5.0.tar", last modified: Wed Apr 19 11:45:25 2023, max compression
+gzip compressed data, was "dist\lovematch-1.6.0.tar", last modified: Wed Apr 19 12:20:51 2023, max compression
```

## Comparing `lovematch-1.5.0.tar` & `lovematch-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/
--rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      641 2023-04-19 11:45:25.000000 lovematch-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-19 11:23:31.000000 lovematch-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/Relation_Calculator/
--rw-rw-rw-   0        0        0      101 2023-04-19 11:44:28.000000 lovematch-1.5.0/Relation_Calculator/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-04-19 11:45:17.000000 lovematch-1.5.0/Relation_Calculator/lovematch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/lovematch.egg-info/
--rw-rw-rw-   0        0        0      641 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-19 11:45:25.000000 lovematch-1.5.0/lovematch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 11:45:25.000000 lovematch-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-04-19 11:42:56.000000 lovematch-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:20:51.000000 lovematch-1.6.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      694 2023-04-19 12:20:51.000000 lovematch-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-04-19 12:17:20.000000 lovematch-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:20:51.000000 lovematch-1.6.0/lovematch/
+-rw-rw-rw-   0        0        0      198 2023-04-19 12:15:32.000000 lovematch-1.6.0/lovematch/__init__.py
+-rw-rw-rw-   0        0        0     1560 2023-04-19 12:15:38.000000 lovematch-1.6.0/lovematch/friendship.py
+-rw-rw-rw-   0        0        0     3072 2023-04-19 12:15:33.000000 lovematch-1.6.0/lovematch/love.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:20:51.000000 lovematch-1.6.0/lovematch.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-19 12:20:50.000000 lovematch-1.6.0/lovematch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-19 12:20:51.000000 lovematch-1.6.0/lovematch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:20:50.000000 lovematch-1.6.0/lovematch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 12:20:50.000000 lovematch-1.6.0/lovematch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:20:51.000000 lovematch-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-19 12:20:28.000000 lovematch-1.6.0/setup.py
```

### Comparing `lovematch-1.5.0/LICENSE` & `lovematch-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lovematch-1.5.0/PKG-INFO` & `lovematch-1.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.5.0
+Version: 1.6.0
 Summary: Love Match Calculator
+Home-page: https://github.com/Devparihar5/lovematch
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: python,love,match,percentage,calculator,lovematch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `lovematch-1.5.0/Relation_Calculator/lovematch.py` & `lovematch-1.6.0/lovematch/love.py`

 * *Files identical despite different names*

### Comparing `lovematch-1.5.0/lovematch.egg-info/PKG-INFO` & `lovematch-1.6.0/lovematch.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.5.0
+Version: 1.6.0
 Summary: Love Match Calculator
+Home-page: https://github.com/Devparihar5/lovematch
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: python,love,match,percentage,calculator,lovematch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `lovematch-1.5.0/setup.py` & `lovematch-1.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.5.0'
+VERSION = '1.6.0'
 DESCRIPTION = 'Love Match Calculator'
 LONG_DESCRIPTION = 'A Python package to calculate love match percentage between two names.'
 
 # Setting up
 setup(
     name="lovematch",
     version=VERSION,
     author="Devendra Parihar",
     author_email="devendraparihar340@gmail.com",
+    url="https://github.com/Devparihar5/lovematch",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'love', 'match', 'percentage', 'calculator', 'lovematch'],
     classifiers=[
```

