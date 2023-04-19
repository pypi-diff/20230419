# Comparing `tmp/crosslab_soa_client-0.2.1.tar.gz` & `tmp/crosslab_soa_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_client-0.2.1.tar", last modified: Tue Feb 21 23:50:50 2023, max compression
+gzip compressed data, was "crosslab_soa_client-0.2.2.tar", last modified: Wed Apr 19 18:28:41 2023, max compression
```

## Comparing `crosslab_soa_client-0.2.1.tar` & `crosslab_soa_client-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)     2634 2023-02-21 23:33:01.000000 crosslab_soa_client-0.2.1/README.md
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      617 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/src/crosslab/soa_client/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1579 2023-02-21 20:05:41.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/connection.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     9260 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/connection_webrtc.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     6056 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/device_handler.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/src/crosslab/soa_client/media/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/media/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      395 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/media/gst_track.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      557 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/media/udp_track.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/message_handling.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1077 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      495 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/src/crosslab/soa_client/service.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-02-21 23:50:50.000000 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      775 2023-02-21 23:50:50.000000 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:50:50.000000 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       36 2023-02-21 23:50:50.000000 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:50:50.000000 crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:50:50.580583 crosslab_soa_client-0.2.1/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)     3095 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/tests/test_device_handler.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     9062 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.1/tests/test_webrtc_connection.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2494 2023-04-19 18:06:55.000000 crosslab_soa_client-0.2.2/README.md
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      617 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.419268 crosslab_soa_client-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.419268 crosslab_soa_client-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1762 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     9539 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection_webrtc.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     6244 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/device_handler.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      395 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/gst_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      557 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/udp_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/message_handling.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1077 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-14 11:45:37.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)      764 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/service.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/
+-rw-r--r--   0 dev       (1000) docker-host   (967)       81 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/connection_stub.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      787 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/dummy_track.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     4298 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/src/crosslab/soa_client/test_helper/service_stub.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      981 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       36 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:28:41.000000 crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:28:41.422602 crosslab_soa_client-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1970 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/tests/test_device_handler.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     5239 2023-04-19 13:37:16.000000 crosslab_soa_client-0.2.2/tests/test_webrtc_connection.py
```

### Comparing `crosslab_soa_client-0.2.1/setup.cfg` & `crosslab_soa_client-0.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_client
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_client-0.2.1/src/crosslab/soa_client/connection.py` & `crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,53 @@
-import asyncio
 from abc import ABC, abstractmethod
 from typing import Any, Literal, Optional, Union
 
-from pyee.asyncio import AsyncIOEventEmitter  # type: ignore
-
 from crosslab.soa_client.messages import SignalingMessage
+from pyee.asyncio import AsyncIOEventEmitter  # type: ignore
 
 MediaStreamTrack = Any
 
 
 class Channel(ABC):
     channel_type: str
 
+    @abstractmethod
+    def close(self) -> None:
+        pass
+
 
 class MediaChannel(Channel, AsyncIOEventEmitter):
     channel_type = "MediaChannel"
     track: Union[MediaStreamTrack, None]
 
     def __init__(self, track: Optional[MediaStreamTrack] = None):
         super().__init__()
         self.track = track
 
+    def close(self):
+        self.emit("close")
+        self.remove_all_listeners()
+
 
 class DataChannel(Channel, AsyncIOEventEmitter):
     channel_type = "DataChannel"
 
     def send(self, data: Union[bytes, str]):
         self.emit("upstreamData", data)
 
     def downstreamData(self, data: Union[bytes, str]):
         self.emit("data", data)
 
     async def opened(self):
-        await asyncio.sleep(0.05)
         self.emit("open")
 
