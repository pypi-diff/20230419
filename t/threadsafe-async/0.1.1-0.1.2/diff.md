# Comparing `tmp/threadsafe-async-0.1.1.tar.gz` & `tmp/threadsafe-async-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe-async-0.1.1.tar", last modified: Wed Apr 19 16:06:15 2023, max compression
+gzip compressed data, was "threadsafe-async-0.1.2.tar", last modified: Wed Apr 19 19:11:38 2023, max compression
```

## Comparing `threadsafe-async-0.1.1.tar` & `threadsafe-async-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.448353 threadsafe-async-0.1.1/
--rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.1.1/LICENSE
--rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 16:06:15.448018 threadsafe-async-0.1.1/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-04-19 15:34:19.000000 threadsafe-async-0.1.1/README.md
--rw-r--r--   0 gleero     (501) staff       (20)     1390 2023-04-19 16:05:43.000000 threadsafe-async-0.1.1/pyproject.toml
--rw-r--r--   0 gleero     (501) staff       (20)       38 2023-04-19 16:06:15.448519 threadsafe-async-0.1.1/setup.cfg
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.443548 threadsafe-async-0.1.1/tests/
--rw-r--r--   0 gleero     (501) staff       (20)     6435 2023-04-18 16:08:11.000000 threadsafe-async-0.1.1/tests/test_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-18 16:08:11.000000 threadsafe-async-0.1.1/tests/test_event.py
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.445459 threadsafe-async-0.1.1/threadsafe_async.egg-info/
--rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)      349 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/SOURCES.txt
--rw-r--r--   0 gleero     (501) staff       (20)        1 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/dependency_links.txt
--rw-r--r--   0 gleero     (501) staff       (20)      163 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/requires.txt
--rw-r--r--   0 gleero     (501) staff       (20)        8 2023-04-19 16:06:15.000000 threadsafe-async-0.1.1/threadsafe_async.egg-info/top_level.txt
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 16:06:15.447649 threadsafe-async-0.1.1/tsasync/
--rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/__init__.py
--rw-r--r--   0 gleero     (501) staff       (20)     2813 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     3719 2023-04-18 16:08:49.000000 threadsafe-async-0.1.1/tsasync/_event.py
--rw-r--r--   0 gleero     (501) staff       (20)      392 2023-04-18 15:51:38.000000 threadsafe-async-0.1.1/tsasync/_utils.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.956094 threadsafe-async-0.1.2/
+-rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.1.2/LICENSE
+-rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 19:11:38.955798 threadsafe-async-0.1.2/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-04-19 15:34:19.000000 threadsafe-async-0.1.2/README.md
+-rw-r--r--   0 gleero     (501) staff       (20)     1415 2023-04-19 19:09:05.000000 threadsafe-async-0.1.2/pyproject.toml
+-rw-r--r--   0 gleero     (501) staff       (20)       38 2023-04-19 19:11:38.956197 threadsafe-async-0.1.2/setup.cfg
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.949518 threadsafe-async-0.1.2/tests/
+-rw-r--r--   0 gleero     (501) staff       (20)     6329 2023-04-19 19:00:13.000000 threadsafe-async-0.1.2/tests/test_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-19 19:06:37.000000 threadsafe-async-0.1.2/tests/test_event.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.952007 threadsafe-async-0.1.2/threadsafe_async.egg-info/
+-rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)      349 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/SOURCES.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        1 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/dependency_links.txt
+-rw-r--r--   0 gleero     (501) staff       (20)      181 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/requires.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        8 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/top_level.txt
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.955058 threadsafe-async-0.1.2/tsasync/
+-rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.1.2/tsasync/__init__.py
+-rw-r--r--   0 gleero     (501) staff       (20)     3089 2023-04-19 19:06:27.000000 threadsafe-async-0.1.2/tsasync/_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     3681 2023-04-19 17:37:59.000000 threadsafe-async-0.1.2/tsasync/_event.py
+-rw-r--r--   0 gleero     (501) staff       (20)      405 2023-04-19 19:05:02.000000 threadsafe-async-0.1.2/tsasync/_utils.py
```

### Comparing `threadsafe-async-0.1.1/LICENSE` & `threadsafe-async-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.1/PKG-INFO` & `threadsafe-async-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.1
+Version: 0.1.2
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `threadsafe-async-0.1.1/README.md` & `threadsafe-async-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.1/pyproject.toml` & `threadsafe-async-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe-async"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Vladimir Perekladov", email = "gleero@gmail.com"},
 ]
 description = "Thread-safe synchronization primitives"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -22,14 +22,15 @@
 dev = [
     "black==23.3.0",
     "flake8==6.0.0",
     "Flake8-pyproject==1.2.3",
     "isort==5.12.0",
     "twine==4.0.2",
     "build==0.10.0",
+    "pre-commit==3.2.2",
 ]
 test = [
     "pytest==7.3.0",
     "pytest-asyncio==0.21.0",
     "pytest-cov==4.0.0",
 ]
 
@@ -44,17 +45,17 @@
 minversion = "7.0"
 testpaths = ["tests"]
 pythonpath = ["."]
 
 [tool.isort]
 src_paths = ["tsasync", "test"]
 profile = "black"
-line_length = 72
+line_length = 88
 include_trailing_comma = "True"
 multi_line_output = 3
 force_grid_wrap = 0
 combine_as_imports = "True"
 lines_after_imports = 2
 
 [tool.flake8]
 exclude = [".git", ".venv", ".idea", ".pytest_cache", "__pycache__"]
-max-line-length = 72
+max-line-length = 88
```

