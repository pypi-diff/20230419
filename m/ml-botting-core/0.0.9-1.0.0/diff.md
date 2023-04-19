# Comparing `tmp/ml_botting_core-0.0.9.tar.gz` & `tmp/ml_botting_core-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-0.0.9.tar", last modified: Sun Apr 16 23:17:04 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.0.tar", last modified: Wed Apr 19 00:58:47 2023, max compression
```

## Comparing `ml_botting_core-0.0.9.tar` & `ml_botting_core-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/classification/universal_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/regression/universal_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/universal_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-0.0.9/LICENSE` & `ml_botting_core-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-0.0.9/setup.cfg` & `ml_botting_core-1.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = ml_botting_core
-version = 0.0.9
+version = 1.0.0
 author = Ryan Susman
 author_email = ryansusman@gmail.com
-description = Making ML more accessible to botting apps
+description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls = 
 	Bug Tracker = https://github.com/darkmatter2222/ml_botting_core/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

