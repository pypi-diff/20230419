# Comparing `tmp/plone.base-1.1.1.tar.gz` & `tmp/plone.base-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.base-1.1.1.tar", last modified: Sat Apr 15 09:08:27 2023, max compression
+gzip compressed data, was "plone.base-1.1.2.tar", last modified: Wed Apr 19 07:21:34 2023, max compression
```

## Comparing `plone.base-1.1.1.tar` & `plone.base-1.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.479372 plone.base-1.1.1/
--rw-r--r--   0 gil       (1000) gil       (1000)     3963 2023-04-15 09:08:26.000000 plone.base-1.1.1/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-15 09:08:26.000000 plone.base-1.1.1/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)     6946 2023-04-15 09:08:27.479372 plone.base-1.1.1/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2026 2023-04-15 09:08:26.000000 plone.base-1.1.1/README.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2834 2023-04-15 09:08:26.000000 plone.base-1.1.1/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)     1623 2023-04-15 09:08:27.479372 plone.base-1.1.1/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)       39 2023-04-15 09:08:26.000000 plone.base-1.1.1/setup.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.474372 plone.base-1.1.1/src/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.474372 plone.base-1.1.1/src/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.476372 plone.base-1.1.1/src/plone/base/
--rw-r--r--   0 gil       (1000) gil       (1000)      238 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2894 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/batch.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5502 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/defaultpage.py
--rw-r--r--   0 gil       (1000) gil       (1000)    12074 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/i18nl10n.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.478372 plone.base-1.1.1/src/plone/base/interfaces/
--rw-r--r--   0 gil       (1000) gil       (1000)     2622 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      305 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/atd.py
--rw-r--r--   0 gil       (1000) gil       (1000)      289 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/basetool.py
--rw-r--r--   0 gil       (1000) gil       (1000)      151 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/breadcrumbs.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3060 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/constrains.py
--rw-r--r--   0 gil       (1000) gil       (1000)    63997 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/controlpanel.py
--rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/defaultpage.py
--rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/events.py
--rw-r--r--   0 gil       (1000) gil       (1000)      776 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/images.py
--rw-r--r--   0 gil       (1000) gil       (1000)      529 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/installable.py
--rw-r--r--   0 gil       (1000) gil       (1000)      697 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/interface.py
--rw-r--r--   0 gil       (1000) gil       (1000)      229 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/language.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1993 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/login.py
--rw-r--r--   0 gil       (1000) gil       (1000)      853 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/migration.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1471 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/password_reset.py
--rw-r--r--   0 gil       (1000) gil       (1000)      243 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/patterns.py
--rw-r--r--   0 gil       (1000) gil       (1000)      496 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/properties.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4824 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/resources.py
--rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/siteroot.py
--rw-r--r--   0 gil       (1000) gil       (1000)      453 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/structure.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6328 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/syndication.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1499 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/translationservice.py
--rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/workflow.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2196 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/navigationroot.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2267 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/permissions.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.479372 plone.base-1.1.1/src/plone/base/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3507 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/messages.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1387 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_batch.py
--rw-r--r--   0 gil       (1000) gil       (1000)      226 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_doctests.py
--rw-r--r--   0 gil       (1000) gil       (1000)    17956 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_i18nl10n.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6869 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)    20178 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/utils.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.475372 plone.base-1.1.1/src/plone.base.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     6946 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      152 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/top_level.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.009000 plone.base-1.1.2/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4115 2023-04-19 07:21:33.000000 plone.base-1.1.2/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-19 07:21:33.000000 plone.base-1.1.2/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     7097 2023-04-19 07:21:34.009000 plone.base-1.1.2/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2025 2023-04-19 07:21:33.000000 plone.base-1.1.2/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2834 2023-04-19 07:21:33.000000 plone.base-1.1.2/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1623 2023-04-19 07:21:34.009000 plone.base-1.1.2/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)       39 2023-04-19 07:21:33.000000 plone.base-1.1.2/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.003000 plone.base-1.1.2/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.004000 plone.base-1.1.2/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.006000 plone.base-1.1.2/src/plone/base/
+-rw-r--r--   0 gil       (1000) gil       (1000)      238 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2894 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/batch.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5502 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/defaultpage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    12074 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/i18nl10n.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.008000 plone.base-1.1.2/src/plone/base/interfaces/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2622 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      305 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/atd.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      289 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/basetool.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      151 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/breadcrumbs.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3060 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/constrains.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    63997 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/defaultpage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      776 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/images.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      529 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/installable.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      697 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/interface.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      229 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/language.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1993 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/login.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      853 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/migration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1471 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/password_reset.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      243 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/patterns.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      496 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/properties.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4824 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/resources.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/siteroot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      453 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/structure.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6328 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/syndication.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1499 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/translationservice.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/interfaces/workflow.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2196 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/navigationroot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2267 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/permissions.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.009000 plone.base-1.1.2/src/plone/base/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3507 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/messages.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1387 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_batch.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      226 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_doctests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    17956 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_i18nl10n.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6869 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20346 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone/base/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-19 07:21:34.005000 plone.base-1.1.2/src/plone.base.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     7097 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      152 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-19 07:21:33.000000 plone.base-1.1.2/src/plone.base.egg-info/top_level.txt
```

### Comparing `plone.base-1.1.1/CHANGES.rst` & `plone.base-1.1.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.2 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Check for container field / attribute when trying to create content with same id [laulaz] (#35)
+
+
 1.1.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.base-1.1.1/PKG-INFO` & `plone.base-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.1
+Version: 1.1.2
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -61,15 +61,14 @@
     Plone specific handling of navigation roots.
     Before those been at ``plone.app.layout.navigation.root``.
 
 ``__init__``
     ``PloneMessageFactory`` with ``plone`` i18n-domain and ``PloneLocalesMessageFactory`` with ``plonelocales`` domain.
     In Plone 5 and below this was at ``Products.CMFPlone.__init__``.
 
-
 Source Code
 ===========
 
 Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
 
 Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.base>`_.
 
@@ -81,14 +80,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.2 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Check for container field / attribute when trying to create content with same id [laulaz] (#35)
+
+
 1.1.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.base-1.1.1/README.rst` & `plone.base-1.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     Plone specific handling of navigation roots.
     Before those been at ``plone.app.layout.navigation.root``.
 
 ``__init__``
     ``PloneMessageFactory`` with ``plone`` i18n-domain and ``PloneLocalesMessageFactory`` with ``plonelocales`` domain.
     In Plone 5 and below this was at ``Products.CMFPlone.__init__``.
 
-
 Source Code
 ===========
 
 Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
 
 Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.base>`_.
```

### Comparing `plone.base-1.1.1/pyproject.toml` & `plone.base-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/setup.cfg` & `plone.base-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.1
+version = 1.1.2
 name = plone.base
 description = Plone Interface contracts, plus basic features and utilities
 long_description = file: README.rst, CHANGES.rst
 keywords = plone
 author = Jens W. Klein
 author_email = jk@kleinundpartner.at
 maintainer = Plone Release Team
```

### Comparing `plone.base-1.1.1/src/plone/base/batch.py` & `plone.base-1.1.2/src/plone/base/batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/defaultpage.py` & `plone.base-1.1.2/src/plone/base/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/i18nl10n.py` & `plone.base-1.1.2/src/plone/base/i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/__init__.py` & `plone.base-1.1.2/src/plone/base/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/constrains.py` & `plone.base-1.1.2/src/plone/base/interfaces/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/controlpanel.py` & `plone.base-1.1.2/src/plone/base/interfaces/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/events.py` & `plone.base-1.1.2/src/plone/base/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/images.py` & `plone.base-1.1.2/src/plone/base/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/installable.py` & `plone.base-1.1.2/src/plone/base/interfaces/installable.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/interface.py` & `plone.base-1.1.2/src/plone/base/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/login.py` & `plone.base-1.1.2/src/plone/base/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/migration.py` & `plone.base-1.1.2/src/plone/base/interfaces/migration.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/password_reset.py` & `plone.base-1.1.2/src/plone/base/interfaces/password_reset.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/resources.py` & `plone.base-1.1.2/src/plone/base/interfaces/resources.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/siteroot.py` & `plone.base-1.1.2/src/plone/base/interfaces/siteroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/syndication.py` & `plone.base-1.1.2/src/plone/base/interfaces/syndication.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/interfaces/translationservice.py` & `plone.base-1.1.2/src/plone/base/interfaces/translationservice.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/navigationroot.py` & `plone.base-1.1.2/src/plone/base/navigationroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/permissions.py` & `plone.base-1.1.2/src/plone/base/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/tests/messages.rst` & `plone.base-1.1.2/src/plone/base/tests/messages.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/tests/test_batch.py` & `plone.base-1.1.2/src/plone/base/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/tests/test_i18nl10n.py` & `plone.base-1.1.2/src/plone/base/tests/test_i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/tests/test_utils.py` & `plone.base-1.1.2/src/plone/base/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.1/src/plone/base/utils.py` & `plone.base-1.1.2/src/plone/base/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,14 +502,18 @@
         existing_obj = getattr(contained_by, cid, None)
         if getattr(aq_base(existing_obj), "portal_type", _marker) is not _marker:
             return _(
                 "There is already an item named ${name} in this folder.",
                 mapping={"name": cid},
             )
 
+    # containers may have a field / attribute of the same name
+    if base_hasattr(contained_by, cid):
+        return _("${name} is reserved.", mapping={"name": cid})
+
     # containers may implement this hook to further restrict ids
     if getattr(aq_base(contained_by), "checkValidId", _marker) is not _marker:
         try:
             contained_by.checkValidId(cid)
         except ConflictError:
             raise
         except Exception:
```

### Comparing `plone.base-1.1.1/src/plone.base.egg-info/PKG-INFO` & `plone.base-1.1.2/src/plone.base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.1
+Version: 1.1.2
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -61,15 +61,14 @@
     Plone specific handling of navigation roots.
     Before those been at ``plone.app.layout.navigation.root``.
 
 ``__init__``
     ``PloneMessageFactory`` with ``plone`` i18n-domain and ``PloneLocalesMessageFactory`` with ``plonelocales`` domain.
     In Plone 5 and below this was at ``Products.CMFPlone.__init__``.
 
-
 Source Code
 ===========
 
 Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
 
 Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.base>`_.
 
@@ -81,14 +80,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.2 (2023-04-19)
+------------------
+
+Bug fixes:
+
+
+- Check for container field / attribute when trying to create content with same id [laulaz] (#35)
+
+
 1.1.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.base-1.1.1/src/plone.base.egg-info/SOURCES.txt` & `plone.base-1.1.2/src/plone.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

