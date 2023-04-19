# Comparing `tmp/klaviyo-3.1.6.tar.gz` & `tmp/klaviyo-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-3.1.6.tar", last modified: Tue Oct 25 17:29:05 2022, max compression
+gzip compressed data, was "klaviyo-3.1.7.tar", last modified: Wed Apr 19 19:54:33 2023, max compression
```

## Comparing `klaviyo-3.1.6.tar` & `klaviyo-3.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 17:29:05.267161 klaviyo-3.1.6/
--rw-r--r--   0 local      (503) staff       (20)      479 2022-10-25 17:29:05.266948 klaviyo-3.1.6/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)     8138 2022-10-25 17:25:38.000000 klaviyo-3.1.6/README.md
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 17:29:05.262893 klaviyo-3.1.6/klaviyo/
--rw-r--r--   0 local      (503) staff       (20)       47 2022-10-25 17:25:38.000000 klaviyo-3.1.6/klaviyo/__init__.py
--rw-r--r--   0 local      (503) staff       (20)     1484 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/api.py
--rw-r--r--   0 local      (503) staff       (20)    10573 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/api_helper.py
--rw-r--r--   0 local      (503) staff       (20)     1882 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/campaigns.py
--rw-r--r--   0 local      (503) staff       (20)     1576 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/data_privacy.py
--rw-r--r--   0 local      (503) staff       (20)     1220 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/exceptions.py
--rw-r--r--   0 local      (503) staff       (20)     7961 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/lists.py
--rw-r--r--   0 local      (503) staff       (20)     4043 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/metrics.py
--rw-r--r--   0 local      (503) staff       (20)     1020 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/middleware.py
--rw-r--r--   0 local      (503) staff       (20)     4413 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/profiles.py
--rw-r--r--   0 local      (503) staff       (20)     5010 2022-10-25 16:50:48.000000 klaviyo-3.1.6/klaviyo/public.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 17:29:05.264523 klaviyo-3.1.6/klaviyo.egg-info/
--rw-r--r--   0 local      (503) staff       (20)      479 2022-10-25 17:29:05.000000 klaviyo-3.1.6/klaviyo.egg-info/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)      595 2022-10-25 17:29:05.000000 klaviyo-3.1.6/klaviyo.egg-info/SOURCES.txt
--rw-r--r--   0 local      (503) staff       (20)        1 2022-10-25 17:29:05.000000 klaviyo-3.1.6/klaviyo.egg-info/dependency_links.txt
--rw-r--r--   0 local      (503) staff       (20)       35 2022-10-25 17:29:05.000000 klaviyo-3.1.6/klaviyo.egg-info/requires.txt
--rw-r--r--   0 local      (503) staff       (20)       14 2022-10-25 17:29:05.000000 klaviyo-3.1.6/klaviyo.egg-info/top_level.txt
--rw-r--r--   0 local      (503) staff       (20)       38 2022-10-25 17:29:05.267233 klaviyo-3.1.6/setup.cfg
--rw-r--r--   0 local      (503) staff       (20)      822 2022-10-25 17:28:56.000000 klaviyo-3.1.6/setup.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 17:29:05.265565 klaviyo-3.1.6/tests/
--rw-r--r--   0 local      (503) staff       (20)        0 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/__init__.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 17:29:05.266626 klaviyo-3.1.6/tests/fixtures/
--rw-r--r--   0 local      (503) staff       (20)        0 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/fixtures/__init__.py
--rw-r--r--   0 local      (503) staff       (20)     3095 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/fixtures/api_helper.py
--rw-r--r--   0 local      (503) staff       (20)      510 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/fixtures/data_privacy.py
--rw-r--r--   0 local      (503) staff       (20)      398 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/fixtures/public.py
--rw-r--r--   0 local      (503) staff       (20)     2356 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/test_api_helper.py
--rw-r--r--   0 local      (503) staff       (20)      609 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/test_data_privacy.py
--rw-r--r--   0 local      (503) staff       (20)      608 2022-10-25 16:50:48.000000 klaviyo-3.1.6/tests/test_public.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:54:33.825148 klaviyo-3.1.7/
+-rw-r--r--   0 local      (503) staff       (20)      479 2023-04-19 19:54:33.824842 klaviyo-3.1.7/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)     8134 2023-04-19 19:46:19.000000 klaviyo-3.1.7/README.md
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:54:33.819720 klaviyo-3.1.7/klaviyo/
+-rw-r--r--   0 local      (503) staff       (20)       47 2023-04-19 19:46:48.000000 klaviyo-3.1.7/klaviyo/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)     1484 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/api.py
+-rw-r--r--   0 local      (503) staff       (20)    10756 2023-04-19 19:50:21.000000 klaviyo-3.1.7/klaviyo/api_helper.py
+-rw-r--r--   0 local      (503) staff       (20)     1882 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/campaigns.py
+-rw-r--r--   0 local      (503) staff       (20)     1576 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/data_privacy.py
+-rw-r--r--   0 local      (503) staff       (20)     1220 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/exceptions.py
+-rw-r--r--   0 local      (503) staff       (20)     7961 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/lists.py
+-rw-r--r--   0 local      (503) staff       (20)     4043 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/metrics.py
+-rw-r--r--   0 local      (503) staff       (20)     1020 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/middleware.py
+-rw-r--r--   0 local      (503) staff       (20)     4413 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/profiles.py
+-rw-r--r--   0 local      (503) staff       (20)     5010 2023-04-19 19:46:19.000000 klaviyo-3.1.7/klaviyo/public.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:54:33.821705 klaviyo-3.1.7/klaviyo.egg-info/
+-rw-r--r--   0 local      (503) staff       (20)      479 2023-04-19 19:54:33.000000 klaviyo-3.1.7/klaviyo.egg-info/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)      595 2023-04-19 19:54:33.000000 klaviyo-3.1.7/klaviyo.egg-info/SOURCES.txt
+-rw-r--r--   0 local      (503) staff       (20)        1 2023-04-19 19:54:33.000000 klaviyo-3.1.7/klaviyo.egg-info/dependency_links.txt
+-rw-r--r--   0 local      (503) staff       (20)       35 2023-04-19 19:54:33.000000 klaviyo-3.1.7/klaviyo.egg-info/requires.txt
+-rw-r--r--   0 local      (503) staff       (20)       14 2023-04-19 19:54:33.000000 klaviyo-3.1.7/klaviyo.egg-info/top_level.txt
+-rw-r--r--   0 local      (503) staff       (20)       38 2023-04-19 19:54:33.825253 klaviyo-3.1.7/setup.cfg
+-rw-r--r--   0 local      (503) staff       (20)      822 2023-04-19 19:53:14.000000 klaviyo-3.1.7/setup.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:54:33.823050 klaviyo-3.1.7/tests/
+-rw-r--r--   0 local      (503) staff       (20)        0 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/__init__.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:54:33.824413 klaviyo-3.1.7/tests/fixtures/
+-rw-r--r--   0 local      (503) staff       (20)        0 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/fixtures/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)     3095 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/fixtures/api_helper.py
+-rw-r--r--   0 local      (503) staff       (20)      510 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/fixtures/data_privacy.py
+-rw-r--r--   0 local      (503) staff       (20)      398 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/fixtures/public.py
+-rw-r--r--   0 local      (503) staff       (20)     2356 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/test_api_helper.py
+-rw-r--r--   0 local      (503) staff       (20)      609 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/test_data_privacy.py
+-rw-r--r--   0 local      (503) staff       (20)      608 2023-04-19 19:46:19.000000 klaviyo-3.1.7/tests/test_public.py
```

### Comparing `klaviyo-3.1.6/README.md` & `klaviyo-3.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # python-klaviyo - DEPRECATED
 
 # Deprecation Notice
 
