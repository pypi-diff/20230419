# Comparing `tmp/flytekitplugins-athena-1.5.0b1.tar.gz` & `tmp/flytekitplugins-athena-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-athena-1.5.0b1.tar", last modified: Wed Mar 29 18:58:35 2023, max compression
+gzip compressed data, was "flytekitplugins-athena-1.6.0b0.tar", last modified: Wed Apr 19 20:54:25 2023, max compression
```

## Comparing `flytekitplugins-athena-1.5.0b1.tar` & `flytekitplugins-athena-1.6.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-29 18:58:20.000000 flytekitplugins-athena-1.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/flytekitplugins/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-29 18:58:20.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-03-29 18:58:20.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins/athena/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:35.000000 flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 18:58:35.300240 flytekitplugins-athena-1.5.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-29 18:58:34.000000 flytekitplugins-athena-1.5.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:25.715016 flytekitplugins-athena-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 20:54:25.715016 flytekitplugins-athena-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 20:54:06.000000 flytekitplugins-athena-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:25.711016 flytekitplugins-athena-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:25.711016 flytekitplugins-athena-1.6.0b0/flytekitplugins/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 20:54:06.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-19 20:54:06.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins/athena/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:25.715016 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:25.715016 flytekitplugins-athena-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-19 20:54:25.000000 flytekitplugins-athena-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-athena-1.5.0b1/PKG-INFO` & `flytekitplugins-athena-1.6.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-athena
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: This package holds the Athena plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-athena-1.5.0b1/flytekitplugins/athena/task.py` & `flytekitplugins-athena-1.6.0b0/flytekitplugins/athena/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-athena-1.5.0b1/flytekitplugins_athena.egg-info/PKG-INFO` & `flytekitplugins-athena-1.6.0b0/flytekitplugins_athena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-athena
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: This package holds the Athena plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-athena-1.5.0b1/setup.py` & `flytekitplugins-athena-1.6.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "athena"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Athena plugins for flytekit",
```

