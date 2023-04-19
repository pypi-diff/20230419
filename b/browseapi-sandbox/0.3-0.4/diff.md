# Comparing `tmp/browseapi_sandbox-0.3.tar.gz` & `tmp/browseapi_sandbox-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browseapi_sandbox-0.3.tar", last modified: Wed Apr 19 16:10:47 2023, max compression
+gzip compressed data, was "browseapi_sandbox-0.4.tar", last modified: Wed Apr 19 16:11:54 2023, max compression
```

## Comparing `browseapi_sandbox-0.3.tar` & `browseapi_sandbox-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:10:47.133320 browseapi_sandbox-0.3/
--rw-rw-rw-   0        0        0     1094 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4690 2023-04-19 16:10:47.132323 browseapi_sandbox-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3234 2023-04-19 14:36:08.000000 browseapi_sandbox-0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 16:10:47.102405 browseapi_sandbox-0.3/browseapi/
--rw-rw-rw-   0        0        0       57 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/browseapi/__init__.py
--rw-rw-rw-   0        0        0    16671 2023-04-19 14:34:58.000000 browseapi_sandbox-0.3/browseapi/client.py
--rw-rw-rw-   0        0        0    36702 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/browseapi/containers.py
--rw-rw-rw-   0        0        0     2191 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/browseapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:10:47.105396 browseapi_sandbox-0.3/browseapi/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/browseapi/tests/__init__.py
--rw-rw-rw-   0        0        0     3477 2023-04-19 14:32:47.000000 browseapi_sandbox-0.3/browseapi/tests/test_client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:10:47.131325 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/
--rw-rw-rw-   0        0        0     4690 2023-04-19 16:10:47.000000 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-19 16:10:47.000000 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:10:47.000000 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 16:10:47.000000 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 16:10:47.000000 browseapi_sandbox-0.3/browseapi_sandbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 16:10:47.133320 browseapi_sandbox-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-04-19 16:10:34.000000 browseapi_sandbox-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.284023 browseapi_sandbox-0.4/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4690 2023-04-19 16:11:54.283026 browseapi_sandbox-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3234 2023-04-19 14:36:08.000000 browseapi_sandbox-0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.252109 browseapi_sandbox-0.4/browseapi/
+-rw-rw-rw-   0        0        0       57 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/__init__.py
+-rw-rw-rw-   0        0        0    16671 2023-04-19 14:34:58.000000 browseapi_sandbox-0.4/browseapi/client.py
+-rw-rw-rw-   0        0        0    36702 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/containers.py
+-rw-rw-rw-   0        0        0     2191 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.255117 browseapi_sandbox-0.4/browseapi/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/tests/__init__.py
+-rw-rw-rw-   0        0        0     3477 2023-04-19 14:32:47.000000 browseapi_sandbox-0.4/browseapi/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:11:54.282037 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/
+-rw-rw-rw-   0        0        0     4690 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 16:11:54.000000 browseapi_sandbox-0.4/browseapi_sandbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:11:54.285036 browseapi_sandbox-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-04-19 16:11:18.000000 browseapi_sandbox-0.4/setup.py
```

### Comparing `browseapi_sandbox-0.3/LICENSE.txt` & `browseapi_sandbox-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/PKG-INFO` & `browseapi_sandbox-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: browseapi_sandbox
-Version: 0.3
+Version: 0.4
 Summary: eBay Browse API Python client
 Home-page: https://github.com/atedrow/browseapi_sandbox
 Author: Alexander Tedrow
 Author-email: atedrow@clemson.edu
 License: MIT
-Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_03.tar.gz
+Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz
 Description: Browse API client
         =================
         
         |coverage| |build_status| |Documentation Status| |PyPI version|
         
         This package is a Python client for eBay Browse API. It is asynchronous
         and designed to send a large number of requests by one function call.
```

### Comparing `browseapi_sandbox-0.3/README.rst` & `browseapi_sandbox-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/browseapi/client.py` & `browseapi_sandbox-0.4/browseapi/client.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/browseapi/containers.py` & `browseapi_sandbox-0.4/browseapi/containers.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/browseapi/exceptions.py` & `browseapi_sandbox-0.4/browseapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/browseapi/tests/test_client.py` & `browseapi_sandbox-0.4/browseapi/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `browseapi_sandbox-0.3/browseapi_sandbox.egg-info/PKG-INFO` & `browseapi_sandbox-0.4/browseapi_sandbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: browseapi-sandbox
-Version: 0.3
+Version: 0.4
 Summary: eBay Browse API Python client
 Home-page: https://github.com/atedrow/browseapi_sandbox
 Author: Alexander Tedrow
 Author-email: atedrow@clemson.edu
 License: MIT
-Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_03.tar.gz
+Download-URL: https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz
 Description: Browse API client
         =================
         
         |coverage| |build_status| |Documentation Status| |PyPI version|
         
         This package is a Python client for eBay Browse API. It is asynchronous
         and designed to send a large number of requests by one function call.
```

### Comparing `browseapi_sandbox-0.3/setup.py` & `browseapi_sandbox-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='browseapi_sandbox',
     packages=find_packages(exclude=['test']),
-    version='0.3',
+    version='0.4',
     license='MIT',
     description='eBay Browse API Python client',
     long_description=long_description,
     author='Alexander Tedrow',
     author_email='atedrow@clemson.edu',
     url='https://github.com/atedrow/browseapi_sandbox',
-    download_url='https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_03.tar.gz',
+    download_url='https://github.com/atedrow/browseapi_sandbox/archive/refs/tags/v_04.tar.gz',
     keywords=['ASYNC', 'BROWSE API', 'CLIENT'],
 
     install_requires=[
         'aiohttp',
     ],
 
     classifiers=[
```

