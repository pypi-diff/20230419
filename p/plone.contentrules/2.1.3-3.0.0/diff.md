# Comparing `tmp/plone.contentrules-2.1.3.tar.gz` & `tmp/plone.contentrules-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.contentrules-2.1.3.tar", last modified: Tue Mar 21 22:49:08 2023, max compression
+gzip compressed data, was "plone.contentrules-3.0.0.tar", last modified: Wed Apr 19 07:14:19 2023, max compression
```

## Comparing `plone.contentrules-2.1.3.tar` & `plone.contentrules-3.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.392800 plone.contentrules-2.1.3/
--rw-r--r--   0 maurits    (501) staff       (20)     3218 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     4600 2023-03-21 22:49:08.392944 plone.contentrules-2.1.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      412 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.380541 plone.contentrules-2.1.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      680 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.380827 plone.contentrules-2.1.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.385805 plone.contentrules-2.1.3/plone/contentrules/
--rw-r--r--   0 maurits    (501) staff       (20)    23656 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)       93 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      175 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.388329 plone.contentrules-2.1.3/plone/contentrules/engine/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3428 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/assignments.py
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1914 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/executor.py
--rw-r--r--   0 maurits    (501) staff       (20)     2439 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      538 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/engine/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      116 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/meta.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.391728 plone.contentrules-2.1.3/plone/contentrules/rule/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      239 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/element.py
--rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/eventvocab.py
--rw-r--r--   0 maurits    (501) staff       (20)     6527 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1430 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/metaconfigure.py
--rw-r--r--   0 maurits    (501) staff       (20)     1971 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/metadirectives.py
--rw-r--r--   0 maurits    (501) staff       (20)     1346 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/rule.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.392452 plone.contentrules-2.1.3/plone/contentrules/rule/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      643 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/rule/tests/elements.py
--rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     3397 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/plone/contentrules/zcml.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:49:08.383660 plone.contentrules-2.1.3/plone.contentrules.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     4600 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      189 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:49:08.000000 plone.contentrules-2.1.3/plone.contentrules.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-03-21 22:49:08.393612 plone.contentrules-2.1.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1638 2023-03-21 22:49:07.000000 plone.contentrules-2.1.3/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.044840 plone.contentrules-3.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3379 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      121 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     4748 2023-04-19 07:14:19.044840 plone.contentrules-3.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      412 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.041840 plone.contentrules-3.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      680 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.041840 plone.contentrules-3.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.042840 plone.contentrules-3.0.0/plone/contentrules/
+-rw-r--r--   0 gil       (1000) gil       (1000)    23656 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       94 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      170 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.043840 plone.contentrules-3.0.0/plone/contentrules/engine/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3414 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/assignments.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      187 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1926 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/executor.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2423 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      532 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/storage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1135 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/engine/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      132 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/meta.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.044840 plone.contentrules-3.0.0/plone/contentrules/rule/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      223 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1129 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/element.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1285 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/eventvocab.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6038 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      552 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/meta.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1593 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/metaconfigure.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1912 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/metadirectives.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1439 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/rule.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.044840 plone.contentrules-3.0.0/plone/contentrules/rule/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      648 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/rule/tests/elements.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1258 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3377 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone/contentrules/zcml.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:14:19.042840 plone.contentrules-3.0.0/plone.contentrules.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4748 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1307 2023-04-19 07:14:19.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       41 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/plone.contentrules.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2900 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-19 07:14:19.044840 plone.contentrules-3.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1397 2023-04-19 07:14:18.000000 plone.contentrules-3.0.0/setup.py
```

### Comparing `plone.contentrules-2.1.3/CHANGES.rst` & `plone.contentrules-3.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Drop python 2.7.
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
 2.1.3 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.contentrules-2.1.3/PKG-INFO` & `plone.contentrules-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.contentrules
-Version: 2.1.3
+Version: 3.0.0
 Summary: Plone ContentRules Engine
 Home-page: https://pypi.org/project/plone.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone content rules events
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope2
 Classifier: Framework :: Zope :: 4
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 
 Overview
 ========
 
 plone.contentrules provides a "pure Zope" implementation of a a rules engine
 which allows arbitrary conditions and actions to be combined into rules, and
 rules to be executed dependent on events.
