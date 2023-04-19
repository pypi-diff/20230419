# Comparing `tmp/dequeai-0.714.tar.gz` & `tmp/dequeai-0.716.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.714.tar", last modified: Wed Apr 12 00:43:21 2023, max compression
+gzip compressed data, was "dequeai-0.716.tar", last modified: Wed Apr 19 19:10:33 2023, max compression
```

## Comparing `dequeai-0.714.tar` & `dequeai-0.716.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.449372 dequeai-0.714/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-12 00:43:21.449372 dequeai-0.714/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.445372 dequeai-0.714/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.714/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.714/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.714/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.714/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.714/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    21134 2023-04-12 00:42:41.000000 dequeai-0.714/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.714/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.714/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.714/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.714/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.445372 dequeai-0.714/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-12 00:43:20.000000 dequeai-0.714/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 00:43:21.449372 dequeai-0.714/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-12 00:42:55.000000 dequeai-0.714/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-19 19:10:33.045097 dequeai-0.716/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.716/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.716/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.716/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.716/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.716/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    19998 2023-04-19 19:08:35.000000 dequeai-0.716/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.716/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.716/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.716/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.716/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 19:10:33.000000 dequeai-0.716/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 19:10:33.045097 dequeai-0.716/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-19 19:10:17.000000 dequeai-0.716/setup.py
```

### Comparing `dequeai-0.714/dequeai/datatypes.py` & `dequeai-0.716/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.714/dequeai/dequeai_run.py` & `dequeai-0.716/dequeai/dequeai_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,146 +1,88 @@
 import datetime
-import json
 import os
-import subprocess
 import traceback
-
 import coolname
-
 from dequeai.rest_connect import RestConnect
 from dequeai.deque_environment import AGENT_API_SERVICE_URL
-#from deque.redis_services import RedisServices
 import pickle
 import multiprocessing
 from dequeai.parsing_service import ParsingService
 from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table #, Plot
 from dequeai.util import MODEL, CODE, DATA, ENVIRONMENT, RESOURCES,TRACKING_ENDPOINT
 import requests
 import glob
 import time
 import psutil
 import GPUtil
 import socket
 import types
-
-'''
-def decode_datetime(obj):
-    if '__datetime__' in obj:
-        obj = datetime.datetime.strptime(obj["as_str"], "%Y%m%dT%H:%M:%S.%f")
-    return obj
-
-
-def encode_datetime(obj):
-    if isinstance(obj, datetime.datetime):
-        return {'__datetime__': True, 'as_str': obj.strftime("%Y%m%dT%H:%M:%S.%f")}
-    return obj
-'''
-
-
-def _start_transport_service():
-    try:
-        print("Starting transport")
-        #import redis_server
-        #bin_path = str(redis_server.REDIS_SERVER_PATH)
-        #subprocess.run([bin_path])
-        print("started successfully")
-    except Exception as e:
-        print(e)
-        traceback.print_exc()
-
-
-#_start_transport_service()
+import pandas as pd
 
 _RESOURCE_MONITORING_INTERVAL = 60
 
-
 class Run:
 
-    # _submission_count = 1
     def __init__(self):
         self.user_name = None
-
         self._workload_type = None
-        # self._submission_id = None
-
         self.project_id = None
         self._project_name = None
         self._workload_id = None
         self._api_key = None
         self._submission_id = None
         self._agent_id = None
         self.params = dict()
         self._history = dict()
         self._step = 1
         self._run_id = None
         self._rest = RestConnect()
-        #self._redis = RedisServices.get_redis_connection()
         self._agent_network_details = self._get_network_details()
         self._run_meta_data = None
         self._model_logged = False
-
         self._code_logged = False
         self._running = False
         self._environment_logged = False
-
         self._resources_logged = False
         self._res_monitor = None
         self._run_start_time =None
 
     def init(self, user_name, api_key,project_name=None):
         os.environ["running"] = "yes"
         is_authenticated = self._authenticate(user_name=user_name, api_key=api_key)
         if is_authenticated:
             self.user_name = user_name
-
             self._api_key = api_key
         else:
             self.user_name = None
             raise ValueError("Invalid user and/or api key")
-
         self._run_start_time = datetime.datetime.now()
         self._running = True
-
         self._workload_type = os.getenv("workload_type")
         self._workload_id = os.getenv("workload_id")
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
-
         if project_name is None:
             if self._workload_id is None:
                 raise ValueError("Project name cannot be empty")
             else:
                 self._project_name = self._workload_id
         else:
             self._project_name = project_name
         self._run_id = str(coolname.generate_slug(2))
         self._step = 1
-
         p2 = multiprocessing.Process(target=self._start_parser)
         p2.start()
