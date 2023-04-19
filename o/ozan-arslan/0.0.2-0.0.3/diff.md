# Comparing `tmp/ozan-arslan-0.0.2.tar.gz` & `tmp/ozan-arslan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozan-arslan-0.0.2.tar", last modified: Tue Apr 18 20:42:31 2023, max compression
+gzip compressed data, was "ozan-arslan-0.0.3.tar", last modified: Wed Apr 19 12:39:53 2023, max compression
```

## Comparing `ozan-arslan-0.0.2.tar` & `ozan-arslan-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.325318 ozan-arslan-0.0.2/
--rw-r--r--   0 MTeke1     (502) staff       (20)     1074 2023-04-18 19:57:50.000000 ozan-arslan-0.0.2/LICENSE
--rw-r--r--   0 MTeke1     (502) staff       (20)      936 2023-04-18 20:42:31.325146 ozan-arslan-0.0.2/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      434 2023-04-18 20:42:07.000000 ozan-arslan-0.0.2/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)      576 2023-04-18 20:38:19.000000 ozan-arslan-0.0.2/pyproject.toml
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-18 20:42:31.325385 ozan-arslan-0.0.2/setup.cfg
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.322578 ozan-arslan-0.0.2/src/
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.323742 ozan-arslan-0.0.2/src/ozan/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:15:23.000000 ozan-arslan-0.0.2/src/ozan/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      686 2023-04-18 20:37:03.000000 ozan-arslan-0.0.2/src/ozan/ozan.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.324770 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)      936 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      226 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        5 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/top_level.txt
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 12:39:53.189252 ozan-arslan-0.0.3/
+-rw-r--r--   0 MTeke1     (502) staff       (20)     1074 2023-04-18 19:57:50.000000 ozan-arslan-0.0.3/LICENSE
+-rw-r--r--   0 MTeke1     (502) staff       (20)      941 2023-04-19 12:39:53.189109 ozan-arslan-0.0.3/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      439 2023-04-19 12:38:19.000000 ozan-arslan-0.0.3/README.md
+-rw-r--r--   0 MTeke1     (502) staff       (20)      576 2023-04-19 12:39:30.000000 ozan-arslan-0.0.3/pyproject.toml
+-rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-19 12:39:53.189298 ozan-arslan-0.0.3/setup.cfg
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 12:39:53.187166 ozan-arslan-0.0.3/src/
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 12:39:53.188148 ozan-arslan-0.0.3/src/ozan/
+-rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:15:23.000000 ozan-arslan-0.0.3/src/ozan/__init__.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)      686 2023-04-18 20:37:03.000000 ozan-arslan-0.0.3/src/ozan/ozan.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 12:39:53.188920 ozan-arslan-0.0.3/src/ozan_arslan.egg-info/
+-rw-r--r--   0 MTeke1     (502) staff       (20)      941 2023-04-19 12:39:53.000000 ozan-arslan-0.0.3/src/ozan_arslan.egg-info/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      226 2023-04-19 12:39:53.000000 ozan-arslan-0.0.3/src/ozan_arslan.egg-info/SOURCES.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-19 12:39:53.000000 ozan-arslan-0.0.3/src/ozan_arslan.egg-info/dependency_links.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        5 2023-04-19 12:39:53.000000 ozan-arslan-0.0.3/src/ozan_arslan.egg-info/top_level.txt
```

### Comparing `ozan-arslan-0.0.2/LICENSE` & `ozan-arslan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ozan-arslan-0.0.2/PKG-INFO` & `ozan-arslan-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozan-arslan
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,14 @@
 
 - Python 3.x
 
 ## Usage
 To use the OzanArslan class, simply create an instance of the class and call its run() method:
 
 ```sh
-from ozan import OzanArslan
+from ozan.ozan import OzanArslan
 
 ozan = OzanArslan()
 ozan.run()
 ```
```

### Comparing `ozan-arslan-0.0.2/pyproject.toml` & `ozan-arslan-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ozan-arslan"
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

### Comparing `ozan-arslan-0.0.2/src/ozan/ozan.py` & `ozan-arslan-0.0.3/src/ozan/ozan.py`

 * *Files identical despite different names*

### Comparing `ozan-arslan-0.0.2/src/ozan_arslan.egg-info/PKG-INFO` & `ozan-arslan-0.0.3/src/ozan_arslan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozan-arslan
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,14 @@
 
 - Python 3.x
 
 ## Usage
 To use the OzanArslan class, simply create an instance of the class and call its run() method:
 
 ```sh
-from ozan import OzanArslan
+from ozan.ozan import OzanArslan
 
 ozan = OzanArslan()
 ozan.run()
 ```
```

