# Comparing `tmp/PRauto-0.12.tar.gz` & `tmp/PRauto-0.121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.12.tar", last modified: Wed Apr 19 01:55:00 2023, max compression
+gzip compressed data, was "PRauto-0.121.tar", last modified: Wed Apr 19 11:36:51 2023, max compression
```

## Comparing `PRauto-0.12.tar` & `PRauto-0.121.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.071836 PRauto-0.12/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.12/LICENSE
--rw-rw-rw-   0        0        0      364 2023-04-19 01:55:00.071319 PRauto-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.049898 PRauto-0.12/PRauto.egg-info/
--rw-rw-rw-   0        0        0      364 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 06:21:00.000000 PRauto-0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.051903 PRauto-0.12/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.12/prauto/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-04-19 01:41:22.000000 PRauto-0.12/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.055314 PRauto-0.12/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.12/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.069318 PRauto-0.12/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.12/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.12/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-19 01:55:00.071836 PRauto-0.12/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-19 01:07:08.000000 PRauto-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.862825 PRauto-0.121/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.121/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-04-19 11:36:51.861824 PRauto-0.121/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.848852 PRauto-0.121/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-04-19 11:33:52.000000 PRauto-0.121/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.851856 PRauto-0.121/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.121/prauto/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-04-19 01:41:22.000000 PRauto-0.121/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.853824 PRauto-0.121/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.121/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.859829 PRauto-0.121/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.121/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.121/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:36:51.862825 PRauto-0.121/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-04-19 11:36:20.000000 PRauto-0.121/setup.py
```

### Comparing `PRauto-0.12/LICENSE` & `PRauto-0.121/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/prauto/__main__.py` & `PRauto-0.121/prauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/prauto/prepauto/__main__.py` & `PRauto-0.121/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/prauto/retriever/get_fasta.py` & `PRauto-0.121/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/prauto/retriever/get_ligand.py` & `PRauto-0.121/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/prauto/retriever/get_pdb.py` & `PRauto-0.121/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.12/setup.py` & `PRauto-0.121/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.12',
+        version = '0.121',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
@@ -22,11 +22,10 @@
            3. Collect sdf file using ChEMBL API
         
         ## With get_preprocess.py, you can perform the following tasks:
 
            1. Extract the target chain from collected PDB files
            2. Align PDB files based on a chosen criterion
            3. Remove unnecessary molecules such as solvents and reagents from PDB files""",
-        long_description = open('README.md').read(),
         python_requires = '>=3',
         install_requires = required)
```

