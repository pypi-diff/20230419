# Comparing `tmp/dagster-airbyte-0.19.0.tar.gz` & `tmp/dagster-airbyte-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.19.0.tar", last modified: Wed Apr 19 19:14:03 2023, max compression
+gzip compressed data, was "dagster-airbyte-1.0.5.tar", last modified: Fri Aug 26 13:45:14 2022, max compression
```

## Comparing `dagster-airbyte-0.19.0.tar` & `dagster-airbyte-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:03.675827 dagster-airbyte-0.19.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      716 2023-04-19 19:14:03.679827 dagster-airbyte-0.19.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:03.667827 dagster-airbyte-0.19.0/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40540 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:03.671826 dagster-airbyte-0.19.0/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:03.675827 dagster-airbyte-0.19.0/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    33410 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14161 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    15443 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2633 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:03.667827 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      716 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 19:14:03.000000 dagster-airbyte-0.19.0/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-19 19:14:03.679827 dagster-airbyte-0.19.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1593 2023-04-19 19:01:30.000000 dagster-airbyte-0.19.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      596 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)      467 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9354 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      596 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       24 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:45:14.000000 dagster-airbyte-1.0.5/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:45:14.452382 dagster-airbyte-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-08-26 13:33:01.000000 dagster-airbyte-1.0.5/setup.py
```

### Comparing `dagster-airbyte-0.19.0/LICENSE` & `dagster-airbyte-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-airbyte-0.19.0/PKG-INFO` & `dagster-airbyte-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.0
+Version: 1.0.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: test
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-airbyte-0.19.0/dagster_airbyte/ops.py` & `dagster-airbyte-1.0.5/dagster_airbyte/ops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,106 @@
-from typing import Any, Iterable, List, Optional
-
-from dagster import Config, In, Nothing, Out, Output, op
-from pydantic import Field
-
+from dagster_airbyte.resources import DEFAULT_POLL_INTERVAL_SECONDS
 from dagster_airbyte.types import AirbyteOutput
-from dagster_airbyte.utils import _get_attempt, generate_materializations
-
-from .resources import DEFAULT_POLL_INTERVAL_SECONDS, AirbyteResource
+from dagster_airbyte.utils import generate_materializations
 
-
-class AirbyteSyncConfig(Config):
-    connection_id: str = Field(
-        ...,
-        description=(
-            "Parsed json dictionary representing the details of the Airbyte connector after the"
-            " sync successfully completes. See the [Airbyte API"
-            " Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview)"
-            " to see detailed information on this response."
-        ),
-    )
-    poll_interval: float = Field(
-        DEFAULT_POLL_INTERVAL_SECONDS,
-        description=(
-            "The maximum time that will waited before this operation is timed out. By "
-            "default, this will never time out."
-        ),
-    )
-    poll_timeout: Optional[float] = Field(
-        None,
-        description=(
-            "The maximum time that will waited before this operation is timed out. By "
-            "default, this will never time out."
-        ),
-    )
-    yield_materializations: bool = Field(
-        True,
-        description=(
-            "If True, materializations corresponding to the results of the Airbyte sync will "
-            "be yielded when the op executes."
-        ),
-    )
-    asset_key_prefix: List[str] = Field(
-        ["airbyte"],
-        description=(
-            "If provided and yield_materializations is True, these components will be used to "
-            "prefix the generated asset keys."
-        ),
-    )
+from dagster import Array, Bool, Field, In, Noneable, Nothing, Out, Output, op
 
 
 @op(
+    required_resource_keys={"airbyte"},
     ins={"start_after": In(Nothing)},
     out=Out(
         AirbyteOutput,
-        description=(
-            "Parsed json dictionary representing the details of the Airbyte connector after the"
-            " sync successfully completes. See the [Airbyte API"
-            " Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview)"
-            " to see detailed information on this response."
-        ),
+        description="Parsed json dictionary representing the details of the Airbyte connector after "
+        "the sync successfully completes. "
+        "See the [Airbyte API Docs](https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview) "
+        "to see detailed information on this response.",
     ),
+    config_schema={
+        "connection_id": Field(
+            str,
+            is_required=True,
+            description="The Airbyte Connection ID that this op will sync. You can retrieve this "
+            'value from the "Connections" tab of a given connector in the Airbyte UI.',
+        ),
+        "poll_interval": Field(
+            float,
+            default_value=DEFAULT_POLL_INTERVAL_SECONDS,
+            description="The time (in seconds) that will be waited between successive polls.",
+        ),
+        "poll_timeout": Field(
+            Noneable(float),
+            default_value=None,
+            description="The maximum time that will waited before this operation is timed out. By "
+            "default, this will never time out.",
+        ),
+        "yield_materializations": Field(
+            config=Bool,
+            default_value=True,
+            description=(
+                "If True, materializations corresponding to the results of the Airbyte sync will "
+                "be yielded when the op executes."
+            ),
+        ),
+        "asset_key_prefix": Field(
+            config=Array(str),
+            default_value=["airbyte"],
+            description=(
+                "If provided and yield_materializations is True, these components will be used to "
+                "prefix the generated asset keys."
+            ),
+        ),
+    },
     tags={"kind": "airbyte"},
 )
