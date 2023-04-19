# Comparing `tmp/pushgateway_py_client-0.3.2.tar.gz` & `tmp/pushgateway_py_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushgateway_py_client-0.3.2.tar", max compression
+gzip compressed data, was "pushgateway_py_client-0.4.1.tar", max compression
```

## Comparing `pushgateway_py_client-0.3.2.tar` & `pushgateway_py_client-0.4.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1064 2023-04-19 09:20:16.374504 pushgateway_py_client-0.3.2/LICENSE
--rw-r--r--   0        0        0      456 2023-04-19 09:20:16.374504 pushgateway_py_client-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3722 2023-04-19 09:20:16.374504 pushgateway_py_client-0.3.2/src/pushgateway_py_client/__init__.py
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 pushgateway_py_client-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-19 12:43:41.604863 pushgateway_py_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0      456 2023-04-19 12:43:41.604863 pushgateway_py_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4593 2023-04-19 12:43:41.604863 pushgateway_py_client-0.4.1/src/pushgateway_py_client/__init__.py
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 pushgateway_py_client-0.4.1/PKG-INFO
```

### Comparing `pushgateway_py_client-0.3.2/LICENSE` & `pushgateway_py_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pushgateway_py_client-0.3.2/src/pushgateway_py_client/__init__.py` & `pushgateway_py_client-0.4.1/src/pushgateway_py_client/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
-from prometheus_client import CollectorRegistry, Gauge, Counter, push_to_gateway
+from prometheus_client import CollectorRegistry, Gauge, Counter, Histogram, push_to_gateway
 
 global_counter = {}
 global_gauges = {}
+global_histograms = {}
 
 
 class MetricsClient:
     def __init__(
         self,
         pushgateway_url: str,
         job_name: str,
@@ -14,14 +15,15 @@
     ):
         self._url = pushgateway_url
         self._job_name = job_name
         self._registry = CollectorRegistry()
         self._push_function = push_function
         self._gauges = (lambda: global_gauges)()
         self._counters = (lambda: global_counter)()
+        self._histograms = (lambda: global_histograms)()
 
     def __push(self):
         """
         Push all metrics to the pushgateway
         :return:
         """
         self._push_function(self._url, job=self._job_name, registry=self._registry)
@@ -30,29 +32,29 @@
         """
         Push a counter metric to the pushgateway
         :param labels:
         :param metric:
         :param value:
         :return:
         """
-        clabelnames = list(labels.keys())
+        counter_label_names = list(labels.keys())
 
         def __add_counter(metric_name: str, help_text: str):
             """
             Add a counter metric to the registry
             :param metric_name:
             :param help_text:
             :return:
             """
             if metric_name not in global_counter:
                 global_counter[metric_name] = Counter(
                     metric_name,
                     help_text,
                     registry=self._registry,
-                    labelnames=clabelnames,
+                    labelnames=counter_label_names,
                 )
 
         def __increment_counter(metric_name: str, value_: float = 1):
             """
             Increment a counter metric by a specific value
             :param metric_name:
             :param value_:
@@ -69,29 +71,29 @@
         Push a gauge metric to the pushgateway
         :param labels:
         :param metric:
         :param value:
         :return:
         """
 
-        glabelnames = list(labels.keys())
+        gauge_label_names = list(labels.keys())
 
         def __add_gauge(metric_name: str, help_text: str):
             """
             Add a gauge metric to the registry
             :param metric_name:
             :param help_text:
             :return:
             """
             if metric_name not in global_gauges:
                 global_gauges[metric_name] = Gauge(
                     metric_name,
                     help_text,
                     registry=self._registry,
-                    labelnames=glabelnames,
+                    labelnames=gauge_label_names,
                 )
 
         def __set_gauge(metric_name: str, metric_value: float):
             """
             Set a gauge metric to a specific value
             :param metric_name:
             :param metric_value:
@@ -99,14 +101,36 @@
             """
             global_gauges[metric_name].labels(**labels).set(metric_value)
 
         __add_gauge(metric, "Gauge metric")
         __set_gauge(metric, value)
         self.__push()
 
+    def histogram(self, metric: str, value: float, labels: dict = {}, buckets = None):
+        """
+        Push a histogram metric to the pushgateway
+        :param buckets:
+        :param labels:
+        :param metric:
+        :param value:
+        :return:
+        """
+
+        histogram_label_names = list(labels.keys())
+        if metric not in global_histograms:
+            global_histograms[metric] = Histogram(
+                metric,
+                "Histogram metric",
+                registry=self._registry,
+                labelnames=histogram_label_names,
+                buckets=Histogram.DEFAULT_BUCKETS if not buckets else buckets,
+            )
+        global_histograms[metric].labels(**labels).observe(value)
+        self.__push()
+
     def timeit(self, metric, labels):
         """
         Decorator to time a function and push the execution time to the pushgateway. (seconds)
         :param labels:
         :param metric:
         """
```

