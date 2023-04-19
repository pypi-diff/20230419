# Comparing `tmp/cgul-0.0.2.tar.gz` & `tmp/cgul-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgul-0.0.2.tar", last modified: Tue Jan  3 16:04:14 2023, max compression
+gzip compressed data, was "cgul-0.0.3.tar", last modified: Wed Apr 19 15:06:38 2023, max compression
```

## Comparing `cgul-0.0.2.tar` & `cgul-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.646817 cgul-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-03 16:03:59.000000 cgul-0.0.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.630817 cgul-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.638817 cgul-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-03 16:03:59.000000 cgul-0.0.2/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-01-03 16:03:59.000000 cgul-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-03 16:03:59.000000 cgul-0.0.2/.pre-commit-config-weekly.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-03 16:03:59.000000 cgul-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-03 16:03:59.000000 cgul-0.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-01-03 16:03:59.000000 cgul-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-03 16:03:59.000000 cgul-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-03 16:04:14.646817 cgul-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-01-03 16:03:59.000000 cgul-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.638817 cgul-0.0.2/cgul/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/cgul/coordinate_models/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/coordinate_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/coordinate_models/cads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/coordinate_models/cads_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/coordinate_models/legacy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/harmonise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/cgul/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/tools/common_unit_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/tools/convert_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/tools/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-01-03 16:03:59.000000 cgul-0.0.2/cgul/translate_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/cgul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-03 16:04:14.000000 cgul-0.0.2/cgul.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.642817 cgul-0.0.2/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/getting_started/installing.md
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/getting_started/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/getting_started/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-03 16:03:59.000000 cgul-0.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-03 16:03:59.000000 cgul-0.0.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-03 16:03:59.000000 cgul-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-03 16:04:14.646817 cgul-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:04:14.646817 cgul-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/_test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/test_05_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/test_10_translate_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/test_15_harmonise.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-03 16:03:59.000000 cgul-0.0.2/tests/test_20_main_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-19 15:06:28.000000 cgul-0.0.3/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-19 15:06:28.000000 cgul-0.0.3/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 15:06:28.000000 cgul-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 15:06:28.000000 cgul-0.0.3/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 15:06:28.000000 cgul-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-19 15:06:28.000000 cgul-0.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-19 15:06:28.000000 cgul-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 15:06:28.000000 cgul-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:06:38.779760 cgul-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-19 15:06:28.000000 cgul-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul/coordinate_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/cads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/cads_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/coordinate_models/legacy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/harmonise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/cgul/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/common_unit_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/convert_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/tools/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-19 15:06:28.000000 cgul-0.0.3/cgul/translate_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.775760 cgul-0.0.3/cgul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 15:06:38.000000 cgul-0.0.3/cgul.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 15:06:28.000000 cgul-0.0.3/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 15:06:28.000000 cgul-0.0.3/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/installing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/getting_started/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-19 15:06:28.000000 cgul-0.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 15:06:28.000000 cgul-0.0.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 15:06:28.000000 cgul-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:06:38.779760 cgul-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:06:38.779760 cgul-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/_test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_05_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_10_translate_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_15_harmonise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 15:06:28.000000 cgul-0.0.3/tests/test_20_main_commands.py
```

### Comparing `cgul-0.0.2/.cruft.json` & `cgul-0.0.3/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89375%*

 * *Differences: {"'commit'": "'5e23a683532ab1ca0d6329402ff7a5be099ee8be'",*

 * * "'context'": "{'cookiecutter': {'integration_tests': 'False'}}"}*

```diff
@@ -1,15 +1,16 @@
 {
     "checkout": null,
-    "commit": "3483d72a2b36a34b0f8ae3bc536b00b3270272cb",
+    "commit": "5e23a683532ab1ca0d6329402ff7a5be099ee8be",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "European Union",
             "copyright_year": "2022",
+            "integration_tests": "False",
             "mypy_strict": "False",
             "project_name": "cgul",
             "project_short_description": "Python package which will be used to ensure consistent data format when working with Xarray type data objects.",
             "project_slug": "cgul"
         }
     },
     "directory": null,
```

### Comparing `cgul-0.0.2/.github/workflows/on-push.yml` & `cgul-0.0.3/.github/workflows/on-push.yml`

 * *Files 21% similar despite different names*

