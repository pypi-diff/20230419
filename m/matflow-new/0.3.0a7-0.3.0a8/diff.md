# Comparing `tmp/matflow_new-0.3.0a7.tar.gz` & `tmp/matflow_new-0.3.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matflow_new-0.3.0a7.tar", max compression
+gzip compressed data, was "matflow_new-0.3.0a8.tar", max compression
```

## Comparing `matflow_new-0.3.0a7.tar` & `matflow_new-0.3.0a8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      560 2022-11-02 13:53:47.152010 matflow_new-0.3.0a7/README.md
--rw-r--r--   0        0        0     1320 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/__init__.py
--rw-r--r--   0        0        0       98 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      211 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/__pyinstaller/hook-matflow.py
--rw-r--r--   0        0        0       24 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/_version.py
--rw-r--r--   0        0        0      228 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/api.py
--rw-r--r--   0        0        0      354 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/cli.py
--rw-r--r--   0        0        0        0 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/data/__init__.py
--rw-r--r--   0        0        0      358 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/data/environments.yaml
--rw-r--r--   0        0        0     1291 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/data/task_schemas.yaml
--rw-r--r--   0        0        0     1247 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/parameters.py
--rw-r--r--   0        0        0      560 2022-11-02 13:53:47.156010 matflow_new-0.3.0a7/matflow/tests/test_cli.py
--rw-r--r--   0        0        0     1402 2022-11-02 13:53:47.160010 matflow_new-0.3.0a7/pyproject.toml
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 matflow_new-0.3.0a7/setup.py
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 matflow_new-0.3.0a7/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-04-19 15:03:40.230501 matflow_new-0.3.0a8/README.md
+-rw-r--r--   0        0        0     1320 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/__pyinstaller/hook-matflow.py
+-rw-r--r--   0        0        0       24 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/_version.py
+-rw-r--r--   0        0        0      228 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/api.py
+-rw-r--r--   0        0        0      354 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/cli.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/data/__init__.py
+-rw-r--r--   0        0        0      358 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/data/environments.yaml
+-rw-r--r--   0        0        0     1291 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/data/task_schemas.yaml
+-rw-r--r--   0        0        0     1247 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/parameters.py
+-rw-r--r--   0        0        0      560 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/matflow/tests/test_cli.py
+-rw-r--r--   0        0        0     1402 2023-04-19 15:03:40.234501 matflow_new-0.3.0a8/pyproject.toml
+-rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 matflow_new-0.3.0a8/PKG-INFO
```

### Comparing `matflow_new-0.3.0a7/README.md` & `matflow_new-0.3.0a8/README.md`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a7/matflow/__init__.py` & `matflow_new-0.3.0a8/matflow/__init__.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a7/matflow/data/task_schemas.yaml` & `matflow_new-0.3.0a8/matflow/data/task_schemas.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a7/matflow/parameters.py` & `matflow_new-0.3.0a8/matflow/parameters.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a7/matflow/tests/test_cli.py` & `matflow_new-0.3.0a8/matflow/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a7/pyproject.toml` & `matflow_new-0.3.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matflow-new"
-version = "0.3.0a7"
+version = "0.3.0a8"
 description = "Computational workflows for materials science"
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "matflow" }
 ]
@@ -43,15 +43,15 @@
 matflow = 'matflow.cli:MatFlow.CLI'
 
 [tool.poetry.plugins.pyinstaller40]
 hook-dirs = "matflow.__pyinstaller:get_hook_dirs"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0a7"
+version = "0.3.0a8"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "matflow/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `matflow_new-0.3.0a7/PKG-INFO` & `matflow_new-0.3.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: matflow-new
-Version: 0.3.0a7
+Version: 0.3.0a8
 Summary: Computational workflows for materials science
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: test
 Requires-Dist: hpcflow-new2 (>=0.2.0a14,<0.3.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0); extra == "test"
+Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
 Description-Content-Type: text/markdown
 
 <img src="https://docs.matflow.io/stable/_static/images/logo-90dpi.png" width="250" alt="MatFlow logo"/>
 
 **Design, run, and share computational materials science workflows**
 
 Documentation: [https://matflow.io/docs](https://matflow.io/docs)
```

