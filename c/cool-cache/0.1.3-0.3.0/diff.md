# Comparing `tmp/cool_cache-0.1.3.tar.gz` & `tmp/cool_cache-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_cache-0.1.3.tar", last modified: Wed Nov  9 17:42:41 2022, max compression
+gzip compressed data, was "cool_cache-0.3.0.tar", last modified: Wed Apr 19 04:11:24 2023, max compression
```

## Comparing `cool_cache-0.1.3.tar` & `cool_cache-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-09 17:42:41.684194 cool_cache-0.1.3/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3194 2022-11-09 17:42:41.684071 cool_cache-0.1.3/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-09 17:42:41.683224 cool_cache-0.1.3/cool_cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4568 2022-11-09 15:26:28.000000 cool_cache-0.1.3/cool_cache/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-09 17:42:41.683903 cool_cache-0.1.3/cool_cache.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3194 2022-11-09 17:42:41.000000 cool_cache-0.1.3/cool_cache.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2022-11-09 17:42:41.000000 cool_cache-0.1.3/cool_cache.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-09 17:42:41.000000 cool_cache-0.1.3/cool_cache.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       57 2022-11-09 17:42:41.000000 cool_cache-0.1.3/cool_cache.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2022-11-09 17:42:41.000000 cool_cache-0.1.3/cool_cache.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-09 17:42:41.684239 cool_cache-0.1.3/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1208 2022-11-09 13:57:56.000000 cool_cache-0.1.3/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.466011 cool_cache-0.3.0/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-19 04:11:24.465872 cool_cache-0.3.0/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.464931 cool_cache-0.3.0/cool_cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7189 2023-04-19 04:10:44.000000 cool_cache-0.3.0/cool_cache/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-19 04:11:24.465706 cool_cache-0.3.0/cool_cache.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       57 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-04-19 04:11:24.000000 cool_cache-0.3.0/cool_cache.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-19 04:11:24.466052 cool_cache-0.3.0/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1208 2022-11-09 13:57:56.000000 cool_cache-0.3.0/setup.py
```

### Comparing `cool_cache-0.1.3/PKG-INFO` & `cool_cache-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: cool_cache
-Version: 0.1.3
+Version: 0.3.0
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # What is this?
 
-The smart way to cache function outputs to permanent storage.
+The smart way to cache outputs to cold storage.
 
 - auto rebuilds cache when you edit function source code
 - uses mutltiprocessing to keep main thread running fast while saving to disk
 - excellent change-tracking of arguments thanks to `super_hash`
 - can watch change-tracking of external vars and method attributes
 - uses python pickle for saving function outputs, if `dill` is available it will use that instead
 
 # How do I use this?
 
 `pip install cool_cache`
 
 ```python
 from cool_cache import cache, settings
 
+settings.default_folder = None # disable caching to cold-storage, and instead cache to ram
 # this is the default, but you can change it
-settings.default_folder="cache.ignore/"
+settings.default_folder = "cache.ignore/"
 
 # 
 # 
 # simple usage (updates whenever function is edited (excluding comments) or when args change)
 # 
 # 
 @cache()
```

### Comparing `cool_cache-0.1.3/cool_cache.egg-info/PKG-INFO` & `cool_cache-0.3.0/cool_cache.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: cool-cache
-Version: 0.1.3
+Version: 0.3.0
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # What is this?
 
-The smart way to cache function outputs to permanent storage.
+The smart way to cache outputs to cold storage.
 
 - auto rebuilds cache when you edit function source code
 - uses mutltiprocessing to keep main thread running fast while saving to disk
 - excellent change-tracking of arguments thanks to `super_hash`
 - can watch change-tracking of external vars and method attributes
 - uses python pickle for saving function outputs, if `dill` is available it will use that instead
 
 # How do I use this?
 
 `pip install cool_cache`
 
 ```python
 from cool_cache import cache, settings
 
+settings.default_folder = None # disable caching to cold-storage, and instead cache to ram
 # this is the default, but you can change it
-settings.default_folder="cache.ignore/"
+settings.default_folder = "cache.ignore/"
 
 # 
 # 
 # simple usage (updates whenever function is edited (excluding comments) or when args change)
 # 
 # 
 @cache()
```

### Comparing `cool_cache-0.1.3/setup.py` & `cool_cache-0.3.0/setup.py`

 * *Files identical despite different names*

