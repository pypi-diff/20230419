# Comparing `tmp/xh-cpu-usage-simulator-0.0.5.tar.gz` & `tmp/xh-cpu-usage-simulator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-cpu-usage-simulator-0.0.5.tar", last modified: Wed Apr 19 07:02:51 2023, max compression
+gzip compressed data, was "xh-cpu-usage-simulator-0.0.6.tar", last modified: Wed Apr 19 07:25:33 2023, max compression
```

## Comparing `xh-cpu-usage-simulator-0.0.5.tar` & `xh-cpu-usage-simulator-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/MovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/PsMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/TaskWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/TestMovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-19 07:02:39.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:02:51.007438 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 07:02:50.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 07:02:51.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:02:50.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 07:02:51.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 07:02:51.000000 xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/MovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/PsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/TaskWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/TestMovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-19 07:25:21.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:25:33.402305 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 07:25:33.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 07:25:33.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:25:33.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 07:25:33.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 07:25:33.000000 xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/top_level.txt
```

### Comparing `xh-cpu-usage-simulator-0.0.5/LICENSE.txt` & `xh-cpu-usage-simulator-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.5/PKG-INFO` & `xh-cpu-usage-simulator-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.0.5/pyproject.toml` & `xh-cpu-usage-simulator-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-cpu-usage-simulator"
-version = "0.0.5"
+version = "0.0.6"
 description = "Tools simulating the cpu usage"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "psutil==5.9.5",]
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/MovingAvg.py` & `xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/MovingAvg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 class MovingAvg():
-    def __init__(self, size: int):
+    def __init__(self, size: float):
         self.data = []
         self.size = size
         self.cur_index = 0
         self.avg = 0
         for _ in range(size):
             self.data.append(0)
 
-    def insert(self, value: int):
+    def insert(self, value: float):
         self.data[self.cur_index] = value
         self.cur_index = (self.cur_index + 1) % self.size
         self.avg = round(sum(self.data) / self.size, 2)
 
     def __repr__(self):
         return f"{self.size} - {self.avg}"
```

### Comparing `xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/TestMovingAvg.py` & `xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/TestMovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator/__main__.py` & `xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,43 +5,52 @@
 
 from xh_cpu_usage_simulator import TaskWorker
 from xh_cpu_usage_simulator.MovingAvg import MovingAvg
 from xh_cpu_usage_simulator.PsMonitor import PsMonitor
 
 if __name__ == '__main__':
     d = dict()
+    r = dict()
     for i in range(psutil.cpu_count(logical=False)):
-        d.update({f"{i}": 10})
-        bucket = MovingAvg(100)
-        Thread(target=TaskWorker.worker, args=[i, d, lambda: bucket.insert(1)]).start()
+        d.update({f"{i}": 10 })
+        r.update({f"{i}-complete": 0})
+        bucket = MovingAvg(10)
+        Thread(target=TaskWorker.worker, args=[i, d, r, lambda: bucket.insert(1)]).start()
 
     total_operation = sum([d[i] for i in d])
 
     m_avg = MovingAvg(10)
 
     target = 70
     rounds = 0
     for m in PsMonitor().monitor():
         if m_avg.cur_index == 0:
             if rounds == 0:
                 rounds += 1
             else:
                 rounds += 1
                 cur_total_operation = round(sum([d[i] for i in d]), 2)
+
+                cur_total_mv = 0
+                for i in d:
+                    mv = r[f"{i}-complete"]
+                    cur_total_mv += mv
+                    # print(f"[Worker {i}] rounds[{rounds}] moving average {mv}")
+
                 if target * 0.95 > m_avg.avg:
                     for i in d:
                         d[i] = d[i] * 1.8
                     new_total_operation = round(sum([d[i] for i in d]), 2)
                     print(
-                        f"{rounds:05d}::Targeting[{target}], now[{m_avg.avg}], increase operation from {cur_total_operation} to {new_total_operation}")
+                        f"{rounds:05d}::Targeting[{target}], now[{m_avg.avg}], increase operation with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
                 elif target * 1.05 < m_avg.avg:
                     for i in d:
                         d[i] = d[i] * 0.85
                     new_total_operation = sum([d[i] for i in d])
                     print(
-                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], decreate operation from {cur_total_operation} to {new_total_operation}")
+                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], decrease operation with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
                 else:
                     print(
-                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], nothing to do")
+                        f"{rounds:05d}Targeting[{target}], now[{m_avg.avg}], nothing to do with loading[{cur_total_mv}]")
         m_avg.insert(m.avg)
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `xh-cpu-usage-simulator-0.0.5/src/xh_cpu_usage_simulator.egg-info/PKG-INFO` & `xh-cpu-usage-simulator-0.0.6/src/xh_cpu_usage_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

