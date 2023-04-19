# Comparing `tmp/crosslab_soa_service_webcam-0.2.1.tar.gz` & `tmp/crosslab_soa_service_webcam-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_webcam-0.2.1.tar", last modified: Tue Feb 21 23:53:44 2023, max compression
+gzip compressed data, was "crosslab_soa_service_webcam-0.2.2.tar", last modified: Wed Apr 19 18:32:35 2023, max compression
```

## Comparing `crosslab_soa_service_webcam-0.2.1.tar` & `crosslab_soa_service_webcam-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.151698 crosslab_soa_service_webcam-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-02-21 23:53:44.151698 crosslab_soa_service_webcam-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-21 14:52:17.000000 crosslab_soa_service_webcam-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-02-21 23:53:44.151698 crosslab_soa_service_webcam-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-21 14:52:17.000000 crosslab_soa_service_webcam-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.141698 crosslab_soa_service_webcam-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.141698 crosslab_soa_service_webcam-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.141698 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.151698 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/
--rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-02-21 15:15:55.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1003 2023-02-21 15:12:46.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/media.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      155 2023-02-21 15:14:10.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-21 14:52:17.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      957 2023-02-21 16:08:37.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/webcam_service.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:53:44.151698 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-02-21 23:53:44.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      532 2023-02-21 23:53:44.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:53:44.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-02-21 23:53:44.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:53:44.000000 crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1066 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/media.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      151 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/webcam_service.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      555 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      628 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/tests/test_standard.py
```

### Comparing `crosslab_soa_service_webcam-0.2.1/setup.cfg` & `crosslab_soa_service_webcam-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_webcam
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Webcam Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/media.py` & `crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/media.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import random
 import socket
 import subprocess
 from typing import Optional
 
-from aiortc import MediaStreamTrack
+from aiortc import MediaStreamTrack  # type: ignore
 
 
 class UDPTrack(MediaStreamTrack):
     def __init__(self, port: int, kind="video") -> None:
         super().__init__()
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)  # Internet  # UDP
         self.sock.bind(("", port))
@@ -18,14 +18,17 @@
 
     async def raw_recv(self):
         return await self.loop.sock_recv(self.sock, 2048)
 
     def recv(self):
         return
 
+    def stop(self):
+        self.sock.close()
+
 
 class GstTrack(UDPTrack):
     def __init__(self, pipeline, port: Optional[int] = None, kind="video") -> None:
         if port is None:
             port = random.randint(10000, 65535)
         super().__init__(port, kind)
         subprocess.Popen(
```

### Comparing `crosslab_soa_service_webcam-0.2.1/src/crosslab/soa_services/webcam/webcam_service.py` & `crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/webcam_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from aiortc import MediaStreamTrack
+from aiortc import MediaStreamTrack  # type: ignore
 from crosslab.soa_client.connection import Connection, MediaChannel
 from crosslab.soa_client.service import Service
 
-from crosslab.soa_services.webcam.messages import ElectricalServiceConfig
+from crosslab.soa_services.webcam.messages import WebcamServiceConfig
 
 
 class WebcamService__Producer(Service):
     service_type = "http://api.goldi-labs.de/serviceTypes/webcam"
     service_direction = "out"
     service_id: str
 
@@ -20,11 +20,14 @@
         return {
             "serviceId": self.service_id,
             "serviceType": self.service_type,
             "serviceDirection": self.service_direction,
         }
 
     def setupConnection(
-        self, connection: Connection, serviceConfig: ElectricalServiceConfig
+        self, connection: Connection, serviceConfig: WebcamServiceConfig
     ):
         channel = MediaChannel(self._track)
         connection.transmit(serviceConfig, "video", channel)
+
+    def teardownConnection(self, connection: Connection):
+        self._track.stop()
```

### Comparing `crosslab_soa_service_webcam-0.2.1/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt` & `crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 src/crosslab/soa_services/webcam/messages.py
 src/crosslab/soa_services/webcam/py.typed
 src/crosslab/soa_services/webcam/webcam_service.py
 src/crosslab_soa_service_webcam.egg-info/PKG-INFO
 src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
 src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
 src/crosslab_soa_service_webcam.egg-info/requires.txt
-src/crosslab_soa_service_webcam.egg-info/top_level.txt
+src/crosslab_soa_service_webcam.egg-info/top_level.txt
+tests/test_standard.py
```

