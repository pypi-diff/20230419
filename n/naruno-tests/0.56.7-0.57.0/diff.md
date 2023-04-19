# Comparing `tmp/naruno_tests-0.56.7.tar.gz` & `tmp/naruno_tests-0.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_tests-0.56.7.tar", last modified: Wed Apr 19 00:40:54 2023, max compression
+gzip compressed data, was "naruno_tests-0.57.0.tar", last modified: Wed Apr 19 11:38:13 2023, max compression
```

## Comparing `naruno_tests-0.56.7.tar` & `naruno_tests-0.57.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:54.371640 naruno_tests-0.56.7/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 00:40:54.371640 naruno_tests-0.56.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:54.371640 naruno_tests-0.56.7/naruno_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:54.000000 naruno_tests-0.56.7/naruno_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:40:54.371640 naruno_tests-0.56.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-19 00:40:28.000000 naruno_tests-0.56.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:38:13.858538 naruno_tests-0.57.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 11:38:13.858538 naruno_tests-0.57.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:38:13.858538 naruno_tests-0.57.0/naruno_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:13.000000 naruno_tests-0.57.0/naruno_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:38:13.858538 naruno_tests-0.57.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-19 11:37:54.000000 naruno_tests-0.57.0/setup.py
```

### Comparing `naruno_tests-0.56.7/setup.py` & `naruno_tests-0.57.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_tests",
-    version="0.56.7",
+    version="0.57.0",
     description="""This is a tool for tests on Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 requests==2.28.2
 pytest==7.1.2
 speed_calculator==0.4.1
-naruno_api==0.56.7
+naruno_api==0.57.0
 """,
     python_requires=">=3.8",
     zip_safe=False,
 )
```

