# Comparing `tmp/async_etcd3gw-0.2.tar.gz` & `tmp/async_etcd3gw-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.2.tar", last modified: Fri Apr 14 23:00:22 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.3.tar", last modified: Wed Apr 19 09:22:21 2023, max compression
```

## Comparing `async_etcd3gw-0.2.tar` & `async_etcd3gw-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/async_etcd3gw/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/async_etcd3gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/tests/test_async_etcd3gw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-19 09:22:21.304426 async_etcd3gw-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 09:22:21.304426 async_etcd3gw-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/tests/test_client.py
```

### Comparing `async_etcd3gw-0.2/LICENSE` & `async_etcd3gw-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/PKG-INFO` & `async_etcd3gw-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_etcd3gw
-Version: 0.2
+Version: 0.3
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.2/README.md` & `async_etcd3gw-0.3/README.md`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/async_etcd3gw/__init__.py` & `async_etcd3gw-0.3/async_etcd3gw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.2"
+__version__ = "0.3"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.2/async_etcd3gw/async_client.py` & `async_etcd3gw-0.3/async_etcd3gw/async_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         cert_key=None,
         cert_cert=None,
         timeout=None,
         api_path=DEFAULT_API_PATH,
     ):
         """Construct an client to talk to etcd3's grpc-gateway's /v3 HTTP API
 
-        :param host:
-        :param port:
-        :param protocol:
+        Args:
+            host (str): The etcd hostname.
+            port (int): The etcd port.
+            protocol (str): The etcd protocol (http/https).
+            timeout (int): The default timeout.
         """
         self.host = host
         self.port = port
         self.protocol = protocol
         self.api_path = api_path
 
         if timeout is not None:
@@ -96,27 +98,50 @@
             self.client_session_kwargs["timeout"] = self.timeout
         if self.connector is not None:
             self.client_session_kwargs["connector"] = self.connector
 
     def get_url(self, path):
         """Construct a full url to the v3 API given a specific path
 
-        :param path:
-        :return: url
+        This method takes a path as an argument and returns a url that points to the v3 API of the host.
+
+        Args:
+            path (str): The path to append to the base url.
+
+        Returns:
+            str: The full url to the v3 API with the given path.
         """
         host = f"[{ self.host }]" if ":" in self.host else self.host
         base_url = f"{ self.protocol }://{ host }:{ self.port }"
         return base_url + self.api_path + path.lstrip("/")
 
     async def post(self, *args, **kwargs):
-        """helper method for HTTP POST
+        """Helper method for HTTP POST
 
-        :param args:
-        :param kwargs:
-        :return: json response
+        This method performs an asynchronous HTTP POST request using aiohttp.
+        It takes arbitrary arguments and keyword arguments that are passed to the session.post method.
+        It returns a json response if the request is successful, or raises an exception if the request
+        fails or times out.
+
+        Example:
+            >>> self.client_session_kwargs = {"timeout": 10}
+            >>> await self.post("https://example.com/api", data={"key": "value"})
+            {'result': 'ok'}
+
+        Args:
+            *args: Positional arguments for the session.post method.
+            **kwargs: Keyword arguments for the session.post method.
+
+        Returns:
+            dict: The json response from the server.
+
+        Raises:
+            AsyncEtcd3Exception: If the status code is not 200 and not in the predefined exceptions.
+            ConnectionTimeoutError: If the request times out.
+            ConnectionFailedError: If the connection fails.
         """
         try:
             async with aiohttp.ClientSession(**self.client_session_kwargs) as session:
                 async with session.post(*args, **kwargs) as resp:
                     if resp.status in _EXCEPTIONS_BY_CODE:
                         raise _EXCEPTIONS_BY_CODE[resp.status](resp.text, resp.reason)
                     if resp.status != 200:
@@ -126,60 +151,94 @@
             raise ConnectionTimeoutError(str(ex))
         except aiohttp.ClientConnectionError as ex:
             raise ConnectionFailedError(str(ex))
 
     async def status(self):
         """Status gets the status of the etcd cluster member.
 
-        :return: json response
+        Returns:
+            dict: The json response from the server.
         """
         return await self.post(self.get_url("/maintenance/status"), json={})
 
     async def members(self):
         """Lists all the members in the cluster.
 
-        :return: json response
+        Returns:
+            dict: The json response from the server.
         """
         result = await self.post(self.get_url("/cluster/member/list"), json={})
         return result["members"]
 
     async def lease(self, ttl=DEFAULT_TIMEOUT):
         """Create a AsyncLease object given a timeout
 
-        :param ttl: timeout
-        :return: AsyncLease object
+        This method performs an post request to the etcd v3 API to create a lease
+        with a specified time to live (TTL). It takes a TTL as an argument,
+        and returns an AsyncLease object that represents the lease.
+        The lease can be used to attach keys to it, keep it alive, or revoke it.
+
+        Example:
+            >>> lease = await self.lease(ttl=10)
+            >>> await self.put("/foo", "bar", lease=lease)
+            True
+
+        Args:
+            ttl (int): The timeout for the lease in seconds.
+
+        Returns:
+            AsyncLease: The lease object.
+
         """
         result = await self.post(self.get_url("/lease/grant"), json={"TTL": ttl, "ID": 0})
         return AsyncLease(int(result["ID"]), async_client=self)
 
     async def lock(self, id=None, ttl=DEFAULT_TIMEOUT):
         """Create a Lock object given an ID and timeout
 
-        :param id: ID for the lock, creates a new uuid if not provided
-        :param ttl: timeout
-        :return: Lock object
+        This method creates a lock with a specified ID and TTL.
+        It takes an ID and a TTL as arguments, and returns an AsyncLock object that represents the lock.
+        The lock can be used to acquire or release the lock on a key.
+
+        Example:
+            >>> lock = await self.lock(id="mylock", ttl=10)
+            >>> await lock.acquire("foo")
+            True
+
+        Args:
+            id (str): The ID for the lock. Creates a new UUID if not provided.
+            ttl (int): The timeout for the lock in seconds.
+
+        Returns:
+            AsyncLock: The lock object.
         """
         if id is None:
             id = str(uuid.uuid4())
         return AsyncLock(id, ttl=ttl, async_client=self)
 
     async def create(self, key, value, lease=None):
         """Atomically create the given key only if the key doesn't exist.
 
         This verifies that the create_revision of a key equales to 0, then
         creates the key with the value.
         This operation takes place in a transaction.
 
-        :param key: key in etcd to create
-        :param value: value of the key
-        :type value: bytes or string
-        :param lease: lease to connect with, optional
-        :returns: status of transaction, ``True`` if the create was
-                  successful, ``False`` otherwise
-        :rtype: bool
+        Example:
+            >>> await self.create("/foo", "bar")
+            True
+            >>> await self.create("/foo", "baz")
+            False
+
+        Args:
+            key (str): The key to create.
+            value (str): The value to store.
+            lease (Lease): The lease object that specifies the expiration time of the key.
+
+        Returns:
+            bool: True if the create was successful, False otherwise.
         """
         base64_key = _encode(key)
         base64_value = _encode(value)
         txn = {
             "compare": [
                 {
                     "key": base64_key,
@@ -201,40 +260,68 @@
         if lease:
             txn["success"][0]["request_put"]["lease"] = lease.id
         result = await self.transaction(txn)
         if "succeeded" in result:
             return result["succeeded"]
         return False
 
-    async def put(self, key, value, lease=None):
+    async def put(self, key, value, lease=None, metadata=False):
         """Put puts the given key into the key-value store.
 
+        This method performs an asynchronous HTTP POST request to the etcd v3 API to store
+        a key-value pair. It takes a key and a value as arguments, and optionally a lease object
+        that specifies the expiration time of the key.
         A put request increments the revision of the key-value store
         and generates one event in the event history.
 
-        :param key:
-        :param value:
-        :param lease:
-        :return: boolean
+        Example:
+            >>> await self.put("/foo", "bar")
+            True
+
+        Args:
+            key (str): The key to store.
+            value (str): The value to store.
+            lease (Lease): The lease object that specifies the expiration time of the key.
+            metadata (bool): Whether to return the metadata.
+
+        Returns:
+            bool, dict: If metadata is True, the json response from the server else True if the put was successful.
         """
         payload = {"key": _encode(key), "value": _encode(value)}
         if lease:
             payload["lease"] = lease.id
-        await self.post(self.get_url("/kv/put"), json=payload)
-        return True
+        result = await self.post(self.get_url("/kv/put"), json=payload)
+        if metadata:
+            return result
+        else:
+            return True
 
     async def get(self, key, metadata=False, sort_order=None, sort_target=None, **kwargs):
         """Range gets the keys in the range from the key-value store.
 
-        :param key:
-        :param metadata:
-        :param sort_order: 'ascend' or 'descend' or None
-        :param sort_target: 'key' or 'version' or 'create' or 'mod' or 'value'
-        :param kwargs:
-        :return:
+         This method performs an asynchronous HTTP POST request to the etcd v3 API to retrieve
+         a range of keys from the key-value store.
+
+        Example:
+            >>> await self.get("/foo")
+            [b'bar']
+            >>> await self.get("/foo", metadata=True)
+            [(b'bar', {'key': 'foo', 'create_revision': 1, 'mod_revision': 1, 'version': 1})]
+            >>> await self.get("/foo", sort_order="descend", sort_target="version")
+            [b'baz', b'bar']
+
+        Args:
+            key (str): The key to query.
+            metadata (bool): Whether to return the metadata of the keys.
+            sort_order (str): The order of the keys. One of "ascend" or "descend" or None.
+            sort_target (str): The criteria for sorting. One of "key", "version", "create", "mod" or "value".
+            **kwargs: Other keyword arguments for the request payload.
+
+        Returns:
+            list: A list of values or a list of tuples of value and metadata.
         """
         try:
             order = 0
             if sort_order:
                 order = _SORT_ORDER.index(sort_order)
         except ValueError:
             raise ValueError('sort_order must be one of "ascend" or "descend"')
@@ -266,55 +353,65 @@
             return [value_with_metadata(item) for item in result["kvs"]]
 
         return [_decode(item.get("value", "")) for item in result["kvs"]]
 
     async def get_all(self, sort_order=None, sort_target="key"):
         """Get all keys currently stored in etcd.
 
-        :returns: sequence of (value, metadata) tuples
+        Returns:
+            list: A sequence of (value, metadata) tuples
         """
         return await self.get(
             key=_encode(b"\0"),
             metadata=True,
             sort_order=sort_order,
             sort_target=sort_target,
             range_end=_encode(b"\0"),
         )
 
     async def get_prefix(self, key_prefix, sort_order=None, sort_target=None):
         """Get a range of keys with a prefix.
 
-        :param sort_order: 'ascend' or 'descend' or None
-        :param key_prefix: first key in range
+        Args:
+            key_prefix (str): The prefix to query.
+            sort_order (str): The order of the keys. One of "ascend" or "descend" or None.
+            sort_target (str): The criteria for sorting. One of "key", "version", "create", "mod" or "value".
 
-        :returns: sequence of (value, metadata) tuples
+        Returns:
+            list: A sequence of (value, metadata) tuples
         """
         return await self.get(
             key_prefix,
             metadata=True,
             range_end=_encode(_increment_last_byte(key_prefix)),
             sort_order=sort_order,
             sort_target=sort_target,
         )
 
-    async def replace(self, key, initial_value, new_value):
+    async def replace(self, key, initial_value, new_value, metadata=False):
         """Atomically replace the value of a key with a new value.
 
         This compares the current value of a key, then replaces it with a new
         value if it is equal to a specified value. This operation takes place
         in a transaction.
 
-        :param key: key in etcd to replace
-        :param initial_value: old value to replace
-        :type initial_value: bytes or string
-        :param new_value: new value of the key
-        :type new_value: bytes or string
-        :returns: status of transaction, ``True`` if the replace was
-                  successful, ``False`` otherwise
-        :rtype: bool
+        Example:
+            >>> await self.replace("/foo", "bar", "baz")
+            True
+            >>> await self.replace("/foo", "bar", "qux")
+            False
+
+        Args:
+            key (str): The key to replace.
+            initial_value (str): The old value to compare.
+            new_value (str): The new value to swap.
+            metadata (bool): Whether to return the metadata.
+
+        Returns:
+            bool, dict: If metadata is True, the json response from the server else True if the replace was successful.
         """
         base64_key = _encode(key)
         base64_initial_value = _encode(initial_value)
         base64_new_value = _encode(new_value)
         txn = {
             "compare": [
                 {
@@ -331,62 +428,75 @@
                         "value": base64_new_value,
                     }
                 }
             ],
             "failure": [],
         }
         result = await self.transaction(txn)
-        if "succeeded" in result:
+        if metadata:
+            return result
+        elif "succeeded" in result:
             return result["succeeded"]
         return False
 
-    async def delete(self, key, **kwargs):
+    async def delete(self, key, metadata=False, **kwargs):
         """DeleteRange deletes the given range from the key-value store.
 
         A delete request increments the revision of the key-value store and
         generates a delete event in the event history for every deleted key.
 
-        :param key:
-        :param kwargs:
-        :return:
+        Args:
+            key (str): The key to delete.
+            metadata (bool): Whether to return the metadata.
+
+        Returns:
+            bool, dict: If metadata is True, the json response from the server else True if the delete was successful.
         """
         payload = {
             "key": _encode(key),
         }
         payload.update(kwargs)
 
         result = await self.post(self.get_url("/kv/deleterange"), json=payload)
-        if "deleted" in result:
-            return True
-        return False
+        if metadata:
+            return result
+        else:
+            return "deleted" in result
 
-    async def delete_prefix(self, key_prefix):
+    async def delete_prefix(self, key_prefix, metadata=False):
         """Delete a range of keys with a prefix in etcd."""
-        return await self.delete(key_prefix, range_end=_encode(_increment_last_byte(key_prefix)))
+        return await self.delete(key_prefix, range_end=_encode(_increment_last_byte(key_prefix)), metadata=metadata)
 
     async def transaction(self, txn):
         """Txn processes multiple requests in a single transaction.
 
         A txn request increments the revision of the key-value store and
         generates events with the same revision for every completed request.
         It is not allowed to modify the same key several times within one txn.
 
-        :param txn:
-        :return:
+        Args:
+            txn: The json request payload.
+        Returns:
+            dict: The json response from the server.
         """
         return await self.post(self.get_url("/kv/txn"), data=json.dumps(txn))
 
     async def watch(self, key, **kwargs):
         """Watch a key.
 
-        :param key: key to watch
+        This method creates a watch request to the etcd v3 API to monitor a key for changes.
+        It returns a tuple of events_iterator and cancel.
+        Use events_iterator to get the events of key changes and cancel to cancel the watch request.
+
+        Args:
+            key (str): The key to watch.
+            **kwargs: Other keyword arguments for the watch request.
 
-        :returns: tuple of ``events_iterator`` and ``cancel``.
-                  Use ``events_iterator`` to get the events of key changes
-                  and ``cancel`` to cancel the watch request
+        Returns:
+            tuple: A tuple of events_iterator and cancel.
         """
         event_queue = asyncio.Queue()
 
         async def callback(event):
             await event_queue.put(event)
 
         w = AsyncWatcher(async_client=self, key=key, callback=callback, **kwargs)
@@ -412,17 +522,24 @@
         """The same as ``watch``, but watches a range of keys with a prefix."""
         kwargs["range_end"] = _increment_last_byte(key_prefix)
         return await self.watch(key_prefix, **kwargs)
 
     async def watch_once(self, key, timeout=None, **kwargs):
         """Watch a key and stops after the first event.
 
-        :param key: key to watch
-        :param timeout: (optional) timeout in seconds.
-        :returns: event
+        Args:
+            key (str): The key to watch.
+            timeout (int): The timeout in seconds. Optional.
+            **kwargs: Other keyword arguments for the watch request.
+
+        Returns:
+            dict: The first event of the key change.
+
+        Raises:
+            WatchTimedOut: If the timeout is reached.
         """
         event_queue = asyncio.Queue()
 
         async def callback(event):
             await event_queue.put(event)
 
         w = AsyncWatcher(async_client=self, key=key, callback=callback, **kwargs)
```

