# Comparing `tmp/pytonconnect-0.0.1.tar.gz` & `tmp/pytonconnect-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonconnect-0.0.1.tar", last modified: Thu Apr 13 13:17:05 2023, max compression
+gzip compressed data, was "pytonconnect-0.0.2.tar", last modified: Wed Apr 19 18:00:48 2023, max compression
```

## Comparing `pytonconnect-0.0.1.tar` & `pytonconnect-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.400750 pytonconnect-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4689 2023-04-13 13:17:05.400750 pytonconnect-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3744 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.370572 pytonconnect-0.0.1/pytonconnect/
--rw-rw-rw-   0        0        0       49 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.400750 pytonconnect-0.0.1/pytonconnect/crypto/
--rw-rw-rw-   0        0        0       43 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/crypto/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/crypto/session_crypto.py
--rw-rw-rw-   0        0        0     1112 2023-04-13 13:16:06.000000 pytonconnect-0.0.1/pytonconnect/exceptions.py
--rw-rw-rw-   0        0        0       96 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.400750 pytonconnect-0.0.1/pytonconnect/provider/
--rw-rw-rw-   0        0        0       88 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/provider/__init__.py
--rw-rw-rw-   0        0        0     4157 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/provider/bridge_gateway.py
--rw-rw-rw-   0        0        0     8586 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/provider/bridge_provider.py
--rw-rw-rw-   0        0        0      876 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/provider/bridge_session.py
--rw-rw-rw-   0        0        0      613 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/provider/provider.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.400750 pytonconnect-0.0.1/pytonconnect/storage/
--rw-rw-rw-   0        0        0       78 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/storage/__init__.py
--rw-rw-rw-   0        0        0      523 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/storage/default_storage.py
--rw-rw-rw-   0        0        0     1009 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/storage/interface.py
--rw-rw-rw-   0        0        0     9628 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/ton_connect.py
--rw-rw-rw-   0        0        0     4737 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/pytonconnect/wallets_list_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:17:05.395448 pytonconnect-0.0.1/pytonconnect.egg-info/
--rw-rw-rw-   0        0        0     4689 2023-04-13 13:17:05.000000 pytonconnect-0.0.1/pytonconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      756 2023-04-13 13:17:05.000000 pytonconnect-0.0.1/pytonconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:17:05.000000 pytonconnect-0.0.1/pytonconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.0.1/pytonconnect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-04-13 13:17:05.000000 pytonconnect-0.0.1/pytonconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 13:17:05.000000 pytonconnect-0.0.1/pytonconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1160 2023-04-13 13:17:05.416383 pytonconnect-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-13 12:49:25.000000 pytonconnect-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.892852 pytonconnect-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4689 2023-04-19 18:00:48.892852 pytonconnect-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3744 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.862851 pytonconnect-0.0.2/pytonconnect/
+-rw-rw-rw-   0        0        0       49 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.882852 pytonconnect-0.0.2/pytonconnect/crypto/
+-rw-rw-rw-   0        0        0       43 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/crypto/session_crypto.py
+-rw-rw-rw-   0        0        0     1414 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/exceptions.py
+-rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.885853 pytonconnect-0.0.2/pytonconnect/parsers/
+-rw-rw-rw-   0        0        0       53 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/__init__.py
+-rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/rpc_parser.py
+-rw-rw-rw-   0        0        0     1493 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/send_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.888851 pytonconnect-0.0.2/pytonconnect/provider/
+-rw-rw-rw-   0        0        0       88 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/__init__.py
+-rw-rw-rw-   0        0        0     4451 2023-04-19 17:58:30.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_gateway.py
+-rw-rw-rw-   0        0        0     8592 2023-04-19 17:56:12.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_provider.py
+-rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_session.py
+-rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/provider.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.890850 pytonconnect-0.0.2/pytonconnect/storage/
+-rw-rw-rw-   0        0        0       78 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/__init__.py
+-rw-rw-rw-   0        0        0      523 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/default_storage.py
+-rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/interface.py
+-rw-rw-rw-   0        0        0     9927 2023-04-19 17:58:30.000000 pytonconnect-0.0.2/pytonconnect/ton_connect.py
+-rw-rw-rw-   0        0        0     4737 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/wallets_list_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.881849 pytonconnect-0.0.2/pytonconnect.egg-info/
+-rw-rw-rw-   0        0        0     4689 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.0.2/pytonconnect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1160 2023-04-19 18:00:48.897850 pytonconnect-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/setup.py
```

### Comparing `pytonconnect-0.0.1/LICENSE` & `pytonconnect-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/PKG-INFO` & `pytonconnect-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytonconnect-0.0.1/README.md` & `pytonconnect-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/crypto/session_crypto.py` & `pytonconnect-0.0.2/pytonconnect/crypto/session_crypto.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/exceptions.py` & `pytonconnect-0.0.2/pytonconnect/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,9 +22,21 @@
     info = "Wallet doesn't support requested feature method."
 
 
 class FetchWalletsError(TonConnectError):
     info = 'An error occurred while fetching the wallets list.'
 
 