-def airbyte_sync_op(context, config: AirbyteSyncConfig, airbyte: AirbyteResource) -> Iterable[Any]:
-    """Executes a Airbyte job sync for a given ``connection_id``, and polls until that sync
+def airbyte_sync_op(context):
+    """
+    Executes a Airbyte job sync for a given ``connection_id``, and polls until that sync
     completes, raising an error if it is unsuccessful. It outputs a AirbyteOutput which contains
     the job details for a given ``connection_id``.
 
     It requires the use of the :py:class:`~dagster_airbyte.airbyte_resource`, which allows it to
     communicate with the Airbyte API.
 
     Examples:
-        .. code-block:: python
 
-            from dagster import job
-            from dagster_airbyte import airbyte_resource, airbyte_sync_op
+    .. code-block:: python
 
-            my_airbyte_resource = airbyte_resource.configured(
-                {
-                    "host": {"env": "AIRBYTE_HOST"},
-                    "port": {"env": "AIRBYTE_PORT"},
-                }
-            )
-
-            sync_foobar = airbyte_sync_op.configured({"connection_id": "foobar"}, name="sync_foobar")
-
-            @job(resource_defs={"airbyte": my_airbyte_resource})
-            def my_simple_airbyte_job():
-                sync_foobar()
-
-            @job(resource_defs={"airbyte": my_airbyte_resource})
-            def my_composed_airbyte_job():
-                final_foobar_state = sync_foobar(start_after=some_op())
-                other_op(final_foobar_state)
+        from dagster import job
+        from dagster_airbyte import airbyte_resource, airbyte_sync_op
+
+        my_airbyte_resource = airbyte_resource.configured(
+            {
+                "host": {"env": "AIRBYTE_HOST"},
+                "port": {"env": "AIRBYTE_PORT"},
+            }
+        )
+
+        sync_foobar = airbyte_sync_op.configured({"connection_id": "foobar"}, name="sync_foobar")
+
+        @job(resource_defs={"airbyte": my_airbyte_resource})
+        def my_simple_airbyte_job():
+            sync_foobar()
+
+        @job(resource_defs={"airbyte": my_airbyte_resource})
+        def my_composed_airbyte_job():
+            final_foobar_state = sync_foobar(start_after=some_op())
+            other_op(final_foobar_state)
     """
-    airbyte_output = airbyte.sync_and_poll(
-        connection_id=config.connection_id,
-        poll_interval=config.poll_interval,
-        poll_timeout=config.poll_timeout,
+
+    airbyte_output = context.resources.airbyte.sync_and_poll(
+        connection_id=context.op_config["connection_id"],
+        poll_interval=context.op_config["poll_interval"],
+        poll_timeout=context.op_config["poll_timeout"],
     )
-    if config.yield_materializations:
+    if context.op_config["yield_materializations"]:
         yield from generate_materializations(
-            airbyte_output, asset_key_prefix=config.asset_key_prefix
+            airbyte_output, asset_key_prefix=context.op_config["asset_key_prefix"]
         )
     yield Output(
         airbyte_output,
         metadata={
-            **_get_attempt(airbyte_output.job_details.get("attempts", [{}])[-1]).get(
-                "totalStats", {}
-            )
+            **airbyte_output.job_details.get("attempts", [{}])[-1]
+            .get("attempt", {})
+            .get("totalStats", {})
         },
     )
```

### Comparing `dagster-airbyte-0.19.0/dagster_airbyte/resources.py` & `dagster-airbyte-1.0.5/dagster_airbyte/resources.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,305 +1,126 @@
-import hashlib
-import json
 import logging
 import sys
 import time
-from contextlib import contextmanager
-from typing import Any, Dict, List, Mapping, Optional, cast
+from typing import Dict, List, Optional, cast
 
 import requests
-from dagster import (
-    ConfigurableResource,
-    Failure,
-    _check as check,
-    get_dagster_logger,
-    resource,
-)
-from dagster._annotations import quiet_experimental_warnings
-from dagster._utils.cached_method import cached_method
-from dagster._utils.merger import deep_merge_dicts
-from pydantic import Field
+from dagster_airbyte.types import AirbyteOutput
 from requests.exceptions import RequestException
 
-from dagster_airbyte.types import AirbyteOutput
+from dagster import Failure, Field, StringSource, __version__
+from dagster import _check as check
+from dagster import get_dagster_logger, resource
 
 DEFAULT_POLL_INTERVAL_SECONDS = 10
 
 
 class AirbyteState:
     RUNNING = "running"
     SUCCEEDED = "succeeded"
     CANCELLED = "cancelled"
     PENDING = "pending"
     FAILED = "failed"
     ERROR = "error"
     INCOMPLETE = "incomplete"
 
 
-class AirbyteResourceState:
-    def __init__(self) -> None:
-        self.request_cache: Dict[str, Optional[Mapping[str, object]]] = {}
-        # Int in case we nest contexts
-        self.cache_enabled = 0
-
-
-class AirbyteResource(ConfigurableResource):
-    """This class exposes methods on top of the Airbyte REST API."""
-
-    host: str = Field(description="The Airbyte server address.")
-    port: str = Field(description="Port used for the Airbyte server.")
-    username: Optional[str] = Field(default=None, description="Username if using basic auth.")
-    password: Optional[str] = Field(default=None, description="Password if using basic auth.")
-    use_https: bool = Field(
-        default=False, description="Whether to use HTTPS to connect to the Airbyte server."
-    )
-    request_max_retries: int = Field(
-        default=3,
-        description=(
-            "The maximum number of times requests to the Airbyte API should be retried "
-            "before failing."
-        ),
-    )
-    request_retry_delay: float = Field(
-        default=0.25,
-        description="Time (in seconds) to wait between each request retry.",
-    )
-    request_timeout: int = Field(
-        default=15,
-        description="Time (in seconds) after which the requests to Airbyte are declared timed out.",
-    )
-    request_additional_params: Mapping[str, Any] = Field(
-        default=dict(),
-        description=(
-            "Any additional kwargs to pass to the requests library when making requests to Airbyte."
-        ),
-    )
-    forward_logs: bool = Field(
-        default=True,
-        description=(
-            "Whether to forward Airbyte logs to the compute log, can be expensive for"
-            " long-running syncs."
-        ),
-    )
-    cancel_sync_on_run_termination: bool = Field(
-        default=True,
-        description=(
-            "Whether to cancel a sync in Airbyte if the Dagster runner is terminated. This may"
-            " be useful to disable if using Airbyte sources that cannot be cancelled and"
-            " resumed easily, or if your Dagster deployment may experience runner interruptions"
-            " that do not impact your Airbyte deployment."
-        ),
-    )
+class AirbyteResource:
+    """
+    This class exposes methods on top of the Airbyte REST API.
+    """
 
-    @property
-    @cached_method
-    def _state(self) -> AirbyteResourceState:
-        return AirbyteResourceState()
+    def __init__(
+        self,
+        host: str,
+        port: str,
+        use_https: bool,
+        request_max_retries: int = 3,
+        request_retry_delay: float = 0.25,
+        log: logging.Logger = get_dagster_logger(),
+    ):
+        self._host = host
+        self._port = port
+        self._use_https = use_https
+        self._request_max_retries = request_max_retries
+        self._request_retry_delay = request_retry_delay
 
-    @property
-    @cached_method
-    def _log(self) -> logging.Logger:
-        return get_dagster_logger()
+        self._log = log
 
     @property
     def api_base_url(self) -> str:
         return (
-            ("https://" if self.use_https else "http://")
-            + (f"{self.host}:{self.port}" if self.port else self.host)
+            ("https://" if self._use_https else "http://")
+            + (f"{self._host}:{self._port}" if self._port else self._host)
             + "/api/v1"
         )
 
-    @contextmanager
-    def cache_requests(self):
-        """Context manager that enables caching certain requests to the Airbyte API,
-        cleared when the context is exited.
-        """
-        self.clear_request_cache()
-        self._state.cache_enabled += 1
-        try:
-            yield
-        finally:
-            self.clear_request_cache()
-            self._state.cache_enabled -= 1
-
-    def clear_request_cache(self) -> None:
-        self._state.request_cache = {}
-
-    def make_request_cached(self, endpoint: str, data: Optional[Mapping[str, object]]):
-        if not self._state.cache_enabled > 0:
-            return self.make_request(endpoint, data)
-        data_json = json.dumps(data, sort_keys=True)
-        sha = hashlib.sha1()
-        sha.update(endpoint.encode("utf-8"))
-        sha.update(data_json.encode("utf-8"))
-        digest = sha.hexdigest()
-
-        if digest not in self._state.request_cache:
-            self._state.request_cache[digest] = self.make_request(endpoint, data)
-        return self._state.request_cache[digest]
-
     def make_request(
-        self, endpoint: str, data: Optional[Mapping[str, object]]
-    ) -> Optional[Mapping[str, object]]:
-        """Creates and sends a request to the desired Airbyte REST API endpoint.
+        self, endpoint: str, data: Optional[Dict[str, object]]
+    ) -> Optional[Dict[str, object]]:
+        """
+        Creates and sends a request to the desired Airbyte REST API endpoint.
 
         Args:
             endpoint (str): The Airbyte API endpoint to send this request to.
             data (Optional[str]): JSON-formatted data string to be included in the request.
 
         Returns:
             Optional[Dict[str, Any]]: Parsed json data from the response to this request
         """
