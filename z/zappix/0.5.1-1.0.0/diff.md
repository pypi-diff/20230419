# Comparing `tmp/zappix-0.5.1.tar.gz` & `tmp/zappix-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zappix-0.5.1.tar", last modified: Wed Mar  8 22:32:24 2023, max compression
+gzip compressed data, was "zappix-1.0.0.tar", last modified: Wed Apr 19 21:43:18 2023, max compression
```

## Comparing `zappix-0.5.1.tar` & `zappix-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 22:32:24.000000 zappix-0.5.1/
--rw-r--r--   0 root         (0) root         (0)     3756 2023-03-08 22:32:24.000000 zappix-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-03-08 22:32:22.000000 zappix-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix/
--rw-rw-rw-   0 root         (0) root         (0)     6451 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/agent_active.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5204 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/dstream.py
--rw-rw-rw-   0 root         (0) root         (0)     6588 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/sender.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/server.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-03-08 22:32:22.000000 zappix-0.5.1/zappix/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3756 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-08 22:32:24.000000 zappix-0.5.1/zappix.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-03-08 22:32:22.000000 zappix-0.5.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-03-08 22:32:22.000000 zappix-0.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 22:32:24.000000 zappix-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.958181 zappix-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-04-19 21:43:17.000000 zappix-1.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-04-19 21:43:18.958181 zappix-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-04-19 21:43:17.000000 zappix-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:43:18.958181 zappix-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-19 21:43:17.000000 zappix-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.956181 zappix-1.0.0/zappix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/agent_active.py
+-rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/dstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/get.py
+-rw-rw-rw-   0 root         (0) root         (0)     6736 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     6889 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-04-19 21:43:17.000000 zappix-1.0.0/zappix/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:43:18.957181 zappix-1.0.0/zappix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 21:43:18.000000 zappix-1.0.0/zappix.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zappix-0.5.1/PKG-INFO` & `zappix-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: zappix
-Version: 0.5.1
+Version: 1.0.0
 Summary: A Python replacement for Zabbix sender and get.
 Home-page: https://gitlab.com/szuro/zappix
 Author: Robert Szulist
 Author-email: r.szulist@gmail.com
-License: UNKNOWN
 Keywords: zabbix get sender
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # zappix - a package for Zabbix sender and get.
@@ -88,9 +87,7 @@
 | envvar          | usage                                                                                                              |
 | --------------- | ------------------------------------------------------------------------------------------------------------------ |
 | ZAPPIX_AGENT    | IP address or DNS name of running Zabbix agent                                                                     |
 | ZAPPIX_SERVER   | IP address or DNS name of running Zabbix Server                                                                    |
 | ZAPPIX_API      | URL of Zabbix fronted. Schema is required                                                                          |
 | ZAPPIX_API_USER | User for creating entities via API. Should have RW permissions to a Host group with ID=2 - Usually 'Linux Servers' |
 | ZAPPIX_API_PASS | Password for that user                                                                                             |
