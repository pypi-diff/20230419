# Comparing `tmp/actipy-2.0.3.post0.tar.gz` & `tmp/actipy-2.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-2.0.3.post0.tar", last modified: Wed Apr 19 17:25:20 2023, max compression
+gzip compressed data, was "actipy-2.0.3.post1.tar", last modified: Wed Apr 19 17:47:17 2023, max compression
```

## Comparing `actipy-2.0.3.post0.tar` & `actipy-2.0.3.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.731829 actipy-2.0.3.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy/
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-19 17:25:10.000000 actipy-2.0.3.post0/src/actipy/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/src/actipy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:25:20.735829 actipy-2.0.3.post0/src/actipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:25:20.000000 actipy-2.0.3.post0/src/actipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 17:25:05.000000 actipy-2.0.3.post0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:47:17.065639 actipy-2.0.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-19 17:47:08.000000 actipy-2.0.3.post1/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 17:47:08.000000 actipy-2.0.3.post1/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-19 17:47:08.000000 actipy-2.0.3.post1/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-19 17:47:08.000000 actipy-2.0.3.post1/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:47:17.069639 actipy-2.0.3.post1/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 17:47:16.000000 actipy-2.0.3.post1/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-19 17:47:17.000000 actipy-2.0.3.post1/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:47:16.000000 actipy-2.0.3.post1/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 17:47:16.000000 actipy-2.0.3.post1/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:47:16.000000 actipy-2.0.3.post1/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 17:47:03.000000 actipy-2.0.3.post1/versioneer.py
```

### Comparing `actipy-2.0.3.post0/LICENSE.md` & `actipy-2.0.3.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/PKG-INFO` & `actipy-2.0.3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.3.post0
+Version: 2.0.3.post1
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
 Download-URL: https://github.com/OxWearables/actipy
```

### Comparing `actipy-2.0.3.post0/README.md` & `actipy-2.0.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/pyproject.toml` & `actipy-2.0.3.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/setup.py` & `actipy-2.0.3.post1/setup.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/ActigraphReader.class` & `actipy-2.0.3.post1/src/actipy/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/ActigraphReader.java` & `actipy-2.0.3.post1/src/actipy/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/AxivityReader.class` & `actipy-2.0.3.post1/src/actipy/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/AxivityReader.java` & `actipy-2.0.3.post1/src/actipy/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/GENEActivReader.class` & `actipy-2.0.3.post1/src/actipy/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/GENEActivReader.java` & `actipy-2.0.3.post1/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/NpyWriter.class` & `actipy-2.0.3.post1/src/actipy/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/NpyWriter.java` & `actipy-2.0.3.post1/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/processing.py` & `actipy-2.0.3.post1/src/actipy/processing.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy/reader.py` & `actipy-2.0.3.post1/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/src/actipy.egg-info/PKG-INFO` & `actipy-2.0.3.post1/src/actipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.0.3.post0
+Version: 2.0.3.post1
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
 Download-URL: https://github.com/OxWearables/actipy
```

### Comparing `actipy-2.0.3.post0/src/actipy.egg-info/SOURCES.txt` & `actipy-2.0.3.post1/src/actipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actipy-2.0.3.post0/versioneer.py` & `actipy-2.0.3.post1/versioneer.py`

 * *Files identical despite different names*

