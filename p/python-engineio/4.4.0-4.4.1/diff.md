# Comparing `tmp/python-engineio-4.4.0.tar.gz` & `tmp/python-engineio-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-engineio-4.4.0.tar", last modified: Thu Mar 16 20:05:38 2023, max compression
+gzip compressed data, was "python-engineio-4.4.1.tar", last modified: Wed Apr 19 15:21:32 2023, max compression
```

## Comparing `python-engineio-4.4.0.tar` & `python-engineio-4.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-16 20:05:38.248035 python-engineio-4.4.0/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:17:59.000000 python-engineio-4.4.0/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:17:59.000000 python-engineio-4.4.0/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-03-16 20:05:38.248327 python-engineio-4.4.0/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1288 2021-06-03 19:08:45.000000 python-engineio-4.4.0/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1012 2021-02-22 00:17:35.000000 python-engineio-4.4.0/README.rst
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-07 19:39:18.000000 python-engineio-4.4.0/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      920 2023-03-16 20:05:38.250126 python-engineio-4.4.0/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-21 22:23:41.000000 python-engineio-4.4.0/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-16 20:05:38.212521 python-engineio-4.4.0/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-16 20:05:38.229379 python-engineio-4.4.0/src/engineio/
--rw-r--r--   0 mgrinberg   (502) staff       (20)      748 2021-11-30 15:30:22.000000 python-engineio-4.4.0/src/engineio/__init__.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-16 20:05:38.240641 python-engineio-4.4.0/src/engineio/async_drivers/
--rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2019-11-17 19:17:59.000000 python-engineio-4.4.0/src/engineio/async_drivers/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3746 2021-02-22 00:17:35.000000 python-engineio-4.4.0/src/engineio/async_drivers/aiohttp.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10181 2022-08-02 18:37:30.000000 python-engineio-4.4.0/src/engineio/async_drivers/asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      981 2019-11-17 19:17:59.000000 python-engineio-4.4.0/src/engineio/async_drivers/eventlet.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1803 2019-11-17 19:17:59.000000 python-engineio-4.4.0/src/engineio/async_drivers/gevent.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5912 2023-02-02 11:35:37.000000 python-engineio-4.4.0/src/engineio/async_drivers/gevent_uwsgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4468 2022-01-04 23:17:35.000000 python-engineio-4.4.0/src/engineio/async_drivers/sanic.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1158 2021-04-18 19:13:36.000000 python-engineio-4.4.0/src/engineio/async_drivers/threading.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5901 2021-02-22 00:17:35.000000 python-engineio-4.4.0/src/engineio/async_drivers/tornado.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    27031 2023-02-11 12:17:10.000000 python-engineio-4.4.0/src/engineio/asyncio_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    22691 2023-03-16 20:03:22.000000 python-engineio-4.4.0/src/engineio/asyncio_server.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10248 2021-11-14 13:11:24.000000 python-engineio-4.4.0/src/engineio/asyncio_socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    30107 2023-02-07 11:49:25.000000 python-engineio-4.4.0/src/engineio/client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      292 2019-11-17 19:17:59.000000 python-engineio-4.4.0/src/engineio/exceptions.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      405 2021-04-14 23:00:40.000000 python-engineio-4.4.0/src/engineio/json.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3823 2021-07-26 22:32:50.000000 python-engineio-4.4.0/src/engineio/middleware.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2884 2022-05-29 14:42:07.000000 python-engineio-4.4.0/src/engineio/packet.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1547 2021-02-22 00:17:35.000000 python-engineio-4.4.0/src/engineio/payload.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    33757 2023-03-16 20:03:22.000000 python-engineio-4.4.0/src/engineio/server.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10299 2021-11-14 13:11:24.000000 python-engineio-4.4.0/src/engineio/socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2064 2021-05-02 23:23:10.000000 python-engineio-4.4.0/src/engineio/static_files.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-16 20:05:38.247199 python-engineio-4.4.0/src/python_engineio.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-03-16 20:05:38.000000 python-engineio-4.4.0/src/python_engineio.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1013 2023-03-16 20:05:38.000000 python-engineio-4.4.0/src/python_engineio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-03-16 20:05:38.000000 python-engineio-4.4.0/src/python_engineio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:44:43.000000 python-engineio-4.4.0/src/python_engineio.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       83 2023-03-16 20:05:38.000000 python-engineio-4.4.0/src/python_engineio.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        9 2023-03-16 20:05:38.000000 python-engineio-4.4.0/src/python_engineio.egg-info/top_level.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.148364 python-engineio-4.4.1/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:17:59.000000 python-engineio-4.4.1/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:17:59.000000 python-engineio-4.4.1/MANIFEST.in
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-04-19 15:21:32.148601 python-engineio-4.4.1/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1288 2021-06-03 19:08:45.000000 python-engineio-4.4.1/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1012 2021-02-22 00:17:35.000000 python-engineio-4.4.1/README.rst
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-07 19:39:18.000000 python-engineio-4.4.1/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      920 2023-04-19 15:21:32.149724 python-engineio-4.4.1/setup.cfg
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-21 22:23:41.000000 python-engineio-4.4.1/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.112815 python-engineio-4.4.1/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.131685 python-engineio-4.4.1/src/engineio/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      748 2021-11-30 15:30:22.000000 python-engineio-4.4.1/src/engineio/__init__.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.142337 python-engineio-4.4.1/src/engineio/async_drivers/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/async_drivers/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3746 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/aiohttp.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10181 2022-08-02 18:37:30.000000 python-engineio-4.4.1/src/engineio/async_drivers/asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      981 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/async_drivers/eventlet.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1803 2023-03-21 23:31:31.000000 python-engineio-4.4.1/src/engineio/async_drivers/gevent.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5912 2023-02-02 11:35:37.000000 python-engineio-4.4.1/src/engineio/async_drivers/gevent_uwsgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4468 2022-01-04 23:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/sanic.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1154 2023-03-21 23:31:12.000000 python-engineio-4.4.1/src/engineio/async_drivers/threading.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5901 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/async_drivers/tornado.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    27033 2023-04-14 11:54:46.000000 python-engineio-4.4.1/src/engineio/asyncio_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    22691 2023-03-16 20:03:22.000000 python-engineio-4.4.1/src/engineio/asyncio_server.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10248 2021-11-14 13:11:24.000000 python-engineio-4.4.1/src/engineio/asyncio_socket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    30109 2023-04-14 11:54:46.000000 python-engineio-4.4.1/src/engineio/client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      292 2019-11-17 19:17:59.000000 python-engineio-4.4.1/src/engineio/exceptions.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      405 2021-04-14 23:00:40.000000 python-engineio-4.4.1/src/engineio/json.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3823 2021-07-26 22:32:50.000000 python-engineio-4.4.1/src/engineio/middleware.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2884 2022-05-29 14:42:07.000000 python-engineio-4.4.1/src/engineio/packet.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1547 2021-02-22 00:17:35.000000 python-engineio-4.4.1/src/engineio/payload.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    33757 2023-03-16 20:03:22.000000 python-engineio-4.4.1/src/engineio/server.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10299 2021-11-14 13:11:24.000000 python-engineio-4.4.1/src/engineio/socket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2064 2021-05-02 23:23:10.000000 python-engineio-4.4.1/src/engineio/static_files.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-19 15:21:32.147822 python-engineio-4.4.1/src/python_engineio.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1976 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1013 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:44:43.000000 python-engineio-4.4.1/src/python_engineio.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       83 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        9 2023-04-19 15:21:32.000000 python-engineio-4.4.1/src/python_engineio.egg-info/top_level.txt
```

### Comparing `python-engineio-4.4.0/LICENSE` & `python-engineio-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/PKG-INFO` & `python-engineio-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.4.0
+Version: 4.4.1
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python-engineio-4.4.0/README.md` & `python-engineio-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/README.rst` & `python-engineio-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/setup.cfg` & `python-engineio-4.4.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-engineio
-version = 4.4.0
+version = 4.4.1
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Engine.IO server and client for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/python-engineio
 project_urls =