-
-
```

### Comparing `zappix-0.5.1/setup.py` & `zappix-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='zappix',
-    version='0.5.1',
+    version='1.0.0',
     description='A Python replacement for Zabbix sender and get.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://gitlab.com/szuro/zappix',
     author='Robert Szulist',
     author_email='r.szulist@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: System :: Monitoring',
         'License :: OSI Approved :: MIT License',
     ],
     keywords='zabbix get sender',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     test_suite="tests",
     install_requires=[
```

### Comparing `zappix-0.5.1/zappix/protocol.py` & `zappix-1.0.0/zappix/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Module containing models for Zabbix protocol.
 """
 
 from typing import List, Any, Optional, Dict, Union
+from dataclasses import dataclass
 import abc
 import json
 from ast import literal_eval
 from uuid import uuid4
 
 
 class _Model(abc.ABC):
@@ -22,16 +23,18 @@
         return json.dumps(self, cls=ModelEncoder).encode("utf-8")
 
 
 class ModelEncoder(json.JSONEncoder):
     """
     Class for encoding to JSON models implemented herein.
     """
+
     def default(self, o: _Model) -> Dict[str, Any]:
-        d = {k: getattr(o, k) for k in type(o).__slots__ if getattr(o, k, False)}
+        d = {k: getattr(o, k)
+             for k in type(o).__slots__ if getattr(o, k, False)}
         return d
 
 
 class ItemData(_Model):
     """
     Class model representing data to be sent to a trapper item.
 
@@ -93,15 +96,16 @@
         self.ns = ns
         self.id = 0
         self.state = state
 
 
 class _TrapperRequest(_Model, abc.ABC):
     __slots__ = ['request', 'data', 'host', 'clock', 'ns', 'session']
-    __supported_requests = ["active checks", "agent data", "sender data", "queue.get", "status.get"]
+    __supported_requests = ["active checks", "agent data",
+                            "sender data", "queue.get", "status.get"]
 
     def __init__(self, request: str, **kwargs) -> None:
         super().__init__()
         if request not in _TrapperRequest.__supported_requests:
             raise ValueError
         self.request = request
         self.host = kwargs.get('host')
@@ -127,14 +131,15 @@
     Class implementing protocol for requesting active checks for host.
 
     Parameters
     ----------
     :host:
         Get active checks for specified host.
     """
+
     def __init__(self, host: str) -> None:
         super().__init__(request="active checks", host=host)
 
 
 class SenderDataRequest(_TrapperRequest):
     """
     Class implementing protocol for sending data with sender protocol.
@@ -147,15 +152,15 @@
     __item_class = SenderData
 
     def __init__(self, data: Optional[List[SenderData]] = None) -> None:
         super().__init__(
             request="sender data",
             data=data,
             item_class=SenderDataRequest.__item_class
-            )
+        )
 
     def add_item(self, item: SenderData) -> None:
         """
         Add data to request.
 
         Parameters
         ----------
@@ -181,15 +186,15 @@
 
     def __init__(self, data: Optional[List[AgentData]] = None) -> None:
         super().__init__(
             request="agent data",
             data=data,
             item_class=AgentDataRequest.__item_class,
             session=uuid4().hex
-            )
+        )
 
         self._item_id = 1
         if self.data:
             for d in self.data:
                 d.id = self._item_id
                 self._item_id += 1
 
@@ -212,28 +217,41 @@
 class ActiveItem:
     """
     Zabbix active item configuration.
     """
 
     __slots__ = ['key', 'delay', 'lastlogsize', 'mtime']
 
-    def __init__(self, key: str, delay: int, lastlogsize: int = 0, mtime: int = 0) -> None:
+    def __init__(self, key: str, delay: str, lastlogsize: int = 0, mtime: int = 0) -> None:
         self.key = key
         self.delay = delay
         self.lastlogsize = lastlogsize
         self.mtime = mtime
 
 
 class ServerRequest(_TrapperRequest):
 
     __slots__ = ['request', 'type', 'sid', 'limit']
-    __supported_request_types = ['overview', 'overview by proxy', 'details', 'ping']
+    __supported_request_types = ['overview',
+                                 'overview by proxy', 'details', 'ping']
 
     def __init__(self, request, request_type, sid, **kwargs) -> None:
         if request_type not in ServerRequest.__supported_request_types:
             raise ValueError
         super().__init__(request=request, type=request_type, sid=sid)
         self.request = request
         self.type = request_type
         self.sid = sid
         if 'limit' in kwargs:
             self.limit = str(kwargs.get("limit"))
+
+
+@dataclass
+class ServerInfo:
+    """
+    Info on items processed by the server.
+    """
+    processed: int
+    failed: int
+    total: int
+    seconds_spent: float
+    response: str
```

### Comparing `zappix-0.5.1/zappix/agent_active.py` & `zappix-1.0.0/zappix/agent_active.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+"""
+Implementaction of Active agent communication.
+"""
+
 from typing import List, Optional, Dict
-from zappix.protocol import ActiveChecksRequest, AgentDataRequest, ModelEncoder, ActiveItem
+from zappix.protocol import ActiveChecksRequest, AgentDataRequest, ModelEncoder, ActiveItem, ServerInfo
 from zappix.dstream import _Dstream
 import json
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -34,39 +38,40 @@
 
         Returns
         -------
         list
             List of ActiveItem objects.
         """
         request = ActiveChecksRequest(self._host)
-        logger.info(f"Getting active checks for host: {self._host} from: {self._ip}:{self._port}")
+        logger.info(
+            f"Getting active checks for host: {self._host} from: {self._ip}:{self._port}")
         result = self._send(request.to_bytes())
         return self._parse_active_check_list(result)
 
