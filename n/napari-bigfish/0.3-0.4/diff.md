# Comparing `tmp/napari-bigfish-0.3.tar.gz` & `tmp/napari-bigfish-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bigfish-0.3.tar", last modified: Wed Apr 12 13:15:13 2023, max compression
+gzip compressed data, was "napari-bigfish-0.4.tar", last modified: Wed Apr 19 12:41:07 2023, max compression
```

## Comparing `napari-bigfish-0.3.tar` & `napari-bigfish-0.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.457942 napari-bigfish-0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.457942 napari-bigfish-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-12 13:14:54.000000 napari-bigfish-0.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-12 13:14:54.000000 napari-bigfish-0.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.457942 napari-bigfish-0.3/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 13:14:54.000000 napari-bigfish-0.3/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 13:14:54.000000 napari-bigfish-0.3/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 13:14:54.000000 napari-bigfish-0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-12 13:14:54.000000 napari-bigfish-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 13:14:54.000000 napari-bigfish-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-12 13:15:13.461942 napari-bigfish-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-12 13:14:54.000000 napari-bigfish-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.457942 napari-bigfish-0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/napari_bigfish.array_util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/napari_bigfish.bigfishapp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/napari_bigfish.napari_util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/napari_bigfish.qtutil.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/napari_bigfish.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/user/batch_processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/user/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/user/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/user/spot_detection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 13:14:54.000000 napari-bigfish-0.3/docs/source/user/user_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 13:14:54.000000 napari-bigfish-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-12 13:15:13.461942 napari-bigfish-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.457942 napari-bigfish-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/src/napari_bigfish/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/src/napari_bigfish/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_array_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_bigfishapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_napari_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_qtutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38099 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/array_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/bigfishapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/napari_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-12 13:14:54.000000 napari-bigfish-0.3/src/napari_bigfish/qtutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:15:13.461942 napari-bigfish-0.3/src/napari_bigfish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 13:15:13.000000 napari-bigfish-0.3/src/napari_bigfish.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 13:14:54.000000 napari-bigfish-0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.298748 napari-bigfish-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.286748 napari-bigfish-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.286748 napari-bigfish-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.github/workflows/create_doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.286748 napari-bigfish-0.4/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-19 12:40:46.000000 napari-bigfish-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-19 12:40:46.000000 napari-bigfish-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 12:40:46.000000 napari-bigfish-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-19 12:41:07.298748 napari-bigfish-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-19 12:40:46.000000 napari-bigfish-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.286748 napari-bigfish-0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.290748 napari-bigfish-0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/napari_bigfish.array_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/napari_bigfish.bigfishapp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/napari_bigfish.napari_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/napari_bigfish.qtutil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/napari_bigfish.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.294748 napari-bigfish-0.4/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/user/batch_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/user/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/user/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/user/spot_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 12:40:46.000000 napari-bigfish-0.4/docs/source/user/user_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-19 12:40:46.000000 napari-bigfish-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-19 12:41:07.298748 napari-bigfish-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.286748 napari-bigfish-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.294748 napari-bigfish-0.4/src/napari_bigfish/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.298748 napari-bigfish-0.4/src/napari_bigfish/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_array_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_bigfishapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_napari_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_qtutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38099 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/array_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/bigfishapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/napari_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-19 12:40:46.000000 napari-bigfish-0.4/src/napari_bigfish/qtutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:07.294748 napari-bigfish-0.4/src/napari_bigfish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 12:41:07.000000 napari-bigfish-0.4/src/napari_bigfish.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 12:40:46.000000 napari-bigfish-0.4/tox.ini
```

### Comparing `napari-bigfish-0.3/.github/workflows/test_and_deploy.yml` & `napari-bigfish-0.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/.gitignore` & `napari-bigfish-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/.napari-hub/config.yml` & `napari-bigfish-0.4/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/.pre-commit-config.yaml` & `napari-bigfish-0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/LICENSE` & `napari-bigfish-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/PKG-INFO` & `napari-bigfish-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: napari-bigfish
-Version: 0.3
+Version: 0.4
 Summary: A napari-plugin providing an alternative GUI for Big-FISH. Big-FISH is a python package for the analysis of smFISH images.
 Home-page: https://github.com/MontpellierRessourcesImagerie/napari-bigfish
 Author: Volker Baecker
 Author-email: volker.baecker@mri.cnrs.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
-Project-URL: Documentation, https://github.com/MontpellierRessourcesImagerie/napari-bigfish#README.md
+Project-URL: Documentation, https://montpellierressourcesimagerie.github.io/napari-bigfish/
 Project-URL: Source Code, https://github.com/MontpellierRessourcesImagerie/napari-bigfish
 Project-URL: User Support, https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-bigfish
