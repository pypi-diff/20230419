# Comparing `tmp/browseapi_sandbox-0.4.tar.gz` & `tmp/browseapi_sandbox-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browseapi_sandbox-0.4.tar", last modified: Wed Apr 19 16:11:54 2023, max compression
+gzip compressed data, was "browseapi_sandbox-0.5.tar", last modified: Wed Apr 19 16:49:27 2023, max compression
```

## Comparing `browseapi_sandbox-0.4.tar` & `browseapi_sandbox-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.284023 browseapi_sandbox-0.4/
--rw-rw-rw-   0        0        0     1094 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4690 2023-04-19 16:11:54.283026 browseapi_sandbox-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3234 2023-04-19 14:36:08.000000 browseapi_sandbox-0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.252109 browseapi_sandbox-0.4/browseapi/
--rw-rw-rw-   0        0        0       57 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/__init__.py
--rw-rw-rw-   0        0        0    16671 2023-04-19 14:34:58.000000 browseapi_sandbox-0.4/browseapi/client.py
--rw-rw-rw-   0        0        0    36702 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/containers.py
--rw-rw-rw-   0        0        0     2191 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.255117 browseapi_sandbox-0.4/browseapi/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/tests/__init__.py
--rw-rw-rw-   0        0        0     3477 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/tests/test_client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.282037 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/
--rw-rw-rw-   0        0        0     4690 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 16:11:54.285036 browseapi_sandbox-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-04-19 16:11:18.000000 browseapi_sandbox-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:49:27.256523 browseapi_sandbox-0.5/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4690 2023-04-19 16:49:27.255523 browseapi_sandbox-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3234 2023-04-19 14:36:08.000000 browseapi_sandbox-0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 16:49:27.203664 browseapi_sandbox-0.5/browseapi/
+-rw-rw-rw-   0        0        0       57 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/browseapi/__init__.py
+-rw-rw-rw-   0        0        0    16663 2023-04-19 16:47:23.000000 browseapi_sandbox-0.5/browseapi/client.py
+-rw-rw-rw-   0        0        0    36702 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/browseapi/containers.py
+-rw-rw-rw-   0        0        0     2191 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/browseapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:49:27.206687 browseapi_sandbox-0.5/browseapi/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/browseapi/tests/__init__.py
+-rw-rw-rw-   0        0        0     3477 2023-04-19 14:32:47.000000 browseapi_sandbox-0.5/browseapi/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:49:27.253531 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/
+-rw-rw-rw-   0        0        0     4690 2023-04-19 16:49:27.000000 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-19 16:49:27.000000 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:49:27.000000 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 16:49:27.000000 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 16:49:27.000000 browseapi_sandbox-0.5/browseapi_sandbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:49:27.256523 browseapi_sandbox-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-04-19 16:47:41.000000 browseapi_sandbox-0.5/setup.py
```

### Comparing `browseapi_sandbox-0.4/LICENSE.txt` & `browseapi_sandbox-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.4/PKG-INFO` & `browseapi_sandbox-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: browseapi_sandbox
-Version: 0.4
+Version: 0.5
 Summary: eBay Browse API Python client
 Home-page: https://github.com/atedrow/browseapi_sandbox
 Author: Alexander Tedrow
 Author-email: atedrow@clemson.edu
 License: MIT
-Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz
+Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_05.tar.gz
 Description: Browse API client
         =================
         
         |coverage| |build_status| |Documentation Status| |PyPI version|
         
         This package is a Python client for eBay Browse API. It is asynchronous
         and designed to send a large number of requests by one function call.
```

### Comparing `browseapi_sandbox-0.4/README.rst` & `browseapi_sandbox-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.4/browseapi/client.py` & `browseapi_sandbox-0.5/browseapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     _get_item_by_legacy_id_uri = _uri + '/item/get_item_by_legacy_id?'
     _get_items_by_item_group_uri = _uri + '/item/get_items_by_item_group?'
     _check_compatibility_uri = _uri + '/item/{item_id}/check_compatibility'
 
     # Client Credential Grant Type
 
     _credentials_grant_type = 'client_credentials'
-    _scope_public_data = 'https://api.sandbox.ebay.com/oauth/api_scope'
+    _scope_public_data = 'https://api.ebay.com/oauth/api_scope'
 
     supported_methods = (
         'search',
         'search_by_image',
         'get_item',
         'get_item_by_legacy_id',
         'get_items_by_item_group',
```

### Comparing `browseapi_sandbox-0.4/browseapi/containers.py` & `browseapi_sandbox-0.5/browseapi/containers.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.4/browseapi/exceptions.py` & `browseapi_sandbox-0.5/browseapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.4/browseapi/tests/test_client.py` & `browseapi_sandbox-0.5/browseapi/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.4/browseapi_sandbox.egg-info/PKG-INFO` & `browseapi_sandbox-0.5/browseapi_sandbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: browseapi-sandbox
-Version: 0.4
+Version: 0.5
 Summary: eBay Browse API Python client
 Home-page: https://github.com/atedrow/browseapi_sandbox
 Author: Alexander Tedrow
 Author-email: atedrow@clemson.edu
 License: MIT
-Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz
+Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_05.tar.gz
 Description: Browse API client
         =================
         
         |coverage| |build_status| |Documentation Status| |PyPI version|
         
         This package is a Python client for eBay Browse API. It is asynchronous
         and designed to send a large number of requests by one function call.
```

### Comparing `browseapi_sandbox-0.4/setup.py` & `browseapi_sandbox-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='browseapi_sandbox',
     packages=find_packages(exclude=['test']),
-    version='0.4',
+    version='0.5',
     license='MIT',
     description='eBay Browse API Python client',
     long_description=long_description,
     author='Alexander Tedrow',
     author_email='atedrow@clemson.edu',
     url='https://github.com/atedrow/browseapi_sandbox',
-    download_url='https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz',
+    download_url='https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_05.tar.gz',
     keywords=['ASYNC', 'BROWSE API', 'CLIENT'],
 
     install_requires=[
         'aiohttp',
     ],
 
     classifiers=[
```