@@ -40,14 +40,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Drop python 2.7.
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
 2.1.3 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.contentrules-2.1.3/docs/LICENSE.GPL` & `plone.contentrules-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.contentrules-2.1.3/docs/LICENSE.txt` & `plone.contentrules-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.contentrules-2.1.3/plone/contentrules/README.rst` & `plone.contentrules-3.0.0/plone/contentrules/README.rst`

 * *Files identical despite different names*

### Comparing `plone.contentrules-2.1.3/plone/contentrules/engine/assignments.py` & `plone.contentrules-3.0.0/plone/contentrules/engine/assignments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-from persistent import Persistent
-
+from BTrees.OOBTree import OOBTree
 from OFS.Uninstalled import BrokenClass
+from persistent import Persistent
+from plone.contentrules.engine.interfaces import IRuleAssignable
+from plone.contentrules.engine.interfaces import IRuleAssignment
+from plone.contentrules.engine.interfaces import IRuleAssignmentManager
+from plone.contentrules.engine.interfaces import IRuleStorage
 from ZODB.broken import PersistentBroken
-from zope.interface import implementer, implementer
-from zope.component import adapter, queryUtility
 from zope.annotation.interfaces import IAnnotations
-from zope.container.ordered import OrderedContainer
+from zope.component import adapter
+from zope.component import queryUtility
 from zope.container.contained import Contained
 from zope.container.interfaces import IObjectAddedEvent
+from zope.container.ordered import OrderedContainer
+from zope.interface import implementer
 
-from plone.contentrules.engine.interfaces import IRuleStorage
-from plone.contentrules.engine.interfaces import IRuleAssignable
-from plone.contentrules.engine.interfaces import IRuleAssignment
-from plone.contentrules.engine.interfaces import IRuleAssignmentManager
-
-from BTrees.OOBTree import OOBTree
 
 try:
     from plone.protect.auto import safeWrite
 except ImportError:
+
     def safeWrite(*args):
         pass
 
 
 def check_rules_with_dotted_name_moved(rule):
     """Migrate on-the-fly added event dotted name
     if Plone has been migrated from any release to 4.3 release.
     Avoids any upgrade to fail when setup profile is re-imported.
     """
     if PersistentBroken in rule.event.__bases__ or BrokenClass in rule.event.__bases__:
-        if rule.event.__name__ == 'IObjectAddedEvent':
+        if rule.event.__name__ == "IObjectAddedEvent":
             rule.event = IObjectAddedEvent
 
-KEY = 'plone.contentrules.localassignments'
+
+KEY = "plone.contentrules.localassignments"
+
 
 @implementer(IRuleAssignment)
 class RuleAssignment(Contained, Persistent):
-    """An assignment of a rule to a context
-    """
+    """An assignment of a rule to a context"""
 
     def __init__(self, ruleid, enabled=True, bubbles=False):
-        super(RuleAssignment, self).__init__()
+        super().__init__()
         self.__name__ = ruleid
         self.enabled = enabled
         self.bubbles = bubbles
 
+
 @implementer(IRuleAssignmentManager)
 class RuleAssignmentManager(OrderedContainer):
-    """A context-specific container for rule assignments
-    """
+    """A context-specific container for rule assignments"""
 
     def __init__(self):
         # XXX: This depends on implementation detail in OrderedContainer,
         # but it uses a PersistentDict, which sucks :-/
         OrderedContainer.__init__(self)
         self._data = OOBTree()
 
     def getRules(self, event, bubbled=False):
         rules = []
         storage = queryUtility(IRuleStorage)
         if storage is not None:
             for a in self.values():
                 if not a.enabled:
                     continue
-                if not (bubbled == False or a.bubbles):
+                if not (bubbled is False or a.bubbles):
                     continue
 
                 r = storage.get(a.__name__, None)
                 if r is None:
                     continue
 
                 try:
@@ -77,14 +78,15 @@
                     provided = r.event.providedBy(event)
 
                 if provided and r.enabled:
                     rules.append(r)
 
         return rules
 
+
 @adapter(IRuleAssignable)
 @implementer(IRuleAssignmentManager)
 def ruleAssignmentManagerAdapterFactory(context):
     """When adapting an IRuleAssignable, get an IRuleAssignmentManager by
     finding one in the object's annotations. The container will be created
     if necessary.
     """
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/engine/executor.py` & `plone.contentrules-3.0.0/plone/contentrules/engine/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from zope.interface import implementer
-from zope.component import adapts, getMultiAdapter
-
-from plone.contentrules.engine.interfaces import IRuleExecutor
 from plone.contentrules.engine.interfaces import IRuleAssignable
 from plone.contentrules.engine.interfaces import IRuleAssignmentManager
-
+from plone.contentrules.engine.interfaces import IRuleExecutor
 from plone.contentrules.engine.interfaces import StopRule
