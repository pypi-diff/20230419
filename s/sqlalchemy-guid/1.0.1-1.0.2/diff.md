# Comparing `tmp/sqlalchemy_guid-1.0.1.tar.gz` & `tmp/sqlalchemy_guid-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_guid-1.0.1.tar", max compression
+gzip compressed data, was "sqlalchemy_guid-1.0.2.tar", max compression
```

## Comparing `sqlalchemy_guid-1.0.1.tar` & `sqlalchemy_guid-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-04-19 07:28:34.454205 sqlalchemy_guid-1.0.1/LICENSE
--rw-r--r--   0        0        0     1401 2023-04-19 11:05:13.948659 sqlalchemy_guid-1.0.1/README.md
--rw-r--r--   0        0        0      434 2023-04-19 11:06:22.727086 sqlalchemy_guid-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 07:31:42.473424 sqlalchemy_guid-1.0.1/sqlalchemy_guid/__init__.py
--rw-r--r--   0        0        0     1352 2023-04-19 10:12:54.704396 sqlalchemy_guid-1.0.1/sqlalchemy_guid/guid.py
--rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 sqlalchemy_guid-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 07:28:34.454205 sqlalchemy_guid-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1401 2023-04-19 11:05:13.948659 sqlalchemy_guid-1.0.2/README.md
+-rw-r--r--   0        0        0      497 2023-04-19 12:46:39.350228 sqlalchemy_guid-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-04-19 12:45:48.039079 sqlalchemy_guid-1.0.2/sqlalchemy_guid/__init__.py
+-rw-r--r--   0        0        0     1352 2023-04-19 10:12:54.704396 sqlalchemy_guid-1.0.2/sqlalchemy_guid/guid.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 sqlalchemy_guid-1.0.2/PKG-INFO
```

### Comparing `sqlalchemy_guid-1.0.1/LICENSE` & `sqlalchemy_guid-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_guid-1.0.1/README.md` & `sqlalchemy_guid-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_guid-1.0.1/sqlalchemy_guid/guid.py` & `sqlalchemy_guid-1.0.2/sqlalchemy_guid/guid.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_guid-1.0.1/PKG-INFO` & `sqlalchemy_guid-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-guid
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 License: MIT
 Author: Alexander Karateev
 Author-email: administrator@gintr1k.space
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlalchemy (>1.0,<3.0)
+Project-URL: Source, https://github.com/gintr1k/sqlalchemy-guid
 Description-Content-Type: text/markdown
 
 # sqlalchemy GUID
 
 This is a simple extension to SQLAlchemy that adds support for UUID with 
 postgresql compatibility to other database dialects.
```

