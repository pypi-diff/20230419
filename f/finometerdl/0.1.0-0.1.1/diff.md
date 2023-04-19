# Comparing `tmp/finometerdl-0.1.0.tar.gz` & `tmp/finometerdl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finometerdl-0.1.0.tar", max compression
+gzip compressed data, was "finometerdl-0.1.1.tar", max compression
```

## Comparing `finometerdl-0.1.0.tar` & `finometerdl-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1018 2023-04-19 11:10:23.346852 finometerdl-0.1.0/README.md
--rw-r--r--   0        0        0       26 2023-04-19 11:38:29.823548 finometerdl-0.1.0/finometerdl/__init__.py
--rw-r--r--   0        0        0      888 2023-04-19 11:25:06.220201 finometerdl-0.1.0/finometerdl/logger.py
--rw-r--r--   0        0        0      427 2023-04-19 11:38:12.560215 finometerdl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 finometerdl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-04-19 11:10:23.346852 finometerdl-0.1.1/README.md
+-rw-r--r--   0        0        0       38 2023-04-19 11:42:04.226885 finometerdl-0.1.1/finometerdl/__init__.py
+-rw-r--r--   0        0        0      888 2023-04-19 11:25:06.220201 finometerdl-0.1.1/finometerdl/logger.py
+-rw-r--r--   0        0        0      427 2023-04-19 11:43:10.870220 finometerdl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 finometerdl-0.1.1/PKG-INFO
```

### Comparing `finometerdl-0.1.0/README.md` & `finometerdl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `finometerdl-0.1.0/finometerdl/logger.py` & `finometerdl-0.1.1/finometerdl/logger.py`

 * *Files identical despite different names*

### Comparing `finometerdl-0.1.0/PKG-INFO` & `finometerdl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finometerdl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A data logger for the Finometer Medical Device
 Home-page: https://github.com/abdrysdale/finometer-data-logger
 License: GPL-3.0-or-later
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

