# Comparing `tmp/crosslab_soa_service_message-0.2.1.tar.gz` & `tmp/crosslab_soa_service_message-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_message-0.2.1.tar", last modified: Tue Feb 21 23:54:44 2023, max compression
+gzip compressed data, was "crosslab_soa_service_message-0.2.2.tar", last modified: Wed Apr 19 18:36:14 2023, max compression
```

## Comparing `crosslab_soa_service_message-0.2.1.tar` & `crosslab_soa_service_message-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-21 21:33:57.000000 crosslab_soa_service_message-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-21 21:33:57.000000 crosslab_soa_service_message-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/
--rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-02-21 21:39:17.000000 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2455 2023-02-21 21:44:12.000000 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/message_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-02-21 21:44:05.000000 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-21 21:33:57.000000 crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/py.typed
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:54:44.482091 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-02-21 23:54:44.000000 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      500 2023-02-21 23:54:44.000000 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:54:44.000000 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-02-21 23:54:44.000000 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:54:44.000000 crosslab_soa_service_message-0.2.1/src/crosslab_soa_service_message.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      580 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.395013 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      213 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2607 2023-04-19 13:37:16.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/message_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      232 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/py.typed
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      350 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      523 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:36:14.000000 crosslab_soa_service_message-0.2.2/src/crosslab_soa_service_message.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:36:14.398347 crosslab_soa_service_message-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      916 2023-04-19 13:37:16.000000 crosslab_soa_service_message-0.2.2/tests/test_standard.py
```

### Comparing `crosslab_soa_service_message-0.2.1/setup.cfg` & `crosslab_soa_service_message-0.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_message
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA message Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_message-0.2.1/src/crosslab/soa_services/message/message_service.py` & `crosslab_soa_service_message-0.2.2/src/crosslab/soa_services/message/message_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Literal, Union
 
 from crosslab.soa_client.connection import Connection, DataChannel
 from crosslab.soa_client.service import Service
-from pyee import AsyncIOEventEmitter
+from pyee.asyncio import AsyncIOEventEmitter
 
 from crosslab.soa_services.message.messages import (
     MessageServiceConfig,
     MessageServiceEvent,
 )
 
 
@@ -31,14 +31,17 @@
     ):
         self.channel = DataChannel()
         if connection.tiebreaker:
             connection.transmit(serviceConfig, "data", self.channel)
         else:
             connection.receive(serviceConfig, "data", self.channel)
 
+    def teardownConnection(self, connection: Connection):
+        pass
+
     async def sendMessage(self, message: str, message_type: Literal["info", "error"]):
         self.channel.send(json.dumps({"messageType": message_type, "message": message}))
 
 
 class MessageService__Consumer(Service, AsyncIOEventEmitter):
     service_type = "https://api.goldi-labs.de/serviceTypes/message"
     service_direction = "in"
@@ -61,14 +64,17 @@
         self.channel = DataChannel()
         self.channel.on("data", lambda data: self.handleData(data))
         if connection.tiebreaker:
             connection.transmit(serviceConfig, "data", self.channel)
         else:
             connection.receive(serviceConfig, "data", self.channel)
 
+    def teardownConnection(self, connection: Connection):
+        pass
+
     def handleData(self, data: Union[str, bytes]):
         if isinstance(data, str):
             msg = json.loads(data)
             event: MessageServiceEvent = {
                 "message_type": msg["messageType"],
                 "message": msg["message"],
             }
```