-        url = self.api_base_url + endpoint
+
         headers = {"accept": "application/json"}
 
         num_retries = 0
         while True:
             try:
                 response = requests.request(
-                    **deep_merge_dicts(  # type: ignore
-                        dict(
-                            method="POST",
-                            url=url,
-                            headers=headers,
-                            json=data,
-                            timeout=self.request_timeout,
-                            auth=(self.username, self.password)
-                            if self.username and self.password
-                            else None,
-                        ),
-                        self.request_additional_params,
-                    ),
+                    method="POST",
+                    url=self.api_base_url + endpoint,
+                    headers=headers,
+                    json=data,
+                    timeout=15,
                 )
                 response.raise_for_status()
                 if response.status_code == 204:
                     return None
                 return response.json()
             except RequestException as e:
                 self._log.error("Request to Airbyte API failed: %s", e)
-                if num_retries == self.request_max_retries:
+                if num_retries == self._request_max_retries:
                     break
                 num_retries += 1
-                time.sleep(self.request_retry_delay)
+                time.sleep(self._request_retry_delay)
 
-        raise Failure(f"Max retries ({self.request_max_retries}) exceeded with url: {url}.")
+        raise Failure("Exceeded max number of retries.")
 
     def cancel_job(self, job_id: int):
         self.make_request(endpoint="/jobs/cancel", data={"id": job_id})
 