```diff
@@ -10,143 +10,187 @@
     branches:
     - main
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
+defaults:
+  run:
+    shell: bash -l {0}
+
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - uses: pre-commit/action@v3.0.0
 
+  combine-environments:
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Install conda-merge
+      run: |
+        $CONDA/bin/python -m pip install conda-merge
+    - name: Combine environments
+      run: |
+        for SUFFIX in ci integration; do
+        $CONDA/bin/conda-merge ci/environment-$SUFFIX.yml environment.yml > ci/combined-environment-$SUFFIX.yml || exit
+        done
+    - name: Archive combined environments
+      uses: actions/upload-artifact@v3
+      with:
+        name: combined-environments
+        path: ci/combined-environment-*.yml
+
   unit-tests:
     name: unit-tests (3.10)
+    needs: combine-environments
     runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
+    - name: Download combined environments
+      uses: actions/download-artifact@v3
+      with:
+        name: combined-environments
+        path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v12
+      uses: mamba-org/provision-with-micromamba@v14
       with:
-        environment-file: environment.yml
+        environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
         channels: conda-forge
         cache-env: true
-        cache-env-key: ubuntu-latest-3.10
         extra-specs: |
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
-        make unit-tests
+        make unit-tests COV_REPORT=xml
 
   type-check:
-    needs: [unit-tests]
+    needs: [combine-environments, unit-tests]
     runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
+    - name: Download combined environments
+      uses: actions/download-artifact@v3
+      with:
+        name: combined-environments
+        path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v12
+      uses: mamba-org/provision-with-micromamba@v14
       with:
-        environment-file: environment.yml
+        environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
         channels: conda-forge
         cache-env: true
-        cache-env-key: ubuntu-latest-3.10
         extra-specs: |
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run code quality checks
       run: |
-        echo type-check not used
+        make type-check
 
-  documentation:
-    needs: [unit-tests]
+  docs-build:
+    needs: [combine-environments, unit-tests]
     runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
+    - name: Download combined environments
+      uses: actions/download-artifact@v3
+      with:
+        name: combined-environments
+        path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v12
+      uses: mamba-org/provision-with-micromamba@v14
       with:
-        environment-file: environment.yml
+        environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
         channels: conda-forge
         cache-env: true
-        cache-env-key: ubuntu-latest-3.10
         extra-specs: |
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Build documentation
       run: |
         make docs-build
 
   integration-tests:
-    needs: [unit-tests]
+    needs: [combine-environments, unit-tests]
+    if: |
+      success() && false
     runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
 
     strategy:
       matrix:
         include:
         - python-version: '3.10'
-          # extra: -minver  # This will need to be uncommented and environment-minver.yml updated if we want to publish on conda
+          extra: -integration
 
     steps:
     - uses: actions/checkout@v3
+    - name: Download combined environments
+      uses: actions/download-artifact@v3
+      with:
+        name: combined-environments
+        path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v12
+      uses: mamba-org/provision-with-micromamba@v14
       with:
-        environment-file: environment${{ matrix.extra }}.yml
+        environment-file: ci/combined-environment${{ matrix.extra }}.yml
         environment-name: DEVELOP${{ matrix.extra }}
         channels: conda-forge
         cache-env: true
-        cache-env-key: ubuntu-latest-${{ matrix.python-version }}${{ matrix.extra }}.
         extra-specs: |
-          python=${{matrix.python-version }}
+          python=${{ matrix.python-version }}
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
-        make unit-tests
+        make unit-tests COV_REPORT=xml
 
   distribution:
     runs-on: ubuntu-latest
-    needs: [integration-tests, type-check, documentation]
+    needs: [unit-tests, type-check, docs-build, integration-tests]
+    if: |
+      always() &&
+      needs.unit-tests.result == 'success' &&
+      needs.type-check.result == 'success' &&
+      needs.docs-build.result == 'success' &&
+      (needs.integration-tests.result == 'success' || needs.integration-tests.result == 'skipped')
 
     steps:
     - uses: actions/checkout@v3
+    - name: Install packages
+      run: |
+        $CONDA/bin/python -m pip install build twine
     - name: Build distributions
       run: |
-        $CONDA/bin/python -m pip install build
         $CONDA/bin/python -m build
+    - name: Check wheels
+      run: |
+        cd dist || exit
+        $CONDA/bin/python -m pip install cgul*.whl || exit
+        $CONDA/bin/python -m twine check * || exit
+        $CONDA/bin/python -c "import cgul"
     - name: Publish a Python distribution to PyPI
       if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `cgul-0.0.2/.gitignore` & `cgul-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/.pre-commit-config.yaml` & `cgul-0.0.3/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-json
   - id: check-yaml
   - id: check-toml
-  # - id: check-added-large-files
+#   - id: check-added-large-files
   - id: debug-statements
   - id: mixed-line-ending
-- repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
-  hooks:
-  - id: isort
 - repo: https://github.com/psf/black
-  rev: 22.6.0
+  rev: 22.12.0
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
-  rev: v0.3.4
+  rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
-- repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.217
   hooks:
-  - id: flake8
+  - id: ruff
+    args: [--fix, --force-exclude]
 - repo: https://github.com/executablebooks/mdformat
-  rev: 0.7.14
+  rev: 0.7.16
   hooks:
   - id: mdformat
-    exclude: cruft-update-template.md
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.4.0
+  rev: v2.5.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
     additional_dependencies: [toml-sort<0.22.0]
