# Comparing `tmp/vegafusion-1.2.1.tar.gz` & `tmp/vegafusion-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.2.1.tar", last modified: Thu Apr 13 12:05:12 2023, max compression
+gzip compressed data, was "vegafusion-1.2.2.tar", last modified: Wed Apr 19 12:57:12 2023, max compression
```

## Comparing `vegafusion-1.2.1.tar` & `vegafusion-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 12:03:45.000000 vegafusion-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:05:12.409984 vegafusion-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 12:03:45.000000 vegafusion-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 12:03:45.000000 vegafusion-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-13 12:05:12.409984 vegafusion-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:03:45.000000 vegafusion-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:57:12.444460 vegafusion-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-19 12:56:10.000000 vegafusion-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 12:57:12.444460 vegafusion-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 12:56:10.000000 vegafusion-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-19 12:56:10.000000 vegafusion-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 12:57:12.444460 vegafusion-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:56:10.000000 vegafusion-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:57:12.440460 vegafusion-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-19 12:56:10.000000 vegafusion-1.2.2/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:57:12.444460 vegafusion-1.2.2/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:57:12.444460 vegafusion-1.2.2/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-19 12:56:10.000000 vegafusion-1.2.2/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:57:12.444460 vegafusion-1.2.2/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 12:57:12.000000 vegafusion-1.2.2/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-19 12:57:12.000000 vegafusion-1.2.2/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:57:12.000000 vegafusion-1.2.2/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 12:57:12.000000 vegafusion-1.2.2/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 12:57:12.000000 vegafusion-1.2.2/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.2.1/LICENSE.txt` & `vegafusion-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/PKG-INFO` & `vegafusion-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.1
+Version: 1.2.2
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.1/README.md` & `vegafusion-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/setup.cfg` & `vegafusion-1.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.2.1
+version = 1.2.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.2.1
+	vegafusion-python-embed==1.2.2
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.2.1/tests/test_conext_manager.py` & `vegafusion-1.2.2/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_input_utc.py` & `vegafusion-1.2.2/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_pretransform.py` & `vegafusion-1.2.2/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_pretransform_specs.py` & `vegafusion-1.2.2/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_row_limit.py` & `vegafusion-1.2.2/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_save.py` & `vegafusion-1.2.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_transformed_data.py` & `vegafusion-1.2.2/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/tests/test_transformer.py` & `vegafusion-1.2.2/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/__init__.py` & `vegafusion-1.2.2/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/compilers.py` & `vegafusion-1.2.2/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/connection/__init__.py` & `vegafusion-1.2.2/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/connection/duckdb.py` & `vegafusion-1.2.2/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/evaluation.py` & `vegafusion-1.2.2/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/local_tz.py` & `vegafusion-1.2.2/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/renderer.py` & `vegafusion-1.2.2/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/runtime.py` & `vegafusion-1.2.2/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/save.py` & `vegafusion-1.2.2/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/transformer.py` & `vegafusion-1.2.2/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion/utils.py` & `vegafusion-1.2.2/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.1/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.2.2/vegafusion.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.1
+Version: 1.2.2
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.1/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.2.2/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

