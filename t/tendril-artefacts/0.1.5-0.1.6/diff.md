# Comparing `tmp/tendril-artefacts-0.1.5.tar.gz` & `tmp/tendril-artefacts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-artefacts-0.1.5.tar", last modified: Mon Mar 27 15:58:40 2023, max compression
+gzip compressed data, was "tendril-artefacts-0.1.6.tar", last modified: Wed Apr 19 09:33:22 2023, max compression
```

## Comparing `tendril-artefacts-0.1.5.tar` & `tendril-artefacts-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3980 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.714516 tendril-artefacts-0.1.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril/artefacts/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/src/tendril/artefacts/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/src/tendril/artefacts/base.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril/artefacts/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/src/tendril/artefacts/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1049 2022-12-11 07:25:27.000000 tendril-artefacts-0.1.5/src/tendril/artefacts/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1716 2023-03-27 15:55:38.000000 tendril-artefacts-0.1.5/src/tendril/artefacts/db/model.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.5/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.5/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.5/src/tendril/authz/roles/artefacts.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3980 2023-03-27 15:58:40.000000 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2023-03-27 15:58:40.000000 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-27 15:58:40.000000 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2023-03-27 15:58:40.000000 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-27 15:58:40.000000 tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-27 15:58:40.718515 tendril-artefacts-0.1.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.985175 tendril-artefacts-0.1.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3170 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.985175 tendril-artefacts-0.1.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/artefacts/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       39 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/base.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/artefacts/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1049 2022-12-11 07:25:27.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1722 2023-04-19 09:30:08.000000 tendril-artefacts-0.1.6/src/tendril/artefacts/db/model.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      205 2023-03-04 01:26:57.000000 tendril-artefacts-0.1.6/src/tendril/authz/roles/artefacts.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.989175 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      932 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      513 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-19 09:33:22.000000 tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 09:33:22.993175 tendril-artefacts-0.1.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-10 17:14:56.000000 tendril-artefacts-0.1.6/tox.ini
```

### Comparing `tendril-artefacts-0.1.5/.gitignore` & `tendril-artefacts-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/.readthedocs.yml` & `tendril-artefacts-0.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/.travis.yml` & `tendril-artefacts-0.1.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/LICENSE` & `tendril-artefacts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/PKG-INFO` & `tendril-artefacts-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-artefacts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Core Artefact Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-artefacts
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-artefacts.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-artefacts/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-artefacts
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-artefacts.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-artefacts
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-artefacts.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-artefacts
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-artefacts.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-artefacts
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-artefacts.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-artefacts
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-artefacts
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-artefacts.svg
-            :target: https://requires.io/github/tendril-framework/tendril-artefacts/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-artefacts.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-artefacts.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-artefacts>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-artefacts`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-artefacts`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-artefacts.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-artefacts
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-artefacts.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-artefacts
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-artefacts.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-artefacts
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-artefacts.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-artefacts
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-artefacts
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-artefacts.svg
+    :target: https://requires.io/github/tendril-framework/tendril-artefacts/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-artefacts.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-artefacts.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-artefacts>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-artefacts`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-artefacts`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-artefacts-0.1.5/README.rst` & `tendril-artefacts-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/Makefile` & `tendril-artefacts-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/_static/custom.css` & `tendril-artefacts-0.1.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/_static/favicon.ico` & `tendril-artefacts-0.1.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/_static/logo.png` & `tendril-artefacts-0.1.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/_static/logo_packed.png` & `tendril-artefacts-0.1.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/_templates/about.html` & `tendril-artefacts-0.1.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/conf.py` & `tendril-artefacts-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/index.rst` & `tendril-artefacts-0.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/docs/installation.rst` & `tendril-artefacts-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/setup.py` & `tendril-artefacts-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/src/tendril/artefacts/db/controller.py` & `tendril-artefacts-0.1.6/src/tendril/artefacts/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/src/tendril/artefacts/db/model.py` & `tendril-artefacts-0.1.6/src/tendril/artefacts/db/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 class ArtefactModel(DeclBase, BaseMixin, TimestampMixin, UserMixin):
     _type_name = "artefact"
     type = Column(String(50), nullable=False, default=_type_name)
     title = Column(String(255), nullable=True)
     label = Column(String(50), nullable=True)
     active = Column(Boolean, nullable=False, default=True)
 
-    @declared_attr
-    def interest_id(cls):
-        return Column(Integer, ForeignKey('Interest.id'))
+    # @declared_attr
+    # def interest_id(cls):
+    #     return Column(Integer, ForeignKey('Interest.id'))
 
     # @declared_attr
     # def interest(cls):
     #     return relationship('InterestModel', back_populates="artefacts")
 
     @declared_attr
     def logs(cls):
```

### Comparing `tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/PKG-INFO` & `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-artefacts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Core Artefact Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-artefacts
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-artefacts.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-artefacts/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-artefacts
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-artefacts.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-artefacts
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-artefacts.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-artefacts
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-artefacts.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-artefacts
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-artefacts.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-artefacts
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-artefacts
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-artefacts.svg
-            :target: https://requires.io/github/tendril-framework/tendril-artefacts/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-artefacts.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-artefacts.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-artefacts>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-artefacts`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-artefacts`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-artefacts.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-artefacts
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-artefacts.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-artefacts
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-artefacts.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-artefacts
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-artefacts.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-artefacts
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-artefacts
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-artefacts.svg
+    :target: https://requires.io/github/tendril-framework/tendril-artefacts/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-artefacts.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-artefacts.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-artefacts>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-artefacts`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-artefacts`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/SOURCES.txt` & `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/src/tendril_artefacts.egg-info/requires.txt` & `tendril-artefacts-0.1.6/src/tendril_artefacts.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/tests/coveralls.py` & `tendril-artefacts-0.1.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-artefacts-0.1.5/tox.ini` & `tendril-artefacts-0.1.6/tox.ini`

 * *Files identical despite different names*