-
 from plone.contentrules.rule.interfaces import IExecutable
+from zope.component import adapts
+from zope.component import getMultiAdapter
+from zope.interface import implementer
+
 
 @implementer(IRuleExecutor)
-class RuleExecutor(object):
-    """An object that can execute rules in its context.
-    """
+class RuleExecutor:
+    """An object that can execute rules in its context."""
+
     adapts(IRuleAssignable)
 
     def __init__(self, context):
         self.context = context
 
     def __call__(self, event, bubbled=False, rule_filter=None):
         assignments = IRuleAssignmentManager(self.context)
         for rule in assignments.getRules(event, bubbled=bubbled):
             # for each rule assigned in this context - bubbled means rule apply on subfolders
-            if rule_filter is None or rule_filter(self.context, rule, event) == True:
-                # execute the rule if it is not filtered, for exemple,
+            if rule_filter is None or rule_filter(self.context, rule, event) is True:
+                # execute the rule if it is not filtered, for example,
                 # it has not been executed on the same content but from an other context
                 # in the same request
 
                 # we store cascading option in the filter. if true, this will allow
                 # rules to be executed because of the actions ran by this rule.
                 if rule_filter is not None:
-                    cascade_before = getattr(rule_filter, 'cascade', False)
+                    cascade_before = getattr(rule_filter, "cascade", False)
                     rule_filter.cascade = rule.cascading
 
                 executable = getMultiAdapter((self.context, rule, event), IExecutable)
                 executable()
 
                 if rule_filter is not None:
                     rule_filter.cascade = cascade_before
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/engine/interfaces.py` & `plone.contentrules-3.0.0/plone/contentrules/engine/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-from zope.interface import Interface, Attribute
 from zope import schema
-
+from zope.annotation.interfaces import IAttributeAnnotatable
+from zope.container.constraints import contains
 from zope.container.interfaces import IContained
-from zope.container.interfaces import IOrderedContainer
 from zope.container.interfaces import IContainerNamesContainer
+from zope.container.interfaces import IOrderedContainer
+from zope.interface import Interface
 
-from zope.container.constraints import contains
-from zope.annotation.interfaces import IAttributeAnnotatable
 
 class StopRule(Exception):
-    """An event that informs us that rule execution should be aborted.
-    """
+    """An event that informs us that rule execution should be aborted."""
 
     def __init__(self, rule):
         self.rule = rule
 
+
 class IRuleStorage(IOrderedContainer, IContainerNamesContainer):
-    """A storage for rules. This is registered as a local utility.
-    """
-    contains('plone.contentrules.rule.interfaces.IRule')
+    """A storage for rules. This is registered as a local utility."""
+
+    contains("plone.contentrules.rule.interfaces.IRule")
+
+    active = schema.Bool(title="Rules in this storage are active")
 
-    active = schema.Bool(title=u"Rules in this storage are active")
 
 class IRuleAssignable(IAttributeAnnotatable):
-    """Marker interface for objects that can be assigned rules
-    """
+    """Marker interface for objects that can be assigned rules"""
+
 
 class IRuleAssignment(IContained):
-    """An assignment of a rule to a context
-    """
+    """An assignment of a rule to a context"""
 
-    __name__ = schema.TextLine(title=u"The id of the rule")
+    __name__ = schema.TextLine(title="The id of the rule")
+
+    enabled = schema.Bool(title="Whether or not the rule is currently enabled")
+    bubbles = schema.Bool(
+        title="Whether or not the rule will apply to objects in subfolders"
+    )
 
-    enabled = schema.Bool(title=u"Whether or not the rule is currently enabled")
-    bubbles = schema.Bool(title=u"Whether or not the rule will apply to objects in subfolders")
 
 class IRuleAssignmentManager(IOrderedContainer):
     """An object that is capable of being assigned rules.
 
     Normally, an object will be adapted to IRuleAssignmentManager in order
     to manipulate the rule assignments in this location.
     """
 
     def getRules(event, bubbled=False):
         """Get all enabled rules registered for the given event and
         assigned to this context. If bubbled is True, only rules that are
         bubbleable will be returned.
         """
 
+
 class IRuleExecutor(Interface):
     """An object that is capable of executing rules.
 
     Typically, a content object will be adapted to this interface
     """
 
     def __call__(event, bubbled=False, rule_filter=None):
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/engine/storage.py` & `plone.contentrules-3.0.0/plone/contentrules/engine/storage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from zope.interface import implementer
-from zope.container.ordered import OrderedContainer
-
+from BTrees.OOBTree import OOBTree
 from plone.contentrules.engine.interfaces import IRuleStorage