-
-        #self._res_monitor = multiprocessing.Process(target=self._monitor_resources, args=(
-        #self._agent_id, self._run_id, self.user_name, self._project_name, self._workload_id,
-        #self._submission_id, self._workload_type, self._run_start_time))
-        #self._res_monitor.start()
-        #self._redis.flushall()
-        #self._redis.sadd("run_ids:", self._run_id)
-
         self._run_meta_data = {"submission_id": self._submission_id, "run_id": self._run_id,
                                "workload_type": self._workload_type, "workload_id": self._workload_id,
                                "project_name": self._project_name, "user_name": user_name}
-
         self._model_logged = False
-
         self._code_logged = False
-
         self._environment_logged = False
-
         self._resources_logged = False
-
         print(f"Run initialized with project name as {self._project_name} for user {self.user_name} and run id {self._run_id}")
 
     def _start_parser(self):
         parser = ParsingService()
         parser.receive()
 
     def finish(self):
@@ -159,28 +101,25 @@
         while running=="yes":
             current = datetime.datetime.now()
             duration_in_min = (current - run_start_time).total_seconds() / 60
             duration_in_hours = duration_in_min / 60
             running = os.getenv("running")
             gpu_count = len(GPUtil.getGPUs())
             gpu_list = []
-
             for i in range(gpu_count):
                 gpu_dict = {}
                 gpu_dict['gpu_name'] = GPUtil.getGPUs()[i].name
                 gpu_dict['gpu_driver'] = GPUtil.getGPUs()[i].driver
                 gpu_dict['total_memory'] = GPUtil.getGPUs(
                 )[i].memoryTotal / 1024  # converted to GB
                 gpu_dict['gpu_free_memory'] = GPUtil.getGPUs()[i].memoryFree
                 gpu_dict['current_gpu_load'] = 100 * GPUtil.getGPUs()[i].load
                 gpu_list.append(gpu_dict)
-
             host_name = socket.gethostname()
             host_ip = socket.gethostbyname(host_name)
-
             monitoring_info = {
                 'agent_id': agent_id,
                 'run_id': run_id,
                 'user_name': user_name,
                 'project_name': project_name,
                 'step': step,
                 'workload_id': workload_id,
@@ -190,109 +129,81 @@
                 'cpu_count': int(psutil.cpu_count()),
                 'cpu_cores': int(psutil.cpu_count(logical=True)),
                 # /(1024*1024*1024) ,# converted to GB
                 'available_memory': int(psutil.virtual_memory()[1]),
                 # / (1024*1024*1024) ,# converted to GB
                 'total_memory': psutil.virtual_memory()[0],
                 'memory_utilization': psutil.virtual_memory()[2],
-
                 'current_network_usage': 'unknown',
                 'current_gpu_usage': gpu_list,
                 'free_disk_space': psutil.disk_usage(os.path.sep)[1],
-
                 'ip_address': host_ip,
                 'gpu_list': gpu_list,
                 'gpu_count': len(gpu_list),
-
                 'agent_network_details': self._agent_network_details,
                 'create_datetime':current,
                 'update_datetime':current,
                 'duration_in_min':duration_in_min,
                 'duration_in_hours':duration_in_hours
 
             }
-
-            # monitoring_info.update({"dq_instance_type":self.dq_instance_type})
-
-            # self.dq_instance_type = dq_instance_type
-
             try:
                 resp = self._rest.post(
                     AGENT_API_SERVICE_URL + '/fex/experiment/monitor/',
                     json=monitoring_info, )
-
             except requests.exceptions.ConnectionError as e:
                 traceback.print_exc(e)
                 time.sleep(10)
                 self._monitor_resources(agent_id, run_id, user_name, project_name, workload_id, submission_id,
                            workload_type)
             except Exception as ge:
                 traceback.print_exc(ge)
                 time.sleep(10)
                 self._monitor_resources(agent_id, run_id, user_name, project_name, workload_id, submission_id,
                            workload_type)
-
             time.sleep(_RESOURCE_MONITORING_INTERVAL)
 
     def _get_network_details(self):
 
         interfaces = psutil.net_if_addrs()
         hostname = socket.gethostname()
         fqdn = socket.getfqdn()
-
         agent_network_details = {'hostname': hostname, 'fqdn': fqdn}
-
         agent_ip_details = []
-
         for name, addrs in interfaces.items():
-            # print(name, addrs)
 
             status = {
                 "ipv4": "-",
                 "ipv6": "-",
                 "mac": "-"
             }
