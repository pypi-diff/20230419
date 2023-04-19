# Comparing `tmp/izy-0.4.0.tar.gz` & `tmp/izy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izy-0.4.0.tar", last modified: Mon Apr 17 10:50:53 2023, max compression
+gzip compressed data, was "izy-0.5.0.tar", last modified: Wed Apr 19 12:15:19 2023, max compression
```

## Comparing `izy-0.4.0.tar` & `izy-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.481352 izy-0.4.0/
--rw-rw-rw-   0        0        0     1090 2021-12-30 20:14:03.000000 izy-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       43 2022-01-09 09:22:38.000000 izy-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    16944 2023-04-17 10:50:53.481352 izy-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    16260 2023-03-27 19:08:49.000000 izy-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.450099 izy-0.4.0/izy/
--rw-rw-rw-   0        0        0      173 2023-03-27 10:36:56.000000 izy-0.4.0/izy/__init__.py
--rw-rw-rw-   0        0        0       21 2023-04-17 10:48:55.000000 izy-0.4.0/izy/__version__.py
--rw-rw-rw-   0        0        0     5439 2023-04-16 21:13:45.000000 izy-0.4.0/izy/bidict.py
--rw-rw-rw-   0        0        0    13199 2023-04-17 10:36:24.000000 izy-0.4.0/izy/decorators.py
--rw-rw-rw-   0        0        0     4722 2023-03-27 10:17:48.000000 izy-0.4.0/izy/discovery.py
--rw-rw-rw-   0        0        0     3765 2023-03-27 11:37:14.000000 izy-0.4.0/izy/misc.py
--rw-rw-rw-   0        0        0    19975 2023-03-27 11:28:22.000000 izy-0.4.0/izy/path.py
--rw-rw-rw-   0        0        0     8709 2023-04-10 22:32:43.000000 izy-0.4.0/izy/regex.py
--rw-rw-rw-   0        0        0     8697 2023-03-27 11:36:43.000000 izy-0.4.0/izy/scorer.py
--rw-rw-rw-   0        0        0     3575 2023-03-27 11:35:55.000000 izy-0.4.0/izy/sorting.py
--rw-rw-rw-   0        0        0     9246 2023-03-27 11:36:24.000000 izy-0.4.0/izy/table.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.481352 izy-0.4.0/izy.egg-info/
--rw-rw-rw-   0        0        0    16944 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:50:53.481352 izy-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     3908 2023-04-17 10:48:55.000000 izy-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:15:19.018423 izy-0.5.0/
+-rw-rw-rw-   0        0        0     1090 2021-12-30 20:14:03.000000 izy-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2022-01-09 09:22:38.000000 izy-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    16944 2023-04-19 12:15:19.015420 izy-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16260 2023-03-27 19:08:49.000000 izy-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:15:18.962687 izy-0.5.0/izy/
+-rw-rw-rw-   0        0        0      173 2023-03-27 10:36:56.000000 izy-0.5.0/izy/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-04-19 12:15:09.000000 izy-0.5.0/izy/__version__.py
+-rw-rw-rw-   0        0        0     5439 2023-04-16 21:13:45.000000 izy-0.5.0/izy/bidict.py
+-rw-rw-rw-   0        0        0    13235 2023-04-19 12:14:07.000000 izy-0.5.0/izy/decorators.py
+-rw-rw-rw-   0        0        0     4722 2023-03-27 10:17:48.000000 izy-0.5.0/izy/discovery.py
+-rw-rw-rw-   0        0        0     3765 2023-03-27 11:37:14.000000 izy-0.5.0/izy/misc.py
+-rw-rw-rw-   0        0        0    19975 2023-03-27 11:28:22.000000 izy-0.5.0/izy/path.py
+-rw-rw-rw-   0        0        0     8709 2023-04-10 22:32:43.000000 izy-0.5.0/izy/regex.py
+-rw-rw-rw-   0        0        0     8697 2023-03-27 11:36:43.000000 izy-0.5.0/izy/scorer.py
+-rw-rw-rw-   0        0        0     3575 2023-03-27 11:35:55.000000 izy-0.5.0/izy/sorting.py
+-rw-rw-rw-   0        0        0     9246 2023-03-27 11:36:24.000000 izy-0.5.0/izy/table.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:15:19.013422 izy-0.5.0/izy.egg-info/
+-rw-rw-rw-   0        0        0    16944 2023-04-19 12:15:18.000000 izy-0.5.0/izy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-04-19 12:15:18.000000 izy-0.5.0/izy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:15:18.000000 izy-0.5.0/izy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 12:15:18.000000 izy-0.5.0/izy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:15:19.018423 izy-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3908 2023-04-19 12:15:09.000000 izy-0.5.0/setup.py
```

### Comparing `izy-0.4.0/LICENSE` & `izy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/PKG-INFO` & `izy-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python functions and classes that make it even easier!
 Home-page: https://github.com/tabasy/izy
 Author: Mohsen Tabasi
 Author-email: m.tabasy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `izy-0.4.0/README.md` & `izy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/bidict.py` & `izy-0.5.0/izy/bidict.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/decorators.py` & `izy-0.5.0/izy/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from .misc import setup_logger
 except:
     def setup_logger(): pass
 
 __all__ = [
     'record_stats', 'register', 'get_function', 'get_class',
     'preprocess', 'postprocess', 'run_before', 'run_after', 
-    'retry', 'thread', 'thread_in_pool', 'timeout',
+    'retries', 'thread', 'thread_in_pool', 'timeout',
     'returns', 'yields', 'fix_this',
     'ignores', 'fallsback', 'returns_time', 'logs',
 ]
 
 
 @dataclass
 class UsageStats:
@@ -75,14 +75,16 @@
         wrapper.stats = stats
         return wrapper
     return decorator
 
 
 # registry --------------------------------------------------------------------
 
+# TODO: make it class-based
+
 function_registry = {}
 class_registry = {}
 
 
 def get_function(name):
     return function_registry[name]
 
@@ -96,16 +98,18 @@
         if isclass(func_or_class):
             class_registry[key] = func_or_class
         else:
             function_registry[key] = func_or_class
         return func_or_class
     return decorator
 
+
 # chain/pipeline --------------------------------------------------------------------
 
+
 def chain_functions(*funcs):
     def chained(*args, **kwargs):
         output = funcs[0](*args, **kwargs)
         for func in funcs[1:]:
             output = func(output)
         return output
     return chained
@@ -415,15 +419,15 @@
                     return fallback
 
         return wrapper
     return decorator
 
 
 ignores = ignore
-fallsbacks = fallback
+fallsback = fallback
 
 
 if __name__ == '__main__':
 
     @returns('x', 'y')
     def myfunction(x):
         return x, x+1
```

### Comparing `izy-0.4.0/izy/discovery.py` & `izy-0.5.0/izy/discovery.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/misc.py` & `izy-0.5.0/izy/misc.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/path.py` & `izy-0.5.0/izy/path.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/regex.py` & `izy-0.5.0/izy/regex.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/scorer.py` & `izy-0.5.0/izy/scorer.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/sorting.py` & `izy-0.5.0/izy/sorting.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy/table.py` & `izy-0.5.0/izy/table.py`

 * *Files identical despite different names*

### Comparing `izy-0.4.0/izy.egg-info/PKG-INFO` & `izy-0.5.0/izy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python functions and classes that make it even easier!
 Home-page: https://github.com/tabasy/izy
 Author: Mohsen Tabasi
 Author-email: m.tabasy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `izy-0.4.0/setup.py` & `izy-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'izy'
 DESCRIPTION = 'Python functions and classes that make it even easier!'
 URL = 'https://github.com/tabasy/izy'
 EMAIL = 'm.tabasy@gmail.com'
 AUTHOR = 'Mohsen Tabasi'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

