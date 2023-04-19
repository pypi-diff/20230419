# Comparing `tmp/tinote-1.2.0.tar.gz` & `tmp/tinote-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.2.0.tar", last modified: Wed Apr 19 04:02:16 2023, max compression
+gzip compressed data, was "tinote-1.2.1.tar", last modified: Wed Apr 19 20:03:18 2023, max compression
```

## Comparing `tinote-1.2.0.tar` & `tinote-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-19 04:02:16.224665 tinote-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-19 04:02:05.000000 tinote-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 04:02:16.224665 tinote-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-19 04:02:05.000000 tinote-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/tinote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/tinote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:03:18.918244 tinote-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 20:03:04.000000 tinote-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-19 20:03:18.918244 tinote-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-19 20:03:04.000000 tinote-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:03:18.918244 tinote-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-19 20:03:04.000000 tinote-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:03:18.914244 tinote-1.2.1/tinote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:03:04.000000 tinote-1.2.1/tinote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-19 20:03:04.000000 tinote-1.2.1/tinote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-19 20:03:04.000000 tinote-1.2.1/tinote/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:03:18.914244 tinote-1.2.1/tinote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-19 20:03:18.000000 tinote-1.2.1/tinote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 20:03:18.000000 tinote-1.2.1/tinote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:03:18.000000 tinote-1.2.1/tinote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 20:03:18.000000 tinote-1.2.1/tinote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 20:03:18.000000 tinote-1.2.1/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.2.0/PKG-INFO` & `tinote-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.2.0
+Version: 1.2.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
 ## No Thought Left Behind.
 
 #### Huh, that's a pretty good idea. I should write that down.
```

### Comparing `tinote-1.2.0/README.md` & `tinote-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tinote-1.2.0/setup.py` & `tinote-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tinote-1.2.0/tinote/main.py` & `tinote-1.2.1/tinote/main.py`

 * *Files identical despite different names*

### Comparing `tinote-1.2.0/tinote/update.py` & `tinote-1.2.1/tinote/update.py`

 * *Files identical despite different names*

### Comparing `tinote-1.2.0/tinote.egg-info/PKG-INFO` & `tinote-1.2.1/tinote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.2.0
+Version: 1.2.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
 ## No Thought Left Behind.
 
 #### Huh, that's a pretty good idea. I should write that down.
```

