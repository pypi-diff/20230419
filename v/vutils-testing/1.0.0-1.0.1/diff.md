# Comparing `tmp/vutils-testing-1.0.0.tar.gz` & `tmp/vutils-testing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-testing-1.0.0.tar", last modified: Tue Apr 18 19:02:12 2023, max compression
+gzip compressed data, was "vutils-testing-1.0.1.tar", last modified: Tue Apr 18 22:34:43 2023, max compression
```

## Comparing `vutils-testing-1.0.0.tar` & `vutils-testing-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/vutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/src/vutils_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.919689 vutils-testing-1.0.1/src/vutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.919689 vutils-testing-1.0.1/src/vutils_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tox.ini
```

### Comparing `vutils-testing-1.0.0/ChangeLog.md` & `vutils-testing-1.0.1/ChangeLog.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## 1.0.1
+
+* Remove unused `pytest-order` from `tox.ini`
+
 ## 1.0.0
 
 * Move the development status to production/stable
 * Code cleanup
 
 ## 0.6.2
```

### Comparing `vutils-testing-1.0.0/LICENSE` & `vutils-testing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/PKG-INFO` & `vutils-testing-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-1.0.0/README.md` & `vutils-testing-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/pyproject.toml` & `vutils-testing-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/setup.cfg` & `vutils-testing-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/src/vutils/testing/__init__.pyi` & `vutils-testing-1.0.1/src/vutils/testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/src/vutils/testing/mock.py` & `vutils-testing-1.0.1/src/vutils/testing/mock.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/src/vutils/testing/testcase.py` & `vutils-testing-1.0.1/src/vutils/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/src/vutils/testing/utils.py` & `vutils-testing-1.0.1/src/vutils/testing/utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/src/vutils_testing.egg-info/PKG-INFO` & `vutils-testing-1.0.1/src/vutils_testing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-1.0.0/src/vutils_testing.egg-info/SOURCES.txt` & `vutils-testing-1.0.1/src/vutils_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tests/unit/test_mock.py` & `vutils-testing-1.0.1/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tests/unit/test_testcase.py` & `vutils-testing-1.0.1/tests/unit/test_testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tests/unit/test_utils.py` & `vutils-testing-1.0.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tests/unit/test_version.py` & `vutils-testing-1.0.1/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tests/unit/utils.py` & `vutils-testing-1.0.1/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.0/tox.ini` & `vutils-testing-1.0.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
     safety
     pytest
     pytest-cov
-    pytest-order
     coveralls
 commands =
     safety check --full-report
     pytest -v --cov=vutils.testing --cov-report=term-missing tests
     {env:COVERALLS_CMD:coveralls --output={envname}-coverage.txt}
 
 [linters]
```

