# Comparing `tmp/fkeycapture-1.2.2.tar.gz` & `tmp/fkeycapture-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fkeycapture-1.2.2.tar", last modified: Wed Apr 19 15:37:16 2023, max compression
+gzip compressed data, was "fkeycapture-1.2.3.tar", last modified: Wed Apr 19 15:40:35 2023, max compression
```

## Comparing `fkeycapture-1.2.2.tar` & `fkeycapture-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2607 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1496 2023-04-19 15:32:07.000000 fkeycapture-1.2.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      827 2023-04-19 15:37:16.317670 fkeycapture-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.301670 fkeycapture-1.2.2/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.305670 fkeycapture-1.2.2/src/fkeycapture/
--rw-r--r--   0 runner    (1000) runner    (1000)     3538 2023-04-19 15:04:10.000000 fkeycapture-1.2.2/src/fkeycapture/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/src/fkeycapture.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2607 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2649 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1534 2023-04-19 15:40:03.000000 fkeycapture-1.2.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-04-19 15:40:35.877558 fkeycapture-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/fkeycapture/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3538 2023-04-19 15:04:10.000000 fkeycapture-1.2.3/src/fkeycapture/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:40:35.873558 fkeycapture-1.2.3/src/fkeycapture.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2649 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 15:40:35.000000 fkeycapture-1.2.3/src/fkeycapture.egg-info/top_level.txt
```

### Comparing `fkeycapture-1.2.2/LICENSE` & `fkeycapture-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fkeycapture-1.2.2/PKG-INFO` & `fkeycapture-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.2
+Version: 1.2.3
 Summary: A way to capture keystrokes
-Home-page: https://github.com/Alexander-Maples/fkeycapture
+Home-page: https://github.com/F1repup650/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
+Project-URL: Bug Tracker, https://github.com/F1repup650/fkeycapture/issues
 Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
         2. Recive key as bytes (get only)
         3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
         2. Use get like this: `get(keycount = any int, bytes = True or False)`
         3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
         4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
         #### Change log:
+        ###### v.1.2.3:
+        Project links updated
         ###### v.1.2.2:
         Internal improvements, Changelog improved
         ###### v.1.2.1:
         Changelog issue fixed, removed the help command from 1.0.10
         ###### v.1.2.0
         Type hinting, docstrings, and int support for getnum!
         ###### v.1.0.10
```

### Comparing `fkeycapture-1.2.2/README.md` & `fkeycapture-1.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 3. Recive key as ints  (getnum only)
 #### How to Use:
 1. from fkeycapture import get, getnum, getchars
 2. Use get like this: `get(keycount = any int, bytes = True or False)`
 3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
 4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
 #### Change log:
+###### v.1.2.3:
+Project links updated
 ###### v.1.2.2:
 Internal improvements, Changelog improved
 ###### v.1.2.1:
 Changelog issue fixed, removed the help command from 1.0.10
 ###### v.1.2.0
 Type hinting, docstrings, and int support for getnum!
 ###### v.1.0.10
```

### Comparing `fkeycapture-1.2.2/src/fkeycapture/__init__.py` & `fkeycapture-1.2.3/src/fkeycapture/__init__.py`

 * *Files identical despite different names*

### Comparing `fkeycapture-1.2.2/src/fkeycapture.egg-info/PKG-INFO` & `fkeycapture-1.2.3/src/fkeycapture.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.2
+Version: 1.2.3
 Summary: A way to capture keystrokes
-Home-page: https://github.com/Alexander-Maples/fkeycapture
+Home-page: https://github.com/F1repup650/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
+Project-URL: Bug Tracker, https://github.com/F1repup650/fkeycapture/issues
 Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
         2. Recive key as bytes (get only)
         3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
         2. Use get like this: `get(keycount = any int, bytes = True or False)`
         3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
         4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
         #### Change log:
+        ###### v.1.2.3:
+        Project links updated
         ###### v.1.2.2:
         Internal improvements, Changelog improved
         ###### v.1.2.1:
         Changelog issue fixed, removed the help command from 1.0.10
         ###### v.1.2.0
         Type hinting, docstrings, and int support for getnum!
         ###### v.1.0.10
```