+    def close(self):
+        self.emit("close")
+        self.remove_all_listeners()
+
 
 class Connection(ABC):
     tiebreaker: bool
     state: Literal["created", "connecting", "connected", "disconnected"]
 
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `crosslab_soa_client-0.2.1/src/crosslab/soa_client/connection_webrtc.py` & `crosslab_soa_client-0.2.2/src/crosslab/soa_client/connection_webrtc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from enum import Enum
-from typing import Any, Dict, Literal, cast
+from typing import Any, Dict, List, Literal, cast
 
 from aiortc import (  # type: ignore
     RTCConfiguration,
     RTCPeerConnection,
     RTCSessionDescription,
 )
 from aiortc.events import RTCTrackEvent  # type: ignore
@@ -26,14 +26,15 @@
     Callee = "Callee"
 
 
 class WebRTCPeerConnection(AsyncIOEventEmitter, Connection):
     _receivingChannelMap: Dict[str, Channel]
     _mediaChannelMap: Dict[str, MediaChannel]
     _transeiverMap: Dict[Any, str]
+    _dataChannels: List[DataChannel]
 
     def __init__(self):
         AsyncIOEventEmitter.__init__(self)
         Connection.__init__(self)
         # config = RTCConfiguration(
         #     [
         #         RTCIceServer(urls="stun:stun.goldi-labs.de:3478"),
@@ -78,24 +79,28 @@
         self.pc.on("iceconnectionstatechange", connectionstatechanged)
         self.pc.on("signalingstatechange", connectionstatechanged)
         self.pc.on("track", self._on_track)
 
         self._receivingChannelMap = dict()
         self._mediaChannelMap = dict()
         self._transeiverMap = dict()
+        self._dataChannels = list()
 
     async def _on_track(self, track: RTCTrackEvent):
         transeiver = track.transceiver
         label = transeiver.receiver.track.id
         channel = self._mediaChannelMap.get(label)
         assert channel is not None  # TODO: handle this
         channel.emit("track", transeiver.receiver.track)
 
     async def close(self):
         await self.pc.close()
+        for channel in self._dataChannels:
+            channel.close()
+
         del self.pc
 
     def _create_label(self, serviceConfig: ServiceConfig, id: str):
         id1 = (
             serviceConfig["serviceId"]
             if self.tiebreaker
             else serviceConfig["remoteServiceId"]
@@ -117,14 +122,15 @@
         channel: Channel,
     ):
         label = self._create_label(serviceConfig, id)
         if channel.channel_type == "MediaChannel":
             self._mediaChannelMap[label] = cast(MediaChannel, channel)
         else:
             dchannel = cast(DataChannel, channel)
+            self._dataChannels.append(dchannel)
             datachannel = self.pc.createDataChannel(label)
 
             async def upstreamData(data):
                 datachannel.send(data)
                 await datachannel._RTCDataChannel__transport._data_channel_flush()  # type: ignore
                 await datachannel._RTCDataChannel__transport._transmit()  # type: ignore
 
@@ -142,14 +148,16 @@
         id: str,
         channel: Channel,
     ):
         label = self._create_label(serviceConfig, id)
         self._receivingChannelMap[label] = channel
         if channel.channel_type == "MediaChannel":
             self._mediaChannelMap[label] = cast(MediaChannel, channel)
+        else:
+            self._dataChannels.append(cast(DataChannel, channel))
 
     async def connect(self):
         self.state = "connecting"
         self.role = WebRTCRole.Caller if self.tiebreaker else WebRTCRole.Callee
         if self.role == WebRTCRole.Caller:
             await self._createMediaChannels()
             await self._makeOffer()
```

### Comparing `crosslab_soa_client-0.2.1/src/crosslab/soa_client/device_handler.py` & `crosslab_soa_client-0.2.2/src/crosslab/soa_client/device_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import asyncio
 import re
 from typing import Dict, Optional
 
 import aiohttp
 from crosslab.api_client import APIClient  # type: ignore
