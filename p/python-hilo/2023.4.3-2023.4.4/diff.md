# Comparing `tmp/python_hilo-2023.4.3.tar.gz` & `tmp/python_hilo-2023.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_hilo-2023.4.3.tar", max compression
+gzip compressed data, was "python_hilo-2023.4.4.tar", max compression
```

## Comparing `python_hilo-2023.4.3.tar` & `python_hilo-2023.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.4.3/LICENSE
--rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.4.3/README.md
--rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.4.3/pyhilo/__init__.py
--rw-r--r--   0        0        0    28803 2023-04-07 15:37:20.467264 python_hilo-2023.4.3/pyhilo/api.py
--rw-r--r--   0        0        0     6950 2023-04-07 15:35:01.807968 python_hilo-2023.4.3/pyhilo/const.py
--rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.4.3/pyhilo/device/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.4.3/pyhilo/device/climate.py
--rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.4.3/pyhilo/device/light.py
--rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.4.3/pyhilo/device/sensor.py
--rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.4.3/pyhilo/device/switch.py
--rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.4.3/pyhilo/devices.py
--rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.4.3/pyhilo/event.py
--rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.4.3/pyhilo/exceptions.py
--rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.4.3/pyhilo/util/__init__.py
--rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.4.3/pyhilo/util/state.py
--rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.4.3/pyhilo/websocket.py
--rw-r--r--   0        0        0     3151 2023-04-12 22:18:20.675701 python_hilo-2023.4.3/pyproject.toml
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 python_hilo-2023.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-02-20 01:13:28.118104 python_hilo-2023.4.4/LICENSE
+-rw-r--r--   0        0        0     1124 2023-02-20 01:13:28.118273 python_hilo-2023.4.4/README.md
+-rw-r--r--   0        0        0      109 2022-03-03 03:33:56.401543 python_hilo-2023.4.4/pyhilo/__init__.py
+-rw-r--r--   0        0        0    28803 2023-04-07 15:37:20.467264 python_hilo-2023.4.4/pyhilo/api.py
+-rw-r--r--   0        0        0     6950 2023-04-07 15:35:01.807968 python_hilo-2023.4.4/pyhilo/const.py
+-rw-r--r--   0        0        0     9103 2022-03-03 03:33:56.402025 python_hilo-2023.4.4/pyhilo/device/__init__.py
+-rw-r--r--   0        0        0     1303 2023-04-07 15:45:29.694634 python_hilo-2023.4.4/pyhilo/device/climate.py
+-rw-r--r--   0        0        0      946 2023-04-07 15:43:25.840649 python_hilo-2023.4.4/pyhilo/device/light.py
+-rw-r--r--   0        0        0      462 2023-04-07 15:43:10.973680 python_hilo-2023.4.4/pyhilo/device/sensor.py
+-rw-r--r--   0        0        0      454 2023-04-07 15:42:51.429777 python_hilo-2023.4.4/pyhilo/device/switch.py
+-rw-r--r--   0        0        0     3836 2023-04-07 15:41:59.052538 python_hilo-2023.4.4/pyhilo/devices.py
+-rw-r--r--   0        0        0     4013 2022-03-03 03:33:56.402480 python_hilo-2023.4.4/pyhilo/event.py
+-rw-r--r--   0        0        0     1191 2022-03-03 03:33:56.402554 python_hilo-2023.4.4/pyhilo/exceptions.py
+-rw-r--r--   0        0        0     1257 2022-03-03 03:33:56.402675 python_hilo-2023.4.4/pyhilo/util/__init__.py
+-rw-r--r--   0        0        0     2988 2023-02-20 01:13:28.119721 python_hilo-2023.4.4/pyhilo/util/state.py
+-rw-r--r--   0        0        0    13020 2023-04-07 15:38:42.902984 python_hilo-2023.4.4/pyhilo/websocket.py
+-rw-r--r--   0        0        0     3151 2023-04-18 22:43:31.630304 python_hilo-2023.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 python_hilo-2023.4.4/PKG-INFO
```

### Comparing `python_hilo-2023.4.3/LICENSE` & `python_hilo-2023.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/README.md` & `python_hilo-2023.4.4/README.md`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/api.py` & `python_hilo-2023.4.4/pyhilo/api.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/const.py` & `python_hilo-2023.4.4/pyhilo/const.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/device/__init__.py` & `python_hilo-2023.4.4/pyhilo/device/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/device/climate.py` & `python_hilo-2023.4.4/pyhilo/device/climate.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/device/light.py` & `python_hilo-2023.4.4/pyhilo/device/light.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/devices.py` & `python_hilo-2023.4.4/pyhilo/devices.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/event.py` & `python_hilo-2023.4.4/pyhilo/event.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/exceptions.py` & `python_hilo-2023.4.4/pyhilo/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/util/__init__.py` & `python_hilo-2023.4.4/pyhilo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/util/state.py` & `python_hilo-2023.4.4/pyhilo/util/state.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyhilo/websocket.py` & `python_hilo-2023.4.4/pyhilo/websocket.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2023.4.3/pyproject.toml` & `python_hilo-2023.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 exclude = ".venv/.*"
 
 [tool.poetry]
 name = "python-hilo"
-version = "2023.04.03"
+version = "2023.04.04"
 description = "A Python3, async interface to the Hilo API"
 readme = "README.md"
 authors = ["David Vallee Delisle <me@dvd.dev>"]
 maintainers = ["David Vallee Delisle <me@dvd.dev>"]
 license = "MIT"
 repository = "https://github.com/dvd-dev/python-hilo"
 packages = [
@@ -68,15 +68,15 @@
 async-timeout = ">=4.0.0"
 attrs = ">=21.2.0"
 backoff = ">=1.11.1"
 python-dateutil = ">=2.8.2"
 ruyaml = ">=0.91.0"
 python = "^3.9.0"
 voluptuous = ">=0.13.1"
-websockets = ">=8.1,<11.0"
+websockets = ">=8.1,<12.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^6.1.3"
 aresponses = "^2.1.4"
 asynctest = "^0.13.0"
 pre-commit = "^3.2.2"
 pytest = "^7.2.0"
```

### Comparing `python_hilo-2023.4.3/PKG-INFO` & `python_hilo-2023.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hilo
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: A Python3, async interface to the Hilo API
 Home-page: https://github.com/dvd-dev/python-hilo
 License: MIT
 Author: David Vallee Delisle
 Author-email: me@dvd.dev
 Maintainer: David Vallee Delisle
 Maintainer-email: me@dvd.dev
@@ -26,15 +26,15 @@
 Requires-Dist: aiosignal (>=1.2.0)
 Requires-Dist: async-timeout (>=4.0.0)
 Requires-Dist: attrs (>=21.2.0)
 Requires-Dist: backoff (>=1.11.1)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: ruyaml (>=0.91.0)
 Requires-Dist: voluptuous (>=0.13.1)
-Requires-Dist: websockets (>=8.1,<11.0)
+Requires-Dist: websockets (>=8.1,<12.0)
 Project-URL: Repository, https://github.com/dvd-dev/python-hilo
 Description-Content-Type: text/markdown
 
 # python-hilo
 
 `python-hilo` (aka `pyhilo`) is a Python 3.9, `asyncio`-driven interface to the unofficial
 Hilo API from Hydro Quebec. This is meant to be integrated into Home Assistant.
```

