# Comparing `tmp/Plone-6.0.2.tar.gz` & `tmp/Plone-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Plone-6.0.2.tar", last modified: Thu Feb 23 22:03:38 2023, max compression
+gzip compressed data, was "Plone-6.0.3.tar", last modified: Thu Mar 23 12:24:23 2023, max compression
```

## Comparing `Plone-6.0.2.tar` & `Plone-6.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 22:03:38.755412 Plone-6.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     6507 2023-02-23 22:03:38.000000 Plone-6.0.2/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-02-23 22:03:38.000000 Plone-6.0.2/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-02-23 22:03:38.000000 Plone-6.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14327 2023-02-23 22:03:38.755582 Plone-6.0.2/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 22:03:38.753693 Plone-6.0.2/Plone.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14327 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      324 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-23 22:03:38.000000 Plone-6.0.2/Plone.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6411 2023-02-23 22:03:38.000000 Plone-6.0.2/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 22:03:38.755167 Plone-6.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-02-23 22:03:38.000000 Plone-6.0.2/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-02-23 22:03:38.000000 Plone-6.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-02-23 22:03:38.000000 Plone-6.0.2/docs/LICENSE.ZPL
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-02-23 22:03:38.000000 Plone-6.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1493 2023-02-23 22:03:38.000000 Plone-6.0.2/docs/UPGRADE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1531 2023-02-23 22:03:38.756279 Plone-6.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-02-23 22:03:38.000000 Plone-6.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.234242 Plone-6.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     6573 2023-03-23 12:24:22.000000 Plone-6.0.3/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:24:22.000000 Plone-6.0.3/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-23 12:24:22.000000 Plone-6.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14393 2023-03-23 12:24:23.234400 Plone-6.0.3/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.232150 Plone-6.0.3/Plone.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14393 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6411 2023-03-23 12:24:22.000000 Plone-6.0.3/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.233880 Plone-6.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/CREDITS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.ZPL
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1493 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/UPGRADE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1531 2023-03-23 12:24:23.234995 Plone-6.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-03-23 12:24:22.000000 Plone-6.0.3/setup.py
```

### Comparing `Plone-6.0.2/CHANGES.md` & `Plone-6.0.3/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 6.0.3 (2023-03-23)
+
+Bug fixes:
+
+- Release 6.0.3.
+  [maurits]
+
+
 ## 6.0.2 (2023-02-23)
 
 
 Bug fixes:
 
 - Release 6.0.2.
   [maurits]
```

### Comparing `Plone-6.0.2/PKG-INFO` & `Plone-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.0.2
+Version: 6.0.3
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -173,14 +173,22 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.0.3 (2023-03-23)
+
+Bug fixes:
+
+- Release 6.0.3.
+  [maurits]
+
+
 ## 6.0.2 (2023-02-23)
 
 
 Bug fixes:
 
 - Release 6.0.2.
   [maurits]
```

### Comparing `Plone-6.0.2/Plone.egg-info/PKG-INFO` & `Plone-6.0.3/Plone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.0.2
+Version: 6.0.3
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -173,14 +173,22 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.0.3 (2023-03-23)
+
+Bug fixes:
+
+- Release 6.0.3.
+  [maurits]
+
+
 ## 6.0.2 (2023-02-23)
 
 
 Bug fixes:
 
 - Release 6.0.2.
   [maurits]
```

### Comparing `Plone-6.0.2/README.md` & `Plone-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/docs/CREDITS.txt` & `Plone-6.0.3/docs/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/docs/LICENSE.GPL` & `Plone-6.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/docs/LICENSE.ZPL` & `Plone-6.0.3/docs/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/docs/LICENSE.txt` & `Plone-6.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/docs/UPGRADE.txt` & `Plone-6.0.3/docs/UPGRADE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.2/setup.cfg` & `Plone-6.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 6.0.2
+version = 6.0.3
 name = Plone
 description = The Plone Content Management System
 long_description = file: README.md, CHANGES.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
```