-- repo: https://github.com/PyCQA/pydocstyle.git
-  rev: 6.1.1
-  hooks:
-  - id: pydocstyle
-    additional_dependencies: [toml]
-    exclude: tests|docs
```

### Comparing `cgul-0.0.2/LICENSE` & `cgul-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/Makefile` & `cgul-0.0.3/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 unit-tests:
 	python -m pytest -vv --cov=. --cov-report=$(COV_REPORT)
 
 type-check:
 	python -m mypy .
 
 conda-env-update:
+	$(CONDA) env update $(CONDAFLAGS) -f ci/environment-ci.yml
 	$(CONDA) env update $(CONDAFLAGS) -f environment.yml
 
 docker-build:
 	docker build -t $(PROJECT) .
 
 docker-run:
 	docker run --rm -ti -v $(PWD):/srv $(PROJECT)
 
 template-update:
-	pre-commit run --all-files cruft -c .pre-commit-config-weekly.yaml
+	pre-commit run --all-files cruft -c .pre-commit-config-cruft.yaml
 
 docs-build:
 	cd docs && rm -fr _api && make clean && make html
 
 #integration-tests:
 #    python -m pytest -vv --cov=. --cov-report=$(COV_REPORT) tests/integration*.py
 #    python -m pytest -vv --doctest-glob='*.md'
```

### Comparing `cgul-0.0.2/PKG-INFO` & `cgul-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cgul
-Version: 0.0.2
-Summary: Python package which will be used to ensure consistent data format when working with Xarray type data objects.
-License: Apache License 2.0
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cgul
 
 **C**ommon **G**eneralised **U**niform and **L**ight. Python package which will be used to ensure consistent data format when working with Xarray type data objects.
 
 ## Usage
 
 The primary function in cgul is `cgul.translate_coords`. This function operates on an `xarray.Dataset` or
```

### Comparing `cgul-0.0.2/cgul/__init__.py` & `cgul-0.0.3/cgul/__init__.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/cli.py` & `cgul-0.0.3/cgul/cli.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/coordinate_models/__init__.py` & `cgul-0.0.3/cgul/coordinate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/coordinate_models/cads.py` & `cgul-0.0.3/cgul/coordinate_models/cads.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/coordinate_models/cads_coordinates.py` & `cgul-0.0.3/cgul/coordinate_models/cads_coordinates.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/coordinate_models/legacy_options.py` & `cgul-0.0.3/cgul/coordinate_models/legacy_options.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/harmonise.py` & `cgul-0.0.3/cgul/harmonise.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/tools/common_unit_fixes.py` & `cgul-0.0.3/cgul/tools/common_unit_fixes.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/tools/convert_units.py` & `cgul-0.0.3/cgul/tools/convert_units.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/tools/error_handler.py` & `cgul-0.0.3/cgul/tools/error_handler.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul/translate_coords.py` & `cgul-0.0.3/cgul/translate_coords.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/cgul.egg-info/SOURCES.txt` & `cgul-0.0.3/cgul.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 .cruft.json
 .gitignore
-.pre-commit-config-weekly.yaml
+.pre-commit-config-cruft.yaml
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 Makefile
 README.md
 environment.yml
 pyproject.toml
-setup.cfg
 .github/workflows/on-push.yml
 cgul/__init__.py
 cgul/cli.py
 cgul/harmonise.py
 cgul/translate_coords.py
 cgul/version.py
 cgul.egg-info/PKG-INFO
@@ -25,14 +24,16 @@
 cgul/coordinate_models/cads.py
 cgul/coordinate_models/cads_coordinates.py
 cgul/coordinate_models/legacy_options.py
 cgul/tools/__init__.py
 cgul/tools/common_unit_fixes.py
 cgul/tools/convert_units.py
 cgul/tools/error_handler.py
+ci/environment-ci.yml
+ci/environment-integration.yml
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/_static/.gitkeep
 docs/_templates/.gitkeep
 docs/getting_started/installing.md
```

### Comparing `cgul-0.0.2/docs/Makefile` & `cgul-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/docs/conf.py` & `cgul-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/docs/getting_started/installing.md` & `cgul-0.0.3/docs/getting_started/installing.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/docs/getting_started/usage.md` & `cgul-0.0.3/docs/getting_started/usage.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/docs/index.md` & `cgul-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/docs/make.bat` & `cgul-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/tests/_test_objects.py` & `cgul-0.0.3/tests/_test_objects.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/tests/test_05_tools.py` & `cgul-0.0.3/tests/test_05_tools.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/tests/test_10_translate_coords.py` & `cgul-0.0.3/tests/test_10_translate_coords.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/tests/test_15_harmonise.py` & `cgul-0.0.3/tests/test_15_harmonise.py`

 * *Files identical despite different names*

### Comparing `cgul-0.0.2/tests/test_20_main_commands.py` & `cgul-0.0.3/tests/test_20_main_commands.py`

 * *Files identical despite different names*

