# Comparing `tmp/Red-Lavalink-0.9.3.tar.gz` & `tmp/Red-Lavalink-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Red-Lavalink-0.9.3.tar", last modified: Tue May 31 23:26:36 2022, max compression
+gzip compressed data, was "Red-Lavalink-0.9.4.tar", last modified: Mon Aug 15 09:48:43 2022, max compression
```

## Comparing `Red-Lavalink-0.9.3.tar` & `Red-Lavalink-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 23:26:36.070110 Red-Lavalink-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    36629 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-05-31 23:26:36.070110 Red-Lavalink-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 23:26:36.066110 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-05-31 23:26:35.000000 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-05-31 23:26:36.000000 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 23:26:35.000000 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-31 23:26:35.000000 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-31 23:26:35.000000 Red-Lavalink-0.9.3/Red_Lavalink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 23:26:36.070110 Red-Lavalink-0.9.3/lavalink/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)    10120 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/lavalink.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    22014 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/node.py
--rw-r--r--   0 runner    (1001) docker     (121)    19725 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/player_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    13610 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/lavalink/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-31 23:26:36.070110 Red-Lavalink-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-05-31 23:26:20.000000 Red-Lavalink-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 09:48:43.557513 Red-Lavalink-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    36629 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-08-15 09:48:43.557513 Red-Lavalink-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 09:48:43.553512 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-08-15 09:48:43.000000 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-08-15 09:48:43.000000 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 09:48:43.000000 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-15 09:48:43.000000 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-15 09:48:43.000000 Red-Lavalink-0.9.4/Red_Lavalink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 09:48:43.557513 Red-Lavalink-0.9.4/lavalink/
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10120 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/lavalink.py
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22045 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19725 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/player_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13610 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/lavalink/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-08-15 09:48:43.557513 Red-Lavalink-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-08-15 09:48:23.000000 Red-Lavalink-0.9.4/setup.py
```

### Comparing `Red-Lavalink-0.9.3/LICENSE` & `Red-Lavalink-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/PKG-INFO` & `Red-Lavalink-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Lavalink
-Version: 0.9.3
+Version: 0.9.4
 Summary: Lavalink client library for Red-DiscordBot
 Home-page: https://github.com/Cog-Creators/Red-Lavalink
 Author: tekulvw
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `Red-Lavalink-0.9.3/README.rst` & `Red-Lavalink-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/Red_Lavalink.egg-info/PKG-INFO` & `Red-Lavalink-0.9.4/Red_Lavalink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Lavalink
-Version: 0.9.3
+Version: 0.9.4
 Summary: Lavalink client library for Red-DiscordBot
 Home-page: https://github.com/Cog-Creators/Red-Lavalink
 Author: tekulvw
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `Red-Lavalink-0.9.3/lavalink/__init__.py` & `Red-Lavalink-0.9.4/lavalink/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .log import set_logging_level, log, socket_log, ws_discord_log, ws_ll_log, ws_rll_log
 
 set_logging_level()
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 from .lavalink import *
 from .node import Node, NodeStats, Stats
 from .player_manager import *
 from .enums import NodeState, PlayerState, TrackEndReason, LavalinkEvents
 from .rest_api import Track
 from . import utils
```

### Comparing `Red-Lavalink-0.9.3/lavalink/enums.py` & `Red-Lavalink-0.9.4/lavalink/enums.py`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/lavalink/lavalink.py` & `Red-Lavalink-0.9.4/lavalink/lavalink.py`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/lavalink/node.py` & `Red-Lavalink-0.9.4/lavalink/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,17 +237,18 @@
 
         ws_ll_log.debug("Creating Lavalink WS listener.")
         if self._listener_task is not None:
             self._listener_task.cancel()
         self._listener_task = self.loop.create_task(self.listener())
         self.loop.create_task(self._configure_resume())
         if self._queue:
-            for data in self._queue:
-                await self.send(data)
+            temp = self._queue.copy()
             self._queue.clear()
+            for data in temp:
+                await self.send(data)
         self._ready_event.set()
         self.update_state(NodeState.READY)
 
     async def _configure_resume(self):
         if self._resuming_configured:
             return
         if self._resume_key and self._resume_timeout and self._resume_timeout > 0:
```

### Comparing `Red-Lavalink-0.9.3/lavalink/player_manager.py` & `Red-Lavalink-0.9.4/lavalink/player_manager.py`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/lavalink/rest_api.py` & `Red-Lavalink-0.9.4/lavalink/rest_api.py`

 * *Files identical despite different names*

### Comparing `Red-Lavalink-0.9.3/setup.cfg` & `Red-Lavalink-0.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 install_requires = 
 	discord.py>=1.5.1
 	aiohttp>=3.6.0
 
 [options.extras_require]
 tests = 
 	pytest>3.0.6
-	pytest-asyncio
+	pytest-asyncio<0.19
 	async_generator
 docs = 
 	sphinx
 	sphinxcontrib-asyncio
 	sphinx_rtd_theme
 
 [egg_info]
```