-    def get_default_workspace(self) -> str:
-        workspaces = cast(
-            List[Dict[str, Any]],
-            check.not_none(self.make_request_cached(endpoint="/workspaces/list", data={})).get(
-                "workspaces", []
-            ),
-        )
-        return workspaces[0]["workspaceId"]
-
-    def get_source_definition_by_name(self, name: str) -> Optional[str]:
-        name_lower = name.lower()
-        definitions = self.make_request_cached(endpoint="/source_definitions/list", data={})
-
-        return next(
-            (
-                definition["sourceDefinitionId"]
-                for definition in definitions["sourceDefinitions"]
-                if definition["name"].lower() == name_lower
-            ),
-            None,
-        )
-
-    def get_destination_definition_by_name(self, name: str):
-        name_lower = name.lower()
-        definitions = cast(
-            Dict[str, List[Dict[str, str]]],
-            check.not_none(
-                self.make_request_cached(endpoint="/destination_definitions/list", data={})
-            ),
-        )
-        return next(
-            (
-                definition["destinationDefinitionId"]
-                for definition in definitions["destinationDefinitions"]
-                if definition["name"].lower() == name_lower
-            ),
-            None,
-        )
-
-    def get_source_catalog_id(self, source_id: str):
-        result = cast(
-            Dict[str, Any],
-            check.not_none(
-                self.make_request(endpoint="/sources/discover_schema", data={"sourceId": source_id})
-            ),
-        )
-        return result["catalogId"]
-
-    def get_source_schema(self, source_id: str) -> Mapping[str, Any]:
-        return cast(
-            Dict[str, Any],
-            check.not_none(
-                self.make_request(endpoint="/sources/discover_schema", data={"sourceId": source_id})
-            ),
-        )
-
-    def does_dest_support_normalization(
-        self, destination_definition_id: str, workspace_id: str
-    ) -> Dict[str, Any]:
-        return cast(
-            Dict[str, Any],
-            check.not_none(
-                self.make_request_cached(
-                    endpoint="/destination_definition_specifications/get",
-                    data={
-                        "destinationDefinitionId": destination_definition_id,
-                        "workspaceId": workspace_id,
-                    },
-                )
-            ),
-        ).get("supportsNormalization", False)
+    def get_job_status(self, job_id: int) -> dict:
+        return check.not_none(self.make_request(endpoint="/jobs/get", data={"id": job_id}))
 
