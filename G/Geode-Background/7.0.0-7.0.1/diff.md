# Comparing `tmp/Geode_Background-7.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,15 @@
-Zip file size: 2375 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-14 06:36 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-14 06:36 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-Apr-14 06:36 geode_background/surface.py
--rw-rw-rw-  2.0 fat     1102 b- defN 23-Apr-14 06:37 Geode_Background-7.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 06:37 Geode_Background-7.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-14 06:37 Geode_Background-7.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      582 b- defN 23-Apr-14 06:37 Geode_Background-7.0.0.dist-info/RECORD
-7 files, 2290 bytes uncompressed, 1333 bytes compressed:  41.8%
+Zip file size: 2391760 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-19 16:12 geode_background/__init__.py
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-19 16:12 geode_background/solid.py
+-rw-rw-rw-  2.0 fat      203 b- defN 23-Apr-19 16:12 geode_background/surface.py
+-rw-rw-rw-  2.0 fat    61440 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_common.dll
+-rw-rw-rw-  2.0 fat  2379776 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_solid.dll
+-rw-rw-rw-  2.0 fat  2171392 b- defN 23-Apr-19 16:13 geode_background/bin/Geode-Background_surface.dll
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Apr-19 16:13 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1102 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1279 b- defN 23-Apr-19 16:13 Geode_Background-7.0.1.dist-info/RECORD
+13 files, 4991915 bytes uncompressed, 2389578 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -3,20 +3,38 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: Geode_Background-7.0.0.dist-info/METADATA
+Filename: geode_background/bin/Geode-Background_common.dll
 Comment: 
 
-Filename: Geode_Background-7.0.0.dist-info/WHEEL
+Filename: geode_background/bin/Geode-Background_solid.dll
 Comment: 
 
-Filename: Geode_Background-7.0.0.dist-info/top_level.txt
+Filename: geode_background/bin/Geode-Background_surface.dll
 Comment: 
 
-Filename: Geode_Background-7.0.0.dist-info/RECORD
+Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+Comment: 
+
+Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+Comment: 
+
+Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+Comment: 
+
+Filename: Geode_Background-7.0.1.dist-info/METADATA
+Comment: 
+
+Filename: Geode_Background-7.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Background-7.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Background-7.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Geode_Background-7.0.0.dist-info/METADATA` & `Geode_Background-7.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Geode-Background
-Version: 7.0.0
+Version: 7.0.1
 Summary: Geode-solutions OpenGeode module for building background meshes
 Home-page: https://github.com/Geode-solutions/Geode-Background
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==25.*,>=25.0.0)
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+Requires-Dist: geode-common (==25.*,>=25.0.2)
+Requires-Dist: opengeode-core (==14.*,>=14.0.1)
 
 <h1 align="center">BackgroundMesh<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Module to generate a background mesh for OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CD/badge.svg" alt="Deploy Status">
```