+ # napari-bigfish
 
 [![License MIT](https://img.shields.io/pypi/l/napari-bigfish.svg?color=green)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-bigfish.svg?color=green)](https://pypi.org/project/napari-bigfish)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-bigfish.svg?color=green)](https://python.org)
 [![tests](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/workflows/tests/badge.svg)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/actions)
 [![codecov](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish/branch/main/graph/badge.svg)](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bigfish)](https://napari-hub.org/plugins/napari-bigfish)
@@ -41,56 +41,47 @@
 The plugin provides a graphical user interface for some of the functionality in Big-FISH. Currently implemented are:
 
  * Gaussian-background subtraction
  * FISH-spot detection with 
 	* Elimination of duplicates
 	* Auto-detection of threshold
 * Dense-region decomposition
-* Dense-region decomposition
 
 The plugin further implements by itself:
 
 * Counting of spots per cell, inside and outside of the nucleus
 * Batch processing on a list of images
 
 
- 
+You can find the user and the api-documentation of napari-bigfish [here](https://montpellierressourcesimagerie.github.io/napari-bigfish/).
  
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
 ## Installation
 
 You can install `napari-bigfish` via [pip]:
 
     pip install napari-bigfish
 
 
-
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 ## License
 
 Distributed under the terms of the [MIT] license,
 "napari-bigfish" is free and open source software
 
+
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

### Comparing `napari-bigfish-0.3/README.md` & `napari-bigfish-0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# napari-bigfish
+ # napari-bigfish
 
 [![License MIT](https://img.shields.io/pypi/l/napari-bigfish.svg?color=green)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-bigfish.svg?color=green)](https://pypi.org/project/napari-bigfish)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-bigfish.svg?color=green)](https://python.org)
 [![tests](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/workflows/tests/badge.svg)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/actions)
 [![codecov](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish/branch/main/graph/badge.svg)](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bigfish)](https://napari-hub.org/plugins/napari-bigfish)
@@ -12,56 +12,47 @@
 The plugin provides a graphical user interface for some of the functionality in Big-FISH. Currently implemented are:
 
  * Gaussian-background subtraction
  * FISH-spot detection with 
 	* Elimination of duplicates
 	* Auto-detection of threshold
 * Dense-region decomposition
-* Dense-region decomposition
 
 The plugin further implements by itself:
 
 * Counting of spots per cell, inside and outside of the nucleus
 * Batch processing on a list of images
 
 
- 
+You can find the user and the api-documentation of napari-bigfish [here](https://montpellierressourcesimagerie.github.io/napari-bigfish/).
  
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
 ## Installation
 
 You can install `napari-bigfish` via [pip]:
 
     pip install napari-bigfish
 
 
-
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 ## License
 
 Distributed under the terms of the [MIT] license,
 "napari-bigfish" is free and open source software
 
+
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

### Comparing `napari-bigfish-0.3/docs/Makefile` & `napari-bigfish-0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/docs/make.bat` & `napari-bigfish-0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/docs/source/conf.py` & `napari-bigfish-0.4/docs/source/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-	'sphinx.ext.autodoc'
+	'sphinx.ext.autodoc',
+	'sphinx.ext.linkcode'
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -52,7 +53,33 @@
 html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+# Options for the linkcode extension
+# ----------------------------------
+# Resolve function
+# This function is used to populate the (source) links in the API
+def linkcode_resolve(domain, info):
+    def find_source():
+        # try to find the file and line number, based on code from numpy:
+        # https://github.com/numpy/numpy/blob/master/doc/source/conf.py#L286
+        obj = sys.modules[info['module']]
+        for part in info['fullname'].split('.'):
+            obj = getattr(obj, part)
+        import inspect
+        import os
+        fn = inspect.getsourcefile(obj)
+        fn = os.path.relpath(fn, start=os.path.abspath('..'))
+        source, lineno = inspect.getsourcelines(obj)
+        return fn, lineno, lineno + len(source) - 1
+
+    if domain != 'py' or not info['module']:
+        return None
+    try:
+        filename = '%s#L%d-L%d' % find_source()
+    except Exception:
+        filename = info['module'].replace('.', '/') + '.py'
+    return "https://github.com/MontpellierRessourcesImagerie/napari-bigfish/blob/main/%s" % (filename)
+
```

### Comparing `napari-bigfish-0.3/docs/source/user/batch_processing.rst` & `napari-bigfish-0.4/docs/source/user/batch_processing.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/docs/source/user/introduction.rst` & `napari-bigfish-0.4/docs/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/docs/source/user/spot_detection.rst` & `napari-bigfish-0.4/docs/source/user/spot_detection.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/setup.cfg` & `napari-bigfish-0.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Image Processing
 project_urls = 
 	Bug Tracker = https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
-	Documentation = https://github.com/MontpellierRessourcesImagerie/napari-bigfish#README.md
+	Documentation = https://montpellierressourcesimagerie.github.io/napari-bigfish/
 	Source Code = https://github.com/MontpellierRessourcesImagerie/napari-bigfish
 	User Support = https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
```

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_sample_data.py` & `napari-bigfish-0.4/src/napari_bigfish/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_tests/test_bigfishapp.py` & `napari-bigfish-0.4/src/napari_bigfish/_tests/test_bigfishapp.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_tests/test_napari_util.py` & `napari-bigfish-0.4/src/napari_bigfish/_tests/test_napari_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_tests/test_qtutil.py` & `napari-bigfish-0.4/src/napari_bigfish/_tests/test_qtutil.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_tests/test_widget.py` & `napari-bigfish-0.4/src/napari_bigfish/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/_widget.py` & `napari-bigfish-0.4/src/napari_bigfish/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/array_util.py` & `napari-bigfish-0.4/src/napari_bigfish/array_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/bigfishapp.py` & `napari-bigfish-0.4/src/napari_bigfish/bigfishapp.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/napari.yaml` & `napari-bigfish-0.4/src/napari_bigfish/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/napari_util.py` & `napari-bigfish-0.4/src/napari_bigfish/napari_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish/qtutil.py` & `napari-bigfish-0.4/src/napari_bigfish/qtutil.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.3/src/napari_bigfish.egg-info/PKG-INFO` & `napari-bigfish-0.4/src/napari_bigfish.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: napari-bigfish
-Version: 0.3
+Version: 0.4
 Summary: A napari-plugin providing an alternative GUI for Big-FISH. Big-FISH is a python package for the analysis of smFISH images.
 Home-page: https://github.com/MontpellierRessourcesImagerie/napari-bigfish
 Author: Volker Baecker
 Author-email: volker.baecker@mri.cnrs.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
-Project-URL: Documentation, https://github.com/MontpellierRessourcesImagerie/napari-bigfish#README.md
+Project-URL: Documentation, https://montpellierressourcesimagerie.github.io/napari-bigfish/
 Project-URL: Source Code, https://github.com/MontpellierRessourcesImagerie/napari-bigfish
 Project-URL: User Support, https://github.com/MontpellierRessourcesImagerie/napari-bigfish/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-bigfish
+ # napari-bigfish
 
 [![License MIT](https://img.shields.io/pypi/l/napari-bigfish.svg?color=green)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-bigfish.svg?color=green)](https://pypi.org/project/napari-bigfish)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-bigfish.svg?color=green)](https://python.org)
 [![tests](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/workflows/tests/badge.svg)](https://github.com/MontpellierRessourcesImagerie/napari-bigfish/actions)
 [![codecov](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish/branch/main/graph/badge.svg)](https://codecov.io/gh/MontpellierRessourcesImagerie/napari-bigfish)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bigfish)](https://napari-hub.org/plugins/napari-bigfish)
@@ -41,56 +41,47 @@
 The plugin provides a graphical user interface for some of the functionality in Big-FISH. Currently implemented are:
 
  * Gaussian-background subtraction
  * FISH-spot detection with 
 	* Elimination of duplicates
 	* Auto-detection of threshold
 * Dense-region decomposition
-* Dense-region decomposition
 
 The plugin further implements by itself:
 
 * Counting of spots per cell, inside and outside of the nucleus
 * Batch processing on a list of images
 
 
- 
+You can find the user and the api-documentation of napari-bigfish [here](https://montpellierressourcesimagerie.github.io/napari-bigfish/).
  
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
 ## Installation
 
 You can install `napari-bigfish` via [pip]:
 
     pip install napari-bigfish
 
 
-
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
+
 ## License
 
 Distributed under the terms of the [MIT] license,
 "napari-bigfish" is free and open source software
 
+
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

### Comparing `napari-bigfish-0.3/src/napari_bigfish.egg-info/SOURCES.txt` & `napari-bigfish-0.4/src/napari_bigfish.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
+.github/workflows/create_doc.yml
 .github/workflows/test_and_deploy.yml
 .napari-hub/DESCRIPTION.md
 .napari-hub/config.yml
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
```

### Comparing `napari-bigfish-0.3/tox.ini` & `napari-bigfish-0.4/tox.ini`

 * *Files identical despite different names*

