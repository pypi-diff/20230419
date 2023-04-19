# Comparing `tmp/xh-cpu-usage-simulator-0.1.0.tar.gz` & `tmp/xh-cpu-usage-simulator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-cpu-usage-simulator-0.1.0.tar", last modified: Wed Apr 19 16:16:14 2023, max compression
+gzip compressed data, was "xh-cpu-usage-simulator-0.1.1.tar", last modified: Wed Apr 19 16:34:09 2023, max compression
```

## Comparing `xh-cpu-usage-simulator-0.1.0.tar` & `xh-cpu-usage-simulator-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/MovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/PsMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/TaskWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/TestMovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 16:16:03.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.493769 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:16:14.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 16:16:14.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:16:14.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 16:16:14.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 16:16:14.000000 xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/MovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/PsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/TaskWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/TestMovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 16:33:57.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:09.172829 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:34:09.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 16:34:09.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:34:09.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 16:34:09.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 16:34:09.000000 xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/top_level.txt
```

### Comparing `xh-cpu-usage-simulator-0.1.0/LICENSE.txt` & `xh-cpu-usage-simulator-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/PKG-INFO` & `xh-cpu-usage-simulator-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.1.0/pyproject.toml` & `xh-cpu-usage-simulator-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-cpu-usage-simulator"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tools simulating the cpu usage"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "psutil==5.9.5", "scikit-learn==1.2.2", "numpy==1.24.2",]
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/MovingAvg.py` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/MovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/TaskWorker.py` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/TaskWorker.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/TestMovingAvg.py` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/TestMovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator/__main__.py` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator/__main__.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/PKG-INFO` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.1.0/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt` & `xh-cpu-usage-simulator-0.1.1/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

