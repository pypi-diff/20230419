# Comparing `tmp/xh-cpu-usage-simulator-0.0.8.tar.gz` & `tmp/xh-cpu-usage-simulator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-cpu-usage-simulator-0.0.8.tar", last modified: Wed Apr 19 09:50:06 2023, max compression
+gzip compressed data, was "xh-cpu-usage-simulator-0.0.9.tar", last modified: Wed Apr 19 09:54:36 2023, max compression
```

## Comparing `xh-cpu-usage-simulator-0.0.8.tar` & `xh-cpu-usage-simulator-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:50:06.877694 xh-cpu-usage-simulator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 09:50:06.877694 xh-cpu-usage-simulator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:50:06.877694 xh-cpu-usage-simulator-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:50:06.873694 xh-cpu-usage-simulator-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:50:06.873694 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/MovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/PsMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/TaskWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/TestMovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-19 09:49:55.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:50:06.877694 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 09:50:06.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 09:50:06.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:50:06.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 09:50:06.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 09:50:06.000000 xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:54:36.629593 xh-cpu-usage-simulator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 09:54:36.629593 xh-cpu-usage-simulator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:54:36.629593 xh-cpu-usage-simulator-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:54:36.625594 xh-cpu-usage-simulator-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:54:36.625594 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/MovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/PsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/TaskWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/TestMovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-19 09:54:18.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:54:36.625594 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 09:54:36.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 09:54:36.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:54:36.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 09:54:36.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 09:54:36.000000 xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/top_level.txt
```

### Comparing `xh-cpu-usage-simulator-0.0.8/LICENSE.txt` & `xh-cpu-usage-simulator-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/PKG-INFO` & `xh-cpu-usage-simulator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.0.8/pyproject.toml` & `xh-cpu-usage-simulator-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-cpu-usage-simulator"
-version = "0.0.8"
+version = "0.0.9"
 description = "Tools simulating the cpu usage"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "psutil==5.9.5", "scikit-learn==1.2.2", "numpy==1.24.2",]
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/MovingAvg.py` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/MovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/TaskWorker.py` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/TaskWorker.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/TestMovingAvg.py` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/TestMovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator/__main__.py` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator/__main__.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/PKG-INFO` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.0.8/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt` & `xh-cpu-usage-simulator-0.0.9/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

