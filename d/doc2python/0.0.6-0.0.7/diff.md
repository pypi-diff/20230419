# Comparing `tmp/doc2python-0.0.6.tar.gz` & `tmp/doc2python-0.0.7.tar.gz`

## Comparing `doc2python-0.0.6.tar` & `doc2python-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 doc2python-0.0.6/config.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.6/src/doc2python/__init__.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 doc2python-0.0.6/src/doc2python/reader.py
--rw-r--r--   0        0        0   333312 2020-02-02 00:00:00.000000 doc2python-0.0.6/tests/test.doc
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 doc2python-0.0.6/tests/test.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 doc2python-0.0.6/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doc2python-0.0.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.6/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 doc2python-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 doc2python-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 doc2python-0.0.7/config.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.7/src/doc2python/__init__.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 doc2python-0.0.7/src/doc2python/reader.py
+-rw-r--r--   0        0        0   333312 2020-02-02 00:00:00.000000 doc2python-0.0.7/tests/test.doc
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 doc2python-0.0.7/tests/test.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 doc2python-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doc2python-0.0.7/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 doc2python-0.0.7/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 doc2python-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 doc2python-0.0.7/PKG-INFO
```

### Comparing `doc2python-0.0.6/src/doc2python/reader.py` & `doc2python-0.0.7/src/doc2python/reader.py`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.6/tests/test.doc` & `doc2python-0.0.7/tests/test.doc`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.6/.gitignore` & `doc2python-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.6/LICENSE` & `doc2python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.6/pyproject.toml` & `doc2python-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "doc2python"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Julian Mecking", email="jmeck2013@gmail.com" },
 ]
 description = "A simple .doc to string converter for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

