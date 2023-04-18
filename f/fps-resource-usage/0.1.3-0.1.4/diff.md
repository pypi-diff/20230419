# Comparing `tmp/fps_resource_usage-0.1.3.tar.gz` & `tmp/fps_resource_usage-0.1.4.tar.gz`

## Comparing `fps_resource_usage-0.1.3.tar` & `fps_resource_usage-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fps_resource_usage-0.1.4/PKG-INFO
```

### Comparing `fps_resource_usage-0.1.3/fps_resource_usage/main.py` & `fps_resource_usage-0.1.4/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `fps_resource_usage-0.1.3/fps_resource_usage/routes.py` & `fps_resource_usage-0.1.4/fps_resource_usage/routes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 import psutil
 from anyio import to_thread
-from fastapi import APIRouter, Depends
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.resource_usage import ResourceUsage, ResourceUsageConfig
 
 
 class _ResourceUsage(ResourceUsage):
     def __init__(
         self,
         app: App,
         auth: Auth,
         resource_usage_config: ResourceUsageConfig,
     ):
-        super().__init__(app)
+        super().__init__(app, auth)
+        self.resource_usage_config = resource_usage_config
 
-        router = APIRouter()
+    async def get_metrics(
+        self,
+        user: User,
+    ):
+        cur_process = psutil.Process()
+        all_processes = [cur_process] + cur_process.children(recursive=True)
 
-        @router.get("/api/metrics/v1")
-        async def get_metrics(
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
+        # Get memory information
+        rss = 0
+        for p in all_processes:
+            try:
+                rss += p.memory_info().rss
+            except (psutil.NoSuchProcess, psutil.AccessDenied):
+                pass
+
+        mem_limit = self.resource_usage_config.mem_limit
+
+        limits = {"memory": {"rss": mem_limit}}
+        if (
+            self.resource_usage_config.mem_limit
+            and self.resource_usage_config.mem_warning_threshold
         ):
-            cur_process = psutil.Process()
-            all_processes = [cur_process] + cur_process.children(recursive=True)
-
-            # Get memory information
-            rss = 0
-            for p in all_processes:
-                try:
-                    rss += p.memory_info().rss
-                except (psutil.NoSuchProcess, psutil.AccessDenied):
-                    pass
-
-            mem_limit = resource_usage_config.mem_limit
-
-            limits = {"memory": {"rss": mem_limit}}
-            if resource_usage_config.mem_limit and resource_usage_config.mem_warning_threshold:
-                limits["memory"]["warn"] = (mem_limit - rss) < (
-                    mem_limit * resource_usage_config.mem_warning_threshold
-                )
-
-            metrics = {"rss": rss, "limits": limits}
-
-            # Optionally get CPU information
-            if resource_usage_config.track_cpu_percent:
-                cpu_count = psutil.cpu_count()
-                cpu_percent = await to_thread.run_sync(_get_cpu_percent, all_processes)
-
-                if resource_usage_config.cpu_limit:
-                    limits["cpu"] = {"cpu": resource_usage_config.cpu_limit}
-                    if resource_usage_config.cpu_warning_threshold:
-                        limits["cpu"]["warn"] = (resource_usage_config.cpu_limit - cpu_percent) < (
-                            resource_usage_config.cpu_limit
-                            * resource_usage_config.cpu_warning_threshold
-                        )
-
-                metrics.update(cpu_percent=cpu_percent, cpu_count=cpu_count)
+            limits["memory"]["warn"] = (mem_limit - rss) < (
+                mem_limit * self.resource_usage_config.mem_warning_threshold
+            )
+
+        metrics = {"rss": rss, "limits": limits}
+
+        # Optionally get CPU information
+        if self.resource_usage_config.track_cpu_percent:
+            cpu_count = psutil.cpu_count()
+            cpu_percent = await to_thread.run_sync(_get_cpu_percent, all_processes)
+
+            if self.resource_usage_config.cpu_limit:
+                limits["cpu"] = {"cpu": self.resource_usage_config.cpu_limit}
+                if self.resource_usage_config.cpu_warning_threshold:
+                    limits["cpu"]["warn"] = (self.resource_usage_config.cpu_limit - cpu_percent) < (
+                        self.resource_usage_config.cpu_limit
+                        * self.resource_usage_config.cpu_warning_threshold
+                    )
 
-            return metrics
+            metrics.update(cpu_percent=cpu_percent, cpu_count=cpu_count)
 
-        self.include_router(router)
+        return metrics
 
 
 def _get_cpu_percent(all_processes):
     def get_cpu_percent(p):
         try:
             return p.cpu_percent(interval=0.05)
         # Avoid littering logs with stack traces complaining
```

### Comparing `fps_resource_usage-0.1.3/.gitignore` & `fps_resource_usage-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_resource_usage-0.1.3/COPYING.md` & `fps_resource_usage-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_resource_usage-0.1.3/pyproject.toml` & `fps_resource_usage-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_resource_usage-0.1.3/PKG-INFO` & `fps_resource_usage-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_resource_usage
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the resource usage API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

