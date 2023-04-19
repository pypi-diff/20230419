# Comparing `tmp/large-image-source-vips-1.20.4.dev70.tar.gz` & `tmp/large-image-source-vips-1.20.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.20.4.dev70.tar", last modified: Wed Apr 19 19:51:03 2023, max compression
+gzip compressed data, was "large-image-source-vips-1.20.4.dev8.tar", last modified: Thu Apr  6 14:42:42 2023, max compression
```

## Comparing `large-image-source-vips-1.20.4.dev70.tar` & `large-image-source-vips-1.20.4.dev8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 19:51:03.705285 large-image-source-vips-1.20.4.dev70/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-04-19 19:51:03.705285 large-image-source-vips-1.20.4.dev70/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 19:51:03.705285 large-image-source-vips-1.20.4.dev70/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24089 2023-04-19 19:48:56.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-04-19 19:48:56.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 19:51:03.705285 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-19 19:51:03.000000 large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-19 19:51:03.705285 large-image-source-vips-1.20.4.dev70/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-04-19 19:48:56.000000 large-image-source-vips-1.20.4.dev70/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-06 14:42:41.999750 large-image-source-vips-1.20.4.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-04-06 14:42:41.999750 large-image-source-vips-1.20.4.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-06 14:42:41.995751 large-image-source-vips-1.20.4.dev8/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24089 2023-04-06 14:40:44.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-04-06 14:40:44.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-06 14:42:41.999750 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-06 14:42:41.000000 large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-06 14:42:41.999750 large-image-source-vips-1.20.4.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-04-06 14:40:44.000000 large-image-source-vips-1.20.4.dev8/setup.py
```

### Comparing `large-image-source-vips-1.20.4.dev70/LICENSE` & `large-image-source-vips-1.20.4.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.20.4.dev70/PKG-INFO` & `large-image-source-vips-1.20.4.dev8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.20.4.dev70
+Version: 1.20.4.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.20.4.dev70/README.rst` & `large-image-source-vips-1.20.4.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.20.4.dev70/large_image_source_vips/__init__.py` & `large-image-source-vips-1.20.4.dev8/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.20.4.dev70/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.20.4.dev8/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.20.4.dev70
+Version: 1.20.4.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.20.4.dev70/setup.py` & `large-image-source-vips-1.20.4.dev8/setup.py`

 * *Files identical despite different names*