+from zope.container.ordered import OrderedContainer
+from zope.interface import implementer
 
-from BTrees.OOBTree import OOBTree
 
 @implementer(IRuleStorage)
 class RuleStorage(OrderedContainer):
-    """A container for rules.
-    """
+    """A container for rules."""
 
     active = True
 
     def __init__(self):
         # XXX: This depends on implementation detail in OrderedContainer,
         # but it uses a PersistentDict, which sucks :-/
         OrderedContainer.__init__(self)
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/engine/utils.py` & `plone.contentrules-3.0.0/plone/contentrules/engine/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,35 @@
+from plone.contentrules.rule.interfaces import IRuleAction
+from plone.contentrules.rule.interfaces import IRuleCondition
 from zope.component import getAllUtilitiesRegisteredFor
-from plone.contentrules.rule.interfaces import IRuleCondition, IRuleAction
+
 
 def getAvailableConditions(context, eventType):
     conditions = getAllUtilitiesRegisteredFor(IRuleCondition)
-    return [c for c in conditions if
-                (c.event is None or eventType.isOrExtends(c.event)) and
-                (c.for_ is None or c.for_.providedBy(context))]
+    return [
+        c
+        for c in conditions
+        if (c.event is None or eventType.isOrExtends(c.event))
+        and (c.for_ is None or c.for_.providedBy(context))
+    ]
+
 
 def allAvailableConditions(eventType):
     conditions = getAllUtilitiesRegisteredFor(IRuleCondition)
-    return [c for c in conditions if
-                (c.event is None or eventType.isOrExtends(c.event))]
+    return [
+        c for c in conditions if (c.event is None or eventType.isOrExtends(c.event))
+    ]
+
 
 def getAvailableActions(context, eventType):
     actions = getAllUtilitiesRegisteredFor(IRuleAction)
-    return [a for a in actions if
-                (a.event is None or eventType.isOrExtends(a.event)) and
-                (a.for_ is None or a.for_.providedBy(context))]
+    return [
+        a
+        for a in actions
+        if (a.event is None or eventType.isOrExtends(a.event))
+        and (a.for_ is None or a.for_.providedBy(context))
+    ]
+
 
 def allAvailableActions(eventType):
     actions = getAllUtilitiesRegisteredFor(IRuleAction)
-    return [a for a in actions if
-                (a.event is None or eventType.isOrExtends(a.event))]
+    return [a for a in actions if (a.event is None or eventType.isOrExtends(a.event))]
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/element.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/element.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-from zope.interface import implementer, Interface
+from plone.contentrules.rule.interfaces import IRuleAction
+from plone.contentrules.rule.interfaces import IRuleCondition
+from plone.contentrules.rule.interfaces import IRuleElement
+from zope.interface import implementer
+from zope.interface import Interface
 
-from plone.contentrules.rule.interfaces import IRuleElement, IRuleCondition, IRuleAction
 
 @implementer(IRuleElement)
-class RuleElement(object):
+class RuleElement:
     """A rule element.
 
     Ordinarily, rule elements will be created via ZCML directives, which will
     register them as utilities.
     """
 
-    title = u''
-    description = u''
+    title = ""
+    description = ""
     for_ = Interface
     event = None
     addview = None
     editview = None
     schema = None
     factory = None
 
+
 @implementer(IRuleCondition)
 class RuleCondition(RuleElement):
     """A rule condition.
 
     Rule conditions are just rule elements, but are registered under a more
     specific interface to enable the UI to differentate between different types
     of elements.
     """
 
