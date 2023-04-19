# Comparing `tmp/challengerteco-0.1.2.tar.gz` & `tmp/challengerteco-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.2.tar", max compression
+gzip compressed data, was "challengerteco-0.1.3.tar", max compression
```

## Comparing `challengerteco-0.1.2.tar` & `challengerteco-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.2/README.md
--rw-r--r--   0        0        0    81982 2023-04-18 13:26:24.964418 challengerteco-0.1.2/challengerteco/Challenger.py
--rw-r--r--   0        0        0       33 2023-04-19 00:58:36.193973 challengerteco-0.1.2/challengerteco/__init__.py
--rw-r--r--   0        0        0      315 2023-04-19 00:59:09.790155 challengerteco-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.3/README.md
+-rw-r--r--   0        0        0    81982 2023-04-18 13:26:24.964418 challengerteco-0.1.3/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       37 2023-04-19 10:31:49.657535 challengerteco-0.1.3/challengerteco/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-19 10:31:59.204062 challengerteco-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.3/PKG-INFO
```

### Comparing `challengerteco-0.1.2/challengerteco/Challenger.py` & `challengerteco-0.1.3/challengerteco/Challenger.py`

 * *Files identical despite different names*

### Comparing `challengerteco-0.1.2/PKG-INFO` & `challengerteco-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengerteco
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Eduardo Pagnone
 Author-email: mlopsaa@teco.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