-    def send_collected_data(self, data: AgentDataRequest) -> Optional[Dict]:
+    def send_collected_data(self, data: AgentDataRequest) -> ServerInfo:
         """
         Sends collected data to Zabbix.
 
         Parameters
         ----------
         :data:
             Instance of AgentDataRequest.
 
         Returns
         -------
-        list
-            List of ActiveItem objects.
+        ServerInfo
+            Information on items processed by server.
         """
         if not isinstance(data, AgentDataRequest):
             logger.error(f"Object {data} is not an instance AgentDataRequest")
             raise ValueError
         result = self._send(data.to_bytes())
         return self._parse_server_response(result)
 
     @staticmethod
     def _parse_active_check_list(data: str) -> List[ActiveItem]:
         response = json.loads(data)
         active_list_raw = response.get('data', [])
         active_list = [ActiveItem(
-                item['key'], item['delay'], item['lastlogsize'], item['mtime']
-                ) for item in active_list_raw]
+            item['key'], item['delay'], int(item['lastlogsize']), int(item['mtime'])
+        ) for item in active_list_raw]
         return active_list
```

### Comparing `zappix-0.5.1/zappix/dstream.py` & `zappix-1.0.0/zappix/dstream.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,170 @@
 """
 Module containing handlers for Zabbix protocol.
 """
 
 from ast import Return
 from typing import Optional, Dict
 import abc
+import re
 import socket
 import struct
 import logging
 import json
 from enum import Flag, IntEnum
 from OpenSSL.SSL import Context, Connection, TLSv1_2_METHOD
 from openssl_psk import patch_context
+from zappix.protocol import ServerInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 ZBX_HEADER_LEN = 13
+INFO_RE = re.compile(
+    r'processed: (\d+); failed: (\d+); total: (\d+); seconds spent: (\d+\.\d+)')
 
 
-class ProtocolFlags(Flag):
-    ZABBIX = b'\x01'
-    COMPRESSION = b"\x02"
-    LARGE_PACKET = b"\x04"
+class ProtocolFlags(IntEnum):
+    ZABBIX = 1
+    COMPRESSION = 2
+    LARGE_PACKET = 4
 
 
 class PSKEnum(IntEnum):
     IDENTITY_MIN_LENGTH = 1
     IDENTITY_MAX_LENGTH = 128
     PSK_MIN_LENGTH = 32
     PSK_MAX_LENGTH = 512
 
 
-
 class _Dstream(abc.ABC):
     def __init__(self, target: str, port: int = 10051, source_address: Optional[str] = None) -> None:
         self._ip = target
         self._port = port
         self._source_address = source_address
+        self._timeout = None
         self._psk = b''
         self._psk_identity = b''
 
+    def set_timeout(timeout: float):
+        """
+        Set timeout for the network connection
+
+        Parameters
+        ----------
+        :timeout:
+            Timeout in seconds.  
+        """
+        self._timeout = timeout
 
     def set_psk_encryption(self, identity: str, psk: str):
         if not (PSKEnum.IDENTITY_MIN_LENGTH <= len(identity) <= PSKEnum.IDENTITY_MAX_LENGTH):
             raise ValueError("PSK identity lenght out of bounds")
-        if  not (PSKEnum.PSK_MIN_LENGTH <= len(psk) <= PSKEnum.PSK_MAX_LENGTH):
+        if not (PSKEnum.PSK_MIN_LENGTH <= len(psk) <= PSKEnum.PSK_MAX_LENGTH):
             raise ValueError("PSK key lenght out of bounds")
 
         patch_context()
         try:
-            self._psk  = bytes.fromhex(psk)
+            self._psk = bytes.fromhex(psk)
             self._psk_identity = identity.encode()
         except ValueError:
             raise ValueError("The provided PSK key is not hexadecimal")
 
-
     def _wrap_psk_socket(self, sock):
         def client_callback(conn, identity_hint):
             return (self._psk_identity, self._psk)
         ctx = Context(TLSv1_2_METHOD)
-        ctx.set_cipher_list(b'EECDH+aRSA+AES128:RSA+aRSA+AES128:kECDHEPSK+AES128:kPSK+AES128')
+        ctx.set_cipher_list(
+            b'EECDH+aRSA+AES128:RSA+aRSA+AES128:kECDHEPSK+AES128:kPSK+AES128')
         ctx.set_psk_client_callback(client_callback)
         return Connection(ctx, sock)
 
