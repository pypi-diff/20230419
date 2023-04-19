# Comparing `tmp/pt-web-vnc-0.3.1.post2.tar.gz` & `tmp/pt-web-vnc-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pt-web-vnc-0.3.1.post2.tar", last modified: Thu Aug 18 16:05:07 2022, max compression
+gzip compressed data, was "dist/pt-web-vnc-0.4.0.post1.tar", last modified: Wed Apr 19 13:04:32 2023, max compression
```

## Comparing `pt-web-vnc-0.3.1.post2.tar` & `pt-web-vnc-0.4.0.post1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/connection_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/display_activity_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc/vnc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-08-18 16:05:06.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 16:05:06.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-18 16:05:06.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-18 16:05:06.000000 pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     9270 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/scripts/pt-web-vnc
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-08-18 16:05:07.000000 pt-web-vnc-0.3.1.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-08-18 16:04:55.000000 pt-web-vnc-0.3.1.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/connection_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/display_activity_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/screenshot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc/vnc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9270 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/scripts/pt-web-vnc
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-19 13:04:32.000000 pt-web-vnc-0.4.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 13:04:22.000000 pt-web-vnc-0.4.0.post1/setup.py
```

### Comparing `pt-web-vnc-0.3.1.post2/PKG-INFO` & `pt-web-vnc-0.4.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-web-vnc
-Version: 0.3.1.post2
+Version: 0.4.0.post1
 Summary: pi-top Web VNC Tool
 Home-page: https://github.com/pi-top/pt-web-vnc
 Author: pi-top (CEED Ltd)
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: pt-web-vnc
         ==========
```

### Comparing `pt-web-vnc-0.3.1.post2/README.rst` & `pt-web-vnc-0.4.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.3.1.post2/pt_web_vnc/connection_details.py` & `pt-web-vnc-0.4.0.post1/pt_web_vnc/connection_details.py`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.3.1.post2/pt_web_vnc/display_activity_monitor.py` & `pt-web-vnc-0.4.0.post1/pt_web_vnc/display_activity_monitor.py`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.3.1.post2/pt_web_vnc/utils.py` & `pt-web-vnc-0.4.0.post1/pt_web_vnc/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from os import environ
 from shlex import split
 from subprocess import run
 
 
-def run_command(command_str: str, timeout: int) -> str:
+def run_command(command_str: str, timeout: int, check: bool = False) -> str:
     def __get_env():
         env = environ.copy()
         # Print output of commands in english
         env["LANG"] = "en_US.UTF-8"
         return env
 
     try:
         resp = run(
             split(command_str),
-            check=False,
+            check=check,
             capture_output=True,
             timeout=timeout,
             env=__get_env(),
         )
         return str(resp.stdout, "utf8")
     except Exception:
         return ""
```

### Comparing `pt-web-vnc-0.3.1.post2/pt_web_vnc/vnc.py` & `pt-web-vnc-0.4.0.post1/pt_web_vnc/vnc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 from typing import Callable, Optional
 
 from .connection_details import VncConnectionDetails
 from .display_activity_monitor import start_activity_monitor, stop_activity_monitor
+from .screenshot_monitor import ScreenshotMonitor
 from .utils import run_command
 
 logger = logging.getLogger(__name__)
 
 
 class PtWebVncCommands:
     @staticmethod
@@ -101,33 +102,32 @@
     return VncConnectionDetails(url=url.strip())
 
 
 def clients(display_id: int) -> int:
     cmd = PtWebVncCommands.clients(display_id)
     logging.info(f"Getting pt-web-vnc clients on display {display_id}: {cmd}")
     try:
-        clients = int(run_command(cmd, timeout=10))
+        return int(run_command(cmd, timeout=10))
     except Exception:
-        clients = 0
-    finally:
-        return clients
+        return 0
 
 
 async def async_start(
     display_id: int,
     window_title: Optional[str] = None,
     ssl_certificate: Optional[str] = None,
     height: Optional[int] = None,
     width: Optional[int] = None,
     depth: Optional[int] = None,
     run: Optional[str] = None,
     background_colour: Optional[str] = None,
     with_window_manager: Optional[bool] = None,
     on_display_activity: Optional[Callable] = None,
-) -> None:
+    screenshot_timeout: int = 0,
+) -> Optional[ScreenshotMonitor]:
     cmd = PtWebVncCommands.start(
         display_id=display_id,
         window_title=window_title,
         ssl_certificate=ssl_certificate,
         height=height,
         width=width,
         depth=depth,
@@ -146,14 +146,19 @@
     )
     await proc.wait()
     if callable(on_display_activity):
         start_activity_monitor(
             display_id, on_display_activity, connection_details(display_id)
         )
 
+    screenshot_monitor = None
+    if screenshot_timeout > 0:
+        screenshot_monitor = ScreenshotMonitor(display_id, screenshot_timeout)
+    return screenshot_monitor
+
 
 async def async_stop(display_id: int) -> None:
     cmd = PtWebVncCommands.stop(display_id)
     logging.info(f"Stopping pt-web-vnc: {cmd}")
     await stop_activity_monitor(display_id)
     proc = await asyncio.create_subprocess_shell(
         cmd,
```

### Comparing `pt-web-vnc-0.3.1.post2/pt_web_vnc.egg-info/PKG-INFO` & `pt-web-vnc-0.4.0.post1/pt_web_vnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-web-vnc
-Version: 0.3.1.post2
+Version: 0.4.0.post1
 Summary: pi-top Web VNC Tool
 Home-page: https://github.com/pi-top/pt-web-vnc
 Author: pi-top (CEED Ltd)
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: pt-web-vnc
         ==========
```

### Comparing `pt-web-vnc-0.3.1.post2/scripts/pt-web-vnc` & `pt-web-vnc-0.4.0.post1/scripts/pt-web-vnc`

 * *Files identical despite different names*

### Comparing `pt-web-vnc-0.3.1.post2/setup.cfg` & `pt-web-vnc-0.4.0.post1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
+install_requires = 
+	Pillow >= 8.1.2
 include_package_data = True
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 per-file-ignores =
```

