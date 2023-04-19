# Comparing `tmp/emmett_prometheus-0.1.1.tar.gz` & `tmp/emmett_prometheus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_prometheus-0.1.1.tar", max compression
+gzip compressed data, was "emmett_prometheus-0.1.2.tar", max compression
```

## Comparing `emmett_prometheus-0.1.1.tar` & `emmett_prometheus-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1486 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/LICENSE
--rw-r--r--   0        0        0     1831 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/README.md
--rw-r--r--   0        0        0       28 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/__init__.py
--rw-r--r--   0        0        0       22 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/__version__.py
--rw-r--r--   0        0        0     6067 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/ext.py
--rw-r--r--   0        0        0     1369 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1831 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/README.md
+-rw-r--r--   0        0        0       28 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/__version__.py
+-rw-r--r--   0        0        0     6067 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/ext.py
+-rw-r--r--   0        0        0     1369 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.2/PKG-INFO
```

### Comparing `emmett_prometheus-0.1.1/LICENSE` & `emmett_prometheus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.1/README.md` & `emmett_prometheus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.1/emmett_prometheus/ext.py` & `emmett_prometheus-0.1.2/emmett_prometheus/ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             )
             self._pipe_ws = PrometheusWSPipe(self)
 
         if self.config.auto_load:
             self.app.route(
                 self.config.metrics_route_path,
                 methods='get',
-                hostname=self.config.metrics_rotue_hostname,
+                hostname=self.config.metrics_route_hostname,
                 output='bytes'
             )(self._metrics_route)
 
     @listen_signal(Signals.before_route)
     def _inject_pipes(self, route, f):
         if not self.config.auto_load:
             return
```

### Comparing `emmett_prometheus-0.1.1/pyproject.toml` & `emmett_prometheus-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-prometheus"
-version = "0.1.1"
+version = "0.1.2"
 description = "Prometheus extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/prometheus"
 repository = "https://github.com/emmett-framework/prometheus"
```

### Comparing `emmett_prometheus-0.1.1/PKG-INFO` & `emmett_prometheus-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-prometheus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prometheus extension for Emmett framework
 Home-page: https://github.com/emmett-framework/prometheus
 License: BSD-3-Clause
 Keywords: prometheus,monitoring,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

