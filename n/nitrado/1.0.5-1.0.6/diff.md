# Comparing `tmp/nitrado-1.0.5.tar.gz` & `tmp/nitrado-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.5.tar", last modified: Wed Apr 19 12:13:17 2023, max compression
+gzip compressed data, was "nitrado-1.0.6.tar", last modified: Wed Apr 19 12:38:59 2023, max compression
```

## Comparing `nitrado-1.0.5.tar` & `nitrado-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.261778 nitrado-1.0.5/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:13:17.261778 nitrado-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.5/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1135 2023-04-19 12:13:17.263776 nitrado-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.231777 nitrado-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.238774 nitrado-1.0.5/src/nitrado/
--rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.5/src/nitrado/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.250779 nitrado-1.0.5/src/nitrado/games/
--rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.5/src/nitrado/games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.252773 nitrado-1.0.5/src/nitrado/games/ark/
--rw-rw-rw-   0        0        0       62 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/games/ark/__init__.py
--rw-rw-rw-   0        0        0     3841 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/games/ark/ark_survival.py
--rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.5/src/nitrado/games/ark/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.255776 nitrado-1.0.5/src/nitrado/lib/
--rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.5/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.5/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.5/src/nitrado/lib/game_server.py
--rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.5/src/nitrado/lib/service.py
--rw-rw-rw-   0        0        0     3165 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.5/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.257775 nitrado-1.0.5/src/nitrado/tools/
--rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.5/src/nitrado/tools/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.5/src/nitrado/tools/client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.249777 nitrado-1.0.5/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.260775 nitrado-1.0.5/tests/
--rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.5/tests/test_connection.py
--rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.5/tests/test_game_server.py
--rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.5/tests/test_nitrado_api.py
--rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.5/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.382990 nitrado-1.0.6/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3435 2023-04-19 12:38:59.382990 nitrado-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.6/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1135 2023-04-19 12:38:59.384990 nitrado-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.348462 nitrado-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.356711 nitrado-1.0.6/src/nitrado/
+-rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.6/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.370735 nitrado-1.0.6/src/nitrado/games/
+-rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.6/src/nitrado/games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.372893 nitrado-1.0.6/src/nitrado/games/ark/
+-rw-rw-rw-   0        0        0       62 2023-04-19 03:43:26.000000 nitrado-1.0.6/src/nitrado/games/ark/__init__.py
+-rw-rw-rw-   0        0        0     3732 2023-04-19 12:32:51.000000 nitrado-1.0.6/src/nitrado/games/ark/ark_survival.py
+-rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.6/src/nitrado/games/ark/logs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.376894 nitrado-1.0.6/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.6/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.6/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.6/src/nitrado/lib/game_server.py
+-rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.6/src/nitrado/lib/service.py
+-rw-rw-rw-   0        0        0     3165 2023-04-19 03:43:26.000000 nitrado-1.0.6/src/nitrado/nitrado_api.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.6/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.378894 nitrado-1.0.6/src/nitrado/tools/
+-rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.6/src/nitrado/tools/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.6/src/nitrado/tools/client.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.369737 nitrado-1.0.6/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3435 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 12:38:59.000000 nitrado-1.0.6/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:38:59.381988 nitrado-1.0.6/tests/
+-rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.6/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.6/tests/test_game_server.py
+-rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.6/tests/test_nitrado_api.py
+-rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.6/tests/test_service.py
```

### Comparing `nitrado-1.0.5/LICENSE` & `nitrado-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/PKG-INFO` & `nitrado-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.5
+Version: 1.0.6
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.5/README.md` & `nitrado-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/pyproject.toml` & `nitrado-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/setup.cfg` & `nitrado-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 350d 0a74 6573  ion = 1.0.5..tes
+00000020: 696f 6e20 3d20 312e 302e 360d 0a74 6573  ion = 1.0.6..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
 00000040: 360d 0a70 726f 6475 6374 696f 6e5f 7665  6..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 350d 0a61  rsion = 1.0.5..a
+00000050: 7273 696f 6e20 3d20 312e 302e 360d 0a61  rsion = 1.0.6..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
```

### Comparing `nitrado-1.0.5/src/nitrado/games/ark/ark_survival.py` & `nitrado-1.0.6/src/nitrado/games/ark/ark_survival.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nitrado.lib.game_server import GameServer
 from nitrado.lib.service import Service
 
 
 class ArkSurvivalServer:
     def __init__(self, gameserver: GameServer):
         self.__service = None
