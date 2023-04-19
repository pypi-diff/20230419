# Comparing `tmp/aiomonitor-ng-0.7.1.tar.gz` & `tmp/aiomonitor-ng-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomonitor-ng-0.7.1.tar", last modified: Sun Apr 16 12:14:52 2023, max compression
+gzip compressed data, was "aiomonitor-ng-0.7.2.tar", last modified: Wed Apr 19 19:06:44 2023, max compression
```

## Comparing `aiomonitor-ng-0.7.1.tar` & `aiomonitor-ng-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192699 aiomonitor-ng-0.7.1/
--rw-r--r--   0 joongi     (501) staff       (20)    11311 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.1/LICENSE
--rw-r--r--   0 joongi     (501) staff       (20)       99 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.1/MANIFEST.in
--rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-16 12:14:52.192547 aiomonitor-ng-0.7.1/PKG-INFO
--rw-r--r--   0 joongi     (501) staff       (20)     5706 2022-10-19 08:55:38.000000 aiomonitor-ng-0.7.1/README.rst
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.191676 aiomonitor-ng-0.7.1/aiomonitor/
--rw-r--r--   0 joongi     (501) staff       (20)      822 2023-04-16 12:11:12.000000 aiomonitor-ng-0.7.1/aiomonitor/__init__.py
--rw-r--r--   0 joongi     (501) staff       (20)      955 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.1/aiomonitor/cli.py
--rw-r--r--   0 joongi     (501) staff       (20)     4818 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.1/aiomonitor/console.py
--rw-r--r--   0 joongi     (501) staff       (20)    31248 2023-04-16 08:39:53.000000 aiomonitor-ng-0.7.1/aiomonitor/monitor.py
--rw-r--r--   0 joongi     (501) staff       (20)     3488 2022-10-19 09:10:28.000000 aiomonitor-ng-0.7.1/aiomonitor/task.py
--rw-r--r--   0 joongi     (501) staff       (20)     9250 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.1/aiomonitor/telnet.py
--rw-r--r--   0 joongi     (501) staff       (20)      556 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.1/aiomonitor/types.py
--rw-r--r--   0 joongi     (501) staff       (20)     7894 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.1/aiomonitor/utils.py
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192247 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/
--rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/PKG-INFO
--rw-r--r--   0 joongi     (501) staff       (20)      425 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/SOURCES.txt
--rw-r--r--   0 joongi     (501) staff       (20)        1 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/dependency_links.txt
--rw-r--r--   0 joongi     (501) staff       (20)       99 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/requires.txt
--rw-r--r--   0 joongi     (501) staff       (20)       11 2023-04-16 12:14:52.000000 aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/top_level.txt
--rw-r--r--   0 joongi     (501) staff       (20)      122 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.1/pyproject.toml
--rw-r--r--   0 joongi     (501) staff       (20)       38 2023-04-16 12:14:52.192735 aiomonitor-ng-0.7.1/setup.cfg
--rw-r--r--   0 joongi     (501) staff       (20)     1991 2022-10-19 09:00:47.000000 aiomonitor-ng-0.7.1/setup.py
-drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-16 12:14:52.192366 aiomonitor-ng-0.7.1/tests/
--rw-r--r--   0 joongi     (501) staff       (20)     5676 2023-04-16 08:39:53.000000 aiomonitor-ng-0.7.1/tests/test_monitor.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-19 19:06:44.024850 aiomonitor-ng-0.7.2/
+-rw-r--r--   0 joongi     (501) staff       (20)    11311 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.2/LICENSE
+-rw-r--r--   0 joongi     (501) staff       (20)       99 2022-08-25 07:44:15.000000 aiomonitor-ng-0.7.2/MANIFEST.in
+-rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-19 19:06:44.024641 aiomonitor-ng-0.7.2/PKG-INFO
+-rw-r--r--   0 joongi     (501) staff       (20)     5706 2022-10-19 08:55:38.000000 aiomonitor-ng-0.7.2/README.rst
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-19 19:06:44.023760 aiomonitor-ng-0.7.2/aiomonitor/
+-rw-r--r--   0 joongi     (501) staff       (20)      822 2023-04-19 19:06:12.000000 aiomonitor-ng-0.7.2/aiomonitor/__init__.py
+-rw-r--r--   0 joongi     (501) staff       (20)      955 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.2/aiomonitor/cli.py
+-rw-r--r--   0 joongi     (501) staff       (20)     4818 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.2/aiomonitor/console.py
+-rw-r--r--   0 joongi     (501) staff       (20)    31248 2023-04-16 08:39:53.000000 aiomonitor-ng-0.7.2/aiomonitor/monitor.py
+-rw-r--r--   0 joongi     (501) staff       (20)     3561 2023-04-19 19:03:26.000000 aiomonitor-ng-0.7.2/aiomonitor/task.py
+-rw-r--r--   0 joongi     (501) staff       (20)     9250 2022-09-25 16:39:01.000000 aiomonitor-ng-0.7.2/aiomonitor/telnet.py
+-rw-r--r--   0 joongi     (501) staff       (20)      556 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.2/aiomonitor/types.py
+-rw-r--r--   0 joongi     (501) staff       (20)     7894 2022-10-19 08:27:30.000000 aiomonitor-ng-0.7.2/aiomonitor/utils.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-19 19:06:44.024345 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/
+-rw-r--r--   0 joongi     (501) staff       (20)     9393 2023-04-19 19:06:43.000000 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/PKG-INFO
+-rw-r--r--   0 joongi     (501) staff       (20)      425 2023-04-19 19:06:44.000000 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 joongi     (501) staff       (20)        1 2023-04-19 19:06:43.000000 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 joongi     (501) staff       (20)       99 2023-04-19 19:06:43.000000 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/requires.txt
+-rw-r--r--   0 joongi     (501) staff       (20)       11 2023-04-19 19:06:43.000000 aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/top_level.txt
+-rw-r--r--   0 joongi     (501) staff       (20)      122 2022-09-23 09:34:54.000000 aiomonitor-ng-0.7.2/pyproject.toml
+-rw-r--r--   0 joongi     (501) staff       (20)       38 2023-04-19 19:06:44.024887 aiomonitor-ng-0.7.2/setup.cfg
+-rw-r--r--   0 joongi     (501) staff       (20)     1991 2022-10-19 09:00:47.000000 aiomonitor-ng-0.7.2/setup.py
+drwxr-xr-x   0 joongi     (501) staff       (20)        0 2023-04-19 19:06:44.024466 aiomonitor-ng-0.7.2/tests/
+-rw-r--r--   0 joongi     (501) staff       (20)     6286 2023-04-19 19:03:26.000000 aiomonitor-ng-0.7.2/tests/test_monitor.py
```

### Comparing `aiomonitor-ng-0.7.1/LICENSE` & `aiomonitor-ng-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/PKG-INFO` & `aiomonitor-ng-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonitor-ng
-Version: 0.7.1
+Version: 0.7.2
 Summary: aiomonitor-ng adds monitor and python REPL capabilities for asyncio application
 Home-page: https://github.com/achimnol/aiomonitor-ng
 Download-URL: https://pypi.python.org/pypi/aiomonitor-ng
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache 2
 Platform: POSIX
