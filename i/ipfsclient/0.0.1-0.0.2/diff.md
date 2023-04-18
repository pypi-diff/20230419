# Comparing `tmp/ipfsclient-0.0.1.tar.gz` & `tmp/ipfsclient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfsclient-0.0.1.tar", last modified: Tue Apr 18 22:47:21 2023, max compression
+gzip compressed data, was "ipfsclient-0.0.2.tar", last modified: Tue Apr 18 22:55:19 2023, max compression
```

## Comparing `ipfsclient-0.0.1.tar` & `ipfsclient-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 22:47:21.520672 ipfsclient-0.0.1/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 22:36:57.000000 ipfsclient-0.0.1/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 22:47:21.520556 ipfsclient-0.0.1/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     2004 2023-04-18 22:38:30.000000 ipfsclient-0.0.1/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 22:47:21.520416 ipfsclient-0.0.1/ipfsclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 22:47:21.000000 ipfsclient-0.0.1/ipfsclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      210 2023-04-18 22:47:21.000000 ipfsclient-0.0.1/ipfsclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 22:47:21.000000 ipfsclient-0.0.1/ipfsclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-18 22:47:21.000000 ipfsclient-0.0.1/ipfsclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 22:47:21.000000 ipfsclient-0.0.1/ipfsclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      647 2023-04-18 22:45:31.000000 ipfsclient-0.0.1/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 22:47:21.520701 ipfsclient-0.0.1/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      898 2023-04-18 22:45:26.000000 ipfsclient-0.0.1/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 22:55:19.060515 ipfsclient-0.0.2/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 22:36:57.000000 ipfsclient-0.0.2/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 22:55:19.060367 ipfsclient-0.0.2/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     2004 2023-04-18 22:38:30.000000 ipfsclient-0.0.2/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 22:55:19.060212 ipfsclient-0.0.2/ipfsclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 22:55:19.000000 ipfsclient-0.0.2/ipfsclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      210 2023-04-18 22:55:19.000000 ipfsclient-0.0.2/ipfsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 22:55:19.000000 ipfsclient-0.0.2/ipfsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-18 22:55:19.000000 ipfsclient-0.0.2/ipfsclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 22:55:19.000000 ipfsclient-0.0.2/ipfsclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      647 2023-04-18 22:53:16.000000 ipfsclient-0.0.2/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 22:55:19.060551 ipfsclient-0.0.2/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      898 2023-04-18 22:53:06.000000 ipfsclient-0.0.2/setup.py
```

### Comparing `ipfsclient-0.0.1/LICENSE` & `ipfsclient-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfsclient-0.0.1/PKG-INFO` & `ipfsclient-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfsclient
-Version: 0.0.1
+Version: 0.0.2
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfsclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfsclient-0.0.1/README.md` & `ipfsclient-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfsclient-0.0.1/ipfsclient.egg-info/PKG-INFO` & `ipfsclient-0.0.2/ipfsclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfsclient
-Version: 0.0.1
+Version: 0.0.2
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfsclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfsclient-0.0.1/pyproject.toml` & `ipfsclient-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 source = ["ipfsclient", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfsclient"
-version = "0.0.1"
+version = "0.0.2"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfsclient/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `ipfsclient-0.0.1/setup.py` & `ipfsclient-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfsclient",
-    version="0.0.1",
+    version="0.0.2",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="IPFS RPC Client",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/ipfsclient",
     project_urls={
```

