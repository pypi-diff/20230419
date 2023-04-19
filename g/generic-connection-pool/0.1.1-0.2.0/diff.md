# Comparing `tmp/generic_connection_pool-0.1.1.tar.gz` & `tmp/generic_connection_pool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_connection_pool-0.1.1.tar", max compression
+gzip compressed data, was "generic_connection_pool-0.2.0.tar", max compression
```

## Comparing `generic_connection_pool-0.1.1.tar` & `generic_connection_pool-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1211 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/LICENSE
--rw-r--r--   0        0        0     7578 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/README.rst
--rw-r--r--   0        0        0       44 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/__init__.py
--rw-r--r--   0        0        0    15845 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/asyncio.py
--rw-r--r--   0        0        0    12560 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/common.py
--rw-r--r--   0        0        0        0 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/contrib/__init__.py
--rw-r--r--   0        0        0     1769 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/contrib/psycopg2.py
--rw-r--r--   0        0        0     2296 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/contrib/socket.py
--rw-r--r--   0        0        0     2268 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/contrib/socket_async.py
--rw-r--r--   0        0        0      171 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/exceptions.py
--rw-r--r--   0        0        0     4810 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/heap.py
--rw-r--r--   0        0        0        0 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/py.typed
--rw-r--r--   0        0        0    15389 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/generic_connection_pool/threding.py
--rw-r--r--   0        0        0     1494 2023-03-16 19:40:55.639849 generic_connection_pool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8767 1970-01-01 00:00:00.000000 generic_connection_pool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7578 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/README.rst
+-rw-r--r--   0        0        0       44 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/__init__.py
+-rw-r--r--   0        0        0    15757 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/asyncio.py
+-rw-r--r--   0        0        0    12570 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/common.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/contrib/__init__.py
+-rw-r--r--   0        0        0     1769 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/contrib/psycopg2.py
+-rw-r--r--   0        0        0     2586 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/contrib/socket.py
+-rw-r--r--   0        0        0     2275 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/contrib/socket_async.py
+-rw-r--r--   0        0        0      171 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/exceptions.py
+-rw-r--r--   0        0        0     4810 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/heap.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/py.typed
+-rw-r--r--   0        0        0    15301 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/generic_connection_pool/threding.py
+-rw-r--r--   0        0        0     1494 2023-04-19 14:43:22.045674 generic_connection_pool-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8767 1970-01-01 00:00:00.000000 generic_connection_pool-0.2.0/PKG-INFO
```

### Comparing `generic_connection_pool-0.1.1/LICENSE` & `generic_connection_pool-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `generic_connection_pool-0.1.1/README.rst` & `generic_connection_pool-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/asyncio.py` & `generic_connection_pool-0.2.0/generic_connection_pool/asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,25 +151,22 @@
         finally:
             await asyncio.shield(self._release_connection(endpoint, conn))
 
         if self._collector is None:
             dispose_batch_size = self._dispose_batch_size or int(math.log2(self._pool_size + 1)) + 1
             await self._collect_disposable_connections(dispose_batch_size)
 
-    async def close(self, graceful_timeout: Optional[float] = None, timeout: Optional[float] = None) -> None:
+    async def close(self, graceful_timeout: float = 0.0, timeout: Optional[float] = None) -> None:
         """
         Closes the connection pool.
 
-        :param graceful_timeout: timeout within which the pool waits all acquired connection to be released
+        :param graceful_timeout: timeout within which the pool waits for all acquired connection to be released
         :param timeout: timeout after which the pool closes all connection despite they are released or not
         """
 
-        if graceful_timeout is None:
-            graceful_timeout = timeout
-
         if graceful_timeout is not None and timeout is not None:
             assert timeout >= graceful_timeout, "timeout can't be less than graceful_timeout"
 
         graceful_timer = Timer(graceful_timeout)
         global_timer = Timer(timeout)
 
         self._stopped.set()
@@ -399,15 +396,15 @@
 
                 if not released and not acquired:
                     break
 
                 try:
                     while released:
                         conn_info = released[-1]
-                        await self._dispose_connection(conn_info, timeout=graceful_timer.remains)
+                        await self._dispose_connection(conn_info, timeout=global_timer.remains)
                         released.pop()
                 except asyncio.TimeoutError:
                     await asyncio.shield(self._return_released_conns(released))
 
                 if graceful_timer.timedout:
                     for conn_info in acquired:
                         await self._dispose_connection(conn_info, timeout=global_timer.remains)
@@ -418,9 +415,9 @@
                 raise
 
     async def _return_released_conns(self, released: List[ConnectionInfo[EndpointT, ConnectionT]]) -> None:
         async with self._lock:
             for conn_info in released:
                 pool = self._pools[conn_info.endpoint]
                 pool.queue[conn_info.conn] = conn_info
-                pool.access_queue.remove((conn_info.accessed_at, conn_info.conn))
+                pool.access_queue.push((conn_info.accessed_at, conn_info.conn))
                 self._pool_size += 1
```

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/common.py` & `generic_connection_pool-0.2.0/generic_connection_pool/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
         Returns number of seconds until the timeout.
         """
 
         if self._timeout is None:
             return None
 
-        return self._timeout - self.elapsed
+        return max(0.0, self._timeout - self.elapsed)
 
     @property
     def timedout(self) -> bool:
         """
         Returns if the timer timed-out.
         """
```

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/contrib/psycopg2.py` & `generic_connection_pool-0.2.0/generic_connection_pool/contrib/psycopg2.py`

 * *Files identical despite different names*

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/contrib/socket.py` & `generic_connection_pool-0.2.0/generic_connection_pool/contrib/socket.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,40 @@
+import contextlib
 import socket
 from ipaddress import IPv4Address, IPv6Address
 from ssl import SSLContext, SSLSocket
-from typing import Optional, Tuple, Union
+from typing import Generator, Optional, Tuple, Union
 
 from generic_connection_pool.threding import BaseConnectionManager
 
 IpAddress = Union[IPv4Address, IPv6Address]
 Hostname = str
 Port = int
 TcpEndpoint = Tuple[IpAddress, Port]
 
 
+@contextlib.contextmanager
+def socket_timeout(sock: socket.socket, timeout: Optional[float]) -> Generator[None, None, None]:
+    if timeout is None:
+        yield
+        return
+
+    orig_timeout = sock.gettimeout()
+    sock.settimeout(max(timeout, 1e-6))  # if timeout is 0 set it a small value to prevent non-blocking socket mode
+    try:
+        yield
+    except OSError as e:
+        if 'timed out' in str(e):
+            raise TimeoutError
+        else:
+            raise
+    finally:
+        sock.settimeout(orig_timeout)
+
+
 class TcpSocketConnectionManager(BaseConnectionManager[TcpEndpoint, socket.socket]):
     """
     TCP socket connection manager.
     """
 
     def create(self, endpoint: TcpEndpoint, timeout: Optional[float] = None) -> socket.socket:
         addr, port = endpoint
@@ -24,25 +44,20 @@
         elif addr.version == 6:
             family = socket.AF_INET6
         else:
             raise RuntimeError("unsupported address version type: %s", addr.version)
 
         sock = socket.socket(family=family, type=socket.SOCK_STREAM)
 
-        orig_timeout = sock.gettimeout()
-        sock.settimeout(timeout)
-        try:
+        with socket_timeout(sock, timeout):
             sock.connect((str(addr), port))
-        finally:
-            sock.settimeout(orig_timeout)
 
         return sock
 
     def dispose(self, endpoint: TcpEndpoint, conn: socket.socket, timeout: Optional[float] = None) -> None:
-        conn.settimeout(timeout)
         try:
             conn.shutdown(socket.SHUT_RDWR)
         except OSError:
             pass
 
         conn.close()
 
@@ -58,24 +73,20 @@
     def __init__(self, ssl: SSLContext):
         self._ssl = ssl
 
     def create(self, endpoint: SslEndpoint, timeout: Optional[float] = None) -> SSLSocket:
         hostname, port = endpoint
 
         sock = self._ssl.wrap_socket(socket.socket(type=socket.SOCK_STREAM), server_hostname=hostname)
-        orig_timeout = sock.gettimeout()
-        sock.settimeout(timeout)
-        try:
+
+        with socket_timeout(sock, timeout):
             sock.connect((hostname, port))
-        finally:
-            sock.settimeout(orig_timeout)
 
         return sock
 
     def dispose(self, endpoint: SslEndpoint, conn: SSLSocket, timeout: Optional[float] = None) -> None:
-        conn.settimeout(timeout)
         try:
             conn.shutdown(socket.SHUT_RDWR)
         except OSError:
             pass
 
         conn.close()
```

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/contrib/socket_async.py` & `generic_connection_pool-0.2.0/generic_connection_pool/contrib/socket_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 class TcpStreamConnectionManager(BaseConnectionManager[TcpStreamEndpoint, TcpStream]):
     """
     TCP stream connection manager.
     """
 
-    def __init__(self, ssl: Union[None, bool, SSLContext]):
+    def __init__(self, ssl: Union[None, bool, SSLContext] = None):
         self._ssl = ssl
 
     async def create(self, endpoint: TcpStreamEndpoint) -> TcpStream:
         hostname, port = endpoint
         server_hostname = hostname if self._ssl is not None else None
 
         reader, writer = await asyncio.open_connection(
```

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/heap.py` & `generic_connection_pool-0.2.0/generic_connection_pool/heap.py`

 * *Files identical despite different names*

### Comparing `generic_connection_pool-0.1.1/generic_connection_pool/threding.py` & `generic_connection_pool-0.2.0/generic_connection_pool/threding.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,25 +155,22 @@
         finally:
             self._release_connection(endpoint, conn)
 
         if self._collector is None:
             dispose_batch_size = self._dispose_batch_size or int(math.log2(self._pool_size + 1)) + 1
             self._collect_disposable_connections(dispose_batch_size)
 
-    def close(self, graceful_timeout: Optional[float] = None, timeout: Optional[float] = None) -> None:
+    def close(self, graceful_timeout: float = 0.0, timeout: Optional[float] = None) -> None:
         """
         Closes the connection pool.
 
