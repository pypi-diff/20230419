# Comparing `tmp/tiff-inspector-0.1.0.tar.gz` & `tmp/tiff-inspector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiff-inspector-0.1.0.tar", last modified: Tue Apr 18 21:29:48 2023, max compression
+gzip compressed data, was "tiff-inspector-0.1.1.tar", last modified: Tue Apr 18 22:08:41 2023, max compression
```

## Comparing `tiff-inspector-0.1.0.tar` & `tiff-inspector-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 21:29:48.079330 tiff-inspector-0.1.0/
--rw-r--r--   0 jasonw     (502) staff       (20)     1074 2023-03-17 14:39:05.000000 tiff-inspector-0.1.0/LICENSE
--rw-r--r--   0 jasonw     (502) staff       (20)     2527 2023-04-18 21:29:48.078827 tiff-inspector-0.1.0/PKG-INFO
--rw-r--r--   0 jasonw     (502) staff       (20)     1717 2023-04-18 21:29:02.000000 tiff-inspector-0.1.0/README.md
-drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 21:29:48.077733 tiff-inspector-0.1.0/schemas/
--rw-r--r--   0 jasonw     (502) staff       (20)      297 2023-03-20 19:48:52.000000 tiff-inspector-0.1.0/schemas/frame_schema.json
--rw-r--r--   0 jasonw     (502) staff       (20)     2131 2023-03-20 19:30:45.000000 tiff-inspector-0.1.0/schemas/level_schema.json
--rw-r--r--   0 jasonw     (502) staff       (20)     7180 2023-03-20 19:57:04.000000 tiff-inspector-0.1.0/schemas/page_schema.json
--rw-r--r--   0 jasonw     (502) staff       (20)     3934 2023-03-20 19:06:55.000000 tiff-inspector-0.1.0/schemas/series_schema.json
--rw-r--r--   0 jasonw     (502) staff       (20)     1991 2023-03-20 18:46:41.000000 tiff-inspector-0.1.0/schemas/tiff_schema.json
--rw-r--r--   0 jasonw     (502) staff       (20)       38 2023-04-18 21:29:48.079502 tiff-inspector-0.1.0/setup.cfg
--rw-r--r--   0 jasonw     (502) staff       (20)     1286 2023-04-18 21:28:03.000000 tiff-inspector-0.1.0/setup.py
-drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 21:29:48.072125 tiff-inspector-0.1.0/tiff_inspector.egg-info/
--rw-r--r--   0 jasonw     (502) staff       (20)     2527 2023-04-18 21:29:47.000000 tiff-inspector-0.1.0/tiff_inspector.egg-info/PKG-INFO
--rw-r--r--   0 jasonw     (502) staff       (20)      481 2023-04-18 21:29:48.000000 tiff-inspector-0.1.0/tiff_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 jasonw     (502) staff       (20)        1 2023-04-18 21:29:48.000000 tiff-inspector-0.1.0/tiff_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 jasonw     (502) staff       (20)       77 2023-04-18 21:29:48.000000 tiff-inspector-0.1.0/tiff_inspector.egg-info/requires.txt
--rw-r--r--   0 jasonw     (502) staff       (20)       14 2023-04-18 21:29:48.000000 tiff-inspector-0.1.0/tiff_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 21:29:48.073476 tiff-inspector-0.1.0/tiffinspector/
--rw-r--r--   0 jasonw     (502) staff       (20)    14287 2023-04-18 14:53:15.000000 tiff-inspector-0.1.0/tiffinspector/__init__.py
--rw-------   0 jasonw     (502) staff       (20)      160 2023-04-18 15:05:39.000000 tiff-inspector-0.1.0/tiffinspector/_version.py
+drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 22:08:41.943551 tiff-inspector-0.1.1/
+-rw-r--r--   0 jasonw     (502) staff       (20)     1074 2023-03-17 14:39:05.000000 tiff-inspector-0.1.1/LICENSE
+-rw-r--r--   0 jasonw     (502) staff       (20)     2527 2023-04-18 22:08:41.943132 tiff-inspector-0.1.1/PKG-INFO
+-rw-r--r--   0 jasonw     (502) staff       (20)     1717 2023-04-18 21:29:02.000000 tiff-inspector-0.1.1/README.md
+drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 22:08:41.942541 tiff-inspector-0.1.1/schemas/
+-rw-r--r--   0 jasonw     (502) staff       (20)      297 2023-03-20 19:48:52.000000 tiff-inspector-0.1.1/schemas/frame_schema.json
+-rw-r--r--   0 jasonw     (502) staff       (20)     2131 2023-03-20 19:30:45.000000 tiff-inspector-0.1.1/schemas/level_schema.json
+-rw-r--r--   0 jasonw     (502) staff       (20)     7180 2023-03-20 19:57:04.000000 tiff-inspector-0.1.1/schemas/page_schema.json
+-rw-r--r--   0 jasonw     (502) staff       (20)     3934 2023-03-20 19:06:55.000000 tiff-inspector-0.1.1/schemas/series_schema.json
+-rw-r--r--   0 jasonw     (502) staff       (20)     1991 2023-03-20 18:46:41.000000 tiff-inspector-0.1.1/schemas/tiff_schema.json
+-rw-r--r--   0 jasonw     (502) staff       (20)       38 2023-04-18 22:08:41.943672 tiff-inspector-0.1.1/setup.cfg
+-rw-r--r--   0 jasonw     (502) staff       (20)     1305 2023-04-18 22:05:12.000000 tiff-inspector-0.1.1/setup.py
+drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 22:08:41.939703 tiff-inspector-0.1.1/tiff_inspector.egg-info/
+-rw-r--r--   0 jasonw     (502) staff       (20)     2527 2023-04-18 22:08:41.000000 tiff-inspector-0.1.1/tiff_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 jasonw     (502) staff       (20)      481 2023-04-18 22:08:41.000000 tiff-inspector-0.1.1/tiff_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonw     (502) staff       (20)        1 2023-04-18 22:08:41.000000 tiff-inspector-0.1.1/tiff_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonw     (502) staff       (20)       85 2023-04-18 22:08:41.000000 tiff-inspector-0.1.1/tiff_inspector.egg-info/requires.txt
+-rw-r--r--   0 jasonw     (502) staff       (20)       14 2023-04-18 22:08:41.000000 tiff-inspector-0.1.1/tiff_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 jasonw     (502) staff       (20)        0 2023-04-18 22:08:41.940577 tiff-inspector-0.1.1/tiffinspector/
+-rw-r--r--   0 jasonw     (502) staff       (20)    14287 2023-04-18 14:53:15.000000 tiff-inspector-0.1.1/tiffinspector/__init__.py
+-rw-------   0 jasonw     (502) staff       (20)      160 2023-04-18 15:05:39.000000 tiff-inspector-0.1.1/tiffinspector/_version.py
```

### Comparing `tiff-inspector-0.1.0/LICENSE` & `tiff-inspector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/PKG-INFO` & `tiff-inspector-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiff-inspector
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for examining the structure and contents of the metadata contained within tiff files
 Home-page: https://github.com/jason-weirather/tiff-inspector
 Author: Jason L Weirather
 Author-email: jason.weirather@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiff-inspector-0.1.0/README.md` & `tiff-inspector-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/schemas/level_schema.json` & `tiff-inspector-0.1.1/schemas/level_schema.json`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/schemas/page_schema.json` & `tiff-inspector-0.1.1/schemas/page_schema.json`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/schemas/series_schema.json` & `tiff-inspector-0.1.1/schemas/series_schema.json`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/schemas/tiff_schema.json` & `tiff-inspector-0.1.1/schemas/tiff_schema.json`

 * *Files identical despite different names*

### Comparing `tiff-inspector-0.1.0/setup.py` & `tiff-inspector-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tiff-inspector",
-    version="0.1.0",
+    version="0.1.1",
     package_dir={"tiffinspector": "tiffinspector"},
     packages=['tiffinspector'],
     install_requires=[
         "importlib_metadata; python_version<'3.8'",
         "tifffile>=2021.1.1",
-        "imagecodecs"
+        "imagecodecs",
+        "ipython"
     ],
     package_data={
         "tiffinspector":["../schemas/*.json"]
     },
     author="Jason L Weirather",
     author_email="jason.weirather@gmail.com",
     description="A package for examining the structure and contents of the metadata contained within tiff files",
```

### Comparing `tiff-inspector-0.1.0/tiff_inspector.egg-info/PKG-INFO` & `tiff-inspector-0.1.1/tiff_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiff-inspector
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for examining the structure and contents of the metadata contained within tiff files
 Home-page: https://github.com/jason-weirather/tiff-inspector
 Author: Jason L Weirather
 Author-email: jason.weirather@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiff-inspector-0.1.0/tiffinspector/__init__.py` & `tiff-inspector-0.1.1/tiffinspector/__init__.py`

 * *Files identical despite different names*

