# Comparing `tmp/nitrado-1.0.4.tar.gz` & `tmp/nitrado-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.4.tar", last modified: Wed Apr 19 12:12:27 2023, max compression
+gzip compressed data, was "nitrado-1.0.5.tar", last modified: Wed Apr 19 12:13:17 2023, max compression
```

## Comparing `nitrado-1.0.4.tar` & `nitrado-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.881235 nitrado-1.0.4/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:12:27.881235 nitrado-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.4/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1135 2023-04-19 12:12:27.886233 nitrado-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.803010 nitrado-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.811607 nitrado-1.0.4/src/nitrado/
--rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.4/src/nitrado/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.827234 nitrado-1.0.4/src/nitrado/games/
--rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.4/src/nitrado/games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.830230 nitrado-1.0.4/src/nitrado/games/ark/
--rw-rw-rw-   0        0        0       62 2023-04-19 03:43:26.000000 nitrado-1.0.4/src/nitrado/games/ark/__init__.py
--rw-rw-rw-   0        0        0     3841 2023-04-19 03:43:26.000000 nitrado-1.0.4/src/nitrado/games/ark/ark_survival.py
--rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.4/src/nitrado/games/ark/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.850231 nitrado-1.0.4/src/nitrado/lib/
--rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.4/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.4/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.4/src/nitrado/lib/game_server.py
--rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.4/src/nitrado/lib/service.py
--rw-rw-rw-   0        0        0     3165 2023-04-19 03:43:26.000000 nitrado-1.0.4/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.4/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.857232 nitrado-1.0.4/src/nitrado/tools/
--rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.4/src/nitrado/tools/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.4/src/nitrado/tools/client.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.827234 nitrado-1.0.4/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3435 2023-04-19 12:12:27.000000 nitrado-1.0.4/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-04-19 12:12:27.000000 nitrado-1.0.4/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:12:27.000000 nitrado-1.0.4/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-19 12:12:27.000000 nitrado-1.0.4/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 12:12:27.000000 nitrado-1.0.4/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:12:27.880229 nitrado-1.0.4/tests/
--rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.4/tests/test_connection.py
--rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.4/tests/test_game_server.py
--rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.4/tests/test_nitrado_api.py
--rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.4/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.261778 nitrado-1.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3435 2023-04-19 12:13:17.261778 nitrado-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.5/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1135 2023-04-19 12:13:17.263776 nitrado-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.231777 nitrado-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.238774 nitrado-1.0.5/src/nitrado/
+-rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.5/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.250779 nitrado-1.0.5/src/nitrado/games/
+-rw-rw-rw-   0        0        0        0 2023-04-16 22:12:29.000000 nitrado-1.0.5/src/nitrado/games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.252773 nitrado-1.0.5/src/nitrado/games/ark/
+-rw-rw-rw-   0        0        0       62 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/games/ark/__init__.py
+-rw-rw-rw-   0        0        0     3841 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/games/ark/ark_survival.py
+-rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.5/src/nitrado/games/ark/logs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.255776 nitrado-1.0.5/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.5/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.5/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0    22391 2023-04-17 02:38:37.000000 nitrado-1.0.5/src/nitrado/lib/game_server.py
+-rw-rw-rw-   0        0        0     3889 2023-04-17 00:46:43.000000 nitrado-1.0.5/src/nitrado/lib/service.py
+-rw-rw-rw-   0        0        0     3165 2023-04-19 03:43:26.000000 nitrado-1.0.5/src/nitrado/nitrado_api.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.5/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.257775 nitrado-1.0.5/src/nitrado/tools/
+-rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.5/src/nitrado/tools/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.5/src/nitrado/tools/client.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.249777 nitrado-1.0.5/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3435 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 12:13:17.000000 nitrado-1.0.5/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:13:17.260775 nitrado-1.0.5/tests/
+-rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.5/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.5/tests/test_game_server.py
+-rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.5/tests/test_nitrado_api.py
+-rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.5/tests/test_service.py
```

### Comparing `nitrado-1.0.4/LICENSE` & `nitrado-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/PKG-INFO` & `nitrado-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.4
+Version: 1.0.5
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.4/README.md` & `nitrado-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/pyproject.toml` & `nitrado-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/setup.cfg` & `nitrado-1.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 340d 0a74 6573  ion = 1.0.4..tes
+00000020: 696f 6e20 3d20 312e 302e 350d 0a74 6573  ion = 1.0.5..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 350d 0a70 726f 6475 6374 696f 6e5f 7665  5..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 340d 0a61  rsion = 1.0.4..a
+00000040: 360d 0a70 726f 6475 6374 696f 6e5f 7665  6..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 350d 0a61  rsion = 1.0.5..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
```

### Comparing `nitrado-1.0.4/src/nitrado/games/ark/ark_survival.py` & `nitrado-1.0.5/src/nitrado/games/ark/ark_survival.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado/lib/errors.py` & `nitrado-1.0.5/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado/lib/game_server.py` & `nitrado-1.0.5/src/nitrado/lib/game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado/lib/service.py` & `nitrado-1.0.5/src/nitrado/lib/service.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado/nitrado_api.py` & `nitrado-1.0.5/src/nitrado/nitrado_api.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado/tools/client.py` & `nitrado-1.0.5/src/nitrado/tools/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.5/src/nitrado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.4
+Version: 1.0.5
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
```

### Comparing `nitrado-1.0.4/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.5/src/nitrado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/tests/test_connection.py` & `nitrado-1.0.5/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/tests/test_game_server.py` & `nitrado-1.0.5/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.4/tests/test_service.py` & `nitrado-1.0.5/tests/test_service.py`

 * *Files identical despite different names*

