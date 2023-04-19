# Comparing `tmp/airgiant-0.0.5.tar.gz` & `tmp/airgiant-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.0.5.tar", last modified: Wed Apr 19 14:49:09 2023, max compression
+gzip compressed data, was "airgiant-0.0.6.tar", last modified: Wed Apr 19 15:01:00 2023, max compression
```

## Comparing `airgiant-0.0.5.tar` & `airgiant-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.541924 airgiant-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-19 14:49:09.540926 airgiant-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.5/README.md
--rw-rw-rw-   0        0        0      595 2023-04-19 14:48:55.000000 airgiant-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 14:49:09.541924 airgiant-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.510681 airgiant-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.515683 airgiant-0.0.5/src/airgiant/
--rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.5/src/airgiant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.537922 airgiant-0.0.5/src/airgiant/state/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:50:53.000000 airgiant-0.0.5/src/airgiant/state/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.539925 airgiant-0.0.5/src/airgiant/zed/
--rw-rw-rw-   0        0        0     3970 2023-04-19 14:46:23.000000 airgiant-0.0.5/src/airgiant/zed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:49:09.536928 airgiant-0.0.5/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-19 14:49:09.000000 airgiant-0.0.5/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-19 14:49:09.000000 airgiant-0.0.5/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:49:09.000000 airgiant-0.0.5/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 14:49:09.000000 airgiant-0.0.5/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.973639 airgiant-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-19 15:01:00.973639 airgiant-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.6/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-19 14:58:59.000000 airgiant-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:01:00.974628 airgiant-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.941447 airgiant-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.945448 airgiant-0.0.6/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.6/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.971633 airgiant-0.0.6/src/airgiant/state/
+-rw-rw-rw-   0        0        0       23 2023-04-19 15:00:35.000000 airgiant-0.0.6/src/airgiant/state/__init__.py
+-rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.0.6/src/airgiant/state/hello.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.972632 airgiant-0.0.6/src/airgiant/zed/
+-rw-rw-rw-   0        0        0     3970 2023-04-19 14:46:23.000000 airgiant-0.0.6/src/airgiant/zed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:01:00.960641 airgiant-0.0.6/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-19 15:01:00.000000 airgiant-0.0.6/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-19 15:01:00.000000 airgiant-0.0.6/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:01:00.000000 airgiant-0.0.6/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 15:01:00.000000 airgiant-0.0.6/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.0.5/LICENSE` & `airgiant-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.5/PKG-INFO` & `airgiant-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.0.5/pyproject.toml` & `airgiant-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.0.5/src/airgiant/zed/__init__.py` & `airgiant-0.0.6/src/airgiant/zed/__init__.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.5/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.0.6/src/airgiant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

