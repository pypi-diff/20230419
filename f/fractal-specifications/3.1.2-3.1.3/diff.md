# Comparing `tmp/fractal-specifications-3.1.2.tar.gz` & `tmp/fractal-specifications-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-specifications-3.1.2.tar", last modified: Tue Apr 18 13:39:02 2023, max compression
+gzip compressed data, was "fractal-specifications-3.1.3.tar", last modified: Wed Apr 19 15:19:22 2023, max compression
```

## Comparing `fractal-specifications-3.1.2.tar` & `fractal-specifications-3.1.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0      187 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.coveragerc
--rw-r--r--   0        0        0      100 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.flake8
--rw-r--r--   0        0        0      965 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.gitignore
--rw-r--r--   0        0        0      161 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/LICENSE
--rw-r--r--   0        0        0     1436 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/Makefile
--rw-r--r--   0        0        0    14207 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/README.md
--rw-r--r--   0        0        0      780 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/align_version.py
--rw-r--r--   0        0        0      157 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2679 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3167 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1599 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     4878 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/generic/dsl_parser.py
--rw-r--r--   0        0        0     4222 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     6567 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0     1713 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/setup.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.257090 fractal-specifications-3.1.2/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/generic/test_collections.py
--rw-r--r--   0        0        0     3807 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/generic/test_operators.py
--rw-r--r--   0        0        0     5624 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     3966 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tests/generic/test_specification.py
--rw-r--r--   0        0        0      705 2023-04-18 13:38:47.261090 fractal-specifications-3.1.2/tox.ini
--rw-r--r--   0        0        0    15099 1970-01-01 00:00:00.000000 fractal-specifications-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.flake8
+-rw-r--r--   0        0        0      965 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.isort.cfg
+-rw-r--r--   0        0        0     1716 2023-04-19 15:19:01.639654 fractal-specifications-3.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/Makefile
+-rw-r--r--   0        0        0    14207 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/README.md
+-rw-r--r--   0        0        0      780 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/align_version.py
+-rw-r--r--   0        0        0      157 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2679 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3167 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4878 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4222 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6567 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0       77 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/fractal_specifications/py.typed
+-rw-r--r--   0        0        0     1713 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/setup.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3807 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5624 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     3966 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      705 2023-04-19 15:19:01.643657 fractal-specifications-3.1.3/tox.ini
+-rw-r--r--   0        0        0    15099 1970-01-01 00:00:00.000000 fractal-specifications-3.1.3/PKG-INFO
```

### Comparing `fractal-specifications-3.1.2/.github/workflows/build.yml` & `fractal-specifications-3.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/.github/workflows/publish.yml` & `fractal-specifications-3.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/.gitignore` & `fractal-specifications-3.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/.pre-commit-config.yaml` & `fractal-specifications-3.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/LICENSE` & `fractal-specifications-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/Makefile` & `fractal-specifications-3.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/README.md` & `fractal-specifications-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/align_version.py` & `fractal-specifications-3.1.3/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/django/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/django/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/mongo/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/mongo/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/pandas/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/pandas/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal-specifications-3.1.3/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/generic/collections.py` & `fractal-specifications-3.1.3/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/generic/dsl_parser.py` & `fractal-specifications-3.1.3/fractal_specifications/generic/dsl_parser.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/generic/operators.py` & `fractal-specifications-3.1.3/fractal_specifications/generic/operators.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/fractal_specifications/generic/specification.py` & `fractal-specifications-3.1.3/fractal_specifications/generic/specification.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/pyproject.toml` & `fractal-specifications-3.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "3.1.2"
+version = "3.1.3"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [tool.poetry.dependencies]
 lark = "*"
 
 [build-system]
```

### Comparing `fractal-specifications-3.1.2/tests/contrib/django/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/contrib/elasticsearch/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/contrib/google_firestore/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/contrib/mongo/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/contrib/pandas/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/contrib/sqlalchemy/test_specifications.py` & `fractal-specifications-3.1.3/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/fixtures/specifications.py` & `fractal-specifications-3.1.3/tests/fixtures/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/generic/test_collections.py` & `fractal-specifications-3.1.3/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/generic/test_operators.py` & `fractal-specifications-3.1.3/tests/generic/test_operators.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/generic/test_serialization.py` & `fractal-specifications-3.1.3/tests/generic/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tests/generic/test_specification.py` & `fractal-specifications-3.1.3/tests/generic/test_specification.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/tox.ini` & `fractal-specifications-3.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.2/PKG-INFO` & `fractal-specifications-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 3.1.2
+Version: 3.1.3
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