### Comparing `threadsafe-async-0.1.1/tests/test_channel.py` & `threadsafe-async-0.1.2/tests/test_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,17 +75,15 @@
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_many_mixed_senders():
     channel = Channel[Optional[int]]()
     senders_coro = []
     senders_threads = []
     for x in range(5):
-        senders_coro.append(
-            asyncio.create_task(asender(channel, [1, 2]))
-        )
+        senders_coro.append(asyncio.create_task(asender(channel, [1, 2])))
         t = PropagatingThread(target=ssender, args=(channel, [3, 4]))
         t.start()
         senders_threads.append(t)
 
     result = []
     cnt = 0
     while True:
@@ -158,78 +156,66 @@
     await sender_task
     result = await receiver_task
     assert result == [1, 2, 3, 4, 5]
 
 
 def test_channel_between_two_threads():
     channel = Channel[Optional[int]]()
-    sender_thread = PropagatingThread(
-        target=ssender, args=(channel, [1, 2, 3, 4, 5])
-    )
+    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
     sender_thread.start()
-    receiver_thread = PropagatingThread(
-        target=sreceiver, args=(channel,)
-    )
+    receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     sender_thread.join()
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
 
 
 def test_channel_between_sync_and_thread_sender():
     channel = Channel[Optional[int]]()
     result = []
-    sender_thread = PropagatingThread(
-        target=ssender, args=(channel, [1, 2, 3, 4, 5])
-    )
+    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
     sender_thread.start()
     while True:
         item = channel.receive()
         if item is None:
             break
         result.append(item)
     sender_thread.join()
     assert result == [1, 2, 3, 4, 5]
 
 
 def test_channel_between_sync_and_thread_receiver():
     channel = Channel[Optional[int]]()
-    receiver_thread = PropagatingThread(
-        target=sreceiver, args=(channel,)
-    )
+    receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     for item in [1, 2, 3, 4, 5]:
         channel.send(item)
     channel.send(None)
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_thread_sender():
     channel = Channel[Optional[int]]()
     result = []
-    sender_thread = PropagatingThread(
-        target=ssender, args=(channel, [1, 2, 3, 4, 5])
-    )
+    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
     sender_thread.start()
     while True:
         item = await channel.receive()
         if item is None:
             break
         result.append(item)
     sender_thread.join()
     assert result == [1, 2, 3, 4, 5]
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_thread_receiver():
     channel = Channel[Optional[int]]()
-    receiver_thread = PropagatingThread(
-        target=sreceiver, args=(channel,)
-    )
+    receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     for item in [1, 2, 3, 4, 5]:
         await channel.send(item)
     await channel.send(None)
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
```

### Comparing `threadsafe-async-0.1.1/tests/test_event.py` & `threadsafe-async-0.1.2/tests/test_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,15 @@
         me.set()
         me.wait()
         assert e.wait() is True
         assert e.is_set() is True
 
     mgm_event = threading.Event()
     event = Event()
-    thread = PropagatingThread(
-        target=wait_event_thread, args=(event, mgm_event)
-    )
+    thread = PropagatingThread(target=wait_event_thread, args=(event, mgm_event))
     thread.start()
     mgm_event.wait()
     mgm_event.clear()
     mgm_event.set()
     event.set()
     thread.join()
 