-
             for addr in addrs:
                 if addr.family == socket.AF_INET and addr.netmask is not None:
                     status["ipv4"] = addr.address
 
                     agent_ip_detail = {'name': name, 'ip_address': addr.address, 'netmask': addr.netmask}
                     agent_ip_details.append(agent_ip_detail)
 
                 if addr.family == socket.AF_INET6:
                     status["ipv6"] = addr.address
 
                 if addr.family == psutil.AF_LINK:
                     status["mac"] = addr.address
-
         agent_network_details.update({'agent_ip_details': agent_ip_details})
-
         return agent_network_details
 
-    def _send_data_to_redis(self, step, data):
-
-        key = "run_id:step:data:" + self._run_id + str(step)
-
-        #self._redis.sadd("run_id:steps:" + self._run_id, str(step))
-
-        data_pickled = pickle.dumps(data)
-
-        #self._redis.set(key, data_pickled)
-
     def log(self, data, step=None, commit=True):
         self._validate_data(data=data)
         full_data = {"experiment_data": data}
         full_data.update(
             {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
              "workload_id": self._workload_id, "submission_id": self._submission_id,
              "project_name": self._project_name, "deque_log_time": datetime.datetime.now(), "step": self._step})
         p = multiprocessing.Process(target=self._log_task, args=(full_data, self._run_meta_data))
         p.start()
-        #self._send_data_to_redis(step=self._step, data=full_data)
         os.environ['step']=str(self._step)
         if commit:
             self._step += 1
 
     def log_hyperparams(self, hyperparams):
         self._validate_hyperparams(hyperparams=hyperparams)
         full_data = {"hyperparams": hyperparams}
@@ -309,58 +220,46 @@
     def _log_task(self, data, run_meta_data):
         pickled_data = pickle.dumps(data)
         self._rest.post_binary(url=TRACKING_ENDPOINT, data=pickled_data)
 
     def log_artifact(self, artifact_type, path):
         if self._run_meta_data is None:
             raise ValueError("Run not initialized. Please call init first")
-        # s3://dequeapp-deque/users/riju@deque.app/projects/dex_audio/runs/adamant-galago/
         if artifact_type == MODEL:
             self._model_logged = True
         elif artifact_type == CODE:
             self._code_logged = True
         elif artifact_type == ENVIRONMENT:
             self._environment_logged = True
         elif artifact_type == RESOURCES:
             self._resources_logged = True
         p2 = multiprocessing.Process(target=self._log_artifact_task, args=(artifact_type, path, self._run_meta_data))
         p2.start()
 
     def _log_artifact_task(self, artifact_type, path, run_meta_data):
 
-        print("I am saving artifact")
         file_name = os.path.basename(path)
-
         if artifact_type == MODEL:
             dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/model/" + file_name
             valid_extensions = [".h5", ".hdf5", ".pt", ".pth", ".pkl", ".pklz", ".pkl.gz", ".pkl.bz2", ".pkl.xz", ".joblib"]
             if not any(file_name.lower().endswith(ext) for ext in valid_extensions):
                 raise ValueError("Model file must be one of the following extensions: " + str(valid_extensions))
         elif artifact_type == CODE:
             dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/code/"+ file_name
             valid_extensions = [".ipynb", ".py"]
             if not any(file_name.lower().endswith(ext) for ext in valid_extensions):
                 raise ValueError("Code file must be one of the following extensions: " + str(valid_extensions))
         elif artifact_type == ENVIRONMENT:
             dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/environment/" + file_name
             if not file_name.lower().endswith("yml"):
                 raise ValueError("Environment file must be a .yml file")
-
-
-
-
-        #elif artifact_type == RESOURCES:
-            #dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/resources/"
         else:
             raise ValueError(
                 "artifact_type must be model (file), environment (file), code (file) ")#or resources (directory)")
 
-        print(AGENT_API_SERVICE_URL + "/fex/drive/contents/upload/presigned_url/read/")
-
-        # Demonstrate how another Python program can use the presigned URL to upload a file
         if os.path.isdir(path):
             artifact_uris = []
             for filename in glob.iglob(path + '**/**', recursive=True):
                 if os.path.isdir(filename):
                     continue
                 dest_path = dest_path + filename
                 req_data = {"user_name": self.user_name, "destination_path": dest_path}
@@ -382,15 +281,14 @@
             artifact_uris.append(dest_path)
             req_data = {"user_name": self.user_name, "destination_path": dest_path, "artifact_type": artifact_type,
                         "project_name": self._project_name, "run_id": self._run_id, "artifact_uris": artifact_uris}
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/create/",
                                  json=req_data)
             res = resp.json()
             print(res)
-
         else:
             req_data = {"user_name": self.user_name, "destination_path": dest_path}
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/drive/contents/upload/presigned_url/read/",
                                  json=req_data)
             res = resp.json()
             with open(path, 'rb') as f:
                 files = {'file': (path, f)}