-
     def _get_socket(self) -> socket.socket:
         address_family = socket.getaddrinfo(self._ip, self._port)[0][0]
-        return socket.socket(address_family)
-
+        s = socket.socket(address_family)
+        s.settimeout(self._timeout)
+        return s
 
     def _send(self, payload: bytes) -> str:
         data = b""
         parsed = ""
         s = None
         try:
             s = self._get_socket()
             if self._source_address:
                 s.bind((self._source_address, 0))
-                logger.info(f"Opening connection to {self._ip}:{self._port} with source address {self._source_address}")
+                logger.info(
+                    f"Opening connection to {self._ip}:{self._port} with source address {self._source_address}")
             else:
                 logger.info(f"Opening connection to {self._ip}:{self._port}")
             if self._psk and self._psk_identity:
                 s = self._wrap_psk_socket(s)
             packed = self._pack_request(payload)
             s.connect((self._ip, self._port))
             s.sendall(packed)
             data = self._recv_response(s)
             parsed = self._unpack_response(data)
-        except socket.error:
-            logger.exception(f"Cannot connect to host {self._ip}:{self._port}:")
-        except struct.error:
-            logger.exception("Recived response is corrupted:")
-        except Exception:
-            logger.exception("Something really bad happened:")
+        except Exception as e:
+            logger.exception(f"Encoutered Exception: {e}")
+            raise e
         finally:
             if s is not None:
                 logger.info(f"Closing connection to {self._ip}:{self._port}")
                 s.close()
-            return parsed
+        return parsed
 
     def _unpack_response(self, response: bytes) -> str:
-        _, protocol, length, _ = struct.unpack('<4s1sLL', response[:ZBX_HEADER_LEN])
+        _, protocol, length, _ = struct.unpack(
+            '<4s1sLL', response[:ZBX_HEADER_LEN])
         data = struct.unpack(
             f'<{length}s',
             response[ZBX_HEADER_LEN:ZBX_HEADER_LEN+length]
-            )[0]
+        )[0]
 
         return data.decode('utf-8')
 
     def _pack_request(self, payload: bytes) -> bytes:
         payload_len = len(payload)
         packed = struct.pack(
             f'<4scL4s{payload_len}s',
             b'ZBXD',
-            ProtocolFlags.ZABBIX.value,
+            ProtocolFlags.ZABBIX.value.to_bytes(1, 'little'),
             payload_len,
             b"\x00\x00\x00\x00",
             payload
-            )
-        logger.debug(f"Packed payload for {self._ip}:{self._port}. Payload length: {payload_len}. Length with headers: {len(packed)}")
+        )
+        logger.debug(
+            f"Packed payload for {self._ip}:{self._port}. Payload length: {payload_len}. Length with headers: {len(packed)}")
         return packed
 
     def _recv_response(self, socket_: socket.socket, buff: int = 1024) -> bytes:
         data = b""
         buffer = socket_.recv(buff)
         _, data_length = struct.unpack('<5sQ', buffer[:ZBX_HEADER_LEN])
         logger.debug(f"Received {len(buffer)} from {self._ip}:{self._port}")
         while buffer:
             data += buffer
             if len(data[ZBX_HEADER_LEN:]) < data_length:
                 buffer = socket_.recv(buff)
-                logger.debug(f"Received {len(buffer)} from {self._ip}:{self._port}")
+                logger.debug(
+                    f"Received {len(buffer)} from {self._ip}:{self._port}")
             else:
                 break
 
-        logger.debug(f"Completed data retrieval from {self._ip}:{self._port}. Total length: {len(data)}")
+        logger.debug(
+            f"Completed data retrieval from {self._ip}:{self._port}. Total length: {len(data)}")
         return data
 
     @staticmethod
