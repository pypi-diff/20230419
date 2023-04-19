# Comparing `tmp/scBC-0.2.0.tar.gz` & `tmp/scBC-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scBC-0.2.0.tar", last modified: Wed Apr 19 03:44:51 2023, max compression
+gzip compressed data, was "scBC-0.2.1.tar", last modified: Wed Apr 19 05:09:37 2023, max compression
```

## Comparing `scBC-0.2.0.tar` & `scBC-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.746107 scBC-0.2.0/
--rw-rw-rw-   0        0        0     1065 2023-04-19 03:17:25.000000 scBC-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    10969 2023-04-19 03:44:51.745112 scBC-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10403 2023-04-19 03:14:30.000000 scBC-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.736101 scBC-0.2.0/scBC/
--rw-rw-rw-   0        0        0     6095 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/DWL.py
--rw-rw-rw-   0        0        0        0 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/__init__.py
--rw-rw-rw-   0        0        0     4240 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/data.py
--rw-rw-rw-   0        0        0    18655 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/model.py
-drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.742107 scBC-0.2.0/scBC.egg-info/
--rw-rw-rw-   0        0        0    10969 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 03:44:51.746107 scBC-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-04-19 03:44:45.000000 scBC-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.830209 scBC-0.2.1/
+-rw-rw-rw-   0        0        0     1065 2023-04-19 03:17:25.000000 scBC-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    10969 2023-04-19 05:09:37.829207 scBC-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10403 2023-04-19 03:14:30.000000 scBC-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.824207 scBC-0.2.1/scBC/
+-rw-rw-rw-   0        0        0     6095 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/DWL.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/__init__.py
+-rw-rw-rw-   0        0        0     4240 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/data.py
+-rw-rw-rw-   0        0        0    18655 2023-04-19 03:14:30.000000 scBC-0.2.1/scBC/model.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:09:37.828208 scBC-0.2.1/scBC.egg-info/
+-rw-rw-rw-   0        0        0    10969 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 05:09:37.000000 scBC-0.2.1/scBC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:09:37.830209 scBC-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      958 2023-04-19 05:09:07.000000 scBC-0.2.1/setup.py
```

### Comparing `scBC-0.2.0/LICENSE` & `scBC-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scBC-0.2.0/PKG-INFO` & `scBC-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBC
-Version: 0.2.0
+Version: 0.2.1
 Summary: a single-cell transcriptome Bayesian biClustering framework
 Home-page: https://github.com/GYQ-form/scBC
 Author: Yuqiao Gong
 Author-email: gyq123@sjtu.edu.cn
 License: MIT
 Keywords: single cell transcriptomics,Biclustering,bioinformatics,variational inference(VI)
 Platform: UNKNOWN
```

### Comparing `scBC-0.2.0/README.md` & `scBC-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scBC-0.2.0/scBC/DWL.py` & `scBC-0.2.1/scBC/DWL.py`

 * *Files identical despite different names*

### Comparing `scBC-0.2.0/scBC/data.py` & `scBC-0.2.1/scBC/data.py`

 * *Files identical despite different names*

### Comparing `scBC-0.2.0/scBC/model.py` & `scBC-0.2.1/scBC/model.py`

 * *Files identical despite different names*

### Comparing `scBC-0.2.0/scBC.egg-info/PKG-INFO` & `scBC-0.2.1/scBC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBC
-Version: 0.2.0
+Version: 0.2.1
 Summary: a single-cell transcriptome Bayesian biClustering framework
 Home-page: https://github.com/GYQ-form/scBC
 Author: Yuqiao Gong
 Author-email: gyq123@sjtu.edu.cn
 License: MIT
 Keywords: single cell transcriptomics,Biclustering,bioinformatics,variational inference(VI)
 Platform: UNKNOWN
```

### Comparing `scBC-0.2.0/setup.py` & `scBC-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="scBC",
     version=__version__,
@@ -12,15 +12,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
     install_requires=[
-        'scvi-tools',
+        'scvi-tools>=0.19.0',
         'biomart',
         "requests",
         "scipy"
         ],
     author="Yuqiao Gong",
     author_email="gyq123@sjtu.edu.cn",
     keywords=["single cell transcriptomics", "Biclustering", "bioinformatics", "variational inference(VI)"],
```

