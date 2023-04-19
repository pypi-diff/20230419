# Comparing `tmp/pool_cue-1.0.0.tar.gz` & `tmp/pool_cue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pool_cue-1.0.0.tar", max compression
+gzip compressed data, was "pool_cue-1.0.1.tar", max compression
```

## Comparing `pool_cue-1.0.0.tar` & `pool_cue-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-04-18 12:09:34.056959 pool_cue-1.0.0/LICENSE
--rw-r--r--   0        0        0     1416 2023-04-18 12:09:34.056959 pool_cue-1.0.0/README.md
--rw-r--r--   0        0        0      284 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/__init__.py
--rw-r--r--   0        0        0      952 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/config.py
--rw-r--r--   0        0        0      158 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/exceptions.py
--rw-r--r--   0        0        0     5093 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/queue.py
--rw-r--r--   0        0        0      426 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/serializers.py
--rw-r--r--   0        0        0     2358 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/tasks.py
--rw-r--r--   0        0        0     4633 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pool_cue/worker.py
--rw-r--r--   0        0        0      666 2023-04-18 12:09:34.056959 pool_cue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 pool_cue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-19 13:28:07.967658 pool_cue-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1416 2023-04-19 13:28:07.967658 pool_cue-1.0.1/README.md
+-rw-r--r--   0        0        0      309 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/config.py
+-rw-r--r--   0        0        0     1053 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/context.py
+-rw-r--r--   0        0        0      158 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/exceptions.py
+-rw-r--r--   0        0        0     5808 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/jobs.py
+-rw-r--r--   0        0        0     3472 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/queue.py
+-rw-r--r--   0        0        0      426 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/serializers.py
+-rw-r--r--   0        0        0     2358 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/threading.py
+-rw-r--r--   0        0        0      968 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/typing.py
+-rw-r--r--   0        0        0      984 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/utils.py
+-rw-r--r--   0        0        0     3967 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/worker.py
+-rw-r--r--   0        0        0      666 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 pool_cue-1.0.1/PKG-INFO
```

### Comparing `pool_cue-1.0.0/LICENSE` & `pool_cue-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.0/README.md` & `pool_cue-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.0/pool_cue/config.py` & `pool_cue-1.0.1/pool_cue/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .serializers import serializer, deserializer
 
 
 @dataclass
 class QueueSettings:
     """Settings class used to hold configuration used by the worker(s) and for communicating with the queue."""
 
-    redis_host: str = "127.0.0.1"
+    redis_host: str
     redis_port: int = 6379
     redis_username: str | None = None
     redis_password: str | None = None
 
     queue_name: str = "pool:queue"
     health_check_key: str = "pool:queue:health"
```

### Comparing `pool_cue-1.0.0/pool_cue/tasks.py` & `pool_cue-1.0.1/pool_cue/threading.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import asyncio
 import functools
 import threading
 import logging
 from typing import Callable, Coroutine
 from concurrent.futures import ThreadPoolExecutor
 
-
-from .worker import Context
+from .context import Context
 
 logger: logging.Logger = logging.getLogger(name="pool_cue")
 
 THREAD_POOL_EVENT_LOOPS: dict[int, asyncio.AbstractEventLoop] = {}
 
 
 def _run_coro_in_thread_pool(coro: Callable, *args, **kwargs) -> None:
```

### Comparing `pool_cue-1.0.0/pool_cue/worker.py` & `pool_cue-1.0.1/pool_cue/worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,38 @@
 from __future__ import annotations
 
-__all__ = ["Context", "WorkerSettings", "create_worker"]
+__all__ = ["WorkerSettings", "create_worker"]
 
 import logging
 import datetime
-from typing import TypedDict, Sequence, Type, Any
+from typing import Sequence, Type, Any
 from types import ModuleType
-from inspect import getmembers, isfunction
-from concurrent.futures import ThreadPoolExecutor
 from arq.worker import Worker, Function
 from arq.typing import WorkerCoroutine, StartupShutdown, SecondsTimedelta
 from arq.jobs import Serializer, Deserializer
 from arq.cron import CronJob
 from arq.connections import RedisSettings, ArqRedis
 
 from .config import QueueSettings