-    def _parse_server_response(info) -> Optional[Dict]:
-        try:
-            response = json.loads(info)
-        except json.decoder.JSONDecodeError:
-            return None
-        data = response.get('info', None)
-        splitted = [x.strip().split(':') for x in data.split(';')]
-        for i, split in enumerate(splitted):
-            name, val = split
-            splitted[i][1] = float(val) if name == 'seconds spent' else int(val)
-        return dict(splitted)
+    def _parse_server_response(info) -> ServerInfo:
+        response = json.loads(info)
+        parsed_data = INFO_RE.match(response.get('info', ''))
+
+        server_info = ServerInfo(
+            response=response.get('response'),
+            processed=int(parsed_data.group(1)),
+            failed=int(parsed_data.group(2)),
+            total=int(parsed_data.group(3)),
+            seconds_spent=float(parsed_data.group(4))
+        )
+        return server_info
```

### Comparing `zappix-0.5.1/zappix/sender.py` & `zappix-1.0.0/zappix/sender.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Python implementation of Zabbix sender.
 """
 
 from typing import List, Any, Optional, Dict, Tuple, Callable, Union, Optional
 from zappix.dstream import _Dstream
-from zappix.protocol import SenderData, SenderDataRequest
+from zappix.protocol import SenderData, SenderDataRequest, ServerInfo
 import csv
 import time
 import functools
 import logging
 
 logger = logging.getLogger(__name__)
 
@@ -26,58 +26,59 @@
     :source_address:
         Source IP address.
     """
 
     def __init__(self, server: str, port: int = 10051, source_address: Optional[str] = None) -> None:
         super().__init__(server, port, source_address)
 
-    def send_value(self, host: str, key: str, value: Any) -> Union[Dict[str, Any], None]:
+    def send_value(self, host: str, key: str, value: Any) -> ServerInfo:
         """
         Send a single value to a Zabbix host.
 
         Parameters
         ----------
         :host:
             Name of a host as visible in Zabbix frontend.
         :key:
             String representing an item key.
         :value:
             Value to be sent.
 
         Returns
         -------
-        dict
-            Information from server.
+        ServerInfo
+            Information on items processed by server.
         """
         payload = SenderDataRequest()
         payload.add_item(SenderData(host, key, value))
 
         response = self._send(payload.to_bytes())
         parsed_response = self._parse_server_response(response)
-        return parsed_response if parsed_response else None
+        return parsed_response
 
-    def send_file(self, file: str, with_timestamps: bool = False, with_ns: bool = False) -> Tuple[Optional[Dict], List[int]]:
+    def send_file(self, file: str, with_timestamps: bool = False, with_ns: bool = False) -> Tuple[ServerInfo, List[int]]:
         """
         Send values contained in a file to specified hosts.
 
         Parameters
         ----------
         :file:
             Path to file with data.
         :with_timestamps:
             Specify whether file contains timestamps for items.
         :with_ns:
             Specify whether file contains ns for items.
 
         Returns
         -------
-        dict
-            Information from server.
+        ServerInfo, list
+            Information on items processed by server and a list of failed line numbers.
         """
