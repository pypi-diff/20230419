# Comparing `tmp/ipfsclient-0.0.4.tar.gz` & `tmp/ipfsclient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfsclient-0.0.4.tar", last modified: Tue Apr 18 23:55:11 2023, max compression
+gzip compressed data, was "ipfsclient-0.0.5.tar", last modified: Wed Apr 19 00:34:09 2023, max compression
```

## Comparing `ipfsclient-0.0.4.tar` & `ipfsclient-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 23:55:11.853057 ipfsclient-0.0.4/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 22:36:57.000000 ipfsclient-0.0.4/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 23:55:11.852936 ipfsclient-0.0.4/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     2004 2023-04-18 22:38:30.000000 ipfsclient-0.0.4/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 23:55:11.852785 ipfsclient-0.0.4/ipfsclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-18 23:55:11.000000 ipfsclient-0.0.4/ipfsclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      210 2023-04-18 23:55:11.000000 ipfsclient-0.0.4/ipfsclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 23:55:11.000000 ipfsclient-0.0.4/ipfsclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-04-18 23:55:11.000000 ipfsclient-0.0.4/ipfsclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 23:55:11.000000 ipfsclient-0.0.4/ipfsclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      631 2023-04-18 23:51:29.000000 ipfsclient-0.0.4/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 23:55:11.853088 ipfsclient-0.0.4/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      898 2023-04-18 23:15:39.000000 ipfsclient-0.0.4/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-19 00:34:09.943309 ipfsclient-0.0.5/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 22:36:57.000000 ipfsclient-0.0.5/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-19 00:34:09.943131 ipfsclient-0.0.5/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     2004 2023-04-18 22:38:30.000000 ipfsclient-0.0.5/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-19 00:34:09.942804 ipfsclient-0.0.5/ipfsclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3903 2023-04-19 00:34:09.000000 ipfsclient-0.0.5/ipfsclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      210 2023-04-19 00:34:09.000000 ipfsclient-0.0.5/ipfsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-19 00:34:09.000000 ipfsclient-0.0.5/ipfsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       34 2023-04-19 00:34:09.000000 ipfsclient-0.0.5/ipfsclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-19 00:34:09.000000 ipfsclient-0.0.5/ipfsclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      616 2023-04-19 00:00:41.000000 ipfsclient-0.0.5/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-19 00:34:09.943362 ipfsclient-0.0.5/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      898 2023-04-19 00:15:07.000000 ipfsclient-0.0.5/setup.py
```

### Comparing `ipfsclient-0.0.4/LICENSE` & `ipfsclient-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfsclient-0.0.4/PKG-INFO` & `ipfsclient-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfsclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfsclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfsclient-0.0.4/README.md` & `ipfsclient-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ipfsclient-0.0.4/ipfsclient.egg-info/PKG-INFO` & `ipfsclient-0.0.5/ipfsclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfsclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfsclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfsclient-0.0.4/pyproject.toml` & `ipfsclient-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 source = ["ipfsclient", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfsclient"
-version = "0.0.4"
+version = "0.0.5"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfsclient/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
 requires-python = '>=3.11'
 readme = 'README.md'
 license = {'file' = 'LICENSE'}
 dependencies = [
     "requests",
     "setuptools",
-    "py-multicodec",
-    "pandas",
+    "py-multicodec"
 ]
```

### Comparing `ipfsclient-0.0.4/setup.py` & `ipfsclient-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfsclient",
-    version="0.0.4",
+    version="0.0.5",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="IPFS RPC Client",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/ipfsclient",
     project_urls={
```