+from .context import Context, init_context, close_context
+from .utils import get_tasks
 
 logger: logging.Logger = logging.getLogger(name="pool_cue")
 
 WorkerSettings = Type[Worker]
 
 
-class Context(TypedDict):
-    redis: ArqRedis
-    job_id: str
-    job_try: int
-    enqueue_time: datetime.datetime
-    score: float
-    pool: ThreadPoolExecutor
-
-
-def _get_tasks(modules: ModuleType | Sequence[ModuleType]) -> Sequence[Function | WorkerCoroutine]:
-    """
-    Returns every callable from the given module (or list of modules).
-    """
-    return (
-        [func for module in modules for _, func in getmembers(module, isfunction)]
-        if isinstance(modules, list)
-        else [func for _, func in getmembers(modules, isfunction)]
-    )
-
-
-async def _on_startup(ctx: Context) -> None:
+async def on_startup(ctx: Context) -> Context:
     """Initialize a new thread pool executor in the worker context."""
-    ctx["pool"] = ThreadPoolExecutor(thread_name_prefix="SubThread", max_workers=None)
+    return await init_context(ctx=ctx)
 
 
-async def _on_shutdown(ctx: Context) -> None:
+async def on_shutdown(ctx: Context) -> None:
     """Shut down the thread pool executor in the worker context."""
-    pool: ThreadPoolExecutor = ctx["pool"]
-    pool.shutdown()
+    await close_context(ctx=ctx)
 
 
 def create_worker(
     settings: QueueSettings,
     tasks: ModuleType | Sequence[ModuleType],
     **kwargs,
 ) -> WorkerSettings:
@@ -70,22 +49,22 @@
 
     :param settings: Queue settings.
     :param tasks: Module(s) containing task functions to register.
     :param kwargs: Extra worker settings, see `arq.worker.Worker` for details.
     """
 
     class Settings(Worker):
-        functions: Sequence[Function | WorkerCoroutine] = _get_tasks(modules=tasks)
+        functions: Sequence[Function | WorkerCoroutine] = get_tasks(modules=tasks)
         queue_name: str = kwargs.get("queue_name", settings.queue_name)
         cron_jobs: Sequence[CronJob] | None = kwargs.get("cron_jobs", None)
         redis_settings: RedisSettings = kwargs.get("redis_settings", settings.redis_settings)
         redis_pool: ArqRedis | None = kwargs.get("redis_pool", None)
         burst: bool = kwargs.get("burst", False)
-        on_startup: StartupShutdown | None = kwargs.get("on_startup", _on_startup)
-        on_shutdown: StartupShutdown | None = kwargs.get("on_shutdown", _on_shutdown)
+        on_startup: StartupShutdown | None = kwargs.get("on_startup", on_startup)
+        on_shutdown: StartupShutdown | None = kwargs.get("on_shutdown", on_shutdown)
         on_job_start: StartupShutdown | None = kwargs.get("on_job_start", None)
         on_job_end: StartupShutdown | None = kwargs.get("on_job_end", None)
         after_job_end: StartupShutdown | None = kwargs.get("after_job_end", None)
         handle_signals: bool = kwargs.get("handle_signals", True)
         job_completion_wait: int = kwargs.get("job_completion_wait", 0)
         max_jobs: int = kwargs.get("max_jobs", 20)
         job_timeout: SecondsTimedelta = kwargs.get("job_timeout", 300)
```

### Comparing `pool_cue-1.0.0/pyproject.toml` & `pool_cue-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pool-cue"
-version = "1.0.0"
+version = "1.0.1"
 description = "Tools for working with arq job queues"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/skarre-r/pool-cue"
 packages = [
     { include = "pool_cue" }
 ]
```

### Comparing `pool_cue-1.0.0/PKG-INFO` & `pool_cue-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pool-cue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for working with arq job queues
 Home-page: https://github.com/skarre-r/pool-cue
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

