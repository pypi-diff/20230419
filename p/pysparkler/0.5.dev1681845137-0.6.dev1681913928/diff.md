# Comparing `tmp/pysparkler-0.5.dev1681845137.tar.gz` & `tmp/pysparkler-0.6.dev1681913928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.5.dev1681845137.tar", max compression
+gzip compressed data, was "pysparkler-0.6.dev1681913928.tar", max compression
```

## Comparing `pysparkler-0.5.dev1681845137.tar` & `pysparkler-0.6.dev1681913928.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/README.md
--rw-r--r--   0        0        0     1203 2023-04-18 19:12:18.141053 pysparkler-0.5.dev1681845137/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/__init__.py
--rw-r--r--   0        0        0     4490 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/api.py
--rw-r--r--   0        0        0     6212 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2206 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10450 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4550 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681845137/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/README.md
+-rw-r--r--   0        0        0     1203 2023-04-19 14:18:48.536914 pysparkler-0.6.dev1681913928/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4490 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/api.py
+-rw-r--r--   0        0        0     6212 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10450 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4550 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.6.dev1681913928/PKG-INFO
```

### Comparing `pysparkler-0.5.dev1681845137/README.md` & `pysparkler-0.6.dev1681913928/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pyproject.toml` & `pysparkler-0.6.dev1681913928/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.5.dev1681845137"
+version = "0.6.dev1681913928"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/__init__.py` & `pysparkler-0.6.dev1681913928/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/api.py` & `pysparkler-0.6.dev1681913928/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/base.py` & `pysparkler-0.6.dev1681913928/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/cli.py` & `pysparkler-0.6.dev1681913928/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.6.dev1681913928/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.6.dev1681913928/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.6.dev1681913928/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.6.dev1681913928/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.6.dev1681913928/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681845137/PKG-INFO` & `pysparkler-0.6.dev1681913928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.5.dev1681845137
+Version: 0.6.dev1681913928
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

