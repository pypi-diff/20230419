# Comparing `tmp/cgul-0.0.3.tar.gz` & `tmp/cgul-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgul-0.0.3.tar", last modified: Wed Apr 19 15:06:38 2023, max compression
+gzip compressed data, was "cgul-0.0.4.tar", last modified: Wed Apr 19 15:22:52 2023, max compression
```

## Comparing `cgul-0.0.3.tar` & `cgul-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-19 15:06:28.000000 cgul-0.0.3/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-19 15:06:28.000000 cgul-0.0.3/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 15:06:28.000000 cgul-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 15:06:28.000000 cgul-0.0.3/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 15:06:28.000000 cgul-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-19 15:06:28.000000 cgul-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-19 15:06:28.000000 cgul-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 15:06:28.000000 cgul-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:06:38.779760 cgul-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-19 15:06:28.000000 cgul-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul/coordinate_models/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/cads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/cads_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/legacy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/harmonise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/cgul/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/common_unit_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/convert_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/translate_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 15:06:28.000000 cgul-0.0.3/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 15:06:28.000000 cgul-0.0.3/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/installing.md
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 15:06:28.000000 cgul-0.0.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 15:06:28.000000 cgul-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:06:38.779760 cgul-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/_test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_05_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_10_translate_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_15_harmonise.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_20_main_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.352333 cgul-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-19 15:22:30.000000 cgul-0.0.4/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.344333 cgul-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-19 15:22:30.000000 cgul-0.0.4/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 15:22:30.000000 cgul-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 15:22:30.000000 cgul-0.0.4/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 15:22:30.000000 cgul-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-19 15:22:30.000000 cgul-0.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-19 15:22:30.000000 cgul-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 15:22:30.000000 cgul-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:22:52.352333 cgul-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-19 15:22:30.000000 cgul-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/cgul/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/cgul/coordinate_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/coordinate_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/coordinate_models/cads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/coordinate_models/cads_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/coordinate_models/legacy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/harmonise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/cgul/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/tools/common_unit_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/tools/convert_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 15:22:30.000000 cgul-0.0.4/cgul/tools/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-19 15:22:31.000000 cgul-0.0.4/cgul/translate_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/cgul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 15:22:52.000000 cgul-0.0.4/cgul.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 15:22:31.000000 cgul-0.0.4/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 15:22:31.000000 cgul-0.0.4/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.348333 cgul-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.352333 cgul-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.352333 cgul-0.0.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.352333 cgul-0.0.4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/getting_started/installing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/getting_started/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/getting_started/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-19 15:22:31.000000 cgul-0.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 15:22:31.000000 cgul-0.0.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 15:22:31.000000 cgul-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:22:52.352333 cgul-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.352333 cgul-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/_test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/test_05_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/test_10_translate_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/test_15_harmonise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 15:22:31.000000 cgul-0.0.4/tests/test_20_main_commands.py
```

### Comparing `cgul-0.0.3/.cruft.json` & `cgul-0.0.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/.github/workflows/on-push.yml` & `cgul-0.0.4/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/.gitignore` & `cgul-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/.pre-commit-config.yaml` & `cgul-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/LICENSE` & `cgul-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/Makefile` & `cgul-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/PKG-INFO` & `cgul-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgul
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package which will be used to ensure consistent data format when working with Xarray type data objects.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cgul-0.0.3/README.md` & `cgul-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/__init__.py` & `cgul-0.0.4/cgul/__init__.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/cli.py` & `cgul-0.0.4/cgul/cli.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/coordinate_models/__init__.py` & `cgul-0.0.4/cgul/coordinate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/coordinate_models/cads.py` & `cgul-0.0.4/cgul/coordinate_models/cads.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/coordinate_models/cads_coordinates.py` & `cgul-0.0.4/cgul/coordinate_models/cads_coordinates.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/coordinate_models/legacy_options.py` & `cgul-0.0.4/cgul/coordinate_models/legacy_options.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/harmonise.py` & `cgul-0.0.4/cgul/harmonise.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/tools/common_unit_fixes.py` & `cgul-0.0.4/cgul/tools/common_unit_fixes.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/tools/convert_units.py` & `cgul-0.0.4/cgul/tools/convert_units.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/tools/error_handler.py` & `cgul-0.0.4/cgul/tools/error_handler.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/cgul/translate_coords.py` & `cgul-0.0.4/cgul/translate_coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Authors:
 #   Edward Comyn-Platt - ECMWF - https://ecmwf.int
 #   Alessandro Amici - B-Open - https://bopen.eu
 #
 
 import logging
 import typing as T
+import warnings
 from copy import deepcopy
 
 import xarray as xr
 
 from . import coordinate_models, tools
 
 LOG = logging.getLogger(__name__)
@@ -167,15 +168,17 @@
                         c_model,
                         common_unit_names=common_unit_names,
                         convert_units=convert_units,
                         error_mode="warn",
                     )
                 }
             )
-            data = data.rename({coordinate: out_name})
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", category=UserWarning)
+                data = data.rename({coordinate: out_name})
         except Exception as err:
             if error_mode == "ignore":
                 pass
             elif error_mode == "raise":
                 raise RuntimeError(
                     f"Error while translating coordinate: {coordinate}.\n Traceback:\n{err}"
                 )
```

### Comparing `cgul-0.0.3/cgul.egg-info/PKG-INFO` & `cgul-0.0.4/cgul.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgul
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package which will be used to ensure consistent data format when working with Xarray type data objects.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cgul-0.0.3/cgul.egg-info/SOURCES.txt` & `cgul-0.0.4/cgul.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/Makefile` & `cgul-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/conf.py` & `cgul-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/getting_started/installing.md` & `cgul-0.0.4/docs/getting_started/installing.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/getting_started/usage.md` & `cgul-0.0.4/docs/getting_started/usage.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/index.md` & `cgul-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/docs/make.bat` & `cgul-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/pyproject.toml` & `cgul-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/tests/_test_objects.py` & `cgul-0.0.4/tests/_test_objects.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/tests/test_05_tools.py` & `cgul-0.0.4/tests/test_05_tools.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/tests/test_10_translate_coords.py` & `cgul-0.0.4/tests/test_10_translate_coords.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/tests/test_15_harmonise.py` & `cgul-0.0.4/tests/test_15_harmonise.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.3/tests/test_20_main_commands.py` & `cgul-0.0.4/tests/test_20_main_commands.py`

 * *Files identical despite different names*