-        self.__gameserver = gameserver
+        self.gameserver = gameserver
 
         self.status = gameserver.status
         self.game_name = gameserver.game_human
         self.settings = gameserver.settings
         self.query = gameserver.query
         self.service_id = gameserver.service_id
         self.memory = gameserver.memory  # in MB
@@ -22,77 +22,74 @@
     def player_max(self) -> int:
         return self.query['player_max']
 
     def player_current(self) -> int:
         return self.query['player_current']
 
     def players(self) -> list:
-        return self.query['players']
+        return self.gameserver.players()
 
     def server_name(self) -> str:
         return self.config()['server-name']
 
     def service(self) -> Service:
         if self.__service is None:
-            self.__service = self.__gameserver.service()
+            self.__service = self.gameserver.service()
         return self.__service
 
-    def gameserver(self) -> GameServer:
-        return self.__gameserver
-
     def log_shooter_game(self) -> str:
         """ Refreshes about every 15+/- minutes """
-        return self.__gameserver.logs_shooter_game()
+        return self.gameserver.logs_shooter_game()
 
     def log_shooter_game_last(self) -> str:
         """ Refreshes about every 15+/- minutes """
-        return self.__gameserver.logs_shooter_game_last()
+        return self.gameserver.logs_shooter_game_last()
 
     def log_restart(self) -> str:
         """ Refreshes about every 15+/- minutes """
-        return self.__gameserver.logs_restart()
+        return self.gameserver.logs_restart()
 
     def config(self) -> dict:
-        return self.__gameserver.settings['config']
+        return self.gameserver.settings['config']
 
     def ini(self) -> dict:
-        return self.__gameserver.settings['gameini']
+        return self.gameserver.settings['gameini']
 
     def general_settings(self) -> dict:
-        return self.__gameserver.settings['general']
+        return self.gameserver.settings['general']
 
     def start_param(self) -> dict:
-        return self.__gameserver.settings['start-param']
+        return self.gameserver.settings['start-param']
 
     def cluster_id(self) -> str:
-        return self.__gameserver.cluster_id()
+        return self.gameserver.cluster_id()
 
     def start_server(self) -> bool:
-        return self.__gameserver.start('arkxb')
+        return self.gameserver.start('arkxb')
 
     def restart_server(self, restart_message: str = None, log_message: str = None) -> bool:
-        return self.__gameserver.restart(restart_message=restart_message, log_message=log_message)
+        return self.gameserver.restart(restart_message=restart_message, log_message=log_message)
 
     def reinstall_server(self) -> bool:
-        return self.__gameserver.install_game('arkxb', modpack=None)
+        return self.gameserver.install_game('arkxb', modpack=None)
 
     def stop_server(self, message: str = None, stop_message: str = None) -> bool:
-        return self.__gameserver.stop(message=message, stop_message=stop_message)
+        return self.gameserver.stop(message=message, stop_message=stop_message)
 
     def uninstall_game(self) -> bool:
-        return self.__gameserver.uninstall_game('arkxb')
+        return self.gameserver.uninstall_game('arkxb')
 
     def white_list_player(self, gamertag: str) -> bool:
-        return self.__gameserver.white_list_player(gamertag)
+        return self.gameserver.white_list_player(gamertag)
 
     def admin_list(self) -> list:
-        return self.__gameserver.admin_list()
+        return self.gameserver.admin_list()
 
     def backups_list(self) -> dict:
-        return self.__gameserver.backups_list()
+        return self.gameserver.backups_list()
 
     def admin_password(self) -> str:
         return self.config()['admin-password']
 
     def server_password(self) -> str:
         return self.config()['server-password']
```

### Comparing `nitrado-1.0.5/src/nitrado/lib/errors.py` & `nitrado-1.0.6/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/src/nitrado/lib/game_server.py` & `nitrado-1.0.6/src/nitrado/lib/game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/src/nitrado/lib/service.py` & `nitrado-1.0.6/src/nitrado/lib/service.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/src/nitrado/nitrado_api.py` & `nitrado-1.0.6/src/nitrado/nitrado_api.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/src/nitrado/tools/client.py` & `nitrado-1.0.6/src/nitrado/tools/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.6/src/nitrado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.5
+Version: 1.0.6
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.5/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.6/src/nitrado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/tests/test_connection.py` & `nitrado-1.0.6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/tests/test_game_server.py` & `nitrado-1.0.6/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.5/tests/test_service.py` & `nitrado-1.0.6/tests/test_service.py`

 * *Files identical despite different names*