+
 @implementer(IRuleAction)
 class RuleAction(RuleElement):
     """A rule action.
 
     Rule action are just rule elements, but are registered under a more
     specific interface to enable the UI to differentate between different types
     of elements.
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/eventvocab.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/eventvocab.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-# -*- coding: utf-8 -*-
 from plone.contentrules.rule.interfaces import IRuleEventType
 from zope.componentvocabulary.vocabulary import UtilityVocabulary
 from zope.i18nmessageid import MessageFactory
-from zope.interface import Interface, provider
+from zope.interface import Interface
+from zope.interface import provider
 from zope.interface.interfaces import IInterface
 from zope.schema.interfaces import IVocabularyFactory
 from zope.schema.vocabulary import SimpleTerm
 
-import six
 import zope.component
 
 
-_ = MessageFactory('plone')
+_ = MessageFactory("plone")
 
 
 @provider(IVocabularyFactory)
 class EventTypesVocabulary(UtilityVocabulary):
     """A vocabulary for event interfaces that can be selected for the 'event'
     attribute of an IRule.
     An internationalized version of UtilityVocabulary
     """
+
     interface = IRuleEventType
 
     def __init__(self, context, **kw):
         if kw:
-            self.nameOnly = bool(kw.get('nameOnly', False))
-            interface = kw.get('interface', Interface)
-            if isinstance(interface, (six.string_types, six.text_type)):
+            self.nameOnly = bool(kw.get("nameOnly", False))
+            interface = kw.get("interface", Interface)
+            if isinstance(interface, ((str,), str)):
                 interface = zope.component.getUtility(IInterface, interface)
             self.interface = interface
 
         utils = zope.component.getUtilitiesFor(self.interface, context)
-        self._terms = dict(
-            (name, SimpleTerm(self.nameOnly and name or util, name, _(name)))
-            for name, util in utils)
+        self._terms = {
+            name: SimpleTerm(self.nameOnly and name or util, name, _(name))
+            for name, util in utils
+        }
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/interfaces.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,180 @@
 """
 """
-__docformat__ = 'restructuredtext'
-
-from zope.interface import Interface
-from zope.interface.interfaces import IInterface
-
-from zope.container.interfaces import IContained
+__docformat__ = "restructuredtext"
 
+from plone.contentrules import PloneMessageFactory as _
 from zope import schema
 from zope.configuration import fields as configuration_fields
-
-from plone.contentrules import PloneMessageFactory as _
+from zope.container.interfaces import IContained
+from zope.interface import Interface
+from zope.interface.interfaces import IInterface
 
 
 class IRuleElementData(Interface):
     """Metadata for rule element data (the configuration of actions
     or conditions).
     """
 
-    element = schema.ASCII(title=u"Rule element",
-                              description=u"The name of the rule action or condition",
-                              required=True)
-
-    summary = schema.Text(title=u"Summary",
-                          description=u"A human-readable description of this element as it is configured",
-                          required=True)
+    element = schema.ASCII(
+        title="Rule element",
+        description="The name of the rule action or condition",
+        required=True,
+    )
+
+    summary = schema.Text(
+        title="Summary",
+        description="A human-readable description of this element as it is configured",
+        required=True,
+    )
+
 
 class IRuleElement(Interface):
     """Base interface for rule elements (actions and conditions)
 
     A rule element is either a condition or an action that can be combined to
     form a rule.Rules can be constructed by the user and invoked by the
     IRuleExecuter
     """
-    title = schema.TextLine(
-        title = u'Title',
-        required = True)
 
-    description = schema.Text(
-        title = u'Description',
-        required = False)
+    title = schema.TextLine(title="Title", required=True)
+
+    description = schema.Text(title="Description", required=False)
 
     for_ = configuration_fields.GlobalInterface(
-        title = u'Available for',
-        description = u'The interface this component is available for',
-        required = False)
+        title="Available for",
+        description="The interface this component is available for",
+        required=False,
+    )
 
     event = configuration_fields.GlobalInterface(
-        title = u'Applicable event',
-        description = u'The event that can trigger this element, None meaning '
-                       'it is not event specific.',
-        required = False)
+        title="Applicable event",
+        description="The event that can trigger this element, None meaning "
+        "it is not event specific.",
+        required=False,
+    )
 
     addview = schema.TextLine(
-        title = u'Add view',
-        description = u'The name of the add view',
-        required = True)
+        title="Add view", description="The name of the add view", required=True
+    )
 
     editview = schema.TextLine(
-        title = u"Edit view",
-        description = u"The name of the edit view",
-        required = True)
+        title="Edit view", description="The name of the edit view", required=True
+    )
 
     schema = configuration_fields.GlobalInterface(
-        title = u'Schema',
-        description = u'Schema interface for configuring the element',
-        required = False)
+        title="Schema",
+        description="Schema interface for configuring the element",
+        required=False,
+    )
 
     factory = configuration_fields.GlobalInterface(
-        title = u'Factory',
-        description = u'Callable which creates an instance of the element',
-        required = False)
+        title="Factory",
+        description="Callable which creates an instance of the element",
+        required=False,
+    )
+
 
 class IRuleCondition(IRuleElement):
     """A condition of a rule
 
     Rule execution will stop if the condition fails. If the condition does not
     fail, the next element will be executed.
     """
 
+
 class IRuleAction(IRuleElement):
     """An action executed as part of a rule.
 
     Actions can perform operations, presuming preceding conditions do not fail.
     Once an action is finished, the next element will be executed.
     """
 
+
 class IRuleEventType(IInterface):
     """Marker interface for event interfaces that can be used as the 'event'
     type of an IRule.
     """
 
+
 class IRuleConfiguration(Interface):
-    """Configurable options for a rule
-    """
+    """Configurable options for a rule"""
+
+    title = schema.TextLine(
+        title=_("Title"),
+        description=_(
+            "description_contentrule_title",
+            default="Please set a descriptive title for the rule.",
+        ),
+        required=True,
+    )
 
-    title = schema.TextLine(title = _(u'Title'),
-                            description = _('description_contentrule_title',
-                                            default=u'Please set a descriptive title for the rule.'),
-                            required = True)
-
-    description = schema.Text(title = _(u'Description'),
-                              description = _('contentrules_description_description',
-                                              default=u'Enter a short description of the rule and its purpose.'),
-                              required = False)
-
-    event = schema.Choice(title = _(u'Triggering event'),
-                          description = _('contentrules_description_trigger',
-                                          default=u'The rule will execute when the following event occurs.'),
-                          required = True,
-                          vocabulary="plone.contentrules.events")
-
-    enabled = schema.Bool(title = _(u'Enabled'),
-                          description = _(u'Whether or not the rule is currently enabled'),
-                          default = True,
-                          required = False)
-
-    stop = schema.Bool(title = _(u"Stop executing rules"),
-                       description = _(u"Whether or not execution of further rules should stop after this rule is executed"),
-                       default = False,
-                       required = False)
-
-    cascading = schema.Bool(title = _(u"Cascading rule"),
-                       description = _(u"Whether or not other rules should be triggered by the actions launched by this rule. Activate this only if you are sure this won't create infinite loops."),
-                       default = False,
-                       required = False)
+    description = schema.Text(
+        title=_("Description"),
+        description=_(
+            "contentrules_description_description",
+            default="Enter a short description of the rule and its purpose.",
+        ),
+        required=False,
+    )
+
+    event = schema.Choice(
+        title=_("Triggering event"),
+        description=_(
+            "contentrules_description_trigger",
+            default="The rule will execute when the following event occurs.",
+        ),
+        required=True,
+        vocabulary="plone.contentrules.events",
+    )
+
+    enabled = schema.Bool(
+        title=_("Enabled"),
+        description=_("Whether or not the rule is currently enabled"),
+        default=True,
+        required=False,
+    )
+
+    stop = schema.Bool(
+        title=_("Stop executing rules"),
+        description=_(
+            "Whether or not execution of further rules should stop after this rule is executed"
+        ),
+        default=False,
+        required=False,
+    )
+
+    cascading = schema.Bool(
+        title=_("Cascading rule"),
+        description=_(
+            "Whether or not other rules should be triggered by the actions launched by this rule. Activate this only if you are sure this won't create infinite loops."
+        ),
+        default=False,
+        required=False,
+    )
 
 
 class IRule(IContained, IRuleConfiguration):
     """A rule - a collection of rule elements.
 
     A rule is composed, normally through the user interface, of conditions and
     actions. Upon some event, rules that are relevant in the given context will
     be executed by adapting them to IExecutable and running its execute()
     method.
 
     When saved in a rule storage, it will be given a name.
     """
 
-
-    conditions = schema.List(title = u'Conditions',
-                             description = u'The conditions of this rule',
-                             required = True)
-
-    actions = schema.List(title = u'Actions',
-                          description = u'The actions of this rule',
-                          required = True)
+    conditions = schema.List(
+        title="Conditions", description="The conditions of this rule", required=True
+    )
+
+    actions = schema.List(
+        title="Actions", description="The actions of this rule", required=True
+    )
 
 
 class IExecutable(Interface):
     """An item which can be executed.
 
     The execution of a rule involves the execution of each one of its elements
     (i.e. conditions and actions). The IRule will be adapted to IExecutable in
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/metaconfigure.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/metaconfigure.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+from plone.contentrules.rule.element import RuleAction
+from plone.contentrules.rule.element import RuleCondition
+from plone.contentrules.rule.interfaces import IRuleAction
+from plone.contentrules.rule.interfaces import IRuleCondition
 from zope.component.zcml import utility
 from zope.interface import Interface
 
