# Comparing `tmp/wozoxutils-0.2.3.tar.gz` & `tmp/wozoxutils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wozoxutils-0.2.3.tar", last modified: Tue Apr 18 10:00:39 2023, max compression
+gzip compressed data, was "wozoxutils-0.2.4.tar", last modified: Wed Apr 19 12:38:13 2023, max compression
```

## Comparing `wozoxutils-0.2.3.tar` & `wozoxutils-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:00:39.118942 wozoxutils-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-18 10:00:39.118942 wozoxutils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:00:39.118942 wozoxutils-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:00:39.118942 wozoxutils-0.2.3/wozoxutils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/wozoxutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/wozoxutils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-18 10:00:21.000000 wozoxutils-0.2.3/wozoxutils/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:00:39.118942 wozoxutils-0.2.3/wozoxutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-18 10:00:39.000000 wozoxutils-0.2.3/wozoxutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 10:00:39.000000 wozoxutils-0.2.3/wozoxutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:00:39.000000 wozoxutils-0.2.3/wozoxutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 10:00:39.000000 wozoxutils-0.2.3/wozoxutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.127840 wozoxutils-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.127840 wozoxutils-0.2.4/wozoxutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/wozoxutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/top_level.txt
```

### Comparing `wozoxutils-0.2.3/LICENSE` & `wozoxutils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.3/PKG-INFO` & `wozoxutils-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.3
+Version: 0.2.4
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wozoxutils-0.2.3/setup.py` & `wozoxutils-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name="wozoxutils",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
-    install_requires=[],  # 添加依赖包
+    install_requires=[
+        'pyyaml>=6.0',
+    ],
     author="illiten",
     author_email="admin@leelib.com",
     description="general-purpose library for Python that contains various commonly used functional modules",
     url="https://github.com/wozox/wozoxutils-py",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='wozox utils',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wozoxutils-0.2.3/wozoxutils/file.py` & `wozoxutils-0.2.4/wozoxutils/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,16 @@
 def load_text(filename: str) -> str:
     """
     Load text from file
 
     :param filename: File path
     :return: Content
     """
-    with open(filename, 'r', encoding='utf-8', newline='\n') as f:
-        content = f.read()
-        return content
+    with open(filename, 'r', encoding='utf-8') as f:
+        return f.read()
 
 
 def save_bytes(filename: str, content: bytes):
     """
     Save bytes to file. If the directory does not exist, it will be created.
 
     :param filename: File path
```

### Comparing `wozoxutils-0.2.3/wozoxutils/hash.py` & `wozoxutils-0.2.4/wozoxutils/hash.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.3/wozoxutils.egg-info/PKG-INFO` & `wozoxutils-0.2.4/wozoxutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.3
+Version: 0.2.4
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