+class UnknownError(TonConnectError):
+    info = 'Unknown error.'
+
+
+class BadRequestError(TonConnectError):
+    info = 'Request to the wallet contains errors.'
+
+
+class UnknownAppError(TonConnectError):
+    info = 'App tries to send rpc request to the injected wallet while not connected.'
+
+
 class UserRejectsError(TonConnectError):
     info = 'User rejects the action in the wallet.'
```

### Comparing `pytonconnect-0.0.1/pytonconnect/provider/bridge_gateway.py` & `pytonconnect-0.0.2/pytonconnect/provider/bridge_gateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,47 +36,56 @@
         self._storage = storage
         self._bridge_url = bridge_url
         self._session_id = session_id
         self._listener = listener
         self._errors_listener = errors_listener
     
 
-    async def listen_event_source(self):
+    async def listen_event_source(self, resolve: asyncio.Future):
         try:
             async with self._event_source:
+                resolve.set_result(True)
                 async for event in self._event_source:
                     await self._messages_handler(event)
 
         except asyncio.exceptions.TimeoutError:
-            _LOGGER.error(f'Bridge error -> TimeoutError')
+            _LOGGER.exception(f'Bridge error -> TimeoutError')
         except asyncio.exceptions.CancelledError:
             pass
         except ClientConnectionError:
-            _LOGGER.error(f'Bridge error -> ClientConnectionError')
+            _LOGGER.exception(f'Bridge error -> ClientConnectionError')
         except Exception:
             _LOGGER.exception(f'Bridge error -> Unknown')
+        
+        if not resolve.done():
+            resolve.set_result(False)
 
 
-    async def register_session(self):
+    async def register_session(self) -> bool:
         if self._is_closed:
-            return
+            return False
 
         bridge_base = self._bridge_url.rstrip('/')
         bridge_url = f'{bridge_base}/{self.SSE_PATH}?client_id={self._session_id}'
         
         last_event_id = await self._storage.get_item(IStorage.KEY_LAST_EVENT_ID)
         if last_event_id:
             bridge_url += f'&last_event_id={last_event_id}'
         _LOGGER.debug(f'Bridge url -> {bridge_url}')
 
         if self._handle_listen is not None:
             self._handle_listen.cancel()
 
+        loop = asyncio.get_running_loop()
+        resolve = loop.create_future()
+
         self._event_source = sse_client.EventSource(bridge_url, timeout=-1, on_error=self._errors_handler)
-        self._handle_listen = asyncio.create_task(self.listen_event_source())
+        self._handle_listen = asyncio.create_task(self.listen_event_source(resolve))
+
+        return await resolve
 
 
     async def send(self, request: str, receiver_public_key: str, topic: str, ttl: int = None):
         bridge_base = self._bridge_url.rstrip('/')
         bridge_url = f'{bridge_base}/{self.POST_PATH}?client_id={self._session_id}'
         bridge_url += f'&to={receiver_public_key}'
         bridge_url += f'&ttl={ttl if ttl else self.DEFAULT_TTL}'
```

### Comparing `pytonconnect-0.0.1/pytonconnect/provider/bridge_provider.py` & `pytonconnect-0.0.2/pytonconnect/provider/bridge_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
             if last_id and id <= last_id:
                 _LOGGER.error(f'Received event id (={id}) must be greater than stored last wallet event id (={last_id})')
                 return
             
             if 'event' in wallet_message and wallet_message['event'] != 'connect':
                 connection['last_wallet_event_id'] = id
-                self._storage.set_item(IStorage.KEY_CONNECTION, json.dumps(connection))
+                await self._storage.set_item(IStorage.KEY_CONNECTION, json.dumps(connection))
 
         # self.listeners might be modified in the event handler
         listeners = self._listeners.copy()
 
         if wallet_message['event'] == 'connect':
             await self._update_session(wallet_message, bridge_incoming_message['from'])
