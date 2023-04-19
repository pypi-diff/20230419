# Comparing `tmp/dkredis-0.1.7.tar.gz` & `tmp/dkredis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkredis-0.1.7.tar", last modified: Wed Apr 19 11:49:33 2023, max compression
+gzip compressed data, was "dkredis-0.1.8.tar", last modified: Wed Apr 19 11:54:55 2023, max compression
```

## Comparing `dkredis-0.1.7.tar` & `dkredis-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 11:49:33.409312 dkredis-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 11:49:18.000000 dkredis-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/dkredis/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/dkredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-19 11:49:18.000000 dkredis-0.1.7/dkredis/rediscache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:49:33.409312 dkredis-0.1.7/dkredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:49:33.000000 dkredis-0.1.7/dkredis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 11:49:33.413312 dkredis-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 11:49:18.000000 dkredis-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 11:54:55.875089 dkredis-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-19 11:54:44.000000 dkredis-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/dkredis/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/dkredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/rediscache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/dkredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 11:54:55.875089 dkredis-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 11:54:44.000000 dkredis-0.1.8/setup.py
```

### Comparing `dkredis-0.1.7/PKG-INFO` & `dkredis-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkredis
-Version: 0.1.7
+Version: 0.1.8
 Summary: dkredis - Python interface to Redis
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -15,17 +15,21 @@
 
 dkredis - Python interface to Redis
 ===================================
 
 .. image:: https://coveralls.io/repos/github/datakortet/dkredis/badge.svg?branch=master
     :target: https://coveralls.io/github/datakortet/dkredis?branch=master
 
-.. image:: https://gitlab.com/norsktest/dkredis/badges/master/pipeline.svg
-   :target: https://gitlab.com/norsktest/dkredis/commits/master
-   :alt: pipeline status
+.. .. image:: https://gitlab.com/norsktest/dkredis/badges/master/pipeline.svg
+..    :target: https://gitlab.com/norsktest/dkredis/commits/master
+..    :alt: pipeline status
+
+.. image:: https://github.com/datakortet/dkredis/actions/workflows/ci-cd.yml/badge.svg
+   :target: https://github.com/datakortet/dkredis/actions/workflows/ci-cd.yml
+   :alt: CI/CD Pipeline
 
 .. image:: https://img.shields.io/badge/docs-darkgreen.svg
    :target: https://norsktest.gitlab.io/dkredis
    :alt: documentation
 
 .. image:: https://codecov.io/gl/norsktest/dkredis/branch/master/graph/badge.svg?token=2QOZN0V09V
   :target: https://codecov.io/gl/norsktest/dkredis
```

### Comparing `dkredis-0.1.7/dkredis/dkredis.py` & `dkredis-0.1.8/dkredis/dkredis.py`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.7/dkredis/rediscache.py` & `dkredis-0.1.8/dkredis/rediscache.py`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.7/dkredis.egg-info/PKG-INFO` & `dkredis-0.1.8/dkredis.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkredis
-Version: 0.1.7
+Version: 0.1.8
 Summary: dkredis - Python interface to Redis
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -15,17 +15,21 @@
 
 dkredis - Python interface to Redis
 ===================================
 
 .. image:: https://coveralls.io/repos/github/datakortet/dkredis/badge.svg?branch=master
     :target: https://coveralls.io/github/datakortet/dkredis?branch=master
 
-.. image:: https://gitlab.com/norsktest/dkredis/badges/master/pipeline.svg
-   :target: https://gitlab.com/norsktest/dkredis/commits/master
-   :alt: pipeline status
+.. .. image:: https://gitlab.com/norsktest/dkredis/badges/master/pipeline.svg
+..    :target: https://gitlab.com/norsktest/dkredis/commits/master
+..    :alt: pipeline status
+
+.. image:: https://github.com/datakortet/dkredis/actions/workflows/ci-cd.yml/badge.svg
+   :target: https://github.com/datakortet/dkredis/actions/workflows/ci-cd.yml
+   :alt: CI/CD Pipeline
 
 .. image:: https://img.shields.io/badge/docs-darkgreen.svg
    :target: https://norsktest.gitlab.io/dkredis
    :alt: documentation
 
 .. image:: https://codecov.io/gl/norsktest/dkredis/branch/master/graph/badge.svg?token=2QOZN0V09V
   :target: https://codecov.io/gl/norsktest/dkredis
```

### Comparing `dkredis-0.1.7/setup.py` & `dkredis-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 Programming Language :: Python
 Programming Language :: Python :: 3
 Topic :: Software Development :: Libraries
 """
 
 import setuptools
 
-version = '0.1.7'
+version = '0.1.8'
 
 setuptools.setup(
     name='dkredis',
     version=version,
     install_requires=[
-        'redis==3.5.3',
+        'redis==4.5.4',
     ],
     description=__doc__.strip(),
     classifiers=[line for line in classifiers.split('\n') if line],
     long_description=open('README.rst').read(),
     packages=['dkredis'],
     zip_safe=False,
 )
```