@@ -405,41 +303,36 @@
             req_data = {"user_name": self.user_name, "destination_path": dest_path, "artifact_type": artifact_type,
                         "project_name": self._project_name, "run_id": self._run_id, "artifact_uris": [dest_path]}
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/create/",
                                  json=req_data)
             res = resp.json()
             print(res)
 
-        # If successful, returns HTTP status code 204
-
     def register_artifacts(self, latest=True, label=None, tags=None):
         if not self._model_logged:
             raise ValueError(
                 "Please log the model (and optionally code and environment) before calling register_artifacts")
         req_data = {"user_name": self.user_name, "latest": latest, "label": label,
                     "project_name": self._project_name, "run_id": self._run_id, "tags": tags}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/artifacts/register/",
                              json=req_data)
         res = resp.json()
         print(res)
 
     def load_artifact(self,  artifact_type, run_id):
-        # Fetch artifact metadata
-
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling load_artifact")
         req_data = {
             "user_name": self.user_name,
             "run_id": run_id,
             "artifact_type": artifact_type
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/read/", json=req_data)
         metadata = resp.json()
 
-        # Check if metadata exists
         if not metadata:
             print("No metadata found for the given run_id and user_name.")
             return
 
         artifact_uris = metadata["artifact_uris"]
 
         # Download the artifacts using the artifact URIs
@@ -447,74 +340,98 @@
             req_data = {
                 "user_name": self.user_name,
                 "complete_object_path": artifact_uri
             }
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/drive/contents/download/presigned_url/read/",
                                  json=req_data)
             res = resp.json()
-
             # Download the artifact using the pre-signed URL
             http_response = requests.get(url=res["url"])
             file_name = os.path.basename(artifact_uri)
-
             with open(file_name, "wb") as f:
                 f.write(http_response.content)
-
             print(f"Downloaded artifact '{file_name}'")
 
     def _validate_data(self, data):
         for key, value in data.items():
             if type(value) is dict:
                 self._validate_data(value)
             else:
-                # print(type(value))
                 if type(value) in [Audio, BoundingBox2D, Histogram,Table,
                                    Image] or type(value) in types.__builtins__.values():
                     pass
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
 
     def _validate_hyperparams(self, hyperparams):
         for key, value in hyperparams.items():
-
             if type(value) in types.__builtins__.values():
                 pass
             else:
                 raise ValueError(
                     "Invalid type in hyperparam dict. Allowed values include builtin types " + str(
                         type(value)) + " " + str(value.__class__.__module__))
 
     def _send_upstream(self):
         self._rest.post(url=AGENT_API_SERVICE_URL + "/fex/python/track/", json=self._history)
         self._history = dict()
 
     def _authenticate(self, user_name, api_key):
-        # Download the artifacts using the artifact URIs
-
         req_data = {
             "user_name": user_name,
             "api_key": api_key
         }
-        print(AGENT_API_SERVICE_URL + "/fex/authenticate/sdk/")
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/authenticate/sdk/", json=req_data)
-
         res = resp.json()
-
         print(res)
-        # Download the artifact using the pre-signed URL
         if "authenticated" in res:
             return res["authenticated"]
         else:
             return False
 
+    def compare_runs(self, run_ids):
+        if self.user_name is None:
+            raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
+        req_data = {
+            "user_name": self.user_name,
+            "run_ids": run_ids
+        }
+        resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
+        res = resp.json()
+        # convert res to a dataframe
+        res_df = pd.DataFrame(res)
+        print(res_df)
+        return res_df
 
+    def search_runs(self,filter_dict):
+        if self.user_name is None:
+            raise ValueError("Please initialize using dequeai.init() before calling search_runs")
+        req_data = {
+            "user_name": self.user_name,
+            "filter_dict": filter_dict
+        }
+        resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/search/", json=req_data)
+        res = resp.json()
+        print(res)
+        return res
 
-
+    def create_report(self, run_ids, file_format="pdf"):
+        if self.user_name is None:
+            raise ValueError("Please initialize using dequeai.init() before calling create_report")
+        req_data = {
+            "user_name": self.user_name,
+            "run_ids": run_ids,
+            "file_format": file_format,
+        }
+        resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/report/create/", json=req_data)
+        res = resp.json()
+        print(res)
+        return res
 
 
 if __name__ == "__main__":
     deque = Run()
     deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
     #deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
        #                     run_meta_data=None)
```

### Comparing `dequeai-0.714/dequeai/parsing_service.py` & `dequeai-0.716/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.714/dequeai/rest_connect.py` & `dequeai-0.716/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.714/dequeai/util.py` & `dequeai-0.716/dequeai/util.py`

 * *Files identical despite different names*

