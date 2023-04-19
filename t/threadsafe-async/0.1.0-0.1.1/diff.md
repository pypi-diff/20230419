# Comparing `tmp/threadsafe-async-0.1.0.tar.gz` & `tmp/threadsafe-async-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe-async-0.1.0.tar", last modified: Wed Apr 19 15:44:45 2023, max compression
+gzip compressed data, was "threadsafe-async-0.1.1.tar", last modified: Wed Apr 19 16:06:15 2023, max compression
```

## Comparing `threadsafe-async-0.1.0.tar` & `threadsafe-async-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 15:44:45.189800 threadsafe-async-0.1.0/
--rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.1.0/LICENSE
--rw-r--r--   0 gleero     (501) staff       (20)     3780 2023-04-19 15:44:45.189574 threadsafe-async-0.1.0/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-04-19 15:34:19.000000 threadsafe-async-0.1.0/README.md
--rw-r--r--   0 gleero     (501) staff       (20)     1125 2023-04-19 15:42:33.000000 threadsafe-async-0.1.0/pyproject.toml
--rw-r--r--   0 gleero     (501) staff       (20)       38 2023-04-19 15:44:45.189916 threadsafe-async-0.1.0/setup.cfg
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 15:44:45.185575 threadsafe-async-0.1.0/tests/
--rw-r--r--   0 gleero     (501) staff       (20)     6435 2023-04-18 16:08:11.000000 threadsafe-async-0.1.0/tests/test_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-18 16:08:11.000000 threadsafe-async-0.1.0/tests/test_event.py
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 15:44:45.186982 threadsafe-async-0.1.0/threadsafe_async.egg-info/
--rw-r--r--   0 gleero     (501) staff       (20)     3780 2023-04-19 15:44:45.000000 threadsafe-async-0.1.0/threadsafe_async.egg-info/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)      310 2023-04-19 15:44:45.000000 threadsafe-async-0.1.0/threadsafe_async.egg-info/SOURCES.txt
--rw-r--r--   0 gleero     (501) staff       (20)        1 2023-04-19 15:44:45.000000 threadsafe-async-0.1.0/threadsafe_async.egg-info/dependency_links.txt
--rw-r--r--   0 gleero     (501) staff       (20)        8 2023-04-19 15:44:45.000000 threadsafe-async-0.1.0/threadsafe_async.egg-info/top_level.txt
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 15:44:45.189150 threadsafe-async-0.1.0/tsasync/
--rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.1.0/tsasync/__init__.py
--rw-r--r--   0 gleero     (501) staff       (20)     2813 2023-04-18 15:51:38.000000 threadsafe-async-0.1.0/tsasync/_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     3719 2023-04-18 16:08:49.000000 threadsafe-async-0.1.0/tsasync/_event.py
--rw-r--r--   0 gleero     (501) staff       (20)      392 2023-04-18 15:51:38.000000 threadsafe-async-0.1.0/tsasync/_utils.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.448353 threadsafe-async-0.1.1/
+-rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.1.1/LICENSE
+-rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 16:06:15.448018 threadsafe-async-0.1.1/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-04-19 15:34:19.000000 threadsafe-async-0.1.1/README.md
+-rw-r--r--   0 gleero     (501) staff       (20)     1390 2023-04-19 16:05:43.000000 threadsafe-async-0.1.1/pyproject.toml
+-rw-r--r--   0 gleero     (501) staff       (20)       38 2023-04-19 16:06:15.448519 threadsafe-async-0.1.1/setup.cfg
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.443548 threadsafe-async-0.1.1/tests/
+-rw-r--r--   0 gleero     (501) staff       (20)     6435 2023-04-18 16:08:11.000000 threadsafe-async-0.1.1/tests/test_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-18 16:08:11.000000 threadsafe-async-0.1.1/tests/test_event.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.445459 threadsafe-async-0.1.1/threadsafe_async.egg-info/
+-rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)      349 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/SOURCES.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        1 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/dependency_links.txt
+-rw-r--r--   0 gleero     (501) staff       (20)      163 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/requires.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        8 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/top_level.txt
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.447649 threadsafe-async-0.1.1/tsasync/
+-rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/__init__.py
+-rw-r--r--   0 gleero     (501) staff       (20)     2813 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     3719 2023-04-18 16:08:49.000000 threadsafe-async-0.1.1/tsasync/_event.py
+-rw-r--r--   0 gleero     (501) staff       (20)      392 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/_utils.py
```

### Comparing `threadsafe-async-0.1.0/LICENSE` & `threadsafe-async-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.0/PKG-INFO` & `threadsafe-async-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.0
+Version: 0.1.1
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # Asyncio ↔ Thread Synchronisation library
 
 This library provides synchronisation primitives between **asyncio** and **threads** in Python. It allows you to coordinate the execution of **asyncio coroutines** and **threads** using familiar synchronisation primitives such as `Event` and `Channel`.
 
 ## Installation
```

### Comparing `threadsafe-async-0.1.0/README.md` & `threadsafe-async-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.0/pyproject.toml` & `threadsafe-async-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe-async"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Vladimir Perekladov", email = "gleero@gmail.com"},
 ]
 description = "Thread-safe synchronization primitives"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,14 +14,29 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
+[project.optional-dependencies]
+dev = [
+    "black==23.3.0",
+    "flake8==6.0.0",
+    "Flake8-pyproject==1.2.3",
+    "isort==5.12.0",
+    "twine==4.0.2",
+    "build==0.10.0",
+]
+test = [
+    "pytest==7.3.0",
+    "pytest-asyncio==0.21.0",
+    "pytest-cov==4.0.0",
+]
+
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
```

### Comparing `threadsafe-async-0.1.0/tests/test_channel.py` & `threadsafe-async-0.1.1/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.0/tests/test_event.py` & `threadsafe-async-0.1.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.0/threadsafe_async.egg-info/PKG-INFO` & `threadsafe-async-0.1.1/threadsafe_async.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.0
+Version: 0.1.1
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # Asyncio ↔ Thread Synchronisation library
 
 This library provides synchronisation primitives between **asyncio** and **threads** in Python. It allows you to coordinate the execution of **asyncio coroutines** and **threads** using familiar synchronisation primitives such as `Event` and `Channel`.
 
 ## Installation
```

### Comparing `threadsafe-async-0.1.0/tsasync/_channel.py` & `threadsafe-async-0.1.1/tsasync/_channel.py`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.0/tsasync/_event.py` & `threadsafe-async-0.1.1/tsasync/_event.py`

 * *Files identical despite different names*