```

### Comparing `pytonconnect-0.0.1/pytonconnect/provider/bridge_session.py` & `pytonconnect-0.0.2/pytonconnect/provider/bridge_session.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/provider/provider.py` & `pytonconnect-0.0.2/pytonconnect/provider/provider.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/storage/default_storage.py` & `pytonconnect-0.0.2/pytonconnect/storage/default_storage.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/storage/interface.py` & `pytonconnect-0.0.2/pytonconnect/storage/interface.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect/ton_connect.py` & `pytonconnect-0.0.2/pytonconnect/ton_connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 from pytonconnect.exceptions import TonConnectError, WalletAlreadyConnectedError, WalletNotConnectedError, WalletNotSupportFeatureError
+from pytonconnect.parsers import SendTransactionParser
 from pytonconnect.storage import IStorage, DefaultStorage
 from pytonconnect.wallets_list_manager import WalletsListManager
 from pytonconnect.provider import BridgeProvider
 from pytonconnect.logger import _LOGGER
 
 
 class TonConnect:
@@ -60,16 +60,17 @@
         :return: unsubscribe callback
         """
         self._status_change_subscriptions.append(callback)
         if errors_handler is not None:
             self._status_change_error_subscriptions.append(errors_handler)
 
         def unsubscribe():
-            self._status_change_subscriptions.remove(callback)
-            if errors_handler is not None:
+            if callback in self._status_change_subscriptions:
+                self._status_change_subscriptions.remove(callback)
+            if errors_handler is not None and errors_handler in self._status_change_error_subscriptions:
                 self._status_change_error_subscriptions.remove(errors_handler)
 
         return unsubscribe
 
 
     async def connect(self, wallet, request = None):
         """Generates universal link for an external wallet and subscribes to the wallet's bridge, or sends connect request to the injected wallet.
@@ -124,18 +125,20 @@
         request = {
             'valid_until': transaction.get('valid_until', None),
             'from': transaction.get('from', self._wallet['account']['address']),
             'network': transaction.get('network', self._wallet['account']['chain']),
             'messages': transaction.get('messages', [])
         }
 
-        response = await self._provider.send_request({'method': 'sendTransaction', 'params': [json.dumps(request)]})
+        response = await self._provider.send_request(SendTransactionParser.convert_to_rpc_request(request))
 
-        # TODO: return converted response
-        return response
+        if SendTransactionParser.is_error(response):
+            return SendTransactionParser.parse_and_throw_error(response)
+
+        return SendTransactionParser.convert_from_rpc_response(response)
 
 
     async def disconnect(self):
         """Disconnect from wallet and drop current session."""
         if not self.connected:
             raise WalletNotConnectedError()
```

### Comparing `pytonconnect-0.0.1/pytonconnect/wallets_list_manager.py` & `pytonconnect-0.0.2/pytonconnect/wallets_list_manager.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.1/pytonconnect.egg-info/PKG-INFO` & `pytonconnect-0.0.2/pytonconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytonconnect-0.0.1/pytonconnect.egg-info/SOURCES.txt` & `pytonconnect-0.0.2/pytonconnect.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 pytonconnect.egg-info/SOURCES.txt
 pytonconnect.egg-info/dependency_links.txt
 pytonconnect.egg-info/not-zip-safe
 pytonconnect.egg-info/requires.txt
 pytonconnect.egg-info/top_level.txt
 pytonconnect/crypto/__init__.py
 pytonconnect/crypto/session_crypto.py
+pytonconnect/parsers/__init__.py
+pytonconnect/parsers/rpc_parser.py
+pytonconnect/parsers/send_transaction.py
 pytonconnect/provider/__init__.py
 pytonconnect/provider/bridge_gateway.py
 pytonconnect/provider/bridge_provider.py
 pytonconnect/provider/bridge_session.py
 pytonconnect/provider/provider.py
 pytonconnect/storage/__init__.py
 pytonconnect/storage/default_storage.py
```

### Comparing `pytonconnect-0.0.1/setup.cfg` & `pytonconnect-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 6f6e 636f 6e6e 6563 740d   = pytonconnect.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 5079 7468 6f6e 2053 444b 2066 6f72 2054  Python SDK for T
 00000050: 4f4e 2043 6f6e 6e65 6374 2032 2e30 0d0a  ON Connect 2.0..
 00000060: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000070: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000080: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000090: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