### Comparing `async_etcd3gw-0.2/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.3/async_etcd3gw/async_lock.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 
 __all__ = ["AsyncLock"]
 
 
 class AsyncLock(object):
     def __init__(self, name, ttl=DEFAULT_TIMEOUT, async_client=None):
         """Create a lock using the given name with specified timeout
-        :param name:
-        :param ttl:
-        :param async_client:
+
+        This class represents a lock that can be acquired or released on a key in the key-value store.
+        A lock has a name and a time to live (TTL) that specifies the expiration time of the lock.
+
+        Args:
+            name (str): The name of the lock.
+            ttl (int): The timeout for the lock in seconds.
+            async_client (AsyncClient): The async client object that communicates with the etcd v3 API.
         """
         self.name = name
         self.ttl = ttl
         self.async_client = async_client
         self.key = LOCK_PREFIX + self.name
         self.lease = None
         self._uuid = str(uuid.uuid1())
@@ -89,17 +94,15 @@
 
         result = await self.async_client.transaction(txn)
         if "succeeded" in result:
             return result["succeeded"]
         return False
 
     async def refresh(self):
-        """Refresh the lease on the lock
-        :return:
-        """
+        """Refresh the lease on the lock"""
         return await self.lease.refresh()
 
     async def is_acquired(self):
         """Check if the lock is acquired"""
         values = await self.async_client.get(self.key)
         return self._uuid.encode("latin-1") in values
```

### Comparing `async_etcd3gw-0.2/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.3/async_etcd3gw/async_watch.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.3/async_etcd3gw/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/async_etcd3gw.egg-info/PKG-INFO` & `async_etcd3gw-0.3/async_etcd3gw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-etcd3gw
-Version: 0.2
+Version: 0.3
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.2/setup.cfg` & `async_etcd3gw-0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.3/tests/test_async_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.2/tests/test_client.py` & `async_etcd3gw-0.3/tests/test_client.py`

 * *Files identical despite different names*