```

### Comparing `aiomonitor-ng-0.7.1/README.rst` & `aiomonitor-ng-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/__init__.py` & `aiomonitor-ng-0.7.2/aiomonitor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "Monitor",
     "monitor_cli",
     "start_monitor",
     "MONITOR_HOST",
     "MONITOR_PORT",
     "CONSOLE_PORT",
 )
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/cli.py` & `aiomonitor-ng-0.7.2/aiomonitor/cli.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/console.py` & `aiomonitor-ng-0.7.2/aiomonitor/console.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/monitor.py` & `aiomonitor-ng-0.7.2/aiomonitor/monitor.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/task.py` & `aiomonitor-ng-0.7.2/aiomonitor/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self,
         *args,
         termination_info_queue: janus._SyncQueueProxy[TerminatedTaskInfo],
         cancellation_chain_queue: janus._SyncQueueProxy[CancellationChain],
         persistent: bool = False,
         **kwargs,
     ) -> None:
+        if sys.version_info < (3, 11):
+            kwargs.pop("context")
         super().__init__(*args, **kwargs)
         self._termination_info_queue = termination_info_queue
         self._cancellation_chain_queue = cancellation_chain_queue
         self._started_at = time.perf_counter()
         self._termination_stack = None
         self.add_done_callback(self._trace_termination)
         self._persistent = persistent
```

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/telnet.py` & `aiomonitor-ng-0.7.2/aiomonitor/telnet.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/types.py` & `aiomonitor-ng-0.7.2/aiomonitor/types.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor/utils.py` & `aiomonitor-ng-0.7.2/aiomonitor/utils.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/aiomonitor_ng.egg-info/PKG-INFO` & `aiomonitor-ng-0.7.2/aiomonitor_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonitor-ng
-Version: 0.7.1
+Version: 0.7.2
 Summary: aiomonitor-ng adds monitor and python REPL capabilities for asyncio application
 Home-page: https://github.com/achimnol/aiomonitor-ng
 Download-URL: https://pypi.python.org/pypi/aiomonitor-ng
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache 2
 Platform: POSIX
```

### Comparing `aiomonitor-ng-0.7.1/setup.py` & `aiomonitor-ng-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `aiomonitor-ng-0.7.1/tests/test_monitor.py` & `aiomonitor-ng-0.7.2/tests/test_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import contextvars
+import sys
 import telnetlib
 import threading
 import time
 
 import pytest
 
 from aiomonitor import Monitor, start_monitor
@@ -143,14 +144,34 @@
     assert "No task 123" in resp
 
 
 myvar = contextvars.ContextVar("myvar", default=42)
 
 
 def test_monitor_task_factory():
+    async def do():
+        await asyncio.sleep(0)
+        myself = asyncio.current_task()
+        assert myself is not None
+        assert myself.get_name() == "mytask"
+
+    async def main():
+        loop = asyncio.get_running_loop()
+        with Monitor(loop, console_enabled=False, hook_task_factory=True):
+            t = asyncio.create_task(do(), name="mytask")
+            await t
+
+    asyncio.run(main())
+
+
+@pytest.mark.skipif(
+    sys.version_info < (3, 11),
+    reason="The context argument of asyncio.create_task() is added in Python 3.11",
+)
+def test_monitor_task_factory_with_context():
     ctx = contextvars.Context()
     # This context is bound at the outermost scope,
     # and inside it the initial value of myvar is kept intact.
 
     async def do():
         await asyncio.sleep(0)
         assert myvar.get() == 42  # we are referring the outer context
```