-from pyee import AsyncIOEventEmitter
+from pyee.asyncio import AsyncIOEventEmitter
 
 from crosslab.soa_client.connection import Connection
 from crosslab.soa_client.connection_webrtc import WebRTCPeerConnection
 from crosslab.soa_client.messages import (
     AuthenticationMessage,
     ClosePeerConnectionMessage,
     CreatePeerConnectionMessage,
@@ -127,15 +128,18 @@
         else:
             raise Exception("Unknown connection type")
         connection.tiebreaker = msg["tiebreaker"]
         for service_config in msg["services"]:
             assert service_config["serviceId"] in self._services  # see Issue #4
             service = self._services.get(service_config["serviceId"], None)
             assert service is not None  # TODO: Error handling
-            service.setupConnection(connection, service_config)
+            if asyncio.iscoroutinefunction(service.setupConnection):
+                await service.setupConnection(connection, service_config)
+            else:
+                service.setupConnection(connection, service_config)
 
         async def onSignalingMessage(message: dict):
             signalingMessage: SignalingMessage = {
                 "connectionUrl": msg["connectionUrl"],
                 "content": message["content"],
                 "signalingType": message["signalingType"],
                 "messageType": "signaling",
```

### Comparing `crosslab_soa_client-0.2.1/src/crosslab/soa_client/media/udp_track.py` & `crosslab_soa_client-0.2.2/src/crosslab/soa_client/media/udp_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.1/src/crosslab/soa_client/messages.py` & `crosslab_soa_client-0.2.2/src/crosslab/soa_client/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.1/src/crosslab_soa_client.egg-info/SOURCES.txt` & `crosslab_soa_client-0.2.2/src/crosslab_soa_client.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 src/crosslab/soa_client/message_handling.py
 src/crosslab/soa_client/messages.py
 src/crosslab/soa_client/py.typed
 src/crosslab/soa_client/service.py
 src/crosslab/soa_client/media/__init__.py
 src/crosslab/soa_client/media/gst_track.py
 src/crosslab/soa_client/media/udp_track.py
+src/crosslab/soa_client/test_helper/__init__.py
+src/crosslab/soa_client/test_helper/connection_stub.py
+src/crosslab/soa_client/test_helper/dummy_track.py
+src/crosslab/soa_client/test_helper/service_stub.py
 src/crosslab_soa_client.egg-info/PKG-INFO
 src/crosslab_soa_client.egg-info/SOURCES.txt
 src/crosslab_soa_client.egg-info/dependency_links.txt
 src/crosslab_soa_client.egg-info/requires.txt
 src/crosslab_soa_client.egg-info/top_level.txt
 tests/test_device_handler.py
 tests/test_webrtc_connection.py
```

### Comparing `crosslab_soa_client-0.2.1/tests/test_device_handler.py` & `crosslab_soa_client-0.2.2/tests/test_device_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,52 +5,15 @@
 import aiohttp
 import pytest
 from helpers import AsyncException, wait
 
 from crosslab.soa_client.connection import DataChannel
 from crosslab.soa_client.device_handler import DeviceHandler
 from crosslab.soa_client.service import Service
-
-
-class DataOnly(Service):
-    service_type = "goldi/legacy/message"
-    service_direction = "inout"
-    service_id: str
-
-    channels: List[DataChannel]
-    messages = []
-
-    def __init__(self, serviceId: str):
-        super().__init__()
-        self.channels = list()
-        self.service_id = serviceId
-
-    def getMeta(self):
-        return {
-            "serviceType": self.service_type,
-            "serviceId": self.service_id,
-            "serviceDirection": self.service_direction,
-        }
-
-    def setupConnection(self, connection, serviceConfig):
-        channel = DataChannel()
-        channel.on("data", lambda data: self.handleData(data))
-        self.channels.append(channel)
-
-        if connection.tiebreaker:
-            connection.transmit(serviceConfig, "data", channel)
-        else:
-            connection.receive(serviceConfig, "data", channel)
-
-    def handleData(self, data: str):
-        self.messages.append(data)
-
-    def _send(self, *args, data: str):
-        for channel in self.channels:
-            channel.send(data)
+from crosslab.soa_client.test_helper.service_stub import ServiceStub
 
 
 @pytest.mark.asyncio
 async def test_connect_and_authenticate(mock_server):
     mock_server.get("/devices/123/websocket", payload="token")
     ws = mock_server.ws("/devices/123/ws")
     ws.expect(
@@ -61,35 +24,32 @@
 
     dh = DeviceHandler()
     await dh.connect(base_url + "/devices/123")
     assert mock_server.asExpected
 
 
 @pytest.mark.asyncio
-@pytest.mark.skip(
-    reason="This test is not working yet. Connection is never build -> timeout"
-)
 async def test_create_peerconnection(mock_server):
     mock_server.get("/devices/123/websocket", payload="token")
 
     ws = mock_server.ws("/devices/123/ws")
     ws.expect(
-        r'{"messageType": "authenticate", "authenticated": null, "deviceUrl": "{base_url}/devices/123", "token": "token"}',
+        r'{"messageType": "authenticate", "token": "token"}',
         answer=r'{"messageType": "authenticate", "authenticated": true, "deviceUrl": "{base_url}/devices/123"}',
     )
     ws.send(
         r'{"messageType": "command", "command": "createPeerconnection", "connectionType": "webrtc", "connectionUrl": "{base_url}/peerconnections/1233",'
         r'"services": [{"serviceType": "dataOnly", "serviceId": "local", "remoteServiceId": "remote"}], "tiebreaker": true}'
     )
     ws.sleep(0.5)
     ws.send(
         r'{"messageType": "command", "command": "closePeerconnection", "connectionUrl": "{base_url}/peerconnections/1233"}'
     )
     base_url = await mock_server.start()
 
     dh = DeviceHandler()
 
-    dataOnlyService = DataOnly("local")
+    dataOnlyService = ServiceStub("local", dataChannel=True)
     dh.add_service(dataOnlyService)
     await wait(dh.connect(base_url + "/devices/123"), mock_server.async_exception)
 
     assert mock_server.asExpected
```

