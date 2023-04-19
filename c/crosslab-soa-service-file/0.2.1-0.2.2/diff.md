# Comparing `tmp/crosslab_soa_service_file-0.2.1.tar.gz` & `tmp/crosslab_soa_service_file-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_file-0.2.1.tar", last modified: Tue Feb 21 23:54:05 2023, max compression
+gzip compressed data, was "crosslab_soa_service_file-0.2.2.tar", last modified: Wed Apr 19 18:34:17 2023, max compression
```

## Comparing `crosslab_soa_service_file-0.2.1.tar` & `crosslab_soa_service_file-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-21 16:30:40.000000 crosslab_soa_service_file-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      574 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-21 16:30:40.000000 crosslab_soa_service_file-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/
--rw-r--r--   0 dev       (1000) docker-host   (967)      192 2023-02-21 20:21:47.000000 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2409 2023-02-21 21:06:02.000000 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/file_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      222 2023-02-21 20:31:11.000000 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-21 16:30:40.000000 crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/py.typed
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:05.501837 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-02-21 23:54:05.000000 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      470 2023-02-21 23:54:05.000000 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:54:05.000000 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-02-21 23:54:05.000000 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:54:05.000000 crosslab_soa_service_file-0.2.1/src/crosslab_soa_service_file.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      574 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.231056 crosslab_soa_service_file-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      192 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2541 2023-04-19 13:37:16.000000 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/file_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      222 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/py.typed
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      344 2023-04-19 18:34:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      493 2023-04-19 18:34:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:34:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:34:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:34:17.000000 crosslab_soa_service_file-0.2.2/src/crosslab_soa_service_file.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:34:17.234390 crosslab_soa_service_file-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      898 2023-04-19 13:37:16.000000 crosslab_soa_service_file-0.2.2/tests/test_standard.py
```

### Comparing `crosslab_soa_service_file-0.2.1/setup.cfg` & `crosslab_soa_service_file-0.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_file
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA file Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_file-0.2.1/src/crosslab/soa_services/file/file_service.py` & `crosslab_soa_service_file-0.2.2/src/crosslab/soa_services/file/file_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Union
 
 from crosslab.soa_client.connection import Connection, DataChannel
 from crosslab.soa_client.service import Service
-from pyee import AsyncIOEventEmitter
+from pyee.asyncio import AsyncIOEventEmitter
 
 from crosslab.soa_services.file.messages import FileServiceConfig, FileServiceEvent
 
 
 class FileService__Producer(Service):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
     service_direction = "out"
@@ -26,14 +26,17 @@
     def setupConnection(self, connection: Connection, serviceConfig: FileServiceConfig):
         self.channel = DataChannel()
         if connection.tiebreaker:
             connection.transmit(serviceConfig, "data", self.channel)
         else:
             connection.receive(serviceConfig, "data", self.channel)
 
+    def teardownConnection(self, connection: Connection):
+        pass
+
     async def sendFile(self, file_type: str, content: bytes):
         self.channel.send(json.dumps({"fileType": file_type, "length": len(content)}))
         self.channel.send(content)
 
 
 class FileService__Consumer(Service, AsyncIOEventEmitter):
     service_type = "https://api.goldi-labs.de/serviceTypes/file"
@@ -48,20 +51,23 @@
         return {
             "serviceId": self.service_id,
             "serviceType": self.service_type,
             "serviceDirection": self.service_direction,
         }
 
     def setupConnection(self, connection: Connection, serviceConfig: FileServiceConfig):
-        self.channel = DataChannel()
-        self.channel.on("data", lambda data: self.handleData(data))
+        channel = DataChannel()
+        channel.on("data", lambda data: self.handleData(data))
         if connection.tiebreaker:
-            connection.transmit(serviceConfig, "data", self.channel)
+            connection.transmit(serviceConfig, "data", channel)
         else:
-            connection.receive(serviceConfig, "data", self.channel)
+            connection.receive(serviceConfig, "data", channel)
+
+    def teardownConnection(self, connection: Connection):
+        pass
 
     def handleData(self, data: Union[str, bytes]):
         if isinstance(data, str):
             header = json.loads(data)
             self.file_type = header["fileType"]
         elif self.file_type is not None:
             event: FileServiceEvent = {"file_type": self.file_type, "content": data}
```