-    def get_job_status(self, connection_id: str, job_id: int) -> Mapping[str, object]:
-        if self.forward_logs:
-            return check.not_none(self.make_request(endpoint="/jobs/get", data={"id": job_id}))
-        else:
-            # the "list all jobs" endpoint doesn't return logs, which actually makes it much more
-            # lightweight for long-running syncs with many logs
-            out = check.not_none(
-                self.make_request(
-                    endpoint="/jobs/list",
-                    data={
-                        "configTypes": ["sync"],
-                        "configId": connection_id,
-                        # sync should be the most recent, so pageSize 5 is sufficient
-                        "pagination": {"pageSize": 5},
-                    },
-                )
-            )
-            job = next((job for job in cast(List, out["jobs"]) if job["job"]["id"] == job_id), None)
-
-            return check.not_none(job)
-
-    def start_sync(self, connection_id: str) -> Mapping[str, object]:
+    def start_sync(self, connection_id: str) -> Dict[str, object]:
         return check.not_none(
             self.make_request(endpoint="/connections/sync", data={"connectionId": connection_id})
         )
 
-    def get_connection_details(self, connection_id: str) -> Mapping[str, object]:
+    def get_connection_details(self, connection_id: str) -> Dict[str, object]:
         return check.not_none(
             self.make_request(endpoint="/connections/get", data={"connectionId": connection_id})
         )
 
     def sync_and_poll(
         self,
         connection_id: str,
         poll_interval: float = DEFAULT_POLL_INTERVAL_SECONDS,
         poll_timeout: Optional[float] = None,
     ) -> AirbyteOutput:
-        """Initializes a sync operation for the given connector, and polls until it completes.
+        """
+        Initializes a sync operation for the given connector, and polls until it completes.
 
         Args:
             connection_id (str): The Airbyte Connector ID. You can retrieve this value from the
                 "Connection" tab of a given connection in the Arbyte UI.
             poll_interval (float): The time (in seconds) that will be waited between successive polls.
             poll_timeout (float): The maximum time that will waited before this operation is timed
                 out. By default, this will never time out.
@@ -319,30 +140,28 @@
         logged_lines = 0
         state = None
 
         try:
             while True:
                 if poll_timeout and start + poll_timeout < time.monotonic():
                     raise Failure(
-                        f"Timeout: Airbyte job {job_id} is not ready after the timeout"
-                        f" {poll_timeout} seconds"
+                        f"Timeout: Airbyte job {job_id} is not ready after the timeout {poll_timeout} seconds"
                     )
                 time.sleep(poll_interval)
-                job_details = self.get_job_status(connection_id, job_id)
+                job_details = self.get_job_status(job_id)
                 attempts = cast(List, job_details.get("attempts", []))
                 cur_attempt = len(attempts)
                 # spit out the available Airbyte log info
                 if cur_attempt:
-                    if self.forward_logs:
-                        log_lines = attempts[logged_attempts].get("logs", {}).get("logLines", [])
+                    log_lines = attempts[logged_attempts].get("logs", {}).get("logLines", [])
 
