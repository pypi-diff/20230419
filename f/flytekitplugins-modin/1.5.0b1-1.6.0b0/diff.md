# Comparing `tmp/flytekitplugins-modin-1.5.0b1.tar.gz` & `tmp/flytekitplugins-modin-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-modin-1.5.0b1.tar", last modified: Wed Mar 29 18:58:41 2023, max compression
+gzip compressed data, was "flytekitplugins-modin-1.6.0b0.tar", last modified: Wed Apr 19 20:54:32 2023, max compression
```

## Comparing `flytekitplugins-modin-1.5.0b1.tar` & `flytekitplugins-modin-1.6.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:41.476241 flytekitplugins-modin-1.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-29 18:58:41.476241 flytekitplugins-modin-1.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-29 18:58:20.000000 flytekitplugins-modin-1.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:41.476241 flytekitplugins-modin-1.5.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:41.476241 flytekitplugins-modin-1.5.0b1/flytekitplugins/modin/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-29 18:58:20.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins/modin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-29 18:58:20.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins/modin/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:41.476241 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:41.000000 flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 18:58:41.480241 flytekitplugins-modin-1.5.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-29 18:58:35.000000 flytekitplugins-modin-1.5.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 20:54:06.000000 flytekitplugins-modin-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/flytekitplugins/modin/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-19 20:54:06.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins/modin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-19 20:54:06.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins/modin/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:32.000000 flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:32.603118 flytekitplugins-modin-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 20:54:25.000000 flytekitplugins-modin-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-modin-1.5.0b1/PKG-INFO` & `flytekitplugins-modin-1.6.0b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.5.0b1/README.md` & `flytekitplugins-modin-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.5.0b1/flytekitplugins/modin/schema.py` & `flytekitplugins-modin-1.6.0b0/flytekitplugins/modin/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.5.0b1/flytekitplugins_modin.egg-info/PKG-INFO` & `flytekitplugins-modin-1.6.0b0/flytekitplugins_modin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.5.0b1/setup.py` & `flytekitplugins-modin-1.6.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit<1.3.0b2,<2.0.0",
     "modin>=0.13.0",
     "fsspec",
     "ray",
 ]
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Intel",
     description="Modin plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

