# Comparing `tmp/SBOannotator-2.0.tar.gz` & `tmp/SBOannotator-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SBOannotator-2.0.tar", last modified: Wed Apr 19 09:17:21 2023, max compression
+gzip compressed data, was "dist/SBOannotator-2.1.tar", last modified: Wed Apr 19 10:36:53 2023, max compression
```

## Comparing `SBOannotator-2.0.tar` & `SBOannotator-2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:17:21.268891 SBOannotator-2.0/
--rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.0/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     4146 2023-04-19 09:17:21.268556 SBOannotator-2.0/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)     3376 2023-04-19 08:25:50.000000 SBOannotator-2.0/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:17:21.267933 SBOannotator-2.0/SBOannotator.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     4146 2023-04-19 09:17:21.000000 SBOannotator-2.0/SBOannotator.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      220 2023-04-19 09:17:21.000000 SBOannotator-2.0/SBOannotator.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:17:21.000000 SBOannotator-2.0/SBOannotator.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       52 2023-04-19 09:17:21.000000 SBOannotator-2.0/SBOannotator.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:17:21.000000 SBOannotator-2.0/SBOannotator.egg-info/top_level.txt
--rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.0/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 09:17:21.269050 SBOannotator-2.0/setup.cfg
--rw-r--r--   0 leonidou   (501) staff       (20)     1122 2023-04-19 09:17:05.000000 SBOannotator-2.0/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 10:36:53.368129 SBOannotator-2.1/
+-rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.1/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     4146 2023-04-19 10:36:53.367784 SBOannotator-2.1/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)     3376 2023-04-19 08:25:50.000000 SBOannotator-2.1/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 10:36:53.367321 SBOannotator-2.1/SBOannotator.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     4146 2023-04-19 10:36:53.000000 SBOannotator-2.1/SBOannotator.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)      244 2023-04-19 10:36:53.000000 SBOannotator-2.1/SBOannotator.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 10:36:53.000000 SBOannotator-2.1/SBOannotator.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       52 2023-04-19 10:36:53.000000 SBOannotator-2.1/SBOannotator.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       25 2023-04-19 10:36:53.000000 SBOannotator-2.1/SBOannotator.egg-info/top_level.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)    20309 2023-02-20 21:46:40.000000 SBOannotator-2.1/SBOannotator.py
+-rw-r--r--   0 leonidou   (501) staff       (20)     1192 2023-02-20 21:45:02.000000 SBOannotator-2.1/main.py
+-rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.1/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 10:36:53.368274 SBOannotator-2.1/setup.cfg
+-rw-r--r--   0 leonidou   (501) staff       (20)     1262 2023-04-19 10:36:21.000000 SBOannotator-2.1/setup.py
```

### Comparing `SBOannotator-2.0/LICENSE` & `SBOannotator-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SBOannotator-2.0/PKG-INFO` & `SBOannotator-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBOannotator
-Version: 2.0
+Version: 2.1
 Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
 Home-page: https://github.com/draeger-lab/SBOannotator
 Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: SBOannotator,SBO Terms,automated tool
 Platform: UNKNOWN
```

### Comparing `SBOannotator-2.0/README.md` & `SBOannotator-2.1/README.md`

 * *Files identical despite different names*

### Comparing `SBOannotator-2.0/SBOannotator.egg-info/PKG-INFO` & `SBOannotator-2.1/SBOannotator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBOannotator
-Version: 2.0
+Version: 2.1
 Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
 Home-page: https://github.com/draeger-lab/SBOannotator
 Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: SBOannotator,SBO Terms,automated tool
 Platform: UNKNOWN
```

### Comparing `SBOannotator-2.0/setup.py` & `SBOannotator-2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SBOannotator',
-    version='2.0',
+    version='2.1',
     description='SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/SBOannotator',
     author='Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
     keywords=['SBOannotator', 'SBO Terms', 'automated tool'],
     install_requires=['python-libsbml',
                       'python-collection',
                       'requests',
                       'pypi-json'],
+    packages=['models'],
+    py_modules=['SBOannotator', 'main'],
+    package_data={'': ['create_dbs.sql']},
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Version Control :: Git",
         "Operating System :: MacOS",
         "Operating System :: Unix"
```