```

### Comparing `python-engineio-4.4.0/src/engineio/__init__.py` & `python-engineio-4.4.1/src/engineio/__init__.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/aiohttp.py` & `python-engineio-4.4.1/src/engineio/async_drivers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/asgi.py` & `python-engineio-4.4.1/src/engineio/async_drivers/asgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/eventlet.py` & `python-engineio-4.4.1/src/engineio/async_drivers/eventlet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/gevent.py` & `python-engineio-4.4.1/src/engineio/async_drivers/gevent.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/gevent_uwsgi.py` & `python-engineio-4.4.1/src/engineio/async_drivers/gevent_uwsgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/sanic.py` & `python-engineio-4.4.1/src/engineio/async_drivers/sanic.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/threading.py` & `python-engineio-4.4.1/src/engineio/async_drivers/threading.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         except ConnectionClosed:
             raise IOError()
 
     def wait(self):
         try:
             return self.ws.receive()
         except ConnectionClosed:
-            raise IOError()
+            return None
 
 
 _async = {
     'thread': threading.Thread,
     'queue': queue.Queue,
     'queue_empty': queue.Empty,
     'event': threading.Event,
```

### Comparing `python-engineio-4.4.0/src/engineio/async_drivers/tornado.py` & `python-engineio-4.4.1/src/engineio/async_drivers/tornado.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/asyncio_client.py` & `python-engineio-4.4.1/src/engineio/asyncio_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,17 @@
 
         Note: this method is a coroutine.
         """
         if self.read_loop_task:
             await self.read_loop_task
 
     async def send(self, data):
-        """Send a message to a client.
+        """Send a message to the server.
 
-        :param data: The data to send to the client. Data can be of type
+        :param data: The data to send to the server. Data can be of type
                      ``str``, ``bytes``, ``list`` or ``dict``. If a ``list``
                      or ``dict``, the data will be serialized as JSON.
 
         Note: this method is a coroutine.
         """
         await self._send_packet(packet.Packet(packet.MESSAGE, data=data))
```

### Comparing `python-engineio-4.4.0/src/engineio/asyncio_server.py` & `python-engineio-4.4.1/src/engineio/asyncio_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/asyncio_socket.py` & `python-engineio-4.4.1/src/engineio/asyncio_socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/client.py` & `python-engineio-4.4.1/src/engineio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,17 +197,17 @@
         Client applications can use this function to block the main thread
         during the life of the connection.
         """
         if self.read_loop_task:
             self.read_loop_task.join()
 
     def send(self, data):
-        """Send a message to a client.
+        """Send a message to the server.
 
-        :param data: The data to send to the client. Data can be of type
+        :param data: The data to send to the server. Data can be of type
                      ``str``, ``bytes``, ``list`` or ``dict``. If a ``list``
                      or ``dict``, the data will be serialized as JSON.
         """
         self._send_packet(packet.Packet(packet.MESSAGE, data=data))
 
     def disconnect(self, abort=False):
         """Disconnect from the server.
```

### Comparing `python-engineio-4.4.0/src/engineio/middleware.py` & `python-engineio-4.4.1/src/engineio/middleware.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/packet.py` & `python-engineio-4.4.1/src/engineio/packet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/payload.py` & `python-engineio-4.4.1/src/engineio/payload.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/server.py` & `python-engineio-4.4.1/src/engineio/server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/socket.py` & `python-engineio-4.4.1/src/engineio/socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/engineio/static_files.py` & `python-engineio-4.4.1/src/engineio/static_files.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.4.0/src/python_engineio.egg-info/PKG-INFO` & `python-engineio-4.4.1/src/python_engineio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.4.0
+Version: 4.4.1
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python-engineio-4.4.0/src/python_engineio.egg-info/SOURCES.txt` & `python-engineio-4.4.1/src/python_engineio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

