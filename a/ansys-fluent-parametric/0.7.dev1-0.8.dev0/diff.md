# Comparing `tmp/ansys_fluent_parametric-0.7.dev1.tar.gz` & `tmp/ansys_fluent_parametric-0.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_parametric-0.7.dev1.tar", max compression
+gzip compressed data, was "ansys_fluent_parametric-0.8.dev0.tar", max compression
```

## Comparing `ansys_fluent_parametric-0.7.dev1.tar` & `ansys_fluent_parametric-0.8.dev0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-04-13 01:02:43.437745 ansys_fluent_parametric-0.7.dev1/LICENSE
--rw-r--r--   0        0        0     4503 2023-04-13 01:02:43.437745 ansys_fluent_parametric-0.7.dev1/README.rst
--rw-r--r--   0        0        0     1202 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/pyproject.toml
--rw-r--r--   0        0        0    24957 2023-04-13 01:02:43.753766 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/__init__.py
--rw-r--r--   0        0        0     9626 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/local/__init__.py
--rw-r--r--   0        0        0    10653 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/parameters.py
--rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-19 01:17:29.086752 ansys_fluent_parametric-0.8.dev0/LICENSE
+-rw-r--r--   0        0        0     4503 2023-04-19 01:17:29.086752 ansys_fluent_parametric-0.8.dev0/README.rst
+-rw-r--r--   0        0        0     1202 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/pyproject.toml
+-rw-r--r--   0        0        0    24957 2023-04-19 01:17:29.478753 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/__init__.py
+-rw-r--r--   0        0        0     9626 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/local/__init__.py
+-rw-r--r--   0        0        0    10653 2023-04-19 01:17:29.090752 ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/parameters.py
+-rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.8.dev0/PKG-INFO
```

### Comparing `ansys_fluent_parametric-0.7.dev1/LICENSE` & `ansys_fluent_parametric-0.8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev1/README.rst` & `ansys_fluent_parametric-0.8.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev1/pyproject.toml` & `ansys_fluent_parametric-0.8.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-parametric"
-version = "0.7.dev1"
+version = "0.8.dev0"
 description = "A python wrapper for Ansys Fluent parametric workflows"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pyfluent-parametric"
 classifiers = [
```

### Comparing `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/__init__.py` & `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 logger = logging.getLogger("ansys.fluent")
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-_VERSION_INFO = "Build date: April 13, 2023 01:02 UTC ShaID: 5a64f4e"
+_VERSION_INFO = "Build date: April 19, 2023 01:17 UTC ShaID: 5f527ac"
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 def version_info() -> str:
     """Method returning the version of PyFluent being used.
 
     Returns
```

### Comparing `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/local/__init__.py` & `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/local/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/parameters.py` & `ansys_fluent_parametric-0.8.dev0/src/ansys/fluent/parametric/parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev1/PKG-INFO` & `ansys_fluent_parametric-0.8.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-fluent-parametric
-Version: 0.7.dev1
+Version: 0.8.dev0
 Summary: A python wrapper for Ansys Fluent parametric workflows
 Home-page: https://github.com/pyansys/pyfluent-parametric
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
```

