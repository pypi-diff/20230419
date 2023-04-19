# Comparing `tmp/challengerteco-0.1.1.tar.gz` & `tmp/challengerteco-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.1.tar", max compression
+gzip compressed data, was "challengerteco-0.1.2.tar", max compression
```

## Comparing `challengerteco-0.1.1.tar` & `challengerteco-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-12 16:13:11.204502 challengerteco-0.1.1/README.md
--rw-r--r--   0        0        0    81982 2023-04-12 16:15:38.458040 challengerteco-0.1.1/challengerteco/Challenger.py
--rw-r--r--   0        0        0        0 2023-04-12 16:13:11.204502 challengerteco-0.1.1/challengerteco/__init__.py
--rw-r--r--   0        0        0      315 2023-04-12 18:19:30.049199 challengerteco-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.2/README.md
+-rw-r--r--   0        0        0    81982 2023-04-18 13:26:24.964418 challengerteco-0.1.2/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       33 2023-04-19 00:58:36.193973 challengerteco-0.1.2/challengerteco/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-19 00:59:09.790155 challengerteco-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 challengerteco-0.1.2/PKG-INFO
```

### Comparing `challengerteco-0.1.1/challengerteco/Challenger.py` & `challengerteco-0.1.2/challengerteco/Challenger.py`

 * *Files identical despite different names*

### Comparing `challengerteco-0.1.1/PKG-INFO` & `challengerteco-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: challengerteco
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Eduardo Pagnone
 Author-email: mlopsaa@teco.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

