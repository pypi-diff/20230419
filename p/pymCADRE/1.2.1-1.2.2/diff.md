# Comparing `tmp/pymCADRE-1.2.1.tar.gz` & `tmp/pymCADRE-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymCADRE-1.2.1.tar", last modified: Fri Apr  7 00:59:32 2023, max compression
+gzip compressed data, was "dist/pymCADRE-1.2.2.tar", last modified: Wed Apr 19 09:37:17 2023, max compression
```

## Comparing `pymCADRE-1.2.1.tar` & `pymCADRE-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-07 00:59:32.609207 pymCADRE-1.2.1/
--rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.1/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     3880 2023-04-07 00:59:32.608847 pymCADRE-1.2.1/PKG-INFO
--rw-rw-r--   0 leonidou   (501) staff       (20)     3278 2021-10-13 11:22:14.000000 pymCADRE-1.2.1/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-07 00:59:32.608415 pymCADRE-1.2.1/pymCADRE.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     3880 2023-04-07 00:59:32.000000 pymCADRE-1.2.1/pymCADRE.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      200 2023-04-07 00:59:32.000000 pymCADRE-1.2.1/pymCADRE.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-07 00:59:32.000000 pymCADRE-1.2.1/pymCADRE.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       33 2023-04-07 00:59:32.000000 pymCADRE-1.2.1/pymCADRE.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-07 00:59:32.000000 pymCADRE-1.2.1/pymCADRE.egg-info/top_level.txt
--rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.1/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-07 00:59:32.609372 pymCADRE-1.2.1/setup.cfg
--rw-rw-r--   0 leonidou   (501) staff       (20)     1015 2023-04-07 00:59:25.000000 pymCADRE-1.2.1/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:37:17.577690 pymCADRE-1.2.2/
+-rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     3948 2023-04-19 09:37:17.577322 pymCADRE-1.2.2/PKG-INFO
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3278 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:37:17.576775 pymCADRE-1.2.2/pymCADRE.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     3948 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)      200 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       33 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:37:17.000000 pymCADRE-1.2.2/pymCADRE.egg-info/top_level.txt
+-rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.2/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 09:37:17.577822 pymCADRE-1.2.2/setup.cfg
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1008 2023-04-19 09:36:13.000000 pymCADRE-1.2.2/setup.py
```

### Comparing `pymCADRE-1.2.1/LICENSE` & `pymCADRE-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.1/PKG-INFO` & `pymCADRE-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.1
+Version: 1.2.2
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
+Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymCADRE 
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
```

### Comparing `pymCADRE-1.2.1/README.md` & `pymCADRE-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.1/pymCADRE.egg-info/PKG-INFO` & `pymCADRE-1.2.2/pymCADRE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.1
+Version: 1.2.2
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
+Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymCADRE 
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
```

### Comparing `pymCADRE-1.2.1/setup.py` & `pymCADRE-1.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymCADRE',
-    version='1.2.1',
+    version='1.2.2',
     description='The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/pymCADRE',
     author='Nantia Leonidou',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
-    packages=find_packages(where='pmCADRE_code/code', include=['check','prune','rank']),
+    keywords=['pymCADRE', 'systems biology', 'tissue-specific metabolic models'],
     install_requires=['pandas',
                       'numpy',
                       'cobrapy',
                       'requests',
                       'os']
 )
```