-This SDK and its associated pip package are set to be deprecated on April 1st 2023 and will not receive further updates.
+This SDK and its associated pip package are set to be deprecated on 2024-01-01 and will not receive further updates.
 
 We recommend migrating over to our [newest SDK](https://github.com/klaviyo/klaviyo-api-python).
 
 You can read more about our SDK release history and support [here](https://developers.klaviyo.com/en/docs/sdk_overview)
 
 For a comparison between our old and new APIs, check out [this guide](https://developers.klaviyo.com/en/docs/apis_comparison_chart).
```

### Comparing `klaviyo-3.1.6/klaviyo/api.py` & `klaviyo-3.1.7/klaviyo/api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/api_helper.py` & `klaviyo-3.1.7/klaviyo/api_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from .exceptions import (
     KlaviyoAPIException,
     KlaviyoConfigurationException,
     KlaviyoAuthenticationError, KlaviyoRateLimitException,
     KlaviyoServerError,
 )
 from klaviyo import __version__
+import warnings
+
+warnings.warn("This SDK is being deprecated on 2024-01-01, please switch to our newest SDK here: https://github.com/klaviyo/klaviyo-api-python", DeprecationWarning)
+
 
 
 class KlaviyoAPIResponse(object):
     def __init__(self, status_code, data):
         self.status_code = status_code
         self.data = data
```

### Comparing `klaviyo-3.1.6/klaviyo/campaigns.py` & `klaviyo-3.1.7/klaviyo/campaigns.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/data_privacy.py` & `klaviyo-3.1.7/klaviyo/data_privacy.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/exceptions.py` & `klaviyo-3.1.7/klaviyo/exceptions.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/lists.py` & `klaviyo-3.1.7/klaviyo/lists.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/metrics.py` & `klaviyo-3.1.7/klaviyo/metrics.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/middleware.py` & `klaviyo-3.1.7/klaviyo/middleware.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/profiles.py` & `klaviyo-3.1.7/klaviyo/profiles.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo/public.py` & `klaviyo-3.1.7/klaviyo/public.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/klaviyo.egg-info/SOURCES.txt` & `klaviyo-3.1.7/klaviyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/setup.py` & `klaviyo-3.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
     # metadata for upload to PyPI
     author = 'Klaviyo',
     author_email = 'developers@klaviyo.com',
     description = "Deprecated Klaviyo SDK",
     long_description = (
 """
-Deprecation Notice: This package is set to be deprecated on 2023-01-01 and will not receive further updates. To continue receiving API and SDK improvements, we recommend switching over to our latest package/sdk: https://pypi.org/project/klaviyo-api/
+Deprecation Notice: This package is set to be deprecated on 2024-01-01 and will not receive further updates. To continue receiving API and SDK improvements, we recommend switching over to our latest package/sdk: https://pypi.org/project/klaviyo-api/
 """
     ),
     license = 'MIT License',
     keywords = 'klaviyo',
     url = 'http://github.com/klaviyo/python-klaviyo',
 )
```

### Comparing `klaviyo-3.1.6/tests/fixtures/api_helper.py` & `klaviyo-3.1.7/tests/fixtures/api_helper.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/tests/test_api_helper.py` & `klaviyo-3.1.7/tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/tests/test_data_privacy.py` & `klaviyo-3.1.7/tests/test_data_privacy.py`

 * *Files identical despite different names*

### Comparing `klaviyo-3.1.6/tests/test_public.py` & `klaviyo-3.1.7/tests/test_public.py`

 * *Files identical despite different names*

