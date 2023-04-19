# Comparing `tmp/valmi_connector_lib-0.1.7.tar.gz` & `tmp/valmi_connector_lib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.7.tar", last modified: Mon Apr 17 12:17:44 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.8.tar", last modified: Wed Apr 19 16:32:40 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.7.tar` & `valmi_connector_lib-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.406148 valmi_connector_lib-0.1.7/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 12:17:44.406208 valmi_connector_lib-0.1.7/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.7/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 12:17:44.406461 valmi_connector_lib-0.1.7/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-17 12:17:28.000000 valmi_connector_lib-0.1.7/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.403209 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 12:17:44.000000 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 12:17:44.000000 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 12:17:44.000000 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-17 12:17:44.000000 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 12:17:44.000000 valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.403318 valmi_connector_lib-0.1.7/valmi_lib/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.7/valmi_lib/__init__.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.404529 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/read_handlers.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.404870 valmi_connector_lib-0.1.7/valmi_lib/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.7/valmi_lib/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.7/valmi_lib/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.405322 valmi_connector_lib-0.1.7/valmi_lib/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.7/valmi_lib/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     6897 2023-04-17 12:13:57.000000 valmi_connector_lib-0.1.7/valmi_lib/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:17:44.405969 valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      573 2023-04-17 12:17:20.000000 valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.463301 valmi_connector_lib-0.1.8/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-19 16:32:40.463343 valmi_connector_lib-0.1.8/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.8/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-19 16:32:40.463564 valmi_connector_lib-0.1.8/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-19 16:17:39.000000 valmi_connector_lib-0.1.8/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.460399 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.460497 valmi_connector_lib-0.1.8/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.8/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.461655 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.461984 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.462469 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     8229 2023-04-19 16:29:23.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.463114 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      573 2023-04-17 12:17:20.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     4238 2023-04-19 16:17:21.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.7/setup.py` & `valmi_connector_lib-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.7",
+    version="0.1.8",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.7/valmi_connector_lib.egg-info/SOURCES.txt` & `valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import argparse
 import io
 import logging
 import sys
 from typing import Any, Iterable, List, Mapping
 
 from airbyte_cdk.destinations import Destination
-from airbyte_cdk.models import AirbyteMessage, Type
+from airbyte_cdk.models import AirbyteMessage, Type, AirbyteConnectionStatus, Status
 from abc import abstractmethod
 from valmi_lib.valmi_protocol import ConfiguredValmiDestinationCatalog, ConfiguredValmiCatalog
 from airbyte_cdk import AirbyteLogger
 
 logger = logging.getLogger("airbyte")
 
 
@@ -76,14 +76,24 @@
             "discover", help="outputs a catalog describing the source's schema", parents=[parent_parser]
         )
         required_discover_parser = discover_parser.add_argument_group("required named arguments")
         required_discover_parser.add_argument(
             "--config", type=str, required=True, help="path to the json configuration file"
         )
 
+        # create object
+        create_parser = subparsers.add_parser(
+            "create", help="create an object on the destination", parents=[parent_parser]
+        )
+        required_create_parser = create_parser.add_argument_group("required named arguments")
+        required_create_parser.add_argument("--object", type=str, required=True, help="path to the json object file")
+        required_create_parser.add_argument(
+            "--config", type=str, required=True, help="path to the json configuration file"
+        )
+
         parsed_args = main_parser.parse_args(args)
         cmd = parsed_args.command
         if not cmd:
             raise Exception("No command entered. ")
         elif cmd not in Destination.VALID_CMDS:
             # This is technically dead code since parse_args() would fail if this was the case
             # But it's non-obvious enough to warrant placing it here anyways
@@ -103,28 +113,47 @@
         config = self.read_config(config_path=parsed_args.config)
 
         if cmd == "discover":
             for msg in self.discover_handler(config, parsed_args):
                 yield msg
             return
 
+        if cmd == "create":
+            for msg in self.create_handler(config, parsed_args):
+                yield msg
+            return
+
         elif cmd == "write":
             # state = self.read_state(parsed_args.state)
 
             # Wrap in UTF-8 to override any other input encodings
             wrapped_stdin = io.TextIOWrapper(sys.stdin.buffer, encoding="utf-8")
             yield from self._run_write(
                 # config=config, configured_catalog_path=parsed_args.catalog, input_stream=wrapped_stdin, state=state
                 config=config,
                 configured_catalog_path=parsed_args.catalog,
                 configured_destination_catalog_path=parsed_args.destination_catalog,
                 input_stream=wrapped_stdin,
             )
             return
 
+    def create_handler(self, config, parsed_args: argparse.Namespace) -> Iterable[AirbyteMessage]:
+        try:
+            object_schema = self.read_config(config_path=parsed_args.object)
+
+            self.create(logger, config, object_schema)
+            yield AirbyteMessage(
+                type=Type.CONNECTION_STATUS, connectionStatus=AirbyteConnectionStatus(status=Status.SUCCEEDED)
+            )
+        except Exception as err:
+            yield AirbyteMessage(
+                type=Type.CONNECTION_STATUS,
+                connectionStatus=AirbyteConnectionStatus(status=Status.Failed, message=str(err)),
+            )
+
     def discover_handler(self, config, parsed_args: argparse.Namespace) -> Iterable[AirbyteMessage]:
         catalog = self.discover(logger, config)
         yield AirbyteMessage(type=Type.CATALOG, catalog=catalog)
 
     @abstractmethod
     def write(
         self,
```

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/__init__.py` & `valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.7/valmi_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,27 +80,31 @@
 # TODO: Hack. Think of a nice way
 @optional
 class ValmiDestinationCatalog(AirbyteCatalog):
     class Config:
         extra = Extra.allow
 
     sinks: Optional[List[ValmiSink]]
+    allow_object_creation: bool = Field(..., description="Allow object creation in destination.")
+    object_schema: Dict[str, Any] = Field(..., description="Object creation schema using Json Schema specs.")
+    more: bool = False
+    type: str = Field(..., description="Type of the object.")
 
 
 class ConfiguredValmiDestinationCatalog(BaseModel):
     class Config:
         extra = Extra.allow
 
     sinks: List[ConfiguredValmiSink]
 
 
 # TODO: Hack. Think of a nice way
 @optional
 class ValmiStream(AirbyteStream):
-    supported_destinaton_sync_modes: List[DestinationSyncMode] = Field(
+    supported_destination_sync_modes: List[DestinationSyncMode] = Field(
         ..., description="List of destination sync modes supported by this stream.", min_items=1
     )
     pass
 
 
 class ConfiguredValmiStream(ConfiguredAirbyteStream):
     class Config:
```