-from plone.contentrules.rule.interfaces import IRuleCondition, IRuleAction
-from plone.contentrules.rule.element import RuleCondition, RuleAction
 
-def ruleConditionDirective(_context, name, title, addview, editview=None,
-        description="", for_=Interface, event=Interface, schema=None, factory=None):
+def ruleConditionDirective(
+    _context,
+    name,
+    title,
+    addview,
+    editview=None,
+    description="",
+    for_=Interface,
+    event=Interface,
+    schema=None,
+    factory=None,
+):
     """Register a utility for IRuleCondition based on the parameters in the
     zcml directive
     """
 
     condition = RuleCondition()
     condition.title = title
     condition.addview = addview
@@ -19,16 +31,26 @@
     condition.event = event
     condition.schema = schema
     condition.factory = factory
 
     utility(_context, provides=IRuleCondition, component=condition, name=name)
 
 
-def ruleActionDirective(_context, name, title, addview, editview=None,
-    description="", for_=Interface, event=Interface, schema=None, factory=None):
+def ruleActionDirective(
+    _context,
+    name,
+    title,
+    addview,
+    editview=None,
+    description="",
+    for_=Interface,
+    event=Interface,
+    schema=None,
+    factory=None,
+):
     """Register a utility for IRuleAction based on the parameters in the
     zcml directive
     """
 
     action = RuleAction()
     action.title = title
     action.addview = addview
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/metadirectives.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/metadirectives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-from zope.interface import Interface
-
 from zope import schema
 from zope.configuration import fields as configuration_fields
