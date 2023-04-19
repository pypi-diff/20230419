# Comparing `tmp/pyjava-0.3.8.tar.gz` & `tmp/pyjava-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjava-0.3.8.tar", last modified: Sun Mar 19 01:52:30 2023, max compression
+gzip compressed data, was "dist/pyjava-0.3.9.tar", last modified: Wed Apr 19 02:37:52 2023, max compression
```

## Comparing `pyjava-0.3.8.tar` & `pyjava-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.302156 pyjava-0.3.8/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      597 2023-03-19 01:52:30.302265 pyjava-0.3.8/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.3.8/README.md
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.295793 pyjava-0.3.8/pyjava/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.3.8/pyjava/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.298251 pyjava-0.3.8/pyjava/api/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/api/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.3.8/pyjava/api/mlsql.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.3.8/pyjava/api/serve.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.298902 pyjava-0.3.8/pyjava/cache/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/cache/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/cache/code_cache.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/cloudpickle.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/daemon.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.299455 pyjava-0.3.8/pyjava/data/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/data/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.3.8/pyjava/data/datasource.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.300125 pyjava-0.3.8/pyjava/datatype/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/datatype/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/datatype/types.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/rayfix.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.3.8/pyjava/serializers.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.301301 pyjava-0.3.8/pyjava/storage/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/storage/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/storage/streaming_tar.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.301774 pyjava-0.3.8/pyjava/udf/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4270 2023-03-06 01:45:39.000000 pyjava-0.3.8/pyjava/udf/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.3.8/pyjava/utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-03-19 01:52:23.000000 pyjava-0.3.8/pyjava/version.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.3.8/pyjava/worker.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-03-19 01:52:30.297158 pyjava-0.3.8/pyjava.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      597 2023-03-19 01:52:30.000000 pyjava-0.3.8/pyjava.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-03-19 01:52:30.000000 pyjava-0.3.8/pyjava.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-03-19 01:52:30.000000 pyjava-0.3.8/pyjava.egg-info/dependency_links.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-03-19 01:52:30.000000 pyjava-0.3.8/pyjava.egg-info/top_level.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-03-19 01:52:30.302792 pyjava-0.3.8/setup.cfg
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.3.8/setup.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-04-19 02:37:52.000000 pyjava-0.3.9/PKG-INFO
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      670 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      596 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        7 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava.egg-info/top_level.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava.egg-info/dependency_links.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42222 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/cloudpickle.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6457 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/worker.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      828 2023-04-19 02:37:35.000000 pyjava-0.3.9/pyjava/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/cache/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      489 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/cache/code_cache.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/cache/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30195 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/serializers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2612 2023-03-06 01:45:39.000000 pyjava-0.3.9/pyjava/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/datatype/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/datatype/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    64554 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/datatype/types.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/storage/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2825 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/storage/streaming_tar.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/storage/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3916 2021-10-03 00:16:16.000000 pyjava-0.3.9/pyjava/utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/api/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16024 2023-03-06 01:45:39.000000 pyjava-0.3.9/pyjava/api/mlsql.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      688 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/api/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4524 2023-03-17 14:55:56.000000 pyjava-0.3.9/pyjava/api/serve.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/udf/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5083 2023-04-19 02:37:35.000000 pyjava-0.3.9/pyjava/udf/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2190 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/rayfix.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-19 02:37:52.000000 pyjava-0.3.9/pyjava/data/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2022-10-12 14:29:02.000000 pyjava-0.3.9/pyjava/data/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1185 2023-03-19 01:36:05.000000 pyjava-0.3.9/pyjava/data/datasource.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7048 2021-01-12 02:30:28.000000 pyjava-0.3.9/pyjava/daemon.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      448 2021-01-12 02:30:28.000000 pyjava-0.3.9/README.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2955 2022-10-12 14:29:02.000000 pyjava-0.3.9/setup.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       79 2023-04-19 02:37:52.000000 pyjava-0.3.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyjava-0.3.8/pyjava/__init__.py` & `pyjava-0.3.9/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/api/__init__.py` & `pyjava-0.3.9/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/api/mlsql.py` & `pyjava-0.3.9/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/api/serve.py` & `pyjava-0.3.9/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/cloudpickle.py` & `pyjava-0.3.9/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/daemon.py` & `pyjava-0.3.9/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/data/datasource.py` & `pyjava-0.3.9/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/datatype/types.py` & `pyjava-0.3.9/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/rayfix.py` & `pyjava-0.3.9/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/serializers.py` & `pyjava-0.3.9/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/storage/streaming_tar.py` & `pyjava-0.3.9/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/udf/__init__.py` & `pyjava-0.3.9/pyjava/udf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 import uuid
+import time
 from typing import Any, NoReturn, Callable, Dict, List
 import ray
