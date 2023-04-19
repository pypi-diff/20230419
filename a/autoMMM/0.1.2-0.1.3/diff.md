# Comparing `tmp/autoMMM-0.1.2.tar.gz` & `tmp/autoMMM-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMMM-0.1.2.tar", last modified: Wed Apr 12 09:56:32 2023, max compression
+gzip compressed data, was "autoMMM-0.1.3.tar", last modified: Wed Apr 19 20:31:14 2023, max compression
```

## Comparing `autoMMM-0.1.2.tar` & `autoMMM-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.586598 autoMMM-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.548220 autoMMM-0.1.2/AutoMMM/
--rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.2/AutoMMM/__init__.py
--rw-rw-rw-   0        0        0    11953 2023-04-12 09:27:13.000000 autoMMM-0.1.2/AutoMMM/automodeller.py
--rw-rw-rw-   0        0        0    10898 2023-04-12 09:56:32.581001 autoMMM-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.581001 autoMMM-0.1.2/autoMMM.egg-info/
--rw-rw-rw-   0        0        0    10898 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:56:32.586598 autoMMM-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-04-12 09:55:16.000000 autoMMM-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.390209 autoMMM-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.374582 autoMMM-0.1.3/AutoMMM/
+-rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.3/AutoMMM/__init__.py
+-rw-rw-rw-   0        0        0     2581 2023-04-19 20:24:50.000000 autoMMM-0.1.3/AutoMMM/autoholidays.py
+-rw-rw-rw-   0        0        0    11953 2023-04-18 11:17:07.000000 autoMMM-0.1.3/AutoMMM/automodeller.py
+-rw-rw-rw-   0        0        0    10898 2023-04-19 20:31:14.390209 autoMMM-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.390209 autoMMM-0.1.3/autoMMM.egg-info/
+-rw-rw-rw-   0        0        0    10898 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:31:14.390209 autoMMM-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      995 2023-04-19 20:28:17.000000 autoMMM-0.1.3/setup.py
```

### Comparing `autoMMM-0.1.2/AutoMMM/automodeller.py` & `autoMMM-0.1.3/AutoMMM/automodeller.py`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.2/PKG-INFO` & `autoMMM-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.2/README.md` & `autoMMM-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.2/autoMMM.egg-info/PKG-INFO` & `autoMMM-0.1.3/autoMMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.2/setup.py` & `autoMMM-0.1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoMMM",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
         "statsmodels",
         "matplotlib",
         "openai",
+        "holidays",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