+from zope.interface import Interface
+
 
 class IRuleElementDirective(Interface):
     """Directive which registers a new rule element.
 
     The actual directives will use IRuleActionDirective or IRuleConditionDirective
     """
 
     name = schema.TextLine(
-        title=u"Name",
-        description=u"A unique name for the element",
-        required=True)
+        title="Name", description="A unique name for the element", required=True
+    )
 
     title = schema.TextLine(
-        title=u"Title",
-        description=u"A user-friendly title for the element",
-        required=True)
+        title="Title",
+        description="A user-friendly title for the element",
+        required=True,
+    )
 
     description = schema.Text(
-        title=u"Description",
-        description=u"A helpful description of the element",
-        required=False)
+        title="Description",
+        description="A helpful description of the element",
+        required=False,
+    )
 
     for_ = configuration_fields.GlobalInterface(
-        title = u"Available for",
-        description = u"The interface this element is available for",
-        required = False)
+        title="Available for",
+        description="The interface this element is available for",
+        required=False,
+    )
 
     event = configuration_fields.GlobalInterface(
-        title = u"Event",
-        description = u"The event this element is available for",
-        required = False)
+        title="Event",
+        description="The event this element is available for",
+        required=False,
+    )
 
     addview = schema.TextLine(
-        title = u"Add view",
-        description = u"Name of the add view",
-        required = True)
+        title="Add view", description="Name of the add view", required=True
+    )
 
     editview = schema.TextLine(
-        title = u"Edit view",
-        description = u"Name of the edit view",
-        required = False)
+        title="Edit view", description="Name of the edit view", required=False
+    )
 
     schema = configuration_fields.GlobalInterface(
-        title = u"Schema",
-        description = u"The schema interface for configuring the element",
-        required = False)
+        title="Schema",
+        description="The schema interface for configuring the element",
+        required=False,
+    )
 
     factory = configuration_fields.GlobalObject(
-        title = u"Factory",
-        description = u"A callable which can create the element",
-        required = False)
+        title="Factory",
+        description="A callable which can create the element",
+        required=False,
+    )
+
 
 class IRuleActionDirective(IRuleElementDirective):
-    """An element directive describing what is logically an action element.
-    """
+    """An element directive describing what is logically an action element."""
+
 
 class IRuleConditionDirective(IRuleElementDirective):