-                        for line in log_lines[logged_lines:]:
-                            sys.stdout.write(line + "\n")
-                            sys.stdout.flush()
-                        logged_lines = len(log_lines)
+                    for line in log_lines[logged_lines:]:
+                        sys.stdout.write(line + "\n")
+                        sys.stdout.flush()
+                    logged_lines = len(log_lines)
 
                     # if there's a next attempt, this one will have no more log messages
                     if logged_attempts < cur_attempt - 1:
                         logged_lines = 0
                         logged_attempts += 1
 
                 job_info = cast(Dict[str, object], job_details.get("job", {}))
@@ -357,27 +176,54 @@
                 elif state == AirbyteState.CANCELLED:
                     raise Failure(f"Job was cancelled: {job_id}")
                 else:
                     raise Failure(f"Encountered unexpected state `{state}` for job_id {job_id}")
         finally:
             # if Airbyte sync has not completed, make sure to cancel it so that it doesn't outlive
             # the python process
-            if (
-                state not in (AirbyteState.SUCCEEDED, AirbyteState.ERROR, AirbyteState.CANCELLED)
-                and self.cancel_sync_on_run_termination
-            ):
+            if state not in (AirbyteState.SUCCEEDED, AirbyteState.ERROR, AirbyteState.CANCELLED):
                 self.cancel_job(job_id)
 
         return AirbyteOutput(job_details=job_details, connection_details=connection_details)
 
 
-@resource(config_schema=AirbyteResource.to_config_schema())
-@quiet_experimental_warnings
+@resource(
+    config_schema={
+        "host": Field(
+            StringSource,
+            is_required=True,
+            description="The Airbyte Server Address.",
+        ),
+        "port": Field(
+            StringSource,
+            is_required=False,
+            description="Port for the Airbyte Server.",
+        ),
+        "use_https": Field(
+            bool,
+            default_value=False,
+            description="Use https to connect in Airbyte Server.",
+        ),
+        "request_max_retries": Field(
+            int,
+            default_value=3,
+            description="The maximum number of times requests to the Airbyte API should be retried "
+            "before failing.",
+        ),
+        "request_retry_delay": Field(
+            float,
+            default_value=0.25,
+            description="Time (in seconds) to wait between each request retry.",
+        ),
+    },
+    description="This resource helps manage Airbyte connectors",
+)
 def airbyte_resource(context) -> AirbyteResource:
-    """This resource allows users to programatically interface with the Airbyte REST API to launch
+    """
+    This resource allows users to programatically interface with the Airbyte REST API to launch
     syncs and monitor their progress. This currently implements only a subset of the functionality
     exposed by the API.
 
     For a complete set of documentation on the Airbyte REST API, including expected response JSON
     schema, see the `Airbyte API Docs <https://airbyte-public-api-docs.s3.us-east-2.amazonaws.com/rapidoc-api-docs.html#overview>`_.
 
     To configure this resource, we recommend using the `configured
@@ -390,19 +236,23 @@
         from dagster import job
         from dagster_airbyte import airbyte_resource
 
         my_airbyte_resource = airbyte_resource.configured(
             {
                 "host": {"env": "AIRBYTE_HOST"},
                 "port": {"env": "AIRBYTE_PORT"},
-                # If using basic auth
-                "username": {"env": "AIRBYTE_USERNAME"},
-                "password": {"env": "AIRBYTE_PASSWORD"},
             }
         )
 
         @job(resource_defs={"airbyte":my_airbyte_resource})
         def my_airbyte_job():
             ...
 
     """
-    return AirbyteResource.from_resource_context(context)
+    return AirbyteResource(
+        host=context.resource_config["host"],
+        port=context.resource_config["port"],
+        use_https=context.resource_config["use_https"],
+        request_max_retries=context.resource_config["request_max_retries"],
+        request_retry_delay=context.resource_config["request_retry_delay"],
+        log=context.log,
+    )
```

### Comparing `dagster-airbyte-0.19.0/dagster_airbyte/utils.py` & `dagster-airbyte-1.0.5/dagster_airbyte/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,40 @@
-from typing import Any, Iterator, Mapping, Sequence
-
-from dagster import AssetMaterialization, MetadataValue
-from dagster._core.definitions.metadata.table import TableColumn, TableSchema
+from typing import Any, Dict, Iterator, List
 
 from dagster_airbyte.types import AirbyteOutput
 