-        :param graceful_timeout: timeout within which the pool waits all acquired connection to be released
+        :param graceful_timeout: timeout within which the pool waits for all acquired connection to be released
         :param timeout: timeout after which the pool closes all connection despite they are released or not
         """
 
-        if graceful_timeout is None:
-            graceful_timeout = timeout
-
         if graceful_timeout is not None and timeout is not None:
             assert timeout >= graceful_timeout, "timeout can't be less than graceful_timeout"
 
         graceful_timer = Timer(graceful_timeout)
         global_timer = Timer(timeout)
 
         self._stopped.set()
@@ -397,15 +394,15 @@
 
                 if not released and not acquired:
                     break
 
                 try:
                     while released:
                         conn_info = released[-1]
-                        self._dispose_connection(conn_info, timeout=graceful_timer.remains)
+                        self._dispose_connection(conn_info, timeout=global_timer.remains)
                         released.pop()
                 except TimeoutError:
                     self._return_released_conns(released)
 
                 if graceful_timer.timedout:
                     for conn_info in acquired:
                         self._dispose_connection(conn_info, timeout=global_timer.remains)
@@ -416,9 +413,9 @@
                 raise
 
     def _return_released_conns(self, released: List[ConnectionInfo[EndpointT, ConnectionT]]) -> None:
         with self._lock:
             for conn_info in released:
                 pool = self._pools[conn_info.endpoint]
                 pool.queue[conn_info.conn] = conn_info
-                pool.access_queue.remove((conn_info.accessed_at, conn_info.conn))
+                pool.access_queue.push((conn_info.accessed_at, conn_info.conn))
                 self._pool_size += 1
```

### Comparing `generic_connection_pool-0.1.1/pyproject.toml` & `generic_connection_pool-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generic-connection-pool"
-version = "0.1.1"
+version = "0.2.0"
 description = "generic connection pool"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/generic-connection-pool"
 repository = "https://github.com/dapper91/generic-connection-pool"
 documentation = "https://github.com/dapper91/generic-connection-pool"
```

### Comparing `generic_connection_pool-0.1.1/PKG-INFO` & `generic_connection_pool-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-connection-pool
-Version: 0.1.1
+Version: 0.2.0
 Summary: generic connection pool
 Home-page: https://github.com/dapper91/generic-connection-pool
 License: Unlicense
 Keywords: pool,connection-pool,generic,asyncio,socket,tcp,db,http
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.9,<4.0
```

