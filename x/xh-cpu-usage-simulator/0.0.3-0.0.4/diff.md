# Comparing `tmp/xh-cpu-usage-simulator-0.0.3.tar.gz` & `tmp/xh-cpu-usage-simulator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-cpu-usage-simulator-0.0.3.tar", last modified: Tue Apr 18 17:20:47 2023, max compression
+gzip compressed data, was "xh-cpu-usage-simulator-0.0.4.tar", last modified: Wed Apr 19 06:50:13 2023, max compression
```

## Comparing `xh-cpu-usage-simulator-0.0.3.tar` & `xh-cpu-usage-simulator-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:20:47.403249 xh-cpu-usage-simulator-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-18 17:20:47.403249 xh-cpu-usage-simulator-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:20:47.403249 xh-cpu-usage-simulator-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:20:47.399249 xh-cpu-usage-simulator-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:20:47.399249 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/MovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/PsMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/TaskWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/TestMovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-18 17:20:34.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:20:47.403249 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-18 17:20:47.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-18 17:20:47.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:20:47.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:20:47.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 17:20:47.000000 xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:50:13.441880 xh-cpu-usage-simulator-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 06:50:13.441880 xh-cpu-usage-simulator-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 06:50:13.441880 xh-cpu-usage-simulator-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:50:13.437880 xh-cpu-usage-simulator-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:50:13.441880 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/MovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/PsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/TaskWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/TestMovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-19 06:49:59.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:50:13.441880 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 06:50:13.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 06:50:13.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:50:13.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 06:50:13.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 06:50:13.000000 xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/top_level.txt
```

### Comparing `xh-cpu-usage-simulator-0.0.3/LICENSE.txt` & `xh-cpu-usage-simulator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.3/PKG-INFO` & `xh-cpu-usage-simulator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.0.3/pyproject.toml` & `xh-cpu-usage-simulator-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-cpu-usage-simulator"
-version = "0.0.3"
+version = "0.0.4"
 description = "Tools simulating the cpu usage"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "psutil==5.9.5",]
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/MovingAvg.py` & `xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/MovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/TestMovingAvg.py` & `xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/TestMovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator/__main__.py` & `xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,14 @@
                     print(
                         f"{rounds:05d}::Targeting[{target}], now[{m_avg.avg}], increase operation from {cur_total_operation} to {new_total_operation}")
                 elif target * 1.05 < m_avg.avg:
                     for i in d:
                         d[i] = d[i] * 0.85
                     new_total_operation = sum([d[i] for i in d])
                     print(
-                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], increase operation from {cur_total_operation} to {new_total_operation}")
+                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], decreate operation from {cur_total_operation} to {new_total_operation}")
                 else:
                     print(
                         f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], nothing to do")
         m_avg.insert(m.avg)
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `xh-cpu-usage-simulator-0.0.3/src/xh_cpu_usage_simulator.egg-info/PKG-INFO` & `xh-cpu-usage-simulator-0.0.4/src/xh_cpu_usage_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