-        items, corrupted_lines = self.parse_data_file(file, with_timestamps, with_ns)
+        items, corrupted_lines = self.parse_data_file(
+            file, with_timestamps, with_ns)
         payload = SenderDataRequest(items)
 
         if with_timestamps:
             now = time.time()
             payload.clock = int(now//1)
             payload.ns = int(now % 1 * 1e9)
 
@@ -105,65 +106,72 @@
             def get_value(*args, **kwargs):
                 result = func(*args, **kwargs)
                 self.send_value(host, key, str(result))
                 return result
             return get_value
         return wrap_function
 
-    def send_bulk(self, request: SenderDataRequest, with_timestamps: bool = False) -> Optional[Dict]:
+    def send_bulk(self, data: List[SenderData], with_timestamps: bool = False) -> ServerInfo:
         """
         Send item values to Zabbix in bulk.
 
         Parameters
         ----------
-        :request:
-            Path to file with data.
+        :data:
+            List of SenderData objects.
         :with_timestamps:
             Specify whether SenderData objects contain timestamps.
 
         Returns
         -------
-        dict
-            Information from server.
+        ServerInfo
+            Information on items processed by server.
         """
+
+        request = SenderDataRequest(data)
         if with_timestamps:
             now = time.time()
             request.clock = int(now//1)
             request.ns = int(now % 1 * 1e9)
 
         response = self._send(request.to_bytes())
         return self._parse_server_response(response)
 
     @staticmethod
     def parse_data_file(file: str, with_timestamps: bool = False, with_ns: bool = False) -> Tuple[List[SenderData], List[int]]:
         items = []
         failed_lines = []
         try:
             with open(file, 'r', encoding='utf-8') as values:
-                reader = csv.reader(values, delimiter=' ', escapechar='\\', skipinitialspace=True)
+                reader = csv.reader(values, delimiter=' ',
+                                    escapechar='\\', skipinitialspace=True)
                 logger.info(f"Reading data from {file}")
 
                 for row in reader:
                     if not all(row):
                         failed_lines.append(reader.line_num)
-                        logger.error(f"Found corrupted line in {file} at row {reader.line_num}")
+                        logger.error(
+                            f"Found corrupted line in {file} at row {reader.line_num}")
                         continue
                     try:
                         if with_timestamps:
                             if with_ns:
-                                data = SenderData(row[0], row[1], row[4], int(row[2]), int(row[3]))
+                                data = SenderData(
+                                    row[0], row[1], row[4], int(row[2]), int(row[3]))
                             else:
-                                data = SenderData(row[0], row[1], row[3], int(row[2]))
+                                data = SenderData(
+                                    row[0], row[1], row[3], int(row[2]))
                         else:
                             data = SenderData(row[0], row[1], row[2])
                         items.append(data)
                         logger.debug(f"Adding {data} to Sender payload")
                     except (IndexError, ValueError):
                         failed_lines.append(reader.line_num)
-                        logger.exception(f"Could not parse {file} at line {reader.line_num}")
+                        logger.exception(
+                            f"Could not parse {file} at line {reader.line_num}")
         except EnvironmentError:
             logger.exception(f'Error while reading file: {file}')
         finally:
             return items, failed_lines
 
 
 if __name__ == '__main__':
@@ -184,10 +192,11 @@
         zab = Sender(args.zabbix, args.port, args.source_address)
     else:
         zab = Sender(args.zabbix, args.port)
 
     if all([args.host, args.key, args.value]):
         result = zab.send_value(args.host, args.key, args.value)
     elif args.input_file:
-        result, corrupted_lines = zab.send_file(args.input_file, True if args.with_timestamps else False, True if args.with_ns else False)
+        result, corrupted_lines = zab.send_file(
+            args.input_file, True if args.with_timestamps else False, True if args.with_ns else False)
 
     print('info from server: "{}"'.format(result))
```

### Comparing `zappix-0.5.1/zappix/get.py` & `zappix-1.0.0/zappix/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,28 +44,28 @@
         -------
         string
             Value of item.
         """
 
         return self._send(
             self._pack_key(key)
-            )
+        )
 
     def get_report(self, keys: List[str]) -> Dict[str, str]:
         """
         Get value of a item identified by keys provided in supplied iterable.
         Note that there are executed synchronously, so the performance might not be ideal.
 
         Parameters
         ----------
         :keys:
             Iterable containing string representing item keys.
 
-        Return
-        ------
+        Returns
+        -------
         dict
             Dict containing keys with corresponding values.
         """
 
         report = {key: self._send(self._pack_key(key)) for key in keys}
         return report
```

### Comparing `zappix-0.5.1/zappix.egg-info/PKG-INFO` & `zappix-1.0.0/zappix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: zappix
-Version: 0.5.1
+Version: 1.0.0
 Summary: A Python replacement for Zabbix sender and get.
 Home-page: https://gitlab.com/szuro/zappix
 Author: Robert Szulist
 Author-email: r.szulist@gmail.com
-License: UNKNOWN
 Keywords: zabbix get sender
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # zappix - a package for Zabbix sender and get.
@@ -88,9 +87,7 @@
 | envvar          | usage                                                                                                              |
 | --------------- | ------------------------------------------------------------------------------------------------------------------ |
 | ZAPPIX_AGENT    | IP address or DNS name of running Zabbix agent                                                                     |
 | ZAPPIX_SERVER   | IP address or DNS name of running Zabbix Server                                                                    |
 | ZAPPIX_API      | URL of Zabbix fronted. Schema is required                                                                          |
 | ZAPPIX_API_USER | User for creating entities via API. Should have RW permissions to a Host group with ID=2 - Usually 'Linux Servers' |
 | ZAPPIX_API_PASS | Password for that user                                                                                             |
-
-
```

### Comparing `zappix-0.5.1/LICENSE.txt` & `zappix-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zappix-0.5.1/README.md` & `zappix-1.0.0/README.md`

 * *Files identical despite different names*

