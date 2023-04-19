# Comparing `tmp/idun_guardian_client-1.1.2.tar.gz` & `tmp/idun_guardian_client-1.1b15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1.2.tar", last modified: Fri Apr 14 12:02:51 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1b15.tar", last modified: Wed Apr 19 12:05:36 2023, max compression
```

## Comparing `idun_guardian_client-1.1.2.tar` & `idun_guardian_client-1.1b15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.053560 idun_guardian_client-1.1.2/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-14 12:02:51.053375 idun_guardian_client-1.1.2/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.2/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      864 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-14 12:02:51.053604 idun_guardian_client-1.1.2/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.047223 idun_guardian_client-1.1.2/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.051267 idun_guardian_client-1.1.2/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     8921 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    11765 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20723 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    31141 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.052429 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.053109 idun_guardian_client-1.1.2/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-19 12:05:36.883720 idun_guardian_client-1.1b15/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-04-19 12:05:36.883402 idun_guardian_client-1.1b15/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1b15/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      870 2023-04-19 12:01:59.000000 idun_guardian_client-1.1b15/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-19 12:05:36.883781 idun_guardian_client-1.1b15/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-19 12:05:36.876475 idun_guardian_client-1.1b15/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-19 12:05:36.880790 idun_guardian_client-1.1b15/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     8921 2023-04-19 11:56:20.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    11765 2023-04-19 11:56:20.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20723 2023-04-19 11:56:20.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    31214 2023-04-19 12:04:48.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-19 12:05:36.882109 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-04-19 12:05:36.000000 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-19 12:05:36.000000 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-19 12:05:36.000000 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-19 12:05:36.000000 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-19 12:05:36.000000 idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-19 12:05:36.882974 idun_guardian_client-1.1b15/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b15/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1.2/PKG-INFO` & `idun_guardian_client-1.1b15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun_guardian_client
-Version: 1.1.2
+Version: 1.1b15
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.2/README.md` & `idun_guardian_client-1.1b15/README.md`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/pyproject.toml` & `idun_guardian_client-1.1b15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idun_guardian_client"
-version = "1.1.2"
+version = "1.1.beta.15"
 authors = [
   { name="IDUN Technologies", email="contact@iduntechnologies.com" },
 ]
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/client.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/debug_logs.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_api.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,19 +122,21 @@
 
         Args:
             device_name (str): Device name
 
         Returns:
             str: MAC address
         """
-        async with BleakClient(self.address) as client:
+        async with BleakClient(self.address, use_cached_services=True) as client:
             logging_searching(self.debug)
             value = bytes(await client.read_gatt_char(self.mac_uuid))
             await asyncio.sleep(self.ble_delay)
-            firmware_version = bytes(await client.read_gatt_char(self.firmware_uuid))
+            firmware_version = bytes(
+                await client.read_gatt_char(self.firmware_uuid, use_cached=True)
+            )
             mac_address = value.decode("utf-8")
             firmware_decoded = firmware_version.decode("utf-8")
             mac_address = mac_address.replace(":", "-")
             logging_device_info(self.debug, mac_address, firmware_decoded)
             return mac_address
 
     async def search_device(self) -> str:
```

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/igeb_utils.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b15/src/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-guardian-client
-Version: 1.1.2
+Version: 1.1b15
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1b15/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/tests/test_ble.py` & `idun_guardian_client-1.1b15/tests/test_ble.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/tests/test_ble_record.py` & `idun_guardian_client-1.1b15/tests/test_ble_record.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.2/tests/test_utils.py` & `idun_guardian_client-1.1b15/tests/test_utils.py`

 * *Files identical despite different names*

