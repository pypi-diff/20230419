# Comparing `tmp/fkeycapture-1.0.9.tar.gz` & `tmp/fkeycapture-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fkeycapture-1.0.9.tar", last modified: Wed Mar  9 18:20:45 2022, max compression
+gzip compressed data, was "fkeycapture-1.2.0.tar", last modified: Wed Apr 19 01:52:38 2023, max compression
```

## Comparing `fkeycapture-1.0.9.tar` & `fkeycapture-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-03-09 18:20:45.553225 fkeycapture-1.0.9/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.0.9/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1436 2022-03-09 18:20:45.557225 fkeycapture-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      552 2022-03-09 18:19:53.000000 fkeycapture-1.0.9/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      832 2022-03-09 18:20:45.561225 fkeycapture-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-03-09 18:20:45.553225 fkeycapture-1.0.9/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-03-09 18:20:45.553225 fkeycapture-1.0.9/src/fkeycapture/
--rw-r--r--   0 runner    (1000) runner    (1000)     1944 2022-03-03 15:41:34.000000 fkeycapture-1.0.9/src/fkeycapture/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-03-09 18:20:45.553225 fkeycapture-1.0.9/src/fkeycapture.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1436 2022-03-09 18:20:44.000000 fkeycapture-1.0.9/src/fkeycapture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2022-03-09 18:20:45.000000 fkeycapture-1.0.9/src/fkeycapture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-03-09 18:20:44.000000 fkeycapture-1.0.9/src/fkeycapture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2022-03-09 18:20:44.000000 fkeycapture-1.0.9/src/fkeycapture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:52:38.686519 fkeycapture-1.2.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1542 2023-04-19 01:52:38.686519 fkeycapture-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      650 2023-04-19 01:51:52.000000 fkeycapture-1.2.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      832 2023-04-19 01:52:38.686519 fkeycapture-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:52:38.682519 fkeycapture-1.2.0/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:52:38.686519 fkeycapture-1.2.0/src/fkeycapture/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3409 2023-04-19 01:41:31.000000 fkeycapture-1.2.0/src/fkeycapture/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:52:38.686519 fkeycapture-1.2.0/src/fkeycapture.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1542 2023-04-19 01:52:38.000000 fkeycapture-1.2.0/src/fkeycapture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 01:52:38.000000 fkeycapture-1.2.0/src/fkeycapture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 01:52:38.000000 fkeycapture-1.2.0/src/fkeycapture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 01:52:38.000000 fkeycapture-1.2.0/src/fkeycapture.egg-info/top_level.txt
```

### Comparing `fkeycapture-1.0.9/LICENSE` & `fkeycapture-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fkeycapture-1.0.9/PKG-INFO` & `fkeycapture-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.0.9
+Version: 1.2.0
 Summary: A way to capture keystrokes
 Home-page: https://github.com/Alexander-Maples/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
 Project-URL: replit, https://replit.com/@ALEXANDERMAPLES/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
-        2. Recive key as bytes
+        2. Recive key as bytes (get only)
+        3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
         2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])
-        3. Use getnum like this: getnum([number of numbers to capture])
-        4. Use getchars like this: get([number of keys to capture],[list of chars to capture])
-        ###### v.1.0.9:
-        Fixed README issues in 1.0.8
+        3. Use getnum like this: getnum([number of numbers to capture], [if you want int output, make this `True`])
+        ###### v.1.2.0:
+        Type hinting, docstrings, and int support for getnum!
+        Now includes a help command! Use fkeycapture.help() to recive help.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `fkeycapture-1.0.9/setup.cfg` & `fkeycapture-1.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fkeycapture
-version = 1.0.9
+version = 1.2.0
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = A way to capture keystrokes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Alexander-Maples/fkeycapture
 project_urls =
```

### Comparing `fkeycapture-1.0.9/src/fkeycapture.egg-info/PKG-INFO` & `fkeycapture-1.2.0/src/fkeycapture.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.0.9
+Version: 1.2.0
 Summary: A way to capture keystrokes
 Home-page: https://github.com/Alexander-Maples/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
 Project-URL: replit, https://replit.com/@ALEXANDERMAPLES/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
-        2. Recive key as bytes
+        2. Recive key as bytes (get only)
+        3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
         2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])
-        3. Use getnum like this: getnum([number of numbers to capture])
-        4. Use getchars like this: get([number of keys to capture],[list of chars to capture])
-        ###### v.1.0.9:
-        Fixed README issues in 1.0.8
+        3. Use getnum like this: getnum([number of numbers to capture], [if you want int output, make this `True`])
+        ###### v.1.2.0:
+        Type hinting, docstrings, and int support for getnum!
+        Now includes a help command! Use fkeycapture.help() to recive help.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