-
-def generate_table_schema(stream_schema_props: Mapping[str, Any]) -> TableSchema:
-    return TableSchema(
-        columns=sorted(
-            [
-                TableColumn(name=name, type=str(info.get("type", "unknown")))
-                for name, info in stream_schema_props.items()
-            ],
-            key=lambda col: col.name,
-        )
-    )
-
-
-def is_basic_normalization_operation(operation_def: Mapping[str, Any]) -> bool:
-    return (
-        operation_def.get("operatorType", operation_def.get("operator_type")) == "normalization"
-        and operation_def.get("normalization", {}).get("option") == "basic"
-    )
+from dagster import AssetMaterialization, MetadataValue
+from dagster._core.definitions.metadata.table import TableColumn, TableSchema
 
 
 def _materialization_for_stream(
     name: str,
-    stream_schema_props: Mapping[str, Any],
-    stream_stats: Mapping[str, Any],
-    asset_key_prefix: Sequence[str],
+    stream_schema_props: Dict[str, Any],
+    stream_stats: Dict[str, Any],
+    asset_key_prefix: List[str],
 ) -> AssetMaterialization:
+
     return AssetMaterialization(
-        asset_key=[*asset_key_prefix, name],
+        asset_key=asset_key_prefix + [name],
         metadata={
-            "schema": MetadataValue.table_schema(generate_table_schema(stream_schema_props)),
+            "schema": MetadataValue.table_schema(
+                TableSchema(
+                    columns=[
+                        TableColumn(name=name, type=str(info.get("type", "unknown")))
+                        for name, info in stream_schema_props.items()
+                    ]
+                )
+            ),
             **{k: v for k, v in stream_stats.items() if v is not None},
         },
     )
 
 
-def _get_attempt(attempt: dict):
-    # the attempt field is nested in some API results, and is not in others
-    return attempt.get("attempt") or attempt
-
-
 def generate_materializations(
-    output: AirbyteOutput, asset_key_prefix: Sequence[str]
+    output: AirbyteOutput, asset_key_prefix: List[str]
 ) -> Iterator[AssetMaterialization]:
     prefix = output.connection_details.get("prefix") or ""
     # all the streams that are set to be sync'd by this connection
     all_stream_props = {
         prefix
         + stream["stream"]["name"]: stream.get("stream", {})
         .get("jsonSchema", {})
@@ -58,15 +42,17 @@
         for stream in output.connection_details.get("syncCatalog", {}).get("streams", [])
         if stream.get("config", {}).get("selected")
     }
 
     # stats for each stream that had data sync'd
     all_stream_stats = {
         s["streamName"]: s.get("stats", {})
-        for s in _get_attempt(output.job_details.get("attempts", [{}])[-1]).get("streamStats", [])
+        for s in output.job_details.get("attempts", [{}])[-1]
+        .get("attempt", {})
+        .get("streamStats", [])
     }
     for stream_name, stream_props in all_stream_props.items():
         yield _materialization_for_stream(
             stream_name,
             stream_props,
             # if no records are sync'd, no stats will be avaiable for this stream
             all_stream_stats.get(stream_name, {}),
```

### Comparing `dagster-airbyte-0.19.0/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-1.0.5/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.0
+Version: 1.0.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: test
-Provides-Extra: managed
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-airbyte-0.19.0/setup.py` & `dagster-airbyte-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,39 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_airbyte/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_airbyte/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-airbyte",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for integrating Airbyte with Dagster.",
-    url=(
-        "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte"
-    ),
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_airbyte_tests*"]),
-    install_requires=[
-        "dagster==1.3.0",
-        "requests",
-    ],
-    zip_safe=False,
-    entry_points={
-        "console_scripts": [
-            "dagster-airbyte = dagster_airbyte.cli:main",
-        ]
-    },
-    extras_require={
-        "test": [
-            "requests-mock",
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-airbyte",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for integrating Airbyte with Dagster.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
         ],
-        "managed": [
-            "dagster-managed-elements==0.19.0",
+        packages=find_packages(exclude=["dagster_airbyte_tests*"]),
+        install_requires=[
+            "dagster==1.0.5",
+            "requests",
         ],
-    },
-)
+        zip_safe=False,
+    )
```

