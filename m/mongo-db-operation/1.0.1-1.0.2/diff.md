# Comparing `tmp/mongo-db-operation-1.0.1.tar.gz` & `tmp/mongo-db-operation-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-db-operation-1.0.1.tar", last modified: Wed Apr 19 14:17:39 2023, max compression
+gzip compressed data, was "mongo-db-operation-1.0.2.tar", last modified: Wed Apr 19 14:30:22 2023, max compression
```

## Comparing `mongo-db-operation-1.0.1.tar` & `mongo-db-operation-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:17:39.288534 mongo-db-operation-1.0.1/
--rw-r--r--   0 MTeke1     (502) staff       (20)    35149 2023-04-19 13:31:34.000000 mongo-db-operation-1.0.1/LICENSE
--rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:17:39.288312 mongo-db-operation-1.0.1/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)     8939 2023-04-19 14:16:52.000000 mongo-db-operation-1.0.1/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)      529 2023-04-19 14:17:19.000000 mongo-db-operation-1.0.1/pyproject.toml
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-19 14:17:39.288582 mongo-db-operation-1.0.1/setup.cfg
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:17:39.285208 mongo-db-operation-1.0.1/src/
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:17:39.287166 mongo-db-operation-1.0.1/src/mongo-db-operation/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-19 13:39:36.000000 mongo-db-operation-1.0.1/src/mongo-db-operation/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      299 2023-04-19 13:46:22.000000 mongo-db-operation-1.0.1/src/mongo-db-operation/environment.py
--rw-r--r--   0 MTeke1     (502) staff       (20)     1958 2023-04-19 14:07:50.000000 mongo-db-operation-1.0.1/src/mongo-db-operation/mongodb_operation.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:17:39.288067 mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:17:39.000000 mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      333 2023-04-19 14:17:39.000000 mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-19 14:17:39.000000 mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)       19 2023-04-19 14:17:39.000000 mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/top_level.txt
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.541299 mongo-db-operation-1.0.2/
+-rw-r--r--   0 MTeke1     (502) staff       (20)    35149 2023-04-19 13:31:34.000000 mongo-db-operation-1.0.2/LICENSE
+-rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:30:22.540949 mongo-db-operation-1.0.2/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)     8939 2023-04-19 14:16:52.000000 mongo-db-operation-1.0.2/README.md
+-rw-r--r--   0 MTeke1     (502) staff       (20)      529 2023-04-19 14:29:56.000000 mongo-db-operation-1.0.2/pyproject.toml
+-rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-19 14:30:22.541412 mongo-db-operation-1.0.2/setup.cfg
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.537249 mongo-db-operation-1.0.2/src/
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.539433 mongo-db-operation-1.0.2/src/mongo_db_operation/
+-rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-19 13:39:36.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/__init__.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)      299 2023-04-19 13:46:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/environment.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)     1958 2023-04-19 14:07:50.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/mongo_client.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.540669 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/
+-rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      328 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/SOURCES.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/dependency_links.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)       19 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/top_level.txt
```

### Comparing `mongo-db-operation-1.0.1/LICENSE` & `mongo-db-operation-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo-db-operation-1.0.1/PKG-INFO` & `mongo-db-operation-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-db-operation
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small package for CRUD operations for Mongo DB
 Author-email: Melih Teke <me@mteke.com>
 Project-URL: Homepage, https://github.com/melihteke/mongo-db-operation
 Project-URL: Bug Tracker, https://github.com/melihteke/mongo-db-operation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mongo-db-operation-1.0.1/README.md` & `mongo-db-operation-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mongo-db-operation-1.0.1/pyproject.toml` & `mongo-db-operation-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mongo-db-operation"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Melih Teke", email="me@mteke.com" },
 ]
 description = "A small package for CRUD operations for Mongo DB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mongo-db-operation-1.0.1/src/mongo-db-operation/mongodb_operation.py` & `mongo-db-operation-1.0.2/src/mongo_db_operation/mongo_client.py`

 * *Files identical despite different names*

### Comparing `mongo-db-operation-1.0.1/src/mongo_db_operation.egg-info/PKG-INFO` & `mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-db-operation
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small package for CRUD operations for Mongo DB
 Author-email: Melih Teke <me@mteke.com>
 Project-URL: Homepage, https://github.com/melihteke/mongo-db-operation
 Project-URL: Bug Tracker, https://github.com/melihteke/mongo-db-operation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