-    """An element directive describing what is logically a condition element.
-    """
+    """An element directive describing what is logically a condition element."""
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/rule/tests/elements.py` & `plone.contentrules-3.0.0/plone/contentrules/rule/tests/elements.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Dummies used in ZCML tests
 """
 
-from zope.interface import Interface, implementer
+from plone.contentrules.rule.interfaces import IRuleElementData
 from zope import schema
+from zope.interface import implementer
+from zope.interface import Interface
 
-from plone.contentrules.rule.interfaces import IRuleElementData
 
 class ITestCondition(Interface):
-    test = schema.TextLine(title=u"Test property")
+    test = schema.TextLine(title="Test property")
+
 
 @implementer(ITestCondition, IRuleElementData)
-class TestCondition(object):
-    test = u""
+class TestCondition:
+    test = ""
+
+    summary = "Test condition"
+    element = "test.condition"
 
-    summary = u"Test condition"
-    element = u"test.condition"
 
 class ITestAction(Interface):
-    test = schema.TextLine(title=u"Test property")
+    test = schema.TextLine(title="Test property")
+
 
 @implementer(ITestAction, IRuleElementData)
-class TestAction(object):
-    test = u""
+class TestAction:
+    test = ""
 
-    summary = u"Test action"
-    element = u"test.action"
+    summary = "Test action"
+    element = "test.action"
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/tests.py` & `plone.contentrules-3.0.0/plone/contentrules/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-import doctest
-import re
-import six
-import unittest
-
 from zope.component.testing import PlacelessSetup as CAPlacelessSetup
 from zope.configuration.xmlconfig import XMLConfig
 from zope.container.testing import PlacelessSetup as ContainerPlacelessSetup
 
-optionflags = doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS
-
+import doctest
+import unittest
 
-class Py23DocChecker(doctest.OutputChecker):
 
-    def check_output(self, want, got, optionflags):
-        if six.PY2:
-            got = re.sub("u'(.*?)'", "'\\1'", got)
-        return doctest.OutputChecker.check_output(self, want, got, optionflags)
+optionflags = doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS
 
 
 class PlacelessSetup(CAPlacelessSetup, ContainerPlacelessSetup):
-
     def setUp(self, doctesttest=None):
         CAPlacelessSetup.setUp(self)
         ContainerPlacelessSetup.setUp(self)
 
+
 ps = PlacelessSetup()
 
 
 def configurationSetUp(test):
     ps.setUp()
     import zope.component
-    XMLConfig('meta.zcml', zope.component)()
+
+    XMLConfig("meta.zcml", zope.component)()
 
     import plone.contentrules
-    XMLConfig('configure.zcml', plone.contentrules)()
+
+    XMLConfig("configure.zcml", plone.contentrules)()
 
 
 def configurationTearDown(test):
     ps.tearDown()
 
 
 def test_suite():
-    return unittest.TestSuite((
-        doctest.DocFileSuite(
-            'README.rst',
-            setUp=configurationSetUp,
-            tearDown=configurationTearDown,
-            optionflags=optionflags,
-            checker=Py23DocChecker(),
+    return unittest.TestSuite(
+        (
+            doctest.DocFileSuite(
+                "README.rst",
+                setUp=configurationSetUp,
+                tearDown=configurationTearDown,
+                optionflags=optionflags,
             ),
-        doctest.DocFileSuite(
-            'zcml.rst',
-            setUp=configurationSetUp,
-            tearDown=configurationTearDown,
-            optionflags=optionflags,
-            checker=Py23DocChecker(),
+            doctest.DocFileSuite(
+                "zcml.rst",
+                setUp=configurationSetUp,
+                tearDown=configurationTearDown,
+                optionflags=optionflags,
             ),
-        ))
+        )
+    )
```

### Comparing `plone.contentrules-2.1.3/plone/contentrules/zcml.rst` & `plone.contentrules-3.0.0/plone/contentrules/zcml.rst`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
     ...         schema=".rule.tests.elements.ITestAction"
     ...         factory=".rule.tests.elements.TestAction"
     ...         />
     ... </configure>
     ... """
 
     >>> from zope.configuration.xmlconfig import xmlconfig
-    >>> import six
-    >>> from six import StringIO
+    >>> from io import StringIO
 
 First, we need to make sure the ZCML directives are defined:
 
     >>> from zope.configuration.xmlconfig import XMLConfig
     >>> import plone.contentrules
     >>> XMLConfig('meta.zcml', plone.contentrules)()
```

### Comparing `plone.contentrules-2.1.3/plone.contentrules.egg-info/PKG-INFO` & `plone.contentrules-3.0.0/plone.contentrules.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.contentrules
-Version: 2.1.3
+Version: 3.0.0
 Summary: Plone ContentRules Engine
 Home-page: https://pypi.org/project/plone.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone content rules events
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope2
 Classifier: Framework :: Zope :: 4
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 
 Overview
 ========
 
 plone.contentrules provides a "pure Zope" implementation of a a rules engine
 which allows arbitrary conditions and actions to be combined into rules, and
 rules to be executed dependent on events.
@@ -40,14 +40,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Drop python 2.7.
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
 2.1.3 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.contentrules-2.1.3/plone.contentrules.egg-info/SOURCES.txt` & `plone.contentrules-3.0.0/plone.contentrules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

