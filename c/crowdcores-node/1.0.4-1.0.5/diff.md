# Comparing `tmp/crowdcores-node-1.0.4.tar.gz` & `tmp/crowdcores-node-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.0.4.tar", last modified: Wed Apr 19 01:23:57 2023, max compression
+gzip compressed data, was "crowdcores-node-1.0.5.tar", last modified: Wed Apr 19 21:35:12 2023, max compression
```

## Comparing `crowdcores-node-1.0.4.tar` & `crowdcores-node-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.4/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-04-18 22:11:04.000000 crowdcores-node-1.0.4/crowdcores_node/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-19 01:23:46.000000 crowdcores-node-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:35:12.755554 crowdcores-node-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:35:12.755554 crowdcores-node-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:35:12.751554 crowdcores-node-1.0.5/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.5/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-04-19 21:34:30.000000 crowdcores-node-1.0.5/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-04-19 21:34:34.000000 crowdcores-node-1.0.5/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:35:12.755554 crowdcores-node-1.0.5/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 21:35:12.000000 crowdcores-node-1.0.5/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 21:35:12.755554 crowdcores-node-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-19 21:34:49.000000 crowdcores-node-1.0.5/setup.py
```

### Comparing `crowdcores-node-1.0.4/LICENSE.txt` & `crowdcores-node-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.0.4/crowdcores_node/node.py` & `crowdcores-node-1.0.5/crowdcores_node/crowdcores_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import websockets
 import time
 import json
 import torch
 from transformers import pipeline
+import sys
 
 model_names=[];
 models_pipelines={};
 
 async def run_async(func, *args, **kwargs):
     loop = asyncio.get_event_loop()
     result = await loop.run_in_executor(None, func, *args, **kwargs)
@@ -85,14 +86,15 @@
 
         if message_json['command'] == 'process_pipeline_request':
             asyncio.create_task(process_pipeline_request(websocket,message_json))
 
 
 async def send_loop(websocket):
     while True:
+        print("sending");
         await asyncio.sleep(15)
         data = {'command': 'ping'}
         await websocket.send(json.dumps(data))
 
 async def start_node(websocket):
         data = {'command': 'node_started'}
         await websocket.send(json.dumps(data))
```