-import time
 from ray.util.client.common import ClientActorHandle, ClientObjectRef
 
 from pyjava.api.mlsql import RayContext
 from pyjava.storage import streaming_tar
 
 
 @ray.remote
 class UDFMaster(object):
     def __init__(self, num: int, conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
-        model_servers = RayContext.parse_servers(conf["modelServers"])
-        items = RayContext.collect_from(model_servers)
-        model_refs = [ray.put(item) for item in items]
-
-        udfWorkerConf = {}
+        udf_worker_conf = {}
 
         if "num_cpus" in conf:
-            udfWorkerConf["num_cpus"] = int(conf["num_cpus"])
+            udf_worker_conf["num_cpus"] = int(conf["num_cpus"])
 
         if "num_gpus" in conf:
-            udfWorkerConf["num_gpus"] = int(conf["num_gpus"])
+            udf_worker_conf["num_gpus"] = int(conf["num_gpus"])
 
         custom_resources = [(key.split("resource.")[1], float(conf[key])) for key in
                             conf.keys() if
                             key.startswith("resource.")]
 
         if len(custom_resources) > 0:
-            udfWorkerConf["resources"] = dict(custom_resources)
+            udf_worker_conf["resources"] = dict(custom_resources)
+                
+        standalone = conf.get("standalone", "false") == "true"
+        
+        model_refs = []
+        print(f"standalone: {standalone} modelServers: {'modelServers' in conf}") 
+        if "modelServers" in conf and not standalone:
+            model_servers = RayContext.parse_servers(conf["modelServers"])
+            print(f"Pull model from {model_servers[0].host}:{model_servers[0].port}")
+            time1 = time.time()
+            items = RayContext.collect_from(model_servers)
+            model_refs = [ray.put(item) for item in items]
+            time2 = time.time()
+            print(f"Success to pull model, time taken:{time2-time1}s. The total refs: {len(model_refs)}")    
+            
 
         self.actors = dict(
-            [(index, UDFWorker.options(**udfWorkerConf).remote(model_refs, conf, init_func, apply_func)) for index in range(num)])
+            [(index,
+              UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, init_func,
+                                                          apply_func)) for index in
+             range(num)])
         self._idle_actors = [index for index in range(num)]
 
     def get(self) -> List[Any]:
         while len(self._idle_actors) == 0:
             time.sleep(0.001)
         index = self._idle_actors.pop()
         return [index, self.actors[index]]
@@ -52,15 +65,19 @@
 @ray.remote
 class UDFWorker(object):
     def __init__(self,
                  model_refs: List[ClientObjectRef],
                  conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
+        print("Init model....")
+        time1 = time.time()
         self.model = init_func(model_refs, conf)
+        time2 = time.time()
+        print(f"Success to init model. Time taken: {time2 - time1}s")
         self.apply_func = apply_func
 
     def apply(self, v: Any) -> Any:
         return self.apply_func(self.model, v)
 
     def shutdown(self):
         ray.actor.exit_actor()
@@ -88,29 +105,30 @@
                     stop_flag = False
                     counter = counter - 1
 
         except Exception as inst:
             print(inst)
             pass
 
-        UDFMaster.options(name=udf_name, lifetime="detached", max_concurrency=max_concurrency).remote(
+        UDFMaster.options(name=udf_name, lifetime="detached",
+                          max_concurrency=max_concurrency).remote(
             max_concurrency, conf, init_func, apply_func)
         ray_context.build_result([])
 
     @staticmethod
     def apply(ray_context: RayContext):
         conf = ray_context.conf()
         udf_name = conf["UDF_CLIENT"]
         udf_master = ray.get_actor(udf_name)
         [index, worker] = ray.get(udf_master.get.remote())
         input_value = [row["value"] for row in ray_context.python_context.fetch_once_as_rows()]
         try:
             res = ray.get(worker.apply.remote(input_value))
         except Exception as inst:
-            res = []
+            res = {}
             print(inst)
         udf_master.give_back.remote(index)
         ray_context.build_result([res])
 
 
 class UDFBuildInFunc(object):
     @staticmethod
```

### Comparing `pyjava-0.3.8/pyjava/utils.py` & `pyjava-0.3.9/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava/version.py` & `pyjava-0.3.9/pyjava/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `pyjava-0.3.8/pyjava/worker.py` & `pyjava-0.3.9/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/pyjava.egg-info/SOURCES.txt` & `pyjava-0.3.9/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.3.8/setup.py` & `pyjava-0.3.9/setup.py`

 * *Files identical despite different names*

