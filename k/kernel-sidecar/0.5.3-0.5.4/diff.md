# Comparing `tmp/kernel_sidecar-0.5.3.tar.gz` & `tmp/kernel_sidecar-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernel_sidecar-0.5.3.tar", max compression
+gzip compressed data, was "kernel_sidecar-0.5.4.tar", max compression
```

## Comparing `kernel_sidecar-0.5.3.tar` & `kernel_sidecar-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/LICENSE
--rw-r--r--   0        0        0     8256 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/README.md
--rw-r--r--   0        0        0     1089 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/__init__.py
--rw-r--r--   0        0        0     4325 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/actions.py
--rw-r--r--   0        0        0     2678 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/cli.py
--rw-r--r--   0        0        0    24262 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/client.py
--rw-r--r--   0        0        0     5207 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/comms.py
--rw-r--r--   0        0        0        0 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/__init__.py
--rw-r--r--   0        0        0     1054 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/base.py
--rw-r--r--   0        0        0     1580 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/debug.py
--rw-r--r--   0        0        0     5919 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/output.py
--rw-r--r--   0        0        0     4395 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/log_utils.py
--rw-r--r--   0        0        0        0 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/__init__.py
--rw-r--r--   0        0        0    14883 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/messages.py
--rw-r--r--   0        0        0     2334 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/notebook.py
--rw-r--r--   0        0        0     9369 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/models/requests.py
--rw-r--r--   0        0        0     5284 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/nb_builder.py
--rw-r--r--   0        0        0      261 2023-04-17 18:52:56.437956 kernel_sidecar-0.5.3/src/kernel_sidecar/settings.py
--rw-r--r--   0        0        0     9080 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-19 13:33:58.397089 kernel_sidecar-0.5.4/LICENSE
+-rw-r--r--   0        0        0     8256 2023-04-19 13:33:58.397089 kernel_sidecar-0.5.4/README.md
+-rw-r--r--   0        0        0     1089 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/__init__.py
+-rw-r--r--   0        0        0     6079 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/actions.py
+-rw-r--r--   0        0        0     2678 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/cli.py
+-rw-r--r--   0        0        0    24314 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/client.py
+-rw-r--r--   0        0        0     5207 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/comms.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/__init__.py
+-rw-r--r--   0        0        0     1054 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/base.py
+-rw-r--r--   0        0        0     1580 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/debug.py
+-rw-r--r--   0        0        0     5919 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/output.py
+-rw-r--r--   0        0        0     4395 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/log_utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/__init__.py
+-rw-r--r--   0        0        0    14893 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/messages.py
+-rw-r--r--   0        0        0     2334 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/notebook.py
+-rw-r--r--   0        0        0     9389 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/requests.py
+-rw-r--r--   0        0        0     5284 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/nb_builder.py
+-rw-r--r--   0        0        0      261 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/settings.py
+-rw-r--r--   0        0        0     9080 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.4/PKG-INFO
```

### Comparing `kernel_sidecar-0.5.3/LICENSE` & `kernel_sidecar-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/README.md` & `kernel_sidecar-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/pyproject.toml` & `kernel_sidecar-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kernel-sidecar"
-version = "0.5.3"
+version = "0.5.4"
 description = "A sidecar "
 authors = ["Matt Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "kernel_sidecar", from = "src"}]
 repository = "https://github.com/kafonek/kernel-sidecar"
```

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/actions.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/actions.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 idle and for it to emit a specific type of reply based on the request.
 
 Business logic, such as updating a document model state or emitting messages back to a central
 server / frontends, should be implemented in handlers that are attached to each Action.
 """
 import asyncio
 import logging
-from typing import List
+from typing import List, Optional
 
 from kernel_sidecar.handlers.base import Handler
 from kernel_sidecar.models import messages, requests
 
 logger = logging.getLogger(__name__)
 
 REPLY_MSG_TYPES = {
@@ -32,35 +32,36 @@
     "comm_close": None,
 }
 
 
 class KernelAction:
     REPLY_MSG_TYPES = REPLY_MSG_TYPES
 
-    def __init__(self, request: requests.Request, handlers: List[Handler] = None):
+    def __init__(self, request: requests.Request, handlers: Optional[List[Handler]] = None):
         self.request = request
         if request.header.msg_type not in self.REPLY_MSG_TYPES:
             raise ValueError(
                 f"Unrecognized request type {request.header.msg_type}. Raising error because "
                 "the KernelAction would not know when the request-reply cycle is finished. If you "
                 "have a custom request type, add it to KernelAction.REPLY_MSG_TYPES."
             )
         self.expected_reply_msg_type = self.REPLY_MSG_TYPES[request.header.msg_type]
 
         # Events tied to making this instance awaitable
         self.running = False
-        self.kernel_idle = asyncio.Event()
-        self.reply_seen = asyncio.Event()
+        self.kernel_idle = asyncio.Event()  # gets set when kernel status reports idle
+        self.reply_seen = asyncio.Event()  # gets set when we see execute_reply or the like
         self.done = asyncio.Event()
+        self.safety_net_task = None  # see .kernel_idle_safety_net docstring
 
         # Routing messages to handlers
         self.handlers = handlers or []
 
         # Flips to True during kernel.send, and kernel.send won't send anything over ZMQ if the
-        # Action.sent is True. Avoid weird edge cases with routing messages to different Action
+        # Action.sent is True. Avoids weird edge cases with routing messages to different Action
         # instances that might have same request msg_id
         self.sent = False
 
     @property
     def msg_id(self):
         return self.request.header.msg_id
 
@@ -80,28 +81,57 @@
         Set the Action as "done", meaning we've seen all expected replies from the Kernel
          - always wait until Kernel has reported being Idle with our parent header msg id
          - Depending on the request type, also wait for an expected reply type, e.g.
            execute_request isn't "complete" until we get execute_reply
         """
         if self.kernel_idle.is_set():
             if self.reply_seen.is_set() or not self.expected_reply_msg_type:
-                self.done.set()
-                self.running = False
                 for handler in self.handlers:
                     await handler.action_complete()
 
+                self.running = False
+                self.done.set()
+                if self.safety_net_task:
+                    self.safety_net_task.cancel()
+
+    async def kernel_idle_safety_net(self):
+        """
+        Sometimes we just don't see the expected reply, who knows why. It seems most common with
+        execute_reply, especially during tests running in CI but I've seen it happen in prod too.
+        """
+        await asyncio.sleep(3)  # Todo: decide if this needs to be a setting
+        if self.running and self.expected_reply_msg_type:
+            logger.warning(
+                f"Action {self} still running 3 seconds after Kernel went idle. Expected to see "
+                f"{self.expected_reply_msg_type} by now but have not. Setting done anyway."
+            )
+            self.reply_seen.set()
+            await self.maybe_set_done()
+
     async def handle_message(self, msg: messages.Message):
-        """Delegate message to the appropriate handler defined in subclasses"""
+        """
+        Delegate message to the appropriate handler defined in subclasses and try to determine
+        if this Action is "done", meaning the Kernel has cycled from busy to idle and we've seen
+        an expected message reply type (or kicked off a "safety net" task since sometimes we do
+        not see the expected reply, especially for execute_request / execute_reply)
+        """
         # Delegate the message to any attached handlers, in the order they were attached
+        # TODO: consider pros and cons of asyncio.gather handlers instead of awaiting serially
         for handler in self.handlers:
             await handler(msg)
 
         # Checking for status / special reply type in order to maybe set "done"
         if msg.msg_type == "status":
             if msg.content.execution_state == "busy":
                 self.running = True
             elif msg.content.execution_state == "idle":
                 self.kernel_idle.set()
                 await self.maybe_set_done()
+                # Normally shouldn't see kernel go idle before we see the expected reply type
+                # but hence the name, this is a safety net
+                if self.running:
+                    logger.debug(f"Creating safety net task for {self}")
+                    self.safety_net_task = asyncio.create_task(self.kernel_idle_safety_net())
+
         elif msg.msg_type == self.expected_reply_msg_type:
             self.reply_seen.set()
             await self.maybe_set_done()
```

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/cli.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/cli.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/client.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,19 @@
 
         # message queue, raw data (dict) from all zmq channels gets dropped into here
         # and a separate asyncio.Task picks them up off the queue to pass into the
         # right Action for handling callbacks
         self.mq = asyncio.Queue()
 
         # Keep track of tasks to cancel while shutting down
-        self.mq_task: asyncio.Task = None
+        self.is_processing = False  # turns to True entering context manager, False when exiting
+        self.mq_task: asyncio.Task = None  # picks things up off the PriorityQueue to process
+        # One parent task with two child tasks per ZMQ channel:
+        # - watch for zmq disconnect
+        # - pick up zmq messages off socket and drop onto PriorityQueue
         self.channel_watching_tasks: List[asyncio.Task] = []
         self.channel_watcher_parent_tasks: List[asyncio.Task] = []
 
         # Handlers to attach to every Action. These will be appended to action.handlers
         # during .send, which means they'll run /after/ other handlers.
         # Fail right away if there's common mistake of init'ing with default_handlers=Handler()
         if default_handlers and not isinstance(default_handlers, list):
@@ -432,23 +436,17 @@
 
             # Log warning if we think we're seeing responses for a new Action and haven't completed
             # the previously running action, e.g. we start getting status / content responses for
             # a new execute_request when we haven't seen execute_reply / status idle for a previous
             # execute request
             if self.running_action and self.running_action is not action:
                 logger.warning(
-                    f"Observed message for {action} while {self.running_action} has not "
-                    "completed. This is a sign that expected messages didn't come over ZMQ or "
-                    "the Action needs a different expected_reply_msg_type. Setting "
-                    "running_action.done to True to avoid app hanging."
+                    f"Observed message for {action} while {self.running_action} has not finished"
                 )
 
-                self.running_action.done.set()
-                self.running_action.running = False
-
             # Optional timeout for callbacks
             try:
                 await asyncio.wait_for(action.handle_message(msg), timeout=self._handler_timeout)
             except asyncio.CancelledError:
                 logger.warning(f"Timeout handling callbacks for {action}")
                 continue
             except:  # noqa: E722
@@ -506,15 +504,15 @@
         # it briefly and it didn't yield out of the context manager like I expected. Also not sure I
         # want to pin to 3.11+ quite yet.
         for channel in ["iopub", "shell", "control", "stdin"]:
             task = asyncio.create_task(self.watch_channel(channel))
             self.channel_watcher_parent_tasks.append(task)
             self.zmq_channels_connected[channel] = True
         self.mq_task = asyncio.create_task(self.process_message())
-        await self.setup()
+        await self.setup()  # in prod, this would be things like importing libs and registering Comms
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         # Exiting the async context / general cleanup consists of:
         # - cancel all tasks
         # - stop zmq channel connections
         for task in self.channel_watcher_parent_tasks:
```

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/comms.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/comms.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/base.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/debug.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/debug.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/handlers/output.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/output.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/log_utils.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/log_utils.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/models/messages.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/models/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
 class UpdateDisplayDataContent(DisplayDataContent):
     output_type: Literal["update_display_data"] = "update_display_data"
     data: dict  # mimebundle
     metadata: dict = Field(default_factory=dict)
     transient: DisplayDataTransient
 
     @property
-    def display_id(self) -> str:
+    def display_id(self) -> Optional[str]:
         return self.transient.display_id
 
 
 class UpdateDisplayData(MessageBase):
     msg_type: Literal["update_display_data"]
     content: UpdateDisplayDataContent
```

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/models/notebook.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/models/notebook.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/models/requests.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/models/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # - execute_result
     # - execute_reply
     # - status (idle)
 """
 
 import uuid
 from datetime import datetime
-from typing import Annotated, Literal, Union
+from typing import Annotated, Literal, Optional, Union
 
 from pydantic import BaseModel, Field, PrivateAttr
 
 SESSION_ID = str(uuid.uuid4())
 
 
 class RequestHeader(BaseModel):
@@ -156,15 +156,15 @@
 
 class KernelInfoRequest(Request):
     header: KernelInfoRequestHeader = Field(default_factory=KernelInfoRequestHeader)
 
 
 # https://jupyter-client.readthedocs.io/en/stable/messaging.html#comm-info
 class CommInfoRequestContent(BaseModel):
-    target_name: str = None
+    target_name: Optional[str] = None
 
 
 class CommInfoRequestHeader(RequestHeader):
     msg_type: str = "comm_info_request"
 
 
 class CommInfoRequest(Request):
```

### Comparing `kernel_sidecar-0.5.3/src/kernel_sidecar/nb_builder.py` & `kernel_sidecar-0.5.4/src/kernel_sidecar/nb_builder.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.3/PKG-INFO` & `kernel_sidecar-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernel-sidecar
-Version: 0.5.3
+Version: 0.5.4
 Summary: A sidecar 
 Home-page: https://github.com/kafonek/kernel-sidecar
 License: MIT
 Author: Matt Kafonek
 Author-email: matt.kafonek@noteable.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.3 Summary: A sidecar
+Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.4 Summary: A sidecar
 Home-page: https://github.com/kafonek/kernel-sidecar License: MIT Author: Matt
 Kafonek Author-email: matt.kafonek@noteable.io Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli Requires-Dist: jupyter-client (>=7.3.4) Requires-Dist:
```