@@ -141,20 +139,19 @@
 
         assert e.is_set() is False
         me.set()
         me.wait()
         loop = asyncio.new_event_loop()
         loop.run_until_complete(async_wait(e))
         assert e.is_set() is True
+        loop.close()
 
     mgm_event = threading.Event()
     event = Event()
-    thread = PropagatingThread(
-        target=wait_event_thread, args=(event, mgm_event)
-    )
+    thread = PropagatingThread(target=wait_event_thread, args=(event, mgm_event))
     thread.start()
     mgm_event.wait()
     mgm_event.clear()
     mgm_event.set()
     event.set()
     thread.join()
 
@@ -167,20 +164,19 @@
 
         loop = asyncio.new_event_loop()
         assert e.is_set() is False
         me.set()
         me.wait()
         loop.run_until_complete(async_wait(e))
         assert e.is_set() is True
+        loop.close()
 
     mgm_event = threading.Event()
     event = Event()
-    thread = PropagatingThread(
-        target=wait_event_thread, args=(event, mgm_event)
-    )
+    thread = PropagatingThread(target=wait_event_thread, args=(event, mgm_event))
     thread.start()
     mgm_event.wait()
     mgm_event.clear()
     mgm_event.set()
     event.set()
     thread.join()
     assert event.loop != asyncio.get_event_loop()
```

### Comparing `threadsafe-async-0.1.1/threadsafe_async.egg-info/PKG-INFO` & `threadsafe-async-0.1.2/threadsafe_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.1
+Version: 0.1.2
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `threadsafe-async-0.1.1/tsasync/_channel.py` & `threadsafe-async-0.1.2/tsasync/_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import inspect
 import threading
 from collections import deque
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Awaitable, Deque, Generic, Union
+from typing import Any, Awaitable, Deque, Generic, Optional, Union
 
 from ._event import Event
 from ._utils import T, in_loop, wrapret
 
 
 class ChannelState(Enum):
     IDLE = 1
 
 
 @dataclass
 class OperationContext:
     event: Event
     value: Any
+    destination: Optional[Event] = None
 
 
 class Channel(Generic[T]):
     _ts_lock: threading.RLock
     _queue: Deque[OperationContext]
     _waiters: Deque[Event]
     _max_size: int
@@ -49,14 +50,15 @@
 
             # Put item to the queue
             self._queue.append(ctx)
 
             # Unlock for waiter in needed
             try:
                 event = self._waiters.popleft()
+                ctx.destination = event
                 event.set()
             except IndexError:
                 pass
 
         # Return awaitable object if in loop
         if in_loop():
             waiter = ctx.event.wait()
@@ -70,41 +72,43 @@
 
     def receive(self) -> Union[T, Awaitable[T]]:
         """
         Get item from the queue
         """
         with self._ts_lock:
             # Queue has pending objects, return it immediately
-            if len(self._queue) > 0:
+            if len(self._queue) > 0 and len(self._waiters) == 0:
                 return wrapret(self._next_item())
 
             # Create event and wait for data
             event = Event()
             self._waiters.append(event)
 
         # Wait for event
         if in_loop():
             return self._areceive(event)
 
         # Get item from the queue
         event.wait()
         with self._ts_lock:
-            return self._next_item()
+            return self._next_item(event)
 
     async def _areceive(self, event: Event) -> T:
         """
         Receive item asynchronly
         :param event: event instance
         """
         waiter = event.wait()
         if inspect.isawaitable(waiter):
             await waiter
         with self._ts_lock:
-            return self._next_item()
+            return self._next_item(event)
 
-    def _next_item(self) -> T:
+    def _next_item(self, event: Optional[Event] = None) -> T:
         """
         Get next item from the queue
         """
         ctx = self._queue.popleft()
+        if ctx.destination is not None:
+            assert ctx.destination == event, f"{ctx.destination} != {event}"
         ctx.event.set()
         return ctx.value
```

### Comparing `threadsafe-async-0.1.1/tsasync/_event.py` & `threadsafe-async-0.1.2/tsasync/_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,15 @@
                     if self._loop != asyncio.get_running_loop():
                         self._loop = None
                         self._async_ev = None
                         self._reinit()
 
             # Prevent for waits in different threads
             if self._wait_thread_id != threading.get_ident():
-                raise RuntimeError(
-                    "Using wait in different threads are not allowed"
-                )
+                raise RuntimeError("Using wait in different threads are not allowed")
 
             # Reinit loop if not exists
             if inloop and self._loop is None:
                 self._reinit()
 
         # Return immediately is set
         if self.is_set():
```

