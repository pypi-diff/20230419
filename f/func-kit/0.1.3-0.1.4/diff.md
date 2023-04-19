# Comparing `tmp/func_kit-0.1.3.tar.gz` & `tmp/func_kit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_kit-0.1.3.tar", max compression
+gzip compressed data, was "func_kit-0.1.4.tar", max compression
```

## Comparing `func_kit-0.1.3.tar` & `func_kit-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-17 09:28:53.186709 func_kit-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      106 2023-04-17 09:28:53.186709 func_kit-0.1.3/README.md
--rw-r--r--   0        0        0       75 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/__init__.py
--rw-r--r--   0        0        0     2848 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/cache.py
--rw-r--r--   0        0        0      721 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/cron.py
--rw-r--r--   0        0        0     2801 2023-04-17 09:28:53.186709 func_kit-0.1.3/func_kit/log.py
--rw-r--r--   0        0        0      462 2023-04-17 09:28:53.186709 func_kit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 func_kit-0.1.3/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 func_kit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-19 16:44:52.363725 func_kit-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      106 2023-04-19 16:44:52.363725 func_kit-0.1.4/README.md
+-rw-r--r--   0        0        0       75 2023-04-19 16:44:52.363725 func_kit-0.1.4/func_kit/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-19 16:44:52.363725 func_kit-0.1.4/func_kit/cache.py
+-rw-r--r--   0        0        0      721 2023-04-19 16:44:52.363725 func_kit-0.1.4/func_kit/cron.py
+-rw-r--r--   0        0        0     2913 2023-04-19 16:44:52.363725 func_kit-0.1.4/func_kit/log.py
+-rw-r--r--   0        0        0      462 2023-04-19 16:44:52.363725 func_kit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 func_kit-0.1.4/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 func_kit-0.1.4/PKG-INFO
```

### Comparing `func_kit-0.1.3/LICENSE.txt` & `func_kit-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.3/func_kit/cron.py` & `func_kit-0.1.4/func_kit/cron.py`

 * *Files identical despite different names*

### Comparing `func_kit-0.1.3/func_kit/log.py` & `func_kit-0.1.4/func_kit/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import inspect
 import logging
 import time
 from functools import wraps
 from typing import Callable
 
 logging.basicConfig(
-    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
+    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    level=logging.INFO,
 )
 
 
-def log_decorator(logger=None, log_args=False, log_return=False, log_time=False):
+def log_decorator(
+    logger=None, log_args=False, log_return=False, log_time=False
+):
     """
     Decorator to log function arguments, return value and execution time.
 
     If logger is not provided, the logger will be created from the module name.
     If log_args is True, the function arguments will be logged.
     If log_return is True, the function return value will be logged.
     If log_time is True, the function execution time will be logged.
@@ -37,32 +40,37 @@
                 # Create logger from the function module.
                 logger_obj = logging.getLogger(func.__module__)
             else:
                 logger_obj = logger
             start_time = time.monotonic()
             try:
                 full_path = (
-                    inspect.getmodule(func.__module__).__name__ + "." + func.__name__
+                    inspect.getmodule(func.__module__).__name__
+                    + "."
+                    + func.__name__
                 )
             except AttributeError:
                 full_path = func.__name__
+            if log_args:
+                # Log the function arguments.
+                logger_obj.info(
+                    "[%s] called with args: %s, kwargs: %s",
+                    full_path,
+                    args,
+                    kwargs,
+                )
 
             try:
                 # Call the function and get the result.
                 # If the function raises an exception, log it and re-raise.
                 result = func(*args, **kwargs)
             except Exception as exception:
                 logger_obj.error("[%s]: %s", full_path, exception)
                 raise exception
             end_time = time.monotonic()
-            if log_args:
-                # Log the function arguments.
-                logger_obj.info(
-                    "[%s] called with args: %s, kwargs: %s", full_path, args, kwargs
-                )
             if log_return:
                 #  Log the function return value.
                 logger_obj.info("[%s] returned %s", full_path, result)
             if log_time:
                 # Log the function execution time.
                 logger_obj.info(
                     "[%s] took %.4f seconds to execute",
```

### Comparing `func_kit-0.1.3/setup.py` & `func_kit-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['croniter>=1.3.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'func-kit',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A set of useful function kits.',
     'long_description': '<!-- ABOUT THE PROJECT -->\n## About The Project\n\nThis is a package consists of some useful function kits.\n',
     'author': 'ranguiquan',
     'author_email': 'ranguiquan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `func_kit-0.1.3/PKG-INFO` & `func_kit-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-kit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of useful function kits.
 License: MIT
 Author: ranguiquan
 Author-email: ranguiquan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

