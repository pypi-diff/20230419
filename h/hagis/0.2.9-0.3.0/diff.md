# Comparing `tmp/hagis-0.2.9.tar.gz` & `tmp/hagis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.9.tar", last modified: Tue Apr 18 09:40:37 2023, max compression
+gzip compressed data, was "hagis-0.3.0.tar", last modified: Wed Apr 19 12:51:07 2023, max compression
```

## Comparing `hagis-0.2.9.tar` & `hagis-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.196305 hagis-0.2.9/
--rw-rw-rw-   0        0        0      941 2023-04-18 09:40:37.196305 hagis-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.156885 hagis-0.2.9/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.9/hagis/__init__.py
--rw-rw-rw-   0        0        0     9790 2023-04-18 09:37:19.000000 hagis-0.2.9/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.187409 hagis-0.2.9/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-18 09:40:11.000000 hagis-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 09:40:37.196305 hagis-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.625820 hagis-0.3.0/
+-rw-rw-rw-   0        0        0      941 2023-04-19 12:51:07.617810 hagis-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.583418 hagis-0.3.0/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.0/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13034 2023-04-19 12:48:44.000000 hagis-0.3.0/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:51:07.609763 hagis-0.3.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 12:51:07.000000 hagis-0.3.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-19 12:50:32.000000 hagis-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:51:07.625820 hagis-0.3.0/setup.cfg
```

### Comparing `hagis-0.2.9/PKG-INFO` & `hagis-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.9
+Version: 0.3.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.9/hagis.egg-info/PKG-INFO` & `hagis-0.3.0/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.9
+Version: 0.3.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.9/pyproject.toml` & `hagis-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.9"
+version = "0.3.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

