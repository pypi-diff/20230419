# Comparing `tmp/emmett_prometheus-0.1.0.tar.gz` & `tmp/emmett_prometheus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_prometheus-0.1.0.tar", max compression
+gzip compressed data, was "emmett_prometheus-0.1.1.tar", max compression
```

## Comparing `emmett_prometheus-0.1.0.tar` & `emmett_prometheus-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1486 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/LICENSE
--rw-r--r--   0        0        0     1831 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/README.md
--rw-r--r--   0        0        0       28 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/emmett_prometheus/__init__.py
--rw-r--r--   0        0        0       22 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/emmett_prometheus/__version__.py
--rw-r--r--   0        0        0     5997 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/emmett_prometheus/ext.py
--rw-r--r--   0        0        0     1369 2023-04-19 13:48:28.344249 emmett_prometheus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1831 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/README.md
+-rw-r--r--   0        0        0       28 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/__version__.py
+-rw-r--r--   0        0        0     6067 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/emmett_prometheus/ext.py
+-rw-r--r--   0        0        0     1369 2023-04-19 14:11:38.798211 emmett_prometheus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.1/PKG-INFO
```

### Comparing `emmett_prometheus-0.1.0/LICENSE` & `emmett_prometheus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.0/README.md` & `emmett_prometheus-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.0/emmett_prometheus/ext.py` & `emmett_prometheus-0.1.1/emmett_prometheus/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     def _inject_pipes(self, route, f):
         if not self.config.auto_load:
             return
         if route.name in self._excluded_routes:
             return
         if f == self._metrics_route:
             return
-        if isinstance(route, HTTPRoutingRule):
+        if self.config.enable_http_metrics and isinstance(route, HTTPRoutingRule):
             route.pipeline.insert(0, self._pipe_http)
-        if isinstance(route, WebsocketRoutingRule):
+        if self.config.enable_ws_metrics and isinstance(route, WebsocketRoutingRule):
             route.pipeline.insert(0, self._pipe_ws)
 
     async def _metrics_route(self):
         response.content_type = prometheus_client.exposition.CONTENT_TYPE_LATEST
         return prometheus_client.exposition.generate_latest(prometheus_client.REGISTRY)
```

### Comparing `emmett_prometheus-0.1.0/pyproject.toml` & `emmett_prometheus-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-prometheus"
-version = "0.1.0"
+version = "0.1.1"
 description = "Prometheus extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/prometheus"
 repository = "https://github.com/emmett-framework/prometheus"
```

### Comparing `emmett_prometheus-0.1.0/PKG-INFO` & `emmett_prometheus-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-prometheus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prometheus extension for Emmett framework
 Home-page: https://github.com/emmett-framework/prometheus
 License: BSD-3-Clause
 Keywords: prometheus,monitoring,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

