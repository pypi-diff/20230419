# Comparing `tmp/medviz-0.0.1.tar.gz` & `tmp/medviz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.0.1.tar", last modified: Wed Apr 19 02:20:38 2023, max compression
+gzip compressed data, was "medviz-0.0.2.tar", last modified: Wed Apr 19 15:21:26 2023, max compression
```

## Comparing `medviz-0.0.1.tar` & `medviz-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 02:20:38.611766 medviz-0.0.1/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.0.1/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       26 2023-02-17 19:26:43.000000 medviz-0.0.1/MANIFEST.in
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      480 2023-04-19 02:20:38.611766 medviz-0.0.1/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        9 2023-04-19 00:29:50.000000 medviz-0.0.1/README.rst
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 02:20:38.607766 medviz-0.0.1/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      504 2023-04-03 16:34:22.000000 medviz-0.0.1/medviz/example.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1449 2023-04-19 00:22:28.000000 medviz-0.0.1/medviz/image_masks_axial.py
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 02:20:38.611766 medviz-0.0.1/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      480 2023-04-19 02:20:38.000000 medviz-0.0.1/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      249 2023-04-19 02:20:38.000000 medviz-0.0.1/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-04-19 02:20:38.000000 medviz-0.0.1/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-04-19 02:20:38.000000 medviz-0.0.1/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-04-19 02:20:38.000000 medviz-0.0.1/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      926 2023-04-19 00:28:51.000000 medviz-0.0.1/pyproject.toml
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       38 2023-04-19 02:20:38.611766 medviz-0.0.1/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.0.1/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.0.2/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       26 2023-02-17 19:26:43.000000 medviz-0.0.2/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1471 2023-04-19 15:21:26.911847 medviz-0.0.2/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1000 2023-04-19 15:21:07.000000 medviz-0.0.2/README.rst
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/medviz/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       27 2023-04-19 14:27:12.000000 medviz-0.0.2/medviz/__init__.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1449 2023-04-19 00:22:28.000000 medviz-0.0.2/medviz/image_masks_axial.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1674 2023-04-19 14:44:02.000000 medviz-0.0.2/medviz/layered_plot.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/medviz.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1471 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      273 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       93 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/top_level.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      987 2023-04-19 15:10:51.000000 medviz-0.0.2/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-04-19 15:21:26.911847 medviz-0.0.2/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.0.2/setup.py
```

### Comparing `medviz-0.0.1/LICENSE` & `medviz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-0.0.1/medviz/image_masks_axial.py` & `medviz-0.0.2/medviz/image_masks_axial.py`

 * *Files identical despite different names*

### Comparing `medviz-0.0.1/pyproject.toml` & `medviz-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "medviz"
-authors = [
-  {name = "Mohsen Hariri", email = "mohsen.hariri@case.eud"},
-]
+authors = [{ name = "Mohsen Hariri", email = "mohsen.hariri@case.eud" }]
 description = "Medical Image Visualization Tool 🐍🚀🎉🦕"
-version = "0.0.1"
+version = "0.0.2"
 keywords = ["MRI", "CT"]
-license = {text = "GPL-3.0 License"}
+license = { text = "GPL-3.0 License" }
 # https://github.com/pypi/warehouse/issues/869
 readme = "README.rst"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3.8",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   # "google-api-python-client==2.60.0",
   # "google-auth-oauthlib==0.5.2",
+  "numpy==1.21.2",
   'importlib-metadata; python_version<"3.8"',
+  "matplotlib==3.4.3",
+  "nibabel==3.2.1",
 ]
 
 [tool.setuptools]
 packages = ["medviz"]
 
 [tool.isort]
 profile = "black"
```

