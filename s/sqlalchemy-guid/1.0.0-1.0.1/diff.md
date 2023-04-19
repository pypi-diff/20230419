# Comparing `tmp/sqlalchemy_guid-1.0.0.tar.gz` & `tmp/sqlalchemy_guid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_guid-1.0.0.tar", max compression
+gzip compressed data, was "sqlalchemy_guid-1.0.1.tar", max compression
```

## Comparing `sqlalchemy_guid-1.0.0.tar` & `sqlalchemy_guid-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-04-19 07:28:34.454205 sqlalchemy_guid-1.0.0/LICENSE
--rw-r--r--   0        0        0       17 2023-04-19 07:28:34.454256 sqlalchemy_guid-1.0.0/README.md
--rw-r--r--   0        0        0      434 2023-04-19 10:08:53.355474 sqlalchemy_guid-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 07:31:42.473424 sqlalchemy_guid-1.0.0/sqlalchemy_guid/__init__.py
--rw-r--r--   0        0        0     1352 2023-04-19 10:12:54.704396 sqlalchemy_guid-1.0.0/sqlalchemy_guid/guid.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 sqlalchemy_guid-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 07:28:34.454205 sqlalchemy_guid-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1401 2023-04-19 11:05:13.948659 sqlalchemy_guid-1.0.1/README.md
+-rw-r--r--   0        0        0      434 2023-04-19 11:06:22.727086 sqlalchemy_guid-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 07:31:42.473424 sqlalchemy_guid-1.0.1/sqlalchemy_guid/__init__.py
+-rw-r--r--   0        0        0     1352 2023-04-19 10:12:54.704396 sqlalchemy_guid-1.0.1/sqlalchemy_guid/guid.py
+-rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 sqlalchemy_guid-1.0.1/PKG-INFO
```

### Comparing `sqlalchemy_guid-1.0.0/LICENSE` & `sqlalchemy_guid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_guid-1.0.0/sqlalchemy_guid/guid.py` & `sqlalchemy_guid-1.0.1/sqlalchemy_guid/guid.py`

 * *Files identical despite different names*

