# Comparing `tmp/airgiant-0.0.2.tar.gz` & `tmp/airgiant-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.0.2.tar", last modified: Tue Apr 18 15:32:20 2023, max compression
+gzip compressed data, was "airgiant-0.0.3.tar", last modified: Wed Apr 19 14:09:52 2023, max compression
```

## Comparing `airgiant-0.0.2.tar` & `airgiant-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 15:32:20.786359 airgiant-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-18 15:32:20.785362 airgiant-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.2/README.md
--rw-rw-rw-   0        0        0      595 2023-04-18 15:27:51.000000 airgiant-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 15:32:20.787358 airgiant-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 15:32:20.769370 airgiant-0.0.2/src/
--rw-rw-rw-   0        0        0      189 2023-04-18 14:28:19.000000 airgiant-0.0.2/src/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:32:20.784361 airgiant-0.0.2/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-18 15:32:20.000000 airgiant-0.0.2/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-04-18 15:32:20.000000 airgiant-0.0.2/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 15:32:20.000000 airgiant-0.0.2/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 15:32:20.000000 airgiant-0.0.2/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.530949 airgiant-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-19 14:09:52.530949 airgiant-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.3/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-19 14:02:37.000000 airgiant-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:09:52.531947 airgiant-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.516952 airgiant-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.520954 airgiant-0.0.3/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.3/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.529950 airgiant-0.0.3/src/airgiant/state/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:50:53.000000 airgiant-0.0.3/src/airgiant/state/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.529950 airgiant-0.0.3/src/airgiant/zed/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:50:53.000000 airgiant-0.0.3/src/airgiant/zed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:09:52.528967 airgiant-0.0.3/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-19 14:09:52.000000 airgiant-0.0.3/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-19 14:09:52.000000 airgiant-0.0.3/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:09:52.000000 airgiant-0.0.3/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 14:09:52.000000 airgiant-0.0.3/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.0.2/LICENSE` & `airgiant-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.2/PKG-INFO` & `airgiant-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.0.2/pyproject.toml` & `airgiant-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.0.2/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.0.3/src/airgiant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

