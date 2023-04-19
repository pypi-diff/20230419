# Comparing `tmp/aioshelly-5.3.1.tar.gz` & `tmp/aioshelly-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioshelly-5.3.1.tar", last modified: Thu Jan 26 20:51:07 2023, max compression
+gzip compressed data, was "aioshelly-5.3.2.tar", last modified: Wed Apr 19 12:17:23 2023, max compression
```

## Comparing `aioshelly-5.3.1.tar` & `aioshelly-5.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-26 20:50:54.000000 aioshelly-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-26 20:50:54.000000 aioshelly-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-01-26 20:51:07.884477 aioshelly-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-01-26 20:50:54.000000 aioshelly-5.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/aioshelly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/aioshelly/ble/
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/ble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/ble/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/aioshelly/block_device/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/block_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/block_device/coap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/block_device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/aioshelly/rpc_device/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/rpc_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/rpc_device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/rpc_device/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-01-26 20:50:54.000000 aioshelly-5.3.1/aioshelly/rpc_device/wsrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:51:07.884477 aioshelly-5.3.1/aioshelly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:51:07.000000 aioshelly-5.3.1/aioshelly.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-26 20:50:54.000000 aioshelly-5.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-26 20:51:07.884477 aioshelly-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-01-26 20:50:54.000000 aioshelly-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-19 12:17:06.000000 aioshelly-5.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 12:17:06.000000 aioshelly-5.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-19 12:17:23.101659 aioshelly-5.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-19 12:17:06.000000 aioshelly-5.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/ble/
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/ble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/ble/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/block_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/coap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/block_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly/rpc_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-04-19 12:17:06.000000 aioshelly-5.3.2/aioshelly/rpc_device/wsrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:17:23.101659 aioshelly-5.3.2/aioshelly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:17:23.000000 aioshelly-5.3.2/aioshelly.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 12:17:06.000000 aioshelly-5.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 12:17:23.105659 aioshelly-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-19 12:17:06.000000 aioshelly-5.3.2/setup.py
```

### Comparing `aioshelly-5.3.1/LICENSE` & `aioshelly-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/PKG-INFO` & `aioshelly-5.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 5.3.1
+Version: 5.3.2
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioshelly-5.3.1/README.md` & `aioshelly-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/ble/__init__.py` & `aioshelly-5.3.2/aioshelly/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/ble/const.py` & `aioshelly-5.3.2/aioshelly/ble/const.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/block_device/coap.py` & `aioshelly-5.3.2/aioshelly/block_device/coap.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/block_device/device.py` & `aioshelly-5.3.2/aioshelly/block_device/device.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/common.py` & `aioshelly-5.3.2/aioshelly/common.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/const.py` & `aioshelly-5.3.2/aioshelly/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     "SNSN-0D24X": "Shelly Plus I4DC",
     "SNSW-001P15UL": "Shelly Plus 1PM UL",
     "SNSW-001P16EU": "Shelly Plus 1PM",
     "SNSW-001X15UL": "Shelly Plus 1 UL",
     "SNSW-001X16EU": "Shelly Plus 1",
     "SNSW-0024X": "Shelly Plus I4",
     "SNSW-002P16EU": "Shelly Plus 2PM",
+    "SNSW-102P16EU": "Shelly Plus 2PM",
     "SPEM-003CEBEU": "Shelly Pro 3EM",
     "SPSW-001PE16EU": "Shelly Pro 1PM",
     "SPSW-001XE16EU": "Shelly Pro 1",
     "SPSW-002PE16EU": "Shelly Pro 2PM",
     "SPSW-002XE16EU": "Shelly Pro 2",
     "SPSW-003XE16EU": "Shelly Pro 3",
     "SPSW-004PE16EU": "Shelly Pro 4PM",
```

### Comparing `aioshelly-5.3.1/aioshelly/exceptions.py` & `aioshelly-5.3.2/aioshelly/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/json.py` & `aioshelly-5.3.2/aioshelly/json.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/rpc_device/device.py` & `aioshelly-5.3.2/aioshelly/rpc_device/device.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/rpc_device/models.py` & `aioshelly-5.3.2/aioshelly/rpc_device/models.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly/rpc_device/wsrpc.py` & `aioshelly-5.3.2/aioshelly/rpc_device/wsrpc.py`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/aioshelly.egg-info/PKG-INFO` & `aioshelly-5.3.2/aioshelly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 5.3.1
+Version: 5.3.2
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioshelly-5.3.1/aioshelly.egg-info/SOURCES.txt` & `aioshelly-5.3.2/aioshelly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioshelly-5.3.1/setup.py` & `aioshelly-5.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for aioshelly."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "5.3.1"
+VERSION = "5.3.2"
 
 
 setup(
     name="aioshelly",
     version=VERSION,
     license="Apache License 2.0",
     url="https://github.com/home-assistant-libs/aioshelly",
```

