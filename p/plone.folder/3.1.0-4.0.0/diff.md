# Comparing `tmp/plone.folder-3.1.0.tar.gz` & `tmp/plone.folder-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.folder-3.1.0.tar", last modified: Tue Jun 15 01:26:48 2021, max compression
+gzip compressed data, was "plone.folder-4.0.0.tar", last modified: Wed Apr 19 07:18:30 2023, max compression
```

## Comparing `plone.folder-3.1.0.tar` & `plone.folder-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.337190 plone.folder-3.1.0/
--rw-r--r--   0 ems174     (502) staff       (20)     6055 2021-06-15 01:26:48.000000 plone.folder-3.1.0/CHANGES.rst
--rw-r--r--   0 ems174     (502) staff       (20)       70 2021-06-15 01:26:48.000000 plone.folder-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 ems174     (502) staff       (20)      171 2021-06-15 01:26:48.000000 plone.folder-3.1.0/MANIFEST.in
--rw-r--r--   0 ems174     (502) staff       (20)    12788 2021-06-15 01:26:48.337286 plone.folder-3.1.0/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)     2631 2021-06-15 01:26:48.000000 plone.folder-3.1.0/README.rst
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.333911 plone.folder-3.1.0/docs/
--rw-r--r--   0 ems174     (502) staff       (20)    15220 2021-06-15 01:26:48.000000 plone.folder-3.1.0/docs/LICENSE.GPL
--rw-r--r--   0 ems174     (502) staff       (20)      674 2021-06-15 01:26:48.000000 plone.folder-3.1.0/docs/LICENSE.txt
--rw-r--r--   0 ems174     (502) staff       (20)      397 2021-06-15 01:26:48.000000 plone.folder-3.1.0/pyproject.toml
--rw-r--r--   0 ems174     (502) staff       (20)      116 2021-06-15 01:26:48.337547 plone.folder-3.1.0/setup.cfg
--rw-r--r--   0 ems174     (502) staff       (20)     1855 2021-06-15 01:26:48.000000 plone.folder-3.1.0/setup.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.332777 plone.folder-3.1.0/src/
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.334008 plone.folder-3.1.0/src/plone/
--rw-r--r--   0 ems174     (502) staff       (20)       80 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/__init__.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.335639 plone.folder-3.1.0/src/plone/folder/
--rw-r--r--   0 ems174     (502) staff       (20)       24 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/__init__.py
--rw-r--r--   0 ems174     (502) staff       (20)      316 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/configure.zcml
--rw-r--r--   0 ems174     (502) staff       (20)     6455 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/default.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.335774 plone.folder-3.1.0/src/plone/folder/dtml/
--rw-r--r--   0 ems174     (502) staff       (20)     1263 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/dtml/addGopipIndex.dtml
--rw-r--r--   0 ems174     (502) staff       (20)     2765 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/interfaces.py
--rw-r--r--   0 ems174     (502) staff       (20)     4306 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/nogopip.py
--rw-r--r--   0 ems174     (502) staff       (20)     9376 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/ordered.py
--rw-r--r--   0 ems174     (502) staff       (20)     6298 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/partial.py
--rw-r--r--   0 ems174     (502) staff       (20)      729 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/testing.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.337076 plone.folder-3.1.0/src/plone/folder/tests/
--rw-r--r--   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/__init__.py
--rw-r--r--   0 ems174     (502) staff       (20)     1025 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/benchmarks.py
--rw-r--r--   0 ems174     (502) staff       (20)     3197 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_dict_interface.py
--rw-r--r--   0 ems174     (502) staff       (20)     1091 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_integration.py
--rw-r--r--   0 ems174     (502) staff       (20)     1447 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_ordering_adapters.py
--rw-r--r--   0 ems174     (502) staff       (20)    15355 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_ordersupport.py
--rw-r--r--   0 ems174     (502) staff       (20)    11927 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_partialordering.py
--rw-r--r--   0 ems174     (502) staff       (20)     1780 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_unorderedordering.py
--rw-r--r--   0 ems174     (502) staff       (20)     1592 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/test_webdav.py
--rw-r--r--   0 ems174     (502) staff       (20)      599 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/tests/utils.py
--rw-r--r--   0 ems174     (502) staff       (20)      685 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone/folder/unordered.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:26:48.334758 plone.folder-3.1.0/src/plone.folder.egg-info/
--rw-r--r--   0 ems174     (502) staff       (20)    12788 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)     1151 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/SOURCES.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/dependency_links.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/namespace_packages.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/not-zip-safe
--rw-r--r--   0 ems174     (502) staff       (20)      174 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/requires.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:26:48.000000 plone.folder-3.1.0/src/plone.folder.egg-info/top_level.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.980250 plone.folder-4.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6230 2023-04-19 07:18:30.000000 plone.folder-4.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-19 07:18:30.000000 plone.folder-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      171 2023-04-19 07:18:30.000000 plone.folder-4.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    10007 2023-04-19 07:18:30.980250 plone.folder-4.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2631 2023-04-19 07:18:30.000000 plone.folder-4.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.976250 plone.folder-4.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-19 07:18:30.000000 plone.folder-4.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      674 2023-04-19 07:18:30.000000 plone.folder-4.0.0/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2913 2023-04-19 07:18:30.000000 plone.folder-4.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-19 07:18:30.980250 plone.folder-4.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1725 2023-04-19 07:18:30.000000 plone.folder-4.0.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.975250 plone.folder-4.0.0/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.977250 plone.folder-4.0.0/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.978250 plone.folder-4.0.0/src/plone/folder/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      326 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6259 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/default.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.978250 plone.folder-4.0.0/src/plone/folder/dtml/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1263 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/dtml/addGopipIndex.dtml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2656 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4197 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/nogopip.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9029 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/ordered.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6200 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/partial.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      696 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.979250 plone.folder-4.0.0/src/plone/folder/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      973 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/benchmarks.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3158 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_dict_interface.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1059 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_integration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1421 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_ordering_adapters.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14914 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_ordersupport.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    11579 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_partialordering.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1621 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_unorderedordering.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1542 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/test_webdav.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      562 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/tests/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      651 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone/folder/unordered.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:18:30.977250 plone.folder-4.0.0/src/plone.folder.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    10007 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1151 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:18:30.000000 plone.folder-4.0.0/src/plone.folder.egg-info/top_level.txt
```

### Comparing `plone.folder-3.1.0/CHANGES.rst` & `plone.folder-4.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2023-04-19)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5cc689e5)
+
+
 3.1.0 (2021-06-14)
 ------------------
 
 New features:
 
 
 - Restore webdav support [frapell] (#16)
@@ -289,15 +306,15 @@
 - Add ``__getitem__``, needed when not using the CMF mix-in.
   [optilude]
 
 - Added ``__setitem__``, ``__contains__`` and ``__delitem__`` to support a
   dict-like API.
   [optilude]
 
-- Fix issue with removing non-orderable content for partial ordering suppport.
+- Fix issue with removing non-orderable content for partial ordering support.
   [witsch]
 
 - Fix ``getObjectPosition`` to return a value representing "no position" for
   non-orderable content instead of raising an error.
   [witsch]
 
 - Fix boolean value of the btree-based folder base class.
```

### Comparing `plone.folder-3.1.0/README.rst` & `plone.folder-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.folder-3.1.0/docs/LICENSE.GPL` & `plone.folder-4.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.folder-3.1.0/docs/LICENSE.txt` & `plone.folder-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.folder-3.1.0/setup.py` & `plone.folder-4.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-version = '3.1.0'
+
+version = "4.0.0"
 
 setup(
-    name='plone.folder',
+    name="plone.folder",
     version=version,
-    description='BTree-based folder implementation with order support',
-    long_description=(open("README.rst").read() + "\n" +
-                      open("CHANGES.rst").read()),
+    description="BTree-based folder implementation with order support",
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope2",
         "Framework :: Zope :: 4",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords='folder btree order',
-    author='Plone Foundation',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://pypi.org/project/plone.folder',
-    license='GPL version 2',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    namespace_packages=['plone'],
+    keywords="folder btree order",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/plone.folder",
+    license="GPL version 2",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    namespace_packages=["plone"],
     include_package_data=True,
-    platforms='Any',
+    platforms="Any",
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        'plone.memoize',
-        'Products.BTreeFolder2',
-        'Products.CMFCore',
-        'Products.ZCatalog',
-        'setuptools',
-        'six',
-        'zope.annotation',
-        'zope.component',
-        'zope.container',
-        'zope.interface',
-        'Zope2',
+        "Products.CMFCore",
+        "Products.ZCatalog",
+        "setuptools",
     ],
     extras_require={
-        'test': [
-            'profilehooks',
+        "test": [
+            "plone.app.testing",
+            "profilehooks",
         ]
     },
 )
```

### Comparing `plone.folder-3.1.0/src/plone/folder/default.py` & `plone.folder-4.0.0/src/plone/folder/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,62 @@
-# -*- coding: utf-8 -*-
 from BTrees.OIBTree import OIBTree
 from persistent.list import PersistentList
 from plone.folder.interfaces import IExplicitOrdering
 from plone.folder.interfaces import IOrderableFolder
 from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
 from zope.container.contained import notifyContainerModified
 from zope.interface import implementer
 
-import six
-
 
 @implementer(IExplicitOrdering)
 @adapter(IOrderableFolder)
-class DefaultOrdering(object):
-    """ This implementation uses annotations to store the order on the
-        object, and supports explicit ordering. """
+class DefaultOrdering:
+    """This implementation uses annotations to store the order on the
+    object, and supports explicit ordering."""
 
     ORDER_KEY = "plone.folder.ordered.order"
     POS_KEY = "plone.folder.ordered.pos"
 
     def __init__(self, context):
         self.context = context
 
     def notifyAdded(self, obj_id):
-        """ see interfaces.py """
+        """see interfaces.py"""
         order = self._order(True)
         pos = self._pos(True)
         order.append(obj_id)
         pos[obj_id] = len(order) - 1
 
     def notifyRemoved(self, obj_id):
-        """ see interfaces.py """
+        """see interfaces.py"""
         order = self._order()
         pos = self._pos()
         try:
             idx = pos[obj_id]
             del order[idx]
         except KeyError:
             pass
         # we now need to rebuild pos since the ids have shifted
         pos.clear()
         for count, obj_id in enumerate(order):
             pos[obj_id] = count
 
-    def moveObjectsByDelta(
-        self,
-        ids,
-        delta,
-        subset_ids=None,
-        suppress_events=False
-    ):
-        """ see interfaces.py """
+    def moveObjectsByDelta(self, ids, delta, subset_ids=None, suppress_events=False):
+        """see interfaces.py"""
         order = self._order()
         pos = self._pos()
         min_position = 0
-        if isinstance(ids, six.string_types):
+        if isinstance(ids, str):
             ids = [ids]
         if subset_ids is None:
             subset_ids = self.idsInOrder()
         elif not isinstance(subset_ids, list):
             subset_ids = list(subset_ids)
-        if delta > 0:                   # unify moving direction
+        if delta > 0:  # unify moving direction
             ids = reversed(ids)
             subset_ids.reverse()
         counter = 0
         for obj_id in ids:
             try:
                 old_position = subset_ids.index(obj_id)
             except ValueError:
@@ -90,80 +81,81 @@
                     continue
                 obj_id = subset_ids[idx]
                 try:
                     order[i] = obj_id
                     pos[obj_id] = i
                     idx += 1
                 except KeyError:
-                    raise ValueError(
-                        'No object with id "{0:s}" exists.'.format(obj_id)
-                    )
+                    raise ValueError(f'No object with id "{obj_id:s}" exists.')
         if not suppress_events:
             notifyContainerModified(self.context)
         return counter
 
     def moveObjectsUp(self, ids, delta=1, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, -delta, subset_ids)
 
     def moveObjectsDown(self, ids, delta=1, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, delta, subset_ids)
 
     def moveObjectsToTop(self, ids, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, -len(self._order()), subset_ids)
 
     def moveObjectsToBottom(self, ids, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, len(self._order()), subset_ids)
 
     def moveObjectToPosition(self, obj_id, position, suppress_events=False):
-        """ see interfaces.py """
+        """see interfaces.py"""
         delta = position - self.getObjectPosition(obj_id)
         if delta:
             return self.moveObjectsByDelta(
-                obj_id,
-                delta,
-                suppress_events=suppress_events
+                obj_id, delta, suppress_events=suppress_events
             )
 
     def orderObjects(self, key=None, reverse=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         if key is None and not reverse:
             return -1
         order = self._order()
         pos = self._pos()
 
         if key is None and reverse:
             # Simply reverse the current ordering.
             order.reverse()
         else:
+
             def keyfn(obj_id):
                 attr = getattr(self.context._getOb(obj_id), key)
                 if callable(attr):
                     return attr()
                 return attr
+
             # order.sort(cmd=None, key=keyfn, reverse=bool(reverse))
             order = sorted(order, key=keyfn, reverse=bool(reverse))
             self._set_order(order)
         for n, obj_id in enumerate(order):
             pos[obj_id] = n
         return -1
 
     def getObjectPosition(self, obj_id):
-        """ see interfaces.py """
+        """see interfaces.py"""
         pos = self._pos()
         if obj_id in pos:
             return pos[obj_id]
-        raise ValueError('No object with id "{0:s}" exists in "{1:s}".'.format(
-            obj_id, '/'.join(self.context.getPhysicalPath())))
+        raise ValueError(
+            'No object with id "{:s}" exists in "{:s}".'.format(
+                obj_id, "/".join(self.context.getPhysicalPath())
+            )
+        )
 
     def idsInOrder(self):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return list(self._order())
 
     def __getitem__(self, index):
         return self._order()[index]
 
     # Annotation lookup with lazy creation
```

### Comparing `plone.folder-3.1.0/src/plone/folder/dtml/addGopipIndex.dtml` & `plone.folder-4.0.0/src/plone/folder/dtml/addGopipIndex.dtml`

 * *Files identical despite different names*

### Comparing `plone.folder-3.1.0/src/plone/folder/interfaces.py` & `plone.folder-4.0.0/src/plone/folder/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Interface
 
 
 class IOrderable(Interface):
-    """ Marker interface for orderable portal content """
+    """Marker interface for orderable portal content"""
 
 
 class IFolder(Interface):
-    """ Marker interface for Plone-like folders """
+    """Marker interface for Plone-like folders"""
 
 
 class IOrderableFolder(IFolder):
-    """ A Plone-like folder with ordering support """
+    """A Plone-like folder with ordering support"""
 
     def getOrdering():
-        """ return the currently active ordering adapter for this folder """
+        """return the currently active ordering adapter for this folder"""
 
-    def setOrdering(ordering=u''):
-        """ (re)set ordering adapter to be used for this folder """
+    def setOrdering(ordering=""):
+        """(re)set ordering adapter to be used for this folder"""
 
 
 class IOrdering(Interface):
-    """ An adapter providing ordering operations on its context folder.
+    """An adapter providing ordering operations on its context folder.
 
-        The OrderedBTreeFolderBase mix-in class will adapt self (the
-        folder) to this interface when trying to get object position or
-        find the order of items. There is a default implementation, but
-        you can provide a different policy.
-
-        Your adapter (which should still adapt to IOrdered) can
-        optionally provide IExplicitOrdering, defined below. This is
-        used to support explicit ordering, e.g. through a UI. """
+    The OrderedBTreeFolderBase mix-in class will adapt self (the
+    folder) to this interface when trying to get object position or
+    find the order of items. There is a default implementation, but
+    you can provide a different policy.
+
+    Your adapter (which should still adapt to IOrdered) can
+    optionally provide IExplicitOrdering, defined below. This is
+    used to support explicit ordering, e.g. through a UI."""
 
     def notifyAdded(obj_id):
-        """ Inform the ordering implementation that an item was added """
+        """Inform the ordering implementation that an item was added"""
 
     def notifyRemoved(obj_id):
-        """ Inform the ordering implementation that an item was removed """
+        """Inform the ordering implementation that an item was removed"""
 
     def getObjectPosition(obj_id):
-        """ Get the position of the given object id """
+        """Get the position of the given object id"""
 
     def idsInOrder():
-        """ Return all object ids, in the correct order """
+        """Return all object ids, in the correct order"""
 
 
 class IExplicitOrdering(IOrdering):
-    """ An adapter allowing explicit ordering """
+    """An adapter allowing explicit ordering"""
 
     def moveObjectsByDelta(ids, delta, subset_ids=None, suppress_events=False):
-        """ Move the specified ids (a sequence, or a single string id)
-            by the given delta (a positive or negative number). By
-            default, this moves the objects within the whole set of
-            sub-items in the context container, but if subset_ids is
-            specified, it gives a subset of ids to consider.
-            Should return the number of objects that changed position. """
+        """Move the specified ids (a sequence, or a single string id)
+        by the given delta (a positive or negative number). By
+        default, this moves the objects within the whole set of
+        sub-items in the context container, but if subset_ids is
+        specified, it gives a subset of ids to consider.
+        Should return the number of objects that changed position."""
 
     def moveObjectsUp(ids, delta=1, subset_ids=None):
-        """ Move specified sub-objects up by delta in container. """
+        """Move specified sub-objects up by delta in container."""
 
     def moveObjectsDown(ids, delta=1, subset_ids=None):
-        """ Move specified sub-objects down by delta in container. """
+        """Move specified sub-objects down by delta in container."""
 
     def moveObjectsToTop(ids, subset_ids=None):
-        """ Move specified sub-objects to top of container. """
+        """Move specified sub-objects to top of container."""
 
     def moveObjectsToBottom(ids, subset_ids=None):
-        """ Move specified sub-objects to bottom of container. """
+        """Move specified sub-objects to bottom of container."""
 
     def moveObjectToPosition(obj_id, position, suppress_events=False):
-        """ Move specified object to absolute position. """
+        """Move specified object to absolute position."""
 
     def orderObjects(key, reverse=None):
-        """ Order sub-objects by key and direction. """
+        """Order sub-objects by key and direction."""
```

### Comparing `plone.folder-3.1.0/src/plone/folder/nogopip.py` & `plone.folder-4.0.0/src/plone/folder/nogopip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from App.special_dtml import DTMLFile
 from inspect import currentframe
 from logging import getLogger
 from OFS.SimpleItem import SimpleItem
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.PluginIndexes.interfaces import IPluggableIndex
 from Products.PluginIndexes.interfaces import ISortIndex
 from zope.component import getUtility
 from zope.interface import implementer
 
+
 logger = getLogger(__name__)
 
 
 def traverse(base, path):
     """simplified fast unrestricted traverse.
     base: the app-root to start from
     path: absolute path from app root as string
     returns: content at the end or None
     """
     current = base
-    for cid in path.split('/'):
+    for cid in path.split("/"):
         if not cid:
             continue
         try:
             current = current[cid]
         except KeyError:
             return None
     return current
 
 
 @implementer(IPluggableIndex)
 class StubIndex(SimpleItem):
-    """ stub catalog index doing nothing """
+    """stub catalog index doing nothing"""
 
     def __init__(self, id, *args, **kw):
         self.id = id
 
     def getId(self):
         return self.id
 
@@ -60,86 +60,76 @@
 
     def clear(self):
         pass
 
 
 @implementer(ISortIndex)
 class GopipIndex(StubIndex):
-    """ fake index for sorting against `getObjPositionInParent` """
+    """fake index for sorting against `getObjPositionInParent`"""
 
-    meta_type = 'GopipIndex'
-    manage_options = dict(label='Settings', action='manage_main'),
+    meta_type = "GopipIndex"
+    manage_options = (dict(label="Settings", action="manage_main"),)
 
     keyForDocument = 42
 
     def __init__(self, id, extra=None, caller=None):
-        super(GopipIndex, self).__init__(id)
+        super().__init__(id)
         self.catalog = aq_base(caller._catalog)
 
     def __len__(self):
         # with python 2.4 returning `sys.maxint` gives:
         # OverflowError: __len__() should return 0 <= outcome < 2**31
         # so...
         return 2**31 - 1
 
     def documentToKeyMap(self):
         # we need to get the containers in order to get the respective
         # positions of the search results, but before that we need those
         # results themselves.  luckily this is only ever called from
         # `sortResults`, so we can get it form there.  oh, and lurker
         # says this won't work in jython, though! :)
-        rs = currentframe().f_back.f_locals['rs']
+        rs = currentframe().f_back.f_locals["rs"]
         rids = {}
         items = []
         containers = {}
         getpath = self.catalog.paths.get
         root = getUtility(ISiteRoot).getPhysicalRoot()
         for rid in rs:
             path = getpath(rid)
-            parent, id = path.rsplit('/', 1)
+            parent, id = path.rsplit("/", 1)
             container = containers.get(parent)
             if container is None:
                 containers[parent] = container = traverse(root, parent)
-            rids[id] = rid              # remember in case of single folder
+            rids[id] = rid  # remember in case of single folder
             items.append((rid, container, id))  # or else for deferred lookup
         pos = {}
         if len(containers) == 1:
             # the usual "all from one folder" case can be optimized
             folder = list(containers.values())[0]
-            if getattr(aq_base(folder), 'getOrdering', None):
+            if getattr(aq_base(folder), "getOrdering", None):
                 ids = folder.getOrdering().idsInOrder()
             else:
                 # site root or old folders
                 ids = folder.objectIds()
             for idx, id in enumerate(ids):
                 rid = rids.get(id)
                 if rid:
                     pos[rid] = idx
             return pos
         # otherwise the entire map needs to be constructed...
         for rid, container, id in items:
-            if getattr(aq_base(container), 'getObjectPosition', None):
+            if getattr(aq_base(container), "getObjectPosition", None):
                 pos[rid] = container.getObjectPosition(id)
             else:
                 # fallback for unordered folders
                 pos[rid] = 0
         return pos
 
 
-manage_addGopipForm = DTMLFile('dtml/addGopipIndex', globals())
+manage_addGopipForm = DTMLFile("dtml/addGopipIndex", globals())
 
 
-def manage_addGopipIndex(
-    self,
-    identifier,
-    REQUEST=None,
-    RESPONSE=None,
-    URL3=None
-):
-    """ add a fake gopip index """
+def manage_addGopipIndex(self, identifier, REQUEST=None, RESPONSE=None, URL3=None):
+    """add a fake gopip index"""
     return self.manage_addIndex(
-        identifier,
-        'GopipIndex',
-        REQUEST=REQUEST,
-        RESPONSE=RESPONSE,
-        URL1=URL3
+        identifier, "GopipIndex", REQUEST=REQUEST, RESPONSE=RESPONSE, URL1=URL3
     )
```

### Comparing `plone.folder-3.1.0/src/plone/folder/ordered.py` & `plone.folder-4.0.0/src/plone/folder/ordered.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from AccessControl import ClassSecurityInfo
 from AccessControl.Permissions import access_contents_information
 from AccessControl.Permissions import manage_properties
 from OFS.interfaces import IOrderedContainer
 from plone.folder.interfaces import IExplicitOrdering
 from plone.folder.interfaces import IOrderableFolder
 from plone.folder.interfaces import IOrdering
@@ -10,14 +9,16 @@
 from Products.BTreeFolder2.BTreeFolder2 import BTreeFolder2Base
 from Products.CMFCore.permissions import ModifyPortalContent
 from Products.CMFCore.PortalFolder import PortalFolderBase
 from zope.annotation.interfaces import IAttributeAnnotatable
 from zope.component import getAdapter
 from zope.component import queryAdapter
 from zope.interface import implementer
+
+
 try:
     from ZTUtils.Lazy import LazyMap
 except ImportError:
     # bbb import for Zope2
     from Products.ZCatalog.Lazy import LazyMap
 
 HAS_WEBDAV = True
@@ -25,69 +26,69 @@
     from webdav.NullResource import NullResource
 except ImportError:
     HAS_WEBDAV = False
 
 
 @implementer(IOrderedContainer, IOrderableFolder, IAttributeAnnotatable)
 class OrderedBTreeFolderBase(BTreeFolder2Base):
-    """ BTree folder base class with ordering support. The ordering
-        is done by a named adapter (to IOrdering), which makes the policy
-        changeable. """
+    """BTree folder base class with ordering support. The ordering
+    is done by a named adapter (to IOrdering), which makes the policy
+    changeable."""
 
-    _ordering = u''         # name of adapter defining ordering policy
+    _ordering = ""  # name of adapter defining ordering policy
 
     security = ClassSecurityInfo()
 
     def __bool__(self):
-        """ a folder is something, even if it's empty """
+        """a folder is something, even if it's empty"""
         return True
 
     @security.protected(access_contents_information)
     def getOrdering(self):
-        """ return the currently active ordering adapter for this folder """
+        """return the currently active ordering adapter for this folder"""
         adapter = queryAdapter(self, IOrdering, name=self._ordering)
         if adapter is None:
             adapter = getAdapter(self, IOrdering)
         return adapter
 
     @security.protected(manage_properties)
-    def setOrdering(self, ordering=u''):
-        """ (re)set ordering adapter to be used for this folder """
+    def setOrdering(self, ordering=""):
+        """(re)set ordering adapter to be used for this folder"""
         if ordering:
             # make sure the adapter exists...
             getAdapter(self, IOrdering, name=ordering)
         self._ordering = ordering
 
     # IObjectManager
 
     def _getOb(self, id, default=_marker):
-        """ Return the named object from the folder. """
+        """Return the named object from the folder."""
         try:
-            return super(OrderedBTreeFolderBase, self)._getOb(id, default)
+            return super()._getOb(id, default)
         except KeyError as e:
             raise AttributeError(e)
 
     def _setOb(self, id, object):
-        """ Store the named object in the folder. """
-        super(OrderedBTreeFolderBase, self)._setOb(id, object)
-        self.getOrdering().notifyAdded(id)     # notify the ordering adapter
+        """Store the named object in the folder."""
+        super()._setOb(id, object)
+        self.getOrdering().notifyAdded(id)  # notify the ordering adapter
 
     def _delOb(self, id):
-        """ Remove the named object from the folder. """
-        super(OrderedBTreeFolderBase, self)._delOb(id)
-        self.getOrdering().notifyRemoved(id)   # notify the ordering adapter
+        """Remove the named object from the folder."""
+        super()._delOb(id)
+        self.getOrdering().notifyRemoved(id)  # notify the ordering adapter
 
     def objectIds(self, spec=None, ordered=True):
         if not ordered:
-            return super(OrderedBTreeFolderBase, self).objectIds(spec)
+            return super().objectIds(spec)
         ordering = self.getOrdering()
         if spec is None:
             return ordering.idsInOrder()
         else:
-            ids = super(OrderedBTreeFolderBase, self).objectIds(spec)
+            ids = super().objectIds(spec)
             idxs = []
             for id in ids:
                 idxs.append((ordering.getObjectPosition(id), id))
             return [x[1] for x in sorted(idxs, key=lambda a: a[0])]
 
     def objectValues(self, spec=None):
         # Returns a list of actual subobjects of the current object.
@@ -95,122 +96,112 @@
         # match 'spec'.
         return LazyMap(self._getOb, self.objectIds(spec))
 
     def objectItems(self, spec=None):
         # Returns a list of (id, subobject) tuples of the current object.
         # If 'spec' is specified, returns only objects whose meta_type match
         # 'spec'
-        return LazyMap(lambda id, _getOb=self._getOb: (id, _getOb(id)),
-                       self.objectIds(spec))
+        return LazyMap(
+            lambda id, _getOb=self._getOb: (id, _getOb(id)), self.objectIds(spec)
+        )
 
     # IOrderSupport - mostly deprecated, use the adapter directly instead
 
     @security.protected(access_contents_information)
     def getObjectPosition(self, id):
-        """ Get the position of an object by its id. """
+        """Get the position of an object by its id."""
         return self.getOrdering().getObjectPosition(id)
 
     @security.protected(manage_properties)
     def moveObjectsUp(self, ids, delta=1, subset_ids=None):
-        """ Move specified sub-objects up by delta in container. """
+        """Move specified sub-objects up by delta in container."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectsUp(ids, delta, subset_ids)
         else:
             return 0
 
     @security.protected(manage_properties)
     def moveObjectsDown(self, ids, delta=1, subset_ids=None):
-        """ Move specified sub-objects down by delta in container. """
+        """Move specified sub-objects down by delta in container."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectsDown(ids, delta, subset_ids)
         else:
             return 0
 
     @security.protected(manage_properties)
     def moveObjectsToTop(self, ids, subset_ids=None):
-        """ Move specified sub-objects to top of container. """
+        """Move specified sub-objects to top of container."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectsToTop(ids, subset_ids)
         else:
             return 0
 
     @security.protected(manage_properties)
     def moveObjectsToBottom(self, ids, subset_ids=None):
-        """ Move specified sub-objects to bottom of container. """
+        """Move specified sub-objects to bottom of container."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectsToBottom(ids, subset_ids)
         else:
             return 0
 
     @security.protected(ModifyPortalContent)
     def moveObject(self, id, position):
-        """ Move specified object to absolute position. """
+        """Move specified object to absolute position."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectToPosition(id, position)
         else:
             return 0
 
     @security.protected(manage_properties)
     def moveObjectToPosition(self, id, position, suppress_events=False):
-        """ Move specified object to absolute position. """
+        """Move specified object to absolute position."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.moveObjectToPosition(id, position, suppress_events)
         else:
             return 0
 
     @security.protected(manage_properties)
-    def moveObjectsByDelta(
-        self, ids, delta, subset_ids=None, suppress_events=False
-    ):
-        """ Move specified sub-objects by delta. """
+    def moveObjectsByDelta(self, ids, delta, subset_ids=None, suppress_events=False):
+        """Move specified sub-objects by delta."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
-            return ordering.moveObjectsByDelta(
-                ids,
-                delta,
-                subset_ids,
-                suppress_events
-            )
+            return ordering.moveObjectsByDelta(ids, delta, subset_ids, suppress_events)
         else:
             return 0
 
     @security.protected(manage_properties)
     def orderObjects(self, key=None, reverse=None):
-        """ Order sub-objects by key and direction. """
+        """Order sub-objects by key and direction."""
         ordering = self.getOrdering()
         if IExplicitOrdering.providedBy(ordering):
             return ordering.orderObjects(key, reverse)
         else:
             return 0
 
     # Overrides for Plone-ish behaviour
 
     def iterkeys(self):
         return iter(self.objectIds())
 
     def manage_renameObject(self, id, new_id, REQUEST=None):
-        """ Rename a particular sub-object without changing its position. """
+        """Rename a particular sub-object without changing its position."""
         old_position = self.getObjectPosition(id)
-        result = super(OrderedBTreeFolderBase, self).manage_renameObject(
-            id,
-            new_id,
-            REQUEST
-        )
+        result = super().manage_renameObject(id, new_id, REQUEST)
         if old_position is None:
             return result
         self.moveObjectToPosition(new_id, old_position, suppress_events=True)
-        reindex = getattr(self._getOb(new_id), 'reindexObject', None)
+        reindex = getattr(self._getOb(new_id), "reindexObject", None)
         if reindex is not None:
-            reindex(idxs=['getObjPositionInParent'])
+            reindex(idxs=["getObjPositionInParent"])
         return result
 
     # Dict interface
 
     def __setitem__(self, key, value):
         self._setObject(key, value)
 
@@ -222,33 +213,36 @@
 
     def __getitem__(self, key):
         value = self._getOb(key, None)
         if value is not None:
             return value
 
         # WebDAV PUT support
-        if hasattr(self, 'REQUEST'):
+        if hasattr(self, "REQUEST"):
             request = self.REQUEST
-            method = request.get('REQUEST_METHOD', 'GET')
-            if (HAS_WEBDAV and getattr(request, 'maybe_webdav_client', False)
-               and method not in ('GET', 'POST')):
+            method = request.get("REQUEST_METHOD", "GET")
+            if (
+                HAS_WEBDAV
+                and getattr(request, "maybe_webdav_client", False)
+                and method not in ("GET", "POST")
+            ):
                 return NullResource(self, key, request).__of__(self)
         raise KeyError(key)
 
     __iter__ = iterkeys
     keys = objectIds
     values = objectValues
     items = objectItems
 
 
 class CMFOrderedBTreeFolderBase(OrderedBTreeFolderBase, PortalFolderBase):
-    """ BTree folder for CMF sites, with ordering support. The ordering
-        is done by adapter (to IOrdering), which makes the policy
-        changeable. """
+    """BTree folder for CMF sites, with ordering support. The ordering
+    is done by adapter (to IOrdering), which makes the policy
+    changeable."""
 
-    def __init__(self, id, title=''):
+    def __init__(self, id, title=""):
         PortalFolderBase.__init__(self, id, title)
         BTreeFolder2Base.__init__(self, id)
 
     def _checkId(self, id, allow_dup=0):
         PortalFolderBase._checkId(self, id, allow_dup)
         BTreeFolder2Base._checkId(self, id, allow_dup)
```

### Comparing `plone.folder-3.1.0/src/plone/folder/partial.py` & `plone.folder-4.0.0/src/plone/folder/partial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from Acquisition import aq_base
-from zope.interface import implementer
-from zope.component import adapts
-from zope.container.contained import notifyContainerModified
-
+from plone.folder.interfaces import IExplicitOrdering
 from plone.folder.interfaces import IOrderable
 from plone.folder.interfaces import IOrderableFolder
-from plone.folder.interfaces import IExplicitOrdering
-
-import six
+from zope.component import adapts
+from zope.container.contained import notifyContainerModified
+from zope.interface import implementer
 
 
-ORDER_ATTR = '_objectordering'
+ORDER_ATTR = "_objectordering"
 
 
 @implementer(IExplicitOrdering)
-class PartialOrdering(object):
-    """ this implementation uses a list to store order information on a
-        regular attribute of the folderish object;  explicit ordering
-        is supported """
+class PartialOrdering:
+    """this implementation uses a list to store order information on a
+    regular attribute of the folderish object;  explicit ordering
+    is supported"""
+
     adapts(IOrderableFolder)
 
     def __init__(self, context):
         self.context = context
 
     @property
     def order(self):
@@ -35,52 +33,51 @@
         # We added a setter because in py2 order is modified inplace
         # with .sort() while in py3 we sort with sorted and thus need to set it
         # explicitly
         context = aq_base(self.context)
         setattr(context, ORDER_ATTR, value)
 
     def notifyAdded(self, id):
-        """ see interfaces.py """
-        assert not id in self.order
+        """see interfaces.py"""
+        assert id not in self.order
         context = aq_base(self.context)
         obj = context._getOb(id)
         if IOrderable.providedBy(obj):
             self.order.append(id)
-            self.context._p_changed = True      # the order was changed
+            self.context._p_changed = True  # the order was changed
 
     def notifyRemoved(self, id):
-        """ see interfaces.py """
+        """see interfaces.py"""
         try:
             self.order.remove(id)
-            self.context._p_changed = True      # the order was changed
-        except ValueError:          # removing non-orderable items is okay
+            self.context._p_changed = True  # the order was changed
+        except ValueError:  # removing non-orderable items is okay
             pass
 
     def idsInOrder(self, onlyOrderables=False):
-        """ see interfaces.py """
+        """see interfaces.py"""
         ordered = list(self.order)
         ordered_set = set(ordered)
         if not onlyOrderables:
             ids = aq_base(self.context).objectIds(ordered=False)
             for id in ids:
                 if id not in ordered_set:
                     ordered.append(id)
         return ordered
 
-    def moveObjectsByDelta(self, ids, delta, subset_ids=None,
-            suppress_events=False):
-        """ see interfaces.py """
+    def moveObjectsByDelta(self, ids, delta, subset_ids=None, suppress_events=False):
+        """see interfaces.py"""
         min_position = 0
-        if isinstance(ids, six.string_types):
+        if isinstance(ids, str):
             ids = [ids]
         if subset_ids is None:
             subset_ids = self.idsInOrder(onlyOrderables=True)
         elif not isinstance(subset_ids, list):
             subset_ids = list(subset_ids)
-        if delta > 0:                   # unify moving direction
+        if delta > 0:  # unify moving direction
             ids = reversed(ids)
             subset_ids.reverse()
         counter = 0
         for id in ids:
             try:
                 old_position = subset_ids.index(id)
             except ValueError:
@@ -103,64 +100,67 @@
                     id = subset_ids[idx]
                     try:
                         self.order[i] = id
                         idx += 1
                     except KeyError:
                         raise ValueError('No object with id "%s" exists.' % id)
             if idx > 0:
-                self.context._p_changed = True      # the order was changed
+                self.context._p_changed = True  # the order was changed
         if not suppress_events:
             notifyContainerModified(self.context)
         return counter
 
     def moveObjectsUp(self, ids, delta=1, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, -delta, subset_ids)
 
     def moveObjectsDown(self, ids, delta=1, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, delta, subset_ids)
 
     def moveObjectsToTop(self, ids, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, -len(self.order), subset_ids)
 
     def moveObjectsToBottom(self, ids, subset_ids=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         return self.moveObjectsByDelta(ids, len(self.order), subset_ids)
 
     def moveObjectToPosition(self, id, position, suppress_events=False):
-        """ see interfaces.py """
+        """see interfaces.py"""
         old_position = self.getObjectPosition(id)
         if old_position is not None:
             delta = position - old_position
             if delta:
-                return self.moveObjectsByDelta(id, delta,
-                    suppress_events=suppress_events)
+                return self.moveObjectsByDelta(
+                    id, delta, suppress_events=suppress_events
+                )
 
     def orderObjects(self, key=None, reverse=None):
-        """ see interfaces.py """
+        """see interfaces.py"""
         if key is None:
             if not reverse:
                 return -1
             else:
                 # Simply reverse the current ordering.
                 self.order.reverse()
         else:
+
             def keyfn(id):
                 attr = getattr(self.context._getOb(id), key)
                 if callable(attr):
                     return attr()
                 return attr
+
             self.order = sorted(self.order, key=keyfn, reverse=bool(reverse))
-        self.context._p_changed = True      # the order was changed
+        self.context._p_changed = True  # the order was changed
         return -1
 
     def getObjectPosition(self, id):
-        """ see interfaces.py """
+        """see interfaces.py"""
         try:
             # using `index` here might not be that efficient for very large
             # lists, but the idea behind this adapter is to use it when the
             # site contains relatively few "orderable" items
             return self.order.index(id)
         except ValueError:
             # non-orderable objects should return "no position" instead of
```

### Comparing `plone.folder-3.1.0/src/plone/folder/testing.py` & `plone.folder-4.0.0/src/plone/folder/testing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 
 import plone.folder
 
 
 class PloneFolderLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         self.loadZCML(package=plone.folder)
 
 
 PLONEFOLDER_FIXTURE = PloneFolderLayer()
 
 PLONEFOLDER_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(PLONEFOLDER_FIXTURE,),
-    name='PloneFolderLayer:IntegrationTesting'
+    bases=(PLONEFOLDER_FIXTURE,), name="PloneFolderLayer:IntegrationTesting"
 )
 
 PLONEFOLDER_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(PLONEFOLDER_FIXTURE,),
-    name='PloneFolderLayer:FunctionalTesting'
+    bases=(PLONEFOLDER_FIXTURE,), name="PloneFolderLayer:FunctionalTesting"
 )
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_dict_interface.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_dict_interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,86 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from plone.folder.ordered import OrderedBTreeFolderBase
 from plone.folder.testing import PLONEFOLDER_INTEGRATION_TESTING
 from plone.folder.tests.utils import DummyObject
 
 import unittest
 
 
 class DictInterfaceTests(unittest.TestCase):
-    """ tests for dict style interface """
+    """tests for dict style interface"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def test_getitem(self):
         folder = OrderedBTreeFolderBase("f1")
-        foo = DummyObject('foo')
-        folder._setOb('foo', foo)
-        self.assertEqual(folder['foo'], foo)
-        self.assertEqual(folder.__getitem__('foo'), foo)
-        self.assertRaises(KeyError, folder.__getitem__, 'bar')
+        foo = DummyObject("foo")
+        folder._setOb("foo", foo)
+        self.assertEqual(folder["foo"], foo)
+        self.assertEqual(folder.__getitem__("foo"), foo)
+        self.assertRaises(KeyError, folder.__getitem__, "bar")
 
     def test_setitem(self):
         folder = OrderedBTreeFolderBase("f1")
-        foo = DummyObject('foo')
-        folder['foo'] = foo
-        self.assertEqual(folder._getOb('foo'), foo)
+        foo = DummyObject("foo")
+        folder["foo"] = foo
+        self.assertEqual(folder._getOb("foo"), foo)
 
     def test_contains(self):
         folder = OrderedBTreeFolderBase("f1")
-        folder._setOb('foo', DummyObject('foo'))
-        folder._setOb('bar', DummyObject('bar'))
-        self.assertTrue('foo' in folder)
-        self.assertTrue('bar' in folder)
+        folder._setOb("foo", DummyObject("foo"))
+        folder._setOb("bar", DummyObject("bar"))
+        self.assertTrue("foo" in folder)
+        self.assertTrue("bar" in folder)
 
     def test_delitem(self):
         folder = OrderedBTreeFolderBase("f1")
-        folder._setOb('foo', DummyObject('foo'))
-        folder._setOb('bar', DummyObject('bar'))
-        self.assertEquals(len(folder.objectIds()), 2)
-        del folder['foo']
-        del folder['bar']
-        self.assertEquals(len(folder.objectIds()), 0)
+        folder._setOb("foo", DummyObject("foo"))
+        folder._setOb("bar", DummyObject("bar"))
+        self.assertEqual(len(folder.objectIds()), 2)
+        del folder["foo"]
+        del folder["bar"]
+        self.assertEqual(len(folder.objectIds()), 0)
 
     def test_len_empty_folder(self):
         folder = OrderedBTreeFolderBase("f1")
-        self.assertEquals(len(folder), 0)
+        self.assertEqual(len(folder), 0)
 
     def test_len_one_child(self):
         folder = OrderedBTreeFolderBase("f1")
-        folder['child'] = DummyObject('child')
-        self.assertEquals(len(folder), 1)
+        folder["child"] = DummyObject("child")
+        self.assertEqual(len(folder), 1)
 
     def test_to_verify_ticket_9120(self):
         folder = OrderedBTreeFolderBase("f1")
-        folder['ob1'] = ob1 = DummyObject('ob1')
-        folder['ob2'] = DummyObject('ob2')
-        folder['ob3'] = DummyObject('ob3')
-        folder['ob4'] = ob4 = DummyObject('ob4')
-        del folder['ob2']
-        del folder['ob3']
-        self.assertEquals(folder.keys(), ['ob1', 'ob4'])
-        self.assertEquals(list(map(aq_base, folder.values())), [ob1, ob4])
-        self.assertEquals([key in folder for key in folder], [True, True])
+        folder["ob1"] = ob1 = DummyObject("ob1")
+        folder["ob2"] = DummyObject("ob2")
+        folder["ob3"] = DummyObject("ob3")
+        folder["ob4"] = ob4 = DummyObject("ob4")
+        del folder["ob2"]
+        del folder["ob3"]
+        self.assertEqual(folder.keys(), ["ob1", "ob4"])
+        self.assertEqual(list(map(aq_base, folder.values())), [ob1, ob4])
+        self.assertEqual([key in folder for key in folder], [True, True])
 
 
 class RelatedToDictInterfaceTests(unittest.TestCase):
-    """ various tests which are related to the dict-like interface """
+    """various tests which are related to the dict-like interface"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def create(self):
         folder = OrderedBTreeFolderBase("f1")
-        folder._setOb('o1', DummyObject('o1', 'mt1'))
-        folder._setOb('o2', DummyObject('o2', 'mt2'))
-        folder._setOb('o3', DummyObject('o3', 'mt1'))
-        folder._setOb('o4', DummyObject('o4', 'mt2'))
+        folder._setOb("o1", DummyObject("o1", "mt1"))
+        folder._setOb("o2", DummyObject("o2", "mt2"))
+        folder._setOb("o3", DummyObject("o3", "mt1"))
+        folder._setOb("o4", DummyObject("o4", "mt2"))
         return folder
 
     def testObjectIdsWithSpec(self):
         folder = self.create()
-        self.assertEquals(['o1', 'o3'], folder.objectIds(spec='mt1'))
-        self.assertEquals(['o2', 'o4'], folder.objectIds(spec='mt2'))
-        folder.moveObjectsToTop(['o3'])
-        folder.moveObjectsDown(['o2'])
-        self.assertEquals(['o3', 'o1'], folder.objectIds(spec='mt1'))
-        self.assertEquals(['o4', 'o2'], folder.objectIds(spec='mt2'))
+        self.assertEqual(["o1", "o3"], folder.objectIds(spec="mt1"))
+        self.assertEqual(["o2", "o4"], folder.objectIds(spec="mt2"))
+        folder.moveObjectsToTop(["o3"])
+        folder.moveObjectsDown(["o2"])
+        self.assertEqual(["o3", "o1"], folder.objectIds(spec="mt1"))
+        self.assertEqual(["o4", "o2"], folder.objectIds(spec="mt2"))
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_integration.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# -*- coding: utf-8 -*-
 from Acquisition import Implicit
+from io import BytesIO
 from plone.folder.interfaces import IOrderable
 from plone.folder.ordered import OrderedBTreeFolderBase
 from plone.folder.testing import PLONEFOLDER_FUNCTIONAL_TESTING
-from six import BytesIO
 from transaction import savepoint
 from zope.interface import implementer
 
 import unittest
 
 
 @implementer(IOrderable)
 class DummyFolder(OrderedBTreeFolderBase, Implicit):
-    """ we need to mix in acquisition """
+    """we need to mix in acquisition"""
 
-    meta_type = 'DummyFolder'
+    meta_type = "DummyFolder"
 
 
 class IntegrationTests(unittest.TestCase):
-
     layer = PLONEFOLDER_FUNCTIONAL_TESTING
 
     def testExportDoesntIncludeParent(self):
-        self.app = self.layer['app']
-        self.app._setOb('foo', DummyFolder('foo'))
+        self.app = self.layer["app"]
+        self.app._setOb("foo", DummyFolder("foo"))
         foo = self.app.foo
-        foo['bar'] = DummyFolder('bar')
-        savepoint(optimistic=True)      # savepoint assigns oids
+        foo["bar"] = DummyFolder("bar")
+        savepoint(optimistic=True)  # savepoint assigns oids
         # now let's export to a buffer and check the objects...
         exp = BytesIO()
         self.app._p_jar.exportFile(foo.bar._p_oid, exp)
-        self.assertTrue(b'bar' in exp.getvalue())
-        self.assertFalse(b'foo' in exp.getvalue())
+        self.assertTrue(b"bar" in exp.getvalue())
+        self.assertFalse(b"foo" in exp.getvalue())
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_ordering_adapters.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_ordering_adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
 from plone.folder.default import DefaultOrdering
 from plone.folder.ordered import OrderedBTreeFolderBase
 from plone.folder.testing import PLONEFOLDER_INTEGRATION_TESTING
 from plone.folder.unordered import UnorderedOrdering
 from zope.component import ComponentLookupError
 
 import unittest
 
 
 class OrderingAdapterTests(unittest.TestCase):
-    """ tests regarding available ordering adapters """
+    """tests regarding available ordering adapters"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def testDefaultAdapter(self):
         folder = OrderedBTreeFolderBase()
         self.assertTrue(isinstance(folder.getOrdering(), DefaultOrdering))
 
     def testUnorderedOrdering(self):
         folder = OrderedBTreeFolderBase()
-        folder._ordering = 'unordered'
+        folder._ordering = "unordered"
         self.assertTrue(isinstance(folder.getOrdering(), UnorderedOrdering))
 
     def testUnknownOrdering(self):
         folder = OrderedBTreeFolderBase()
-        folder._ordering = 'foo'
+        folder._ordering = "foo"
         self.assertTrue(isinstance(folder.getOrdering(), DefaultOrdering))
 
     def testSetOrdering(self):
         folder = OrderedBTreeFolderBase()
-        folder.setOrdering('unordered')
+        folder.setOrdering("unordered")
         self.assertTrue(isinstance(folder.getOrdering(), UnorderedOrdering))
         folder.setOrdering()
         self.assertTrue(isinstance(folder.getOrdering(), DefaultOrdering))
 
     def testSetUnknownOrdering(self):
         folder = OrderedBTreeFolderBase()
-        self.assertRaises(ComponentLookupError, folder.setOrdering, 'foo')
+        self.assertRaises(ComponentLookupError, folder.setOrdering, "foo")
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_ordersupport.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_ordersupport.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,363 +1,355 @@
-# -*- coding: utf-8 -*-
 from OFS.Traversable import Traversable
 from plone.folder.interfaces import IOrdering
 from plone.folder.ordered import OrderedBTreeFolderBase
 from plone.folder.testing import PLONEFOLDER_INTEGRATION_TESTING
 from plone.folder.tests.utils import DummyObject
 
-import six
 import unittest
 
 
 class TestFolder(OrderedBTreeFolderBase, Traversable):
     """ """
 
     def getId(self):
         return self.id
 
 
 class OFSOrderSupportTests(unittest.TestCase):
-    """ tests borrowed from OFS.tests.testOrderSupport """
+    """tests borrowed from OFS.tests.testOrderSupport"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def create(self):
-        folder = TestFolder('f1')
-        folder['o1'] = DummyObject('o1', 'mt1')
-        folder['o2'] = DummyObject('o2', 'mt2')
-        folder['o3'] = DummyObject('o3', 'mt1')
-        folder['o4'] = DummyObject('o4', 'mt2')
+        folder = TestFolder("f1")
+        folder["o1"] = DummyObject("o1", "mt1")
+        folder["o2"] = DummyObject("o2", "mt2")
+        folder["o3"] = DummyObject("o3", "mt1")
+        folder["o4"] = DummyObject("o4", "mt2")
         return folder
 
     # Test for ordering of basic methods
 
     def test_objectIdsOrdered(self):
         folder = self.create()
-        self.assertEquals(["o1", "o2", "o3", "o4"], folder.objectIds())
+        self.assertEqual(["o1", "o2", "o3", "o4"], folder.objectIds())
         folder.moveObjectsUp(("o2",), 1)
-        self.assertEquals(["o2", "o1", "o3", "o4"], folder.objectIds())
+        self.assertEqual(["o2", "o1", "o3", "o4"], folder.objectIds())
 
     def test_objectValuesOrdered(self):
         folder = self.create()
-        self.assertEquals(
-            ["o1", "o2", "o3", "o4"],
-            [x.id for x in folder.objectValues()]
+        self.assertEqual(
+            ["o1", "o2", "o3", "o4"], [x.id for x in folder.objectValues()]
         )
         folder.moveObjectsUp(("o2",), 1)
-        self.assertEquals(
-            ["o2", "o1", "o3", "o4"],
-            [x.id for x in folder.objectValues()]
+        self.assertEqual(
+            ["o2", "o1", "o3", "o4"], [x.id for x in folder.objectValues()]
         )
 
     def test_objectItemsOrdered(self):
         folder = self.create()
-        self.assertEquals(
-            ["o1", "o2", "o3", "o4"],
-            [x for x, y in folder.objectItems()]
-        )
+        self.assertEqual(["o1", "o2", "o3", "o4"], [x for x, y in folder.objectItems()])
         folder.moveObjectsUp(("o2",), 1)
-        self.assertEquals(
-            ["o2", "o1", "o3", "o4"],
-            [x for x, y in folder.objectItems()]
-        )
+        self.assertEqual(["o2", "o1", "o3", "o4"], [x for x, y in folder.objectItems()])
 
     def test_iterkeys(self):
         folder = self.create()
-        self.assertEquals(
-            ["o1", "o2", "o3", "o4"],
-            [x for x in six.iterkeys(folder)]
-        )
+        self.assertEqual(["o1", "o2", "o3", "o4"], [x for x in folder.keys()])
         folder.moveObjectsUp(("o2",), 1)
-        self.assertEquals(
-            ["o2", "o1", "o3", "o4"],
-            [x for x in six.iterkeys(folder)]
-        )
+        self.assertEqual(["o2", "o1", "o3", "o4"], [x for x in folder.keys()])
 
     def test_iter(self):
         folder = self.create()
-        self.assertEquals(["o1", "o2", "o3", "o4"], [x for x in folder])
+        self.assertEqual(["o1", "o2", "o3", "o4"], [x for x in folder])
         folder.moveObjectsUp(("o2",), 1)
-        self.assertEquals(["o2", "o1", "o3", "o4"], [x for x in folder])
+        self.assertEqual(["o2", "o1", "o3", "o4"], [x for x in folder])
 
     def test_getitem(self):
         ordering = IOrdering(self.create())
-        self.assertEquals(ordering[1], 'o2')
-        self.assertEquals(ordering[-1], 'o4')
-        self.assertEquals(ordering[1:2], ['o2'])
-        self.assertEquals(ordering[1:-1], ['o2', 'o3'])
-        self.assertEquals(ordering[1:], ['o2', 'o3', 'o4'])
+        self.assertEqual(ordering[1], "o2")
+        self.assertEqual(ordering[-1], "o4")
+        self.assertEqual(ordering[1:2], ["o2"])
+        self.assertEqual(ordering[1:-1], ["o2", "o3"])
+        self.assertEqual(ordering[1:], ["o2", "o3", "o4"])
 
     # Tests borrowed from OFS.tests.testsOrderSupport
 
     def runTableTests(self, methodname, table):
         for args, order, rval in table:
             f = self.create()
             method = getattr(f, methodname)
-            if rval == 'ValueError':
+            if rval == "ValueError":
                 self.assertRaises(ValueError, method, *args)
             else:
                 self.assertEqual(method(*args), rval)
             self.assertEqual(f.objectIds(), order)
 
     def test_moveObjectsUp(self):
-        self.runTableTests('moveObjectsUp',
-              ( ( ( 'o4', 1 ),         ['o1', 'o2', 'o4', 'o3'], 1 )
-              , ( ( 'o4', 2 ),         ['o1', 'o4', 'o2', 'o3'], 1 )
-              , ( ( ('o1', 'o3'), 1 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o1', 'o3'), 9 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o2', 'o3'), 1 ), ['o2', 'o3', 'o1', 'o4'], 2 )
-              , ( ( ('o2', 'o3'), 1, ('o1', 'o2', 'o3', 'o4') ),
-                                       ['o2', 'o3', 'o1', 'o4'], 2 )
-              , ( ( ('o2', 'o3'), 1, ('o2', 'o3', 'o4') ),
-                                       ['o1', 'o2', 'o3', 'o4'], 0 )
-              , ( ( ('n2', 'o3'), 1 ), ['o1', 'o3', 'o2', 'o4'], 1)
-              , ( ( ('o3', 'o1'), 1 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              )
-            )
+        self.runTableTests(
+            "moveObjectsUp",
+            (
+                (("o4", 1), ["o1", "o2", "o4", "o3"], 1),
+                (("o4", 2), ["o1", "o4", "o2", "o3"], 1),
+                ((("o1", "o3"), 1), ["o1", "o3", "o2", "o4"], 1),
+                ((("o1", "o3"), 9), ["o1", "o3", "o2", "o4"], 1),
+                ((("o2", "o3"), 1), ["o2", "o3", "o1", "o4"], 2),
+                (
+                    (("o2", "o3"), 1, ("o1", "o2", "o3", "o4")),
+                    ["o2", "o3", "o1", "o4"],
+                    2,
+                ),
+                ((("o2", "o3"), 1, ("o2", "o3", "o4")), ["o1", "o2", "o3", "o4"], 0),
+                ((("n2", "o3"), 1), ["o1", "o3", "o2", "o4"], 1),
+                ((("o3", "o1"), 1), ["o1", "o3", "o2", "o4"], 1),
+            ),
+        )
 
     def test_moveObjectsDown(self):
-        self.runTableTests('moveObjectsDown',
-              ( ( ( 'o1', 1 ),         ['o2', 'o1', 'o3', 'o4'], 1 )
-              , ( ( 'o1', 2 ),         ['o2', 'o3', 'o1', 'o4'], 1 )
-              , ( ( ('o2', 'o4'), 1 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o2', 'o4'), 9 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o2', 'o3'), 1 ), ['o1', 'o4', 'o2', 'o3'], 2 )
-              , ( ( ('o2', 'o3'), 1, ('o1', 'o2', 'o3', 'o4') ),
-                                       ['o1', 'o4', 'o2', 'o3'], 2 )
-              , ( ( ('o2', 'o3'), 1, ('o1', 'o2', 'o3') ),
-                                       ['o1', 'o2', 'o3', 'o4'], 0 )
-              , ( ( ('n2', 'o3'), 1 ), ['o1', 'o2', 'o4', 'o3'], 1)
-              , ( ( ('o4', 'o2'), 1 ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              )
-            )
+        self.runTableTests(
+            "moveObjectsDown",
+            (
+                (("o1", 1), ["o2", "o1", "o3", "o4"], 1),
+                (("o1", 2), ["o2", "o3", "o1", "o4"], 1),
+                ((("o2", "o4"), 1), ["o1", "o3", "o2", "o4"], 1),
+                ((("o2", "o4"), 9), ["o1", "o3", "o2", "o4"], 1),
+                ((("o2", "o3"), 1), ["o1", "o4", "o2", "o3"], 2),
+                (
+                    (("o2", "o3"), 1, ("o1", "o2", "o3", "o4")),
+                    ["o1", "o4", "o2", "o3"],
+                    2,
+                ),
+                ((("o2", "o3"), 1, ("o1", "o2", "o3")), ["o1", "o2", "o3", "o4"], 0),
+                ((("n2", "o3"), 1), ["o1", "o2", "o4", "o3"], 1),
+                ((("o4", "o2"), 1), ["o1", "o3", "o2", "o4"], 1),
+            ),
+        )
 
     def test_moveObjectsToTop(self):
-        self.runTableTests('moveObjectsToTop',
-              ( ( ( 'o4', ),         ['o4', 'o1', 'o2', 'o3'], 1 )
-              , ( ( ('o1', 'o3'), ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o2', 'o3'), ), ['o2', 'o3', 'o1', 'o4'], 2 )
-              , ( ( ('o2', 'o3'), ('o1', 'o2', 'o3', 'o4') ),
-                                     ['o2', 'o3', 'o1', 'o4'], 2 )
-              , ( ( ('o2', 'o3'), ('o2', 'o3', 'o4') ),
-                                     ['o1', 'o2', 'o3', 'o4'], 0 )
-              , ( ( ('n2', 'o3'), ), ['o3', 'o1', 'o2', 'o4'], 1)
-              , ( ( ('o3', 'o1'), ), ['o3', 'o1', 'o2', 'o4'], 1 )
-              )
-            )
+        self.runTableTests(
+            "moveObjectsToTop",
+            (
+                (("o4",), ["o4", "o1", "o2", "o3"], 1),
+                ((("o1", "o3"),), ["o1", "o3", "o2", "o4"], 1),
+                ((("o2", "o3"),), ["o2", "o3", "o1", "o4"], 2),
+                ((("o2", "o3"), ("o1", "o2", "o3", "o4")), ["o2", "o3", "o1", "o4"], 2),
+                ((("o2", "o3"), ("o2", "o3", "o4")), ["o1", "o2", "o3", "o4"], 0),
+                ((("n2", "o3"),), ["o3", "o1", "o2", "o4"], 1),
+                ((("o3", "o1"),), ["o3", "o1", "o2", "o4"], 1),
+            ),
+        )
 
     def test_moveObjectsToBottom(self):
-        self.runTableTests('moveObjectsToBottom',
-              ( ( ( 'o1', ),         ['o2', 'o3', 'o4', 'o1'], 1 )
-              , ( ( ('o2', 'o4'), ), ['o1', 'o3', 'o2', 'o4'], 1 )
-              , ( ( ('o2', 'o3'), ), ['o1', 'o4', 'o2', 'o3'], 2 )
-              , ( ( ('o2', 'o3'), ('o1', 'o2', 'o3', 'o4') ),
-                                     ['o1', 'o4', 'o2', 'o3'], 2 )
-              , ( ( ('o2', 'o3'), ('o1', 'o2', 'o3') ),
-                                     ['o1', 'o2', 'o3', 'o4'], 0 )
-              , ( ( ('n2', 'o3'), ), ['o1', 'o2', 'o4', 'o3'], 1)
-              , ( ( ('o4', 'o2'), ), ['o1', 'o3', 'o4', 'o2'], 1 )
-              )
-            )
+        self.runTableTests(
+            "moveObjectsToBottom",
+            (
+                (("o1",), ["o2", "o3", "o4", "o1"], 1),
+                ((("o2", "o4"),), ["o1", "o3", "o2", "o4"], 1),
+                ((("o2", "o3"),), ["o1", "o4", "o2", "o3"], 2),
+                ((("o2", "o3"), ("o1", "o2", "o3", "o4")), ["o1", "o4", "o2", "o3"], 2),
+                ((("o2", "o3"), ("o1", "o2", "o3")), ["o1", "o2", "o3", "o4"], 0),
+                ((("n2", "o3"),), ["o1", "o2", "o4", "o3"], 1),
+                ((("o4", "o2"),), ["o1", "o3", "o4", "o2"], 1),
+            ),
+        )
 
     def test_orderObjects(self):
-        self.runTableTests('orderObjects',
-              ( ( ( 'id', 'id' ),       ['o4', 'o3', 'o2', 'o1'], -1)
-              , ( ( 'meta_type', '' ),  ['o1', 'o3', 'o2', 'o4'], -1)
-              # for the next line the sort order is different from the
-              # original test in OFS, since the current implementation
-              # keeps the original order as much as possible, i.e. minimize
-              # exchange operations within the list;  this is correct as
-              # far as the test goes, since it didn't specify a secondary
-              # sort key...
-              , ( ( 'meta_type', 'n' ), ['o2', 'o4', 'o1', 'o3'], -1)
-              )
-            )
+        self.runTableTests(
+            "orderObjects",
+            (
+                (("id", "id"), ["o4", "o3", "o2", "o1"], -1),
+                (("meta_type", ""), ["o1", "o3", "o2", "o4"], -1)
+                # for the next line the sort order is different from the
+                # original test in OFS, since the current implementation
+                # keeps the original order as much as possible, i.e. minimize
+                # exchange operations within the list;  this is correct as
+                # far as the test goes, since it didn't specify a secondary
+                # sort key...
+                ,
+                (("meta_type", "n"), ["o2", "o4", "o1", "o3"], -1),
+            ),
+        )
 
     def test_getObjectPosition(self):
-        self.runTableTests('getObjectPosition',
-              ( ( ( 'o2', ), ['o1', 'o2', 'o3', 'o4'], 1)
-              , ( ( 'o4', ), ['o1', 'o2', 'o3', 'o4'], 3)
-              , ( ( 'n2', ), ['o1', 'o2', 'o3', 'o4'], 'ValueError')
-              )
-            )
+        self.runTableTests(
+            "getObjectPosition",
+            (
+                (("o2",), ["o1", "o2", "o3", "o4"], 1),
+                (("o4",), ["o1", "o2", "o3", "o4"], 3),
+                (("n2",), ["o1", "o2", "o3", "o4"], "ValueError"),
+            ),
+        )
 
     def test_moveObjectToPosition(self):
-        self.runTableTests('moveObjectToPosition',
-              ( ( ( 'o2', 2 ), ['o1', 'o3', 'o2', 'o4'], 1)
-              , ( ( 'o4', 2 ), ['o1', 'o2', 'o4', 'o3'], 1)
-              , ( ( 'n2', 2 ), ['o1', 'o2', 'o3', 'o4'], 'ValueError')
-              )
-            )
+        self.runTableTests(
+            "moveObjectToPosition",
+            (
+                (("o2", 2), ["o1", "o3", "o2", "o4"], 1),
+                (("o4", 2), ["o1", "o2", "o4", "o3"], 1),
+                (("n2", 2), ["o1", "o2", "o3", "o4"], "ValueError"),
+            ),
+        )
 
     def test_getObjectPosition_error_message(self):
         folder = self.create()
         try:
-            folder.getObjectPosition('n4')
+            folder.getObjectPosition("n4")
             self.assertFail()
         except ValueError as err:
-            self.assertEqual(
-                str(err), 'No object with id "n4" exists in "f1".')
+            self.assertEqual(str(err), 'No object with id "n4" exists in "f1".')
 
 
 class PloneOrderSupportTests(unittest.TestCase):
-    """ tests borrowed from Products.CMFPlone.tests.testOrderSupport """
+    """tests borrowed from Products.CMFPlone.tests.testOrderSupport"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def setUp(self):
         self.folder = OrderedBTreeFolderBase("f1")
-        self.folder['foo'] = DummyObject('foo', 'mt1')
-        self.folder['bar'] = DummyObject('bar', 'mt1')
-        self.folder['baz'] = DummyObject('baz', 'mt1')
+        self.folder["foo"] = DummyObject("foo", "mt1")
+        self.folder["bar"] = DummyObject("bar", "mt1")
+        self.folder["baz"] = DummyObject("baz", "mt1")
 
     def testGetObjectPosition(self):
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObject(self):
-        self.folder.moveObjectToPosition('foo', 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectToPosition("foo", 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectToSamePos(self):
-        self.folder.moveObjectToPosition('bar', 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectToPosition("bar", 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectToFirstPos(self):
-        self.folder.moveObjectToPosition('bar', 0)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectToPosition("bar", 0)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectToLastPos(self):
-        self.folder.moveObjectToPosition('bar', 2)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectToPosition("bar", 2)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testMoveObjectOutLowerBounds(self):
         # Pos will be normalized to 0
-        self.folder.moveObjectToPosition('bar', -1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectToPosition("bar", -1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectOutUpperBounds(self):
         # Pos will be normalized to 2
-        self.folder.moveObjectToPosition('bar', 3)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectToPosition("bar", 3)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testMoveObjectsUp(self):
-        self.folder.moveObjectsUp(['bar'])
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectsUp(["bar"])
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectsDown(self):
-        self.folder.moveObjectsDown(['bar'])
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectsDown(["bar"])
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testMoveObjectsToTop(self):
-        self.folder.moveObjectsToTop(['bar'])
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectsToTop(["bar"])
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testMoveObjectsToBottom(self):
-        self.folder.moveObjectsToBottom(['bar'])
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectsToBottom(["bar"])
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testMoveTwoObjectsUp(self):
-        self.folder.moveObjectsUp(['bar', 'baz'])
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.folder.moveObjectsUp(["bar", "baz"])
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testMoveTwoObjectsDown(self):
-        self.folder.moveObjectsDown(['foo', 'bar'])
-        self.assertEqual(self.folder.getObjectPosition('baz'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectsDown(["foo", "bar"])
+        self.assertEqual(self.folder.getObjectPosition("baz"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testMoveTwoObjectsToTop(self):
-        self.folder.moveObjectsToTop(['bar', 'baz'])
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.folder.moveObjectsToTop(["bar", "baz"])
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testMoveTwoObjectsToBottom(self):
-        self.folder.moveObjectsToBottom(['foo', 'bar'])
-        self.assertEqual(self.folder.getObjectPosition('baz'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectsToBottom(["foo", "bar"])
+        self.assertEqual(self.folder.getObjectPosition("baz"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testOrderObjects(self):
-        self.folder.orderObjects('id')
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.folder.orderObjects("id")
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testOrderObjectsReverse(self):
-        self.folder.orderObjects('id', reverse=True)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.orderObjects("id", reverse=True)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testOrderObjectsByMethod(self):
-        self.folder.orderObjects('dummy_method')
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.folder.orderObjects("dummy_method")
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testOrderObjectsOnlyReverse(self):
         self.folder.orderObjects(reverse=True)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 0)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 1)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 0)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 1)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testSubsetIds(self):
-        self.folder.moveObjectsByDelta(['baz'], -1, ['foo', 'bar', 'baz'])
-        self.assertEqual(self.folder.getObjectPosition('foo'), 0)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 2)
+        self.folder.moveObjectsByDelta(["baz"], -1, ["foo", "bar", "baz"])
+        self.assertEqual(self.folder.getObjectPosition("foo"), 0)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 2)
 
     def testSkipObjectsNotInSubsetIds(self):
-        self.folder.moveObjectsByDelta(['baz'], -1, ['foo', 'baz'])
-        self.assertEqual(self.folder.getObjectPosition('baz'), 0)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 1)  # no move
-        self.assertEqual(self.folder.getObjectPosition('foo'), 2)
+        self.folder.moveObjectsByDelta(["baz"], -1, ["foo", "baz"])
+        self.assertEqual(self.folder.getObjectPosition("baz"), 0)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 1)  # no move
+        self.assertEqual(self.folder.getObjectPosition("foo"), 2)
 
     def testIgnoreNonObjects(self):
         # Fix for (http://dev.plone.org/plone/ticket/3959) non
         # contentish objects cause errors, we should just ignore them
-        self.folder.moveObjectsByDelta(['bar', 'blah'], -1)
-        self.assertEqual(self.folder.getObjectPosition('bar'), 0)
-        self.assertEqual(self.folder.getObjectPosition('foo'), 1)
-        self.assertEqual(self.folder.getObjectPosition('baz'), 2)
+        self.folder.moveObjectsByDelta(["bar", "blah"], -1)
+        self.assertEqual(self.folder.getObjectPosition("bar"), 0)
+        self.assertEqual(self.folder.getObjectPosition("foo"), 1)
+        self.assertEqual(self.folder.getObjectPosition("baz"), 2)
 
     def testNotifyRemoved(self):
         ordering = self.folder.getOrdering()
-        self.assertEqual(
-            ordering.idsInOrder(),
-            ['foo', 'bar', 'baz']
-        )
+        self.assertEqual(ordering.idsInOrder(), ["foo", "bar", "baz"])
 
         # make sure notifyRemoved with non-existent id does not throw error
-        ordering.notifyRemoved('foobar')
+        ordering.notifyRemoved("foobar")
 
         # normal
-        ordering.notifyRemoved('foo')
-        self.assertEqual(
-            ordering.idsInOrder(),
-            ['bar', 'baz']
-        )
+        ordering.notifyRemoved("foo")
+        self.assertEqual(ordering.idsInOrder(), ["bar", "baz"])
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_unorderedordering.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_unorderedordering.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,42 @@
 from plone.folder.ordered import OrderedBTreeFolderBase
-from plone.folder.unordered import UnorderedOrdering
-from plone.folder.tests.utils import DummyObject
 from plone.folder.testing import PLONEFOLDER_INTEGRATION_TESTING
+from plone.folder.tests.utils import DummyObject
+from plone.folder.unordered import UnorderedOrdering
 
 import unittest
 
 
 class UnorderedOrderingTests(unittest.TestCase):
-    """ tests regarding order-support for folders with unordered ordering """
+    """tests regarding order-support for folders with unordered ordering"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def create(self):
         container = OrderedBTreeFolderBase()
-        container._ordering = u'unordered'
-        container._setOb('o1', DummyObject('o1', 'mt1'))
-        container._setOb('o2', DummyObject('o2', 'mt2'))
-        container._setOb('o3', DummyObject('o3', 'mt1'))
-        container._setOb('o4', DummyObject('o4', 'mt2'))
+        container._ordering = "unordered"
+        container._setOb("o1", DummyObject("o1", "mt1"))
+        container._setOb("o2", DummyObject("o2", "mt2"))
+        container._setOb("o3", DummyObject("o3", "mt1"))
+        container._setOb("o4", DummyObject("o4", "mt2"))
         return container
 
     def testAdapter(self):
         container = self.create()
         ordering = container.getOrdering()
         self.assertTrue(isinstance(ordering, UnorderedOrdering))
 
     def testNotifyAdded(self):
         container = self.create()
-        self.assertEqual(
-            set(container.objectIds()),
-            set(['o1', 'o2', 'o3', 'o4'])
-        )
-        container._setOb('o5', DummyObject('o5', 'mt1'))
-        self.assertEqual(
-            set(container.objectIds()),
-            set(['o1', 'o2', 'o3', 'o4', 'o5'])
-        )
+        self.assertEqual(set(container.objectIds()), {"o1", "o2", "o3", "o4"})
+        container._setOb("o5", DummyObject("o5", "mt1"))
+        self.assertEqual(set(container.objectIds()), {"o1", "o2", "o3", "o4", "o5"})
 
     def testNotifyRemoved(self):
         container = self.create()
-        self.assertEqual(
-            set(container.objectIds()),
-            set(['o1', 'o2', 'o3', 'o4'])
-        )
-        container._delOb('o3')
-        self.assertEqual(
-            set(container.objectIds()),
-            set(['o1', 'o2', 'o4'])
-        )
+        self.assertEqual(set(container.objectIds()), {"o1", "o2", "o3", "o4"})
+        container._delOb("o3")
+        self.assertEqual(set(container.objectIds()), {"o1", "o2", "o4"})
 
     def testGetObjectPosition(self):
         container = self.create()
-        self.assertEqual(container.getObjectPosition('o2'), None)
+        self.assertEqual(container.getObjectPosition("o2"), None)
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/test_webdav.py` & `plone.folder-4.0.0/src/plone/folder/tests/test_webdav.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,55 @@
-# -*- coding: utf-8 -*-
 from Acquisition import Explicit
 from plone.folder.ordered import CMFOrderedBTreeFolderBase
 from plone.folder.testing import PLONEFOLDER_INTEGRATION_TESTING
 from plone.folder.tests.utils import DummyObject
 from zope.publisher.browser import TestRequest
 
-import pkg_resources
 import unittest
 
 
 HAS_WEBDAV = True
 try:
     from webdav.NullResource import NullResource
 except ImportError:
     HAS_WEBDAV = False
 
 
 class TestRequestContainer(Explicit):
-
     REQUEST = TestRequest()
 
 
 class WebDAVTests(unittest.TestCase):
-    """ tests regarding support for WebDAV NullResources """
+    """tests regarding support for WebDAV NullResources"""
 
     layer = PLONEFOLDER_INTEGRATION_TESTING
 
     def test_getitem_not_dav_request(self):
         root = TestRequestContainer()
         folder = CMFOrderedBTreeFolderBase("f1").__of__(root)
 
         root.REQUEST.maybe_webdav_client = False
-        root.REQUEST._environ['REQUEST_METHOD'] = 'GET'
+        root.REQUEST._environ["REQUEST_METHOD"] = "GET"
 
-        foo = DummyObject('foo')
-        folder['foo'] = foo
+        foo = DummyObject("foo")
+        folder["foo"] = foo
 
-        self.assertEquals(folder['foo'], foo)
+        self.assertEqual(folder["foo"], foo)
         try:
-            folder['bar']
+            folder["bar"]
             self.fail()
         except KeyError:
             pass
 
-    @unittest.skipUnless(HAS_WEBDAV, 'ZServer is optional')
+    @unittest.skipUnless(HAS_WEBDAV, "ZServer is optional")
     def test_getitem_dav_request(self):
         root = TestRequestContainer()
         folder = CMFOrderedBTreeFolderBase("f1").__of__(root)
 
         root.REQUEST.maybe_webdav_client = True
-        root.REQUEST._environ['REQUEST_METHOD'] = 'PUT'
+        root.REQUEST._environ["REQUEST_METHOD"] = "PUT"
 
-        foo = DummyObject('foo')
-        folder['foo'] = foo
+        foo = DummyObject("foo")
+        folder["foo"] = foo
 
-        self.assertEquals(folder['foo'], foo)
-        self.assertTrue(isinstance(folder['bar'], NullResource))
+        self.assertEqual(folder["foo"], foo)
+        self.assertTrue(isinstance(folder["bar"], NullResource))
```

### Comparing `plone.folder-3.1.0/src/plone/folder/tests/utils.py` & `plone.folder-4.0.0/src/plone/folder/tests/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
 from plone.folder.interfaces import IOrderable
 from zope.interface import implementer
 
 
-class DummyObject(object):
-
+class DummyObject:
     def __init__(self, id, meta_type=None):
         self.id = id
         self.meta_type = meta_type
 
     def __of__(self, obj):
         return self
 
@@ -17,12 +15,12 @@
 
     def dummy_method(self):
         return self.id
 
 
 @implementer(IOrderable)
 class Orderable(DummyObject):
-    """ orderable mock object """
+    """orderable mock object"""
 
 
 class Chaoticle(DummyObject):
-    """ non-orderable mock object;  this does not implement `IOrderable` """
+    """non-orderable mock object;  this does not implement `IOrderable`"""
```

### Comparing `plone.folder-3.1.0/src/plone/folder/unordered.py` & `plone.folder-4.0.0/src/plone/folder/unordered.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from plone.folder.interfaces import IOrderableFolder
 from plone.folder.interfaces import IOrdering
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IOrdering)
 @adapter(IOrderableFolder)
-class UnorderedOrdering(object):
-    """ This implementation provides no ordering. """
+class UnorderedOrdering:
+    """This implementation provides no ordering."""
 
     def __init__(self, context):
         self.context = context
 
     def notifyAdded(self, obj_id):
         pass
```

### Comparing `plone.folder-3.1.0/src/plone.folder.egg-info/SOURCES.txt` & `plone.folder-4.0.0/src/plone.folder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

