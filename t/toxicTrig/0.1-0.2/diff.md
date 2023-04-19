# Comparing `tmp/toxicTrig-0.1.tar.gz` & `tmp/toxicTrig-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toxicTrig-0.1.tar", last modified: Tue Apr 18 17:53:06 2023, max compression
+gzip compressed data, was "toxicTrig-0.2.tar", last modified: Wed Apr 19 02:09:16 2023, max compression
```

## Comparing `toxicTrig-0.1.tar` & `toxicTrig-0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-18 17:53:06.441765 toxicTrig-0.1/
--rw-r--r--   0 xuhuizhou   (501) staff       (20)     1071 2023-04-18 16:06:43.000000 toxicTrig-0.1/LICENSE
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       33 2023-04-18 16:03:47.000000 toxicTrig-0.1/MANIFEST.in
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      616 2023-04-18 17:53:06.441641 toxicTrig-0.1/PKG-INFO
--rw-r--r--   0 xuhuizhou   (501) staff       (20)     1575 2023-04-18 16:12:05.000000 toxicTrig-0.1/README.md
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       38 2023-04-18 17:53:06.441802 toxicTrig-0.1/setup.cfg
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      730 2023-04-18 17:52:23.000000 toxicTrig-0.1/setup.py
-drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-18 17:53:06.441473 toxicTrig-0.1/toxicTrig.egg-info/
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      616 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/PKG-INFO
--rw-r--r--   0 xuhuizhou   (501) staff       (20)      202 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/SOURCES.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)        1 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/dependency_links.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)       18 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/requires.txt
--rw-r--r--   0 xuhuizhou   (501) staff       (20)        1 2023-04-18 17:53:06.000000 toxicTrig-0.1/toxicTrig.egg-info/top_level.txt
+drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-19 02:09:16.302014 toxicTrig-0.2/
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)     1071 2023-04-18 16:06:43.000000 toxicTrig-0.2/LICENSE
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)       28 2023-04-19 00:47:33.000000 toxicTrig-0.2/MANIFEST.in
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)     2224 2023-04-19 02:09:16.301879 toxicTrig-0.2/PKG-INFO
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)     1575 2023-04-18 16:12:05.000000 toxicTrig-0.2/README.md
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)       38 2023-04-19 02:09:16.302054 toxicTrig-0.2/setup.cfg
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)      878 2023-04-19 01:30:42.000000 toxicTrig-0.2/setup.py
+drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-19 02:09:16.300469 toxicTrig-0.2/toxicTrig/
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)       37 2023-04-19 02:01:37.000000 toxicTrig-0.2/toxicTrig/__init__.py
+drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-19 02:09:16.301354 toxicTrig-0.2/toxicTrig/data/
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)    16940 2023-04-18 15:55:07.000000 toxicTrig-0.2/toxicTrig/data/word_based_bias_list.csv
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)      549 2023-04-19 01:03:57.000000 toxicTrig-0.2/toxicTrig/toxic_triggers.py
+drwxr-xr-x   0 xuhuizhou   (501) staff       (20)        0 2023-04-19 02:09:16.301247 toxicTrig-0.2/toxicTrig.egg-info/
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)     2224 2023-04-19 02:09:16.000000 toxicTrig-0.2/toxicTrig.egg-info/PKG-INFO
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)      292 2023-04-19 02:09:16.000000 toxicTrig-0.2/toxicTrig.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)        1 2023-04-19 02:09:16.000000 toxicTrig-0.2/toxicTrig.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)       18 2023-04-19 02:09:16.000000 toxicTrig-0.2/toxicTrig.egg-info/requires.txt
+-rw-r--r--   0 xuhuizhou   (501) staff       (20)       10 2023-04-19 02:09:16.000000 toxicTrig-0.2/toxicTrig.egg-info/top_level.txt
```

### Comparing `toxicTrig-0.1/LICENSE` & `toxicTrig-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toxicTrig-0.1/README.md` & `toxicTrig-0.2/README.md`

 * *Files identical despite different names*

### Comparing `toxicTrig-0.1/setup.py` & `toxicTrig-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
+with open("README.md", "r") as fh:
+    description = fh.read()
 
 setup(
     name='toxicTrig',
-    version='0.1',
+    version='0.2',
     description='full set of words that trigger toxicity',
+    long_description=description,
+    long_description_content_type="text/markdown",
     author='Xuhui Zhou, Maarten Sap',
     author_email='xuhuiz@cs.cmu.edu',
     url='https://github.com/XuhuiZhou/toxtrig',
     packages=find_packages(),
     install_requires=[
        'setuptools',
        'pandas',
```

