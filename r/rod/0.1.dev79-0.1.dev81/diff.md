# Comparing `tmp/rod-0.1.dev79.tar.gz` & `tmp/rod-0.1.dev81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.1.dev79.tar", last modified: Mon Feb 20 11:26:26 2023, max compression
+gzip compressed data, was "rod-0.1.dev81.tar", last modified: Wed Apr 19 08:54:33 2023, max compression
```

## Comparing `rod-0.1.dev79.tar` & `rod-0.1.dev81.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.108695 rod-0.1.dev79/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.092695 rod-0.1.dev79/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.100695 rod-0.1.dev79/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-02-20 11:26:08.000000 rod-0.1.dev79/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-20 11:26:08.000000 rod-0.1.dev79/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-20 11:26:08.000000 rod-0.1.dev79/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-20 11:26:08.000000 rod-0.1.dev79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-02-20 11:26:26.108695 rod-0.1.dev79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-02-20 11:26:08.000000 rod-0.1.dev79/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-20 11:26:08.000000 rod-0.1.dev79/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-20 11:26:26.108695 rod-0.1.dev79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 11:26:08.000000 rod-0.1.dev79/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.092695 rod-0.1.dev79/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.100695 rod-0.1.dev79/src/rod/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.100695 rod-0.1.dev79/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.100695 rod-0.1.dev79/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.104695 rod-0.1.dev79/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.104695 rod-0.1.dev79/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.104695 rod-0.1.dev79/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.108695 rod-0.1.dev79/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-20 11:26:08.000000 rod-0.1.dev79/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:26:26.100695 rod-0.1.dev79/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-02-20 11:26:26.000000 rod-0.1.dev79/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-20 11:26:26.000000 rod-0.1.dev79/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:26:26.000000 rod-0.1.dev79/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:26:25.000000 rod-0.1.dev79/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-20 11:26:26.000000 rod-0.1.dev79/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 11:26:26.000000 rod-0.1.dev79/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.639509 rod-0.1.dev81/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.631509 rod-0.1.dev81/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-19 08:54:15.000000 rod-0.1.dev81/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-19 08:54:15.000000 rod-0.1.dev81/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 08:54:15.000000 rod-0.1.dev81/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-19 08:54:15.000000 rod-0.1.dev81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-19 08:54:33.639509 rod-0.1.dev81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-19 08:54:15.000000 rod-0.1.dev81/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 08:54:15.000000 rod-0.1.dev81/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 08:54:33.639509 rod-0.1.dev81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:54:15.000000 rod-0.1.dev81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/src/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/src/rod/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/builder/primitive_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/builder/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/src/rod/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/kinematics/kinematic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/kinematics/tree_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.639509 rod-0.1.dev81/src/rod/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/sdf/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.639509 rod-0.1.dev81/src/rod/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/tree/directed_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/tree/tree_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.639509 rod-0.1.dev81/src/rod/urdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/urdf/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.639509 rod-0.1.dev81/src/rod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/utils/frame_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/utils/gazebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/utils/resolve_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-19 08:54:15.000000 rod-0.1.dev81/src/rod/utils/resolve_uris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:54:33.635509 rod-0.1.dev81/src/rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 08:54:33.000000 rod-0.1.dev81/src/rod.egg-info/top_level.txt
```

### Comparing `rod-0.1.dev79/.github/workflows/ci_cd.yml` & `rod-0.1.dev81/.github/workflows/ci_cd.yml`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 on:
   push:
   pull_request:
   release:
     types:
       - published
+  schedule:
+    # * is a special character in YAML so you have to quote this string
+    # Execute a "nightly" build at 2 AM UTC
+    - cron:  '0 2 * * *'
 
 jobs:
 
   package:
     name: Package the project
     runs-on: ubuntu-22.04
 
@@ -36,14 +40,15 @@
       - name: Check wheel's abi and platform tags
         run: test $(find dist/ -name *-none-any.whl | wc -l) -gt 0
 
       - name: Run twine check
         run: twine check dist/*
 
       - name: Upload artifacts
+        if: github.event_name != 'schedule'
         uses: actions/upload-artifact@v3
         with:
           path: dist/*
           name: dist
 
   test:
     name: 'Python${{ matrix.python }}@${{ matrix.os }}'
@@ -81,14 +86,15 @@
 
       - name: Import the package
         run: python -c "import rod"
 
   publish:
     name: Publish to PyPI
     needs: test
+    if: github.event_name != 'schedule'
     runs-on: ubuntu-22.04
 
     steps:
 
       - name: Download Python packages
         uses: actions/download-artifact@v3
         with:
```

### Comparing `rod-0.1.dev79/.github/workflows/style.yml` & `rod-0.1.dev81/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/.gitignore` & `rod-0.1.dev81/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/LICENSE` & `rod-0.1.dev81/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/PKG-INFO` & `rod-0.1.dev81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev79
+Version: 0.1.dev81
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev79/README.md` & `rod-0.1.dev81/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/setup.cfg` & `rod-0.1.dev81/setup.cfg`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/__init__.py` & `rod-0.1.dev81/src/rod/__init__.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/builder/primitive_builder.py` & `rod-0.1.dev81/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/builder/primitives.py` & `rod-0.1.dev81/src/rod/builder/primitives.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/kinematics/kinematic_tree.py` & `rod-0.1.dev81/src/rod/kinematics/kinematic_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/kinematics/tree_transforms.py` & `rod-0.1.dev81/src/rod/kinematics/tree_transforms.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/logging.py` & `rod-0.1.dev81/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/pretty_printer.py` & `rod-0.1.dev81/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/common.py` & `rod-0.1.dev81/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/element.py` & `rod-0.1.dev81/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/geometry.py` & `rod-0.1.dev81/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/joint.py` & `rod-0.1.dev81/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/link.py` & `rod-0.1.dev81/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/material.py` & `rod-0.1.dev81/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/model.py` & `rod-0.1.dev81/src/rod/sdf/model.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/physics.py` & `rod-0.1.dev81/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/scene.py` & `rod-0.1.dev81/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/sdf.py` & `rod-0.1.dev81/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/sdf/world.py` & `rod-0.1.dev81/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/tree/directed_tree.py` & `rod-0.1.dev81/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/tree/tree_elements.py` & `rod-0.1.dev81/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/urdf/exporter.py` & `rod-0.1.dev81/src/rod/urdf/exporter.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/utils/frame_convention.py` & `rod-0.1.dev81/src/rod/utils/frame_convention.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/utils/gazebo.py` & `rod-0.1.dev81/src/rod/utils/gazebo.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/utils/resolve_frames.py` & `rod-0.1.dev81/src/rod/utils/resolve_frames.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod/utils/resolve_uris.py` & `rod-0.1.dev81/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.1.dev79/src/rod.egg-info/PKG-INFO` & `rod-0.1.dev81/src/rod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.1.dev79
+Version: 0.1.dev81
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
```

### Comparing `rod-0.1.dev79/src/rod.egg-info/SOURCES.txt` & `rod-0.1.dev81/src/rod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

