# Comparing `tmp/Products.isurlinportal-2.0.0.tar.gz` & `tmp/Products.isurlinportal-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.isurlinportal-2.0.0.tar", last modified: Tue Mar 14 16:05:48 2023, max compression
+gzip compressed data, was "Products.isurlinportal-2.0.1.tar", last modified: Wed Apr 19 21:04:08 2023, max compression
```

## Comparing `Products.isurlinportal-2.0.0.tar` & `Products.isurlinportal-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:05:48.941651 Products.isurlinportal-2.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)     1584 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      111 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     9215 2023-03-14 16:05:48.941799 Products.isurlinportal-2.0.0/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:05:48.938169 Products.isurlinportal-2.0.0/Products/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:05:48.941332 Products.isurlinportal-2.0.0/Products/isurlinportal/
--rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products/isurlinportal/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     9152 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products/isurlinportal/tests.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:05:48.940655 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9215 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      485 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6872 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      136 2023-03-14 16:05:48.942421 Products.isurlinportal-2.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1303 2023-03-14 16:05:48.000000 Products.isurlinportal-2.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-19 21:04:08.162752 Products.isurlinportal-2.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      111 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     9345 2023-04-19 21:04:08.162859 Products.isurlinportal-2.0.1/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-19 21:04:08.159968 Products.isurlinportal-2.0.1/Products/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/Products/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-19 21:04:08.162555 Products.isurlinportal-2.0.1/Products/isurlinportal/
+-rw-r--r--   0 maurits    (501) staff       (20)     7157 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/Products/isurlinportal/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9152 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/Products/isurlinportal/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-19 21:04:08.162046 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     9345 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      485 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       48 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-04-19 21:04:08.000000 Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6872 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-19 21:04:08.163348 Products.isurlinportal-2.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-04-19 21:04:07.000000 Products.isurlinportal-2.0.1/setup.py
```

### Comparing `Products.isurlinportal-2.0.0/CHANGES.rst` & `Products.isurlinportal-2.0.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-19)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 2.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2 and lower.
```

### Comparing `Products.isurlinportal-2.0.0/PKG-INFO` & `Products.isurlinportal-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.isurlinportal
-Version: 2.0.0
+Version: 2.0.1
 Summary: Replacement for isURLInPortal method in Plone
 Home-page: https://github.org/plone/Products.isurlinportal
 Author: Plone Security Team
 Author-email: security@plone.org
 License: GPL
 Keywords: plone security hotfix patch
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: test
 
 isURLInPortal patch for Plone
 =============================
 
 This patches the ``isURLInPortal`` method in Plone.
 The method is in ``Products.CMFPlone/URLTool.py`` in the ``URLTool`` class.
 Basic use in a page template is::
@@ -178,14 +179,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-19)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 2.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2 and lower.
```

### Comparing `Products.isurlinportal-2.0.0/Products/isurlinportal/__init__.py` & `Products.isurlinportal-2.0.1/Products/isurlinportal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from html import unescape
 from plone.base.interfaces import ILoginSchema
 from plone.registry.interfaces import IRegistry
 from posixpath import normpath
+
 # This is the class we will patch:
 from Products.CMFPlone.URLTool import URLTool
 from urllib.parse import urljoin
 from urllib.parse import urlparse
 from zope.component import getUtility
 
 import re
```

### Comparing `Products.isurlinportal-2.0.0/Products/isurlinportal/tests.py` & `Products.isurlinportal-2.0.1/Products/isurlinportal/tests.py`

 * *Files identical despite different names*

### Comparing `Products.isurlinportal-2.0.0/Products.isurlinportal.egg-info/PKG-INFO` & `Products.isurlinportal-2.0.1/Products.isurlinportal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.isurlinportal
-Version: 2.0.0
+Version: 2.0.1
 Summary: Replacement for isURLInPortal method in Plone
 Home-page: https://github.org/plone/Products.isurlinportal
 Author: Plone Security Team
 Author-email: security@plone.org
 License: GPL
 Keywords: plone security hotfix patch
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: test
 
 isURLInPortal patch for Plone
 =============================
 
 This patches the ``isURLInPortal`` method in Plone.
 The method is in ``Products.CMFPlone/URLTool.py`` in the ``URLTool`` class.
 Basic use in a page template is::
@@ -178,14 +179,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-19)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 2.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2 and lower.
```

### Comparing `Products.isurlinportal-2.0.0/README.rst` & `Products.isurlinportal-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Products.isurlinportal-2.0.0/setup.py` & `Products.isurlinportal-2.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("CHANGES.rst") as myfile:
     changes = myfile.read()
 long_description = readme + "\n" + changes
 
 
 setup(
     name="Products.isurlinportal",
-    version="2.0.0",
+    version="2.0.1",
     description="Replacement for isURLInPortal method in Plone",
     long_description=long_description,
     # Get more strings from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
@@ -32,9 +32,17 @@
     url="https://github.org/plone/Products.isurlinportal",
     license="GPL",
     packages=find_packages(),
     namespace_packages=["Products"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
-    install_requires=["setuptools"],
+    install_requires=[
+        "setuptools",
+        "plone.base",
+    ],
+    extras_require={
+        "test": [
+            "Products.CMFPlone",
+        ]
+    },
 )
```

