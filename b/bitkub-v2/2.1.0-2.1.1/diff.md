# Comparing `tmp/bitkub-v2-2.1.0.tar.gz` & `tmp/bitkub-v2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitkub-v2-2.1.0.tar", last modified: Wed Apr 19 07:50:24 2023, max compression
+gzip compressed data, was "bitkub-v2-2.1.1.tar", last modified: Wed Apr 19 07:53:44 2023, max compression
```

## Comparing `bitkub-v2-2.1.0.tar` & `bitkub-v2-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:50:24.952343 bitkub-v2-2.1.0/
--rw-rw-rw-   0        0        0       68 2023-03-29 02:51:21.000000 bitkub-v2-2.1.0/.gitignore
--rw-rw-rw-   0        0        0    28629 2023-04-19 07:50:24.953344 bitkub-v2-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    27169 2023-03-29 03:32:13.000000 bitkub-v2-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:50:24.946838 bitkub-v2-2.1.0/bitkub-v2/
--rw-rw-rw-   0        0        0      100 2023-03-29 02:51:21.000000 bitkub-v2-2.1.0/bitkub-v2/__init__.py
--rw-rw-rw-   0        0        0    10431 2023-04-18 08:02:49.000000 bitkub-v2-2.1.0/bitkub-v2/bitkub.py
--rw-rw-rw-   0        0        0     2240 2023-03-29 07:41:01.000000 bitkub-v2-2.1.0/bitkub-v2/constants.py
--rw-rw-rw-   0        0        0      593 2023-03-29 02:51:21.000000 bitkub-v2-2.1.0/bitkub-v2/decorators.py
--rw-rw-rw-   0        0        0       39 2023-03-29 02:51:21.000000 bitkub-v2-2.1.0/bitkub-v2/error.py
--rw-rw-rw-   0        0        0      153 2023-03-29 02:51:21.000000 bitkub-v2-2.1.0/bitkub-v2/request.py
--rw-rw-rw-   0        0        0     3800 2023-03-29 04:08:11.000000 bitkub-v2-2.1.0/bitkub-v2/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:50:24.952343 bitkub-v2-2.1.0/bitkub_v2.egg-info/
--rw-rw-rw-   0        0        0    28629 2023-04-19 07:50:24.000000 bitkub-v2-2.1.0/bitkub_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-19 07:50:24.000000 bitkub-v2-2.1.0/bitkub_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:50:24.000000 bitkub-v2-2.1.0/bitkub_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 07:50:24.000000 bitkub-v2-2.1.0/bitkub_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 07:50:24.000000 bitkub-v2-2.1.0/bitkub_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1702 2023-04-18 07:45:04.000000 bitkub-v2-2.1.0/sample.py
--rw-rw-rw-   0        0        0       86 2023-04-19 07:50:24.954343 bitkub-v2-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      585 2023-04-19 07:50:15.000000 bitkub-v2-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:53:44.679452 bitkub-v2-2.1.1/
+-rw-rw-rw-   0        0        0       68 2023-03-29 02:51:21.000000 bitkub-v2-2.1.1/.gitignore
+-rw-rw-rw-   0        0        0    28629 2023-04-19 07:53:44.679452 bitkub-v2-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27169 2023-03-29 03:32:13.000000 bitkub-v2-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 07:53:44.671456 bitkub-v2-2.1.1/bitkub/
+-rw-rw-rw-   0        0        0      100 2023-03-29 02:51:21.000000 bitkub-v2-2.1.1/bitkub/__init__.py
+-rw-rw-rw-   0        0        0    10431 2023-04-18 08:02:49.000000 bitkub-v2-2.1.1/bitkub/bitkub.py
+-rw-rw-rw-   0        0        0     2240 2023-03-29 07:41:01.000000 bitkub-v2-2.1.1/bitkub/constants.py
+-rw-rw-rw-   0        0        0      593 2023-03-29 02:51:21.000000 bitkub-v2-2.1.1/bitkub/decorators.py
+-rw-rw-rw-   0        0        0       39 2023-03-29 02:51:21.000000 bitkub-v2-2.1.1/bitkub/error.py
+-rw-rw-rw-   0        0        0      153 2023-03-29 02:51:21.000000 bitkub-v2-2.1.1/bitkub/request.py
+-rw-rw-rw-   0        0        0     3800 2023-03-29 04:08:11.000000 bitkub-v2-2.1.1/bitkub/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:53:44.678451 bitkub-v2-2.1.1/bitkub_v2.egg-info/
+-rw-rw-rw-   0        0        0    28629 2023-04-19 07:53:44.000000 bitkub-v2-2.1.1/bitkub_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-19 07:53:44.000000 bitkub-v2-2.1.1/bitkub_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:53:44.000000 bitkub-v2-2.1.1/bitkub_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 07:53:44.000000 bitkub-v2-2.1.1/bitkub_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 07:53:44.000000 bitkub-v2-2.1.1/bitkub_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1702 2023-04-18 07:45:04.000000 bitkub-v2-2.1.1/sample.py
+-rw-rw-rw-   0        0        0       86 2023-04-19 07:53:44.681452 bitkub-v2-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-04-19 07:52:44.000000 bitkub-v2-2.1.1/setup.py
```

### Comparing `bitkub-v2-2.1.0/PKG-INFO` & `bitkub-v2-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitkub-v2
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python library for Bitkub API v2
 Home-page: https://github.com/appcorner/bitkub
 Author: appcorner
 Author-email: appcorner@yahoo.com
 License: MIT
 Keywords: bitkub,bitkub-python,bitkub-python-sdk
 Description-Content-Type: text/markdown
```

### Comparing `bitkub-v2-2.1.0/README.md` & `bitkub-v2-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/bitkub-v2/bitkub.py` & `bitkub-v2-2.1.1/bitkub/bitkub.py`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/bitkub-v2/constants.py` & `bitkub-v2-2.1.1/bitkub/constants.py`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/bitkub-v2/decorators.py` & `bitkub-v2-2.1.1/bitkub/decorators.py`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/bitkub-v2/tests.py` & `bitkub-v2-2.1.1/bitkub/tests.py`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/bitkub_v2.egg-info/PKG-INFO` & `bitkub-v2-2.1.1/bitkub_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitkub-v2
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python library for Bitkub API v2
 Home-page: https://github.com/appcorner/bitkub
 Author: appcorner
 Author-email: appcorner@yahoo.com
 License: MIT
 Keywords: bitkub,bitkub-python,bitkub-python-sdk
 Description-Content-Type: text/markdown
```

### Comparing `bitkub-v2-2.1.0/sample.py` & `bitkub-v2-2.1.1/sample.py`

 * *Files identical despite different names*

### Comparing `bitkub-v2-2.1.0/setup.py` & `bitkub-v2-2.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='bitkub-v2',
-    version='2.1.0',
+    version='2.1.1',
     description='A Python library for Bitkub API v2',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/appcorner/bitkub',
     author='appcorner',
     author_email='appcorner@yahoo.com',
     license='MIT',
     scripts=[],
     keywords=['bitkub', 'bitkub-python', 'bitkub-python-sdk'],
-    packages=['bitkub-v2'],
+    packages=['bitkub'],
     install_requires=['requests'],
 )
```

