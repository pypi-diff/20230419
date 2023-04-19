# Comparing `tmp/searchium-0.0.1rc2.tar.gz` & `tmp/searchium-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchium-0.0.1rc2.tar", max compression
+gzip compressed data, was "searchium-0.0.1rc3.tar", max compression
```

## Comparing `searchium-0.0.1rc2.tar` & `searchium-0.0.1rc3.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      775 2023-03-31 10:34:28.944216 searchium-0.0.1rc2/README.md
--rw-r--r--   0        0        0      380 2023-03-31 10:37:52.768242 searchium-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-03-31 10:13:18.878690 searchium-0.0.1rc2/searchium/__init__.py
--rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc2/searchium/fvs/__init__.py
--rw-r--r--   0        0        0     5023 2023-03-31 09:39:03.376537 searchium-0.0.1rc2/searchium/fvs/client.py
--rw-r--r--   0        0        0     1262 2023-03-31 09:39:03.420538 searchium-0.0.1rc2/searchium/fvs/model.py
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 searchium-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0     1423 2023-04-19 16:01:41.103149 searchium-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      380 2023-04-04 07:50:38.111647 searchium-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-04-18 08:39:12.058174 searchium-0.0.1rc3/searchium/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-04 10:24:52.278850 searchium-0.0.1rc3/searchium/client/__init__.py
+-rw-r--r--   0        0        0     6395 2023-04-19 16:01:41.123149 searchium-0.0.1rc3/searchium/client/func.py
+-rw-r--r--   0        0        0     1176 2023-04-18 14:33:48.839524 searchium-0.0.1rc3/searchium/client/init.py
+-rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc3/searchium/fvs/__init__.py
+-rw-r--r--   0        0        0     5331 2023-04-03 12:04:06.397449 searchium-0.0.1rc3/searchium/fvs/client.py
+-rw-r--r--   0        0        0     1965 2023-04-19 13:39:57.422802 searchium-0.0.1rc3/searchium/fvs/model.py
+-rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 searchium-0.0.1rc3/PKG-INFO
```

### Comparing `searchium-0.0.1rc2/README.md` & `searchium-0.0.1rc3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,23 +8,35 @@
 - validate_allocation(self) -> bool
 - get_loaded_dataset(self) -> List[LoadedDataset]:
 - get_datasets -> List[Dataset]
 - delete_dataset(dataset_id: str) -> bool
 - load_dataset(self, dataset_id: str) -> bool
 - unload_dataset(self, dataset_id: str) -> bool
 - search(self, dataset_id: str, query: List[List[float]], topk: int = 5) -> SearchResponse
+- create_dataset(dataset_id: Optional[str] = None) -> CreateDatasetResponse
+- add_chunk(dataset_id: str, list_documents: List[dict]) -> Response
+- train_dataset(dataset_id: str) -> Response
+- train_status(dataset_id: str) -> TrainStatus
+- get_dataset(dataset_id: str) -> Dataset
+- delete_document(dataset_id: str, document_id: List[str] = None, delete_all: bool = False) -> ResponseDeleteDocument
 ---
 
 ***example:***
 
-***from searchium import fvs***
+***import searchium***
 
-***client = fvs.get_client("your_allocation_id", "your_url")***
+***searchium.init("your_allocation_id", "your_url")***
 
-***dataset_id = 'your_dataset_id'***
+***dataset_id = 'your_dataset_uuid'***
 
-***client.load_dataset(dataset_id)***
+***searchium.create_dataset(dataset_id)***
 
-***client.search(dataset_id, query, 1)***
+***searchium.add_chunk(dataset_id: str, [{"document_id": str=doc_id, "vector": List[float]=embedding, "metadata": dict=metadata}])***
 
-***client.unload_dataset(dataset_id)***
+***searchium.train_dataset(dataset_id)***
+
+***searchium.load_dataset(dataset_id)***
+
+***searchium.search(dataset_id: str, query: List[List[float]], topk: int = 5)***
+
+***searchium.unload_dataset(dataset_id)***
```

### Comparing `searchium-0.0.1rc2/searchium/fvs/client.py` & `searchium-0.0.1rc3/searchium/fvs/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import uuid
+
 import requests
 from pydantic.tools import parse_obj_as
 
 from searchium.fvs.model import *
 
 
 class ClientFVS(object):
@@ -113,28 +115,34 @@
         get = requests.post(link, json=body, headers=self._headers)
         if get.status_code == 200:
             obj_as = parse_obj_as(SearchResponse, get.json())
             return obj_as.dict(exclude_none=True)
         else:
             raise Exception(get.json())
 
+    def create_dataset(self, dataset_name: Optional[str] = None) -> str:
+        """
+        :return: str dataset_id
+        """
+        link = f"{self._link}/dataset/create"
+        get = requests.post(link, headers=self._headers)
+        if get.status_code == 200:
+            obj_as = parse_obj_as(str, get.json())
+            return obj_as
+        else:
+            raise Exception(get.json())
+
     def _train_dataset(self, dataset_id):
         # /dataset/train
         # {
         #     "datasetId": "",
         #     "trainType": "Regular"
         # }
         pass
-
-    def _create_dataset(self) -> str:
-        """
-        :return: str dataset_id
-        """
-        pass
-
+    
     def _add_chunk(self, dataset_id: str) -> None:
         pass
 
     def _check_connection(self) -> bool:
         # Alive
         # /alive
         pass
```

### Comparing `searchium-0.0.1rc2/PKG-INFO` & `searchium-0.0.1rc3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchium
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: 
 Author: GSI Technology, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,24 +23,36 @@
 - validate_allocation(self) -> bool
 - get_loaded_dataset(self) -> List[LoadedDataset]:
 - get_datasets -> List[Dataset]
 - delete_dataset(dataset_id: str) -> bool
 - load_dataset(self, dataset_id: str) -> bool
 - unload_dataset(self, dataset_id: str) -> bool
 - search(self, dataset_id: str, query: List[List[float]], topk: int = 5) -> SearchResponse
+- create_dataset(dataset_id: Optional[str] = None) -> CreateDatasetResponse
+- add_chunk(dataset_id: str, list_documents: List[dict]) -> Response
+- train_dataset(dataset_id: str) -> Response
+- train_status(dataset_id: str) -> TrainStatus
+- get_dataset(dataset_id: str) -> Dataset
+- delete_document(dataset_id: str, document_id: List[str] = None, delete_all: bool = False) -> ResponseDeleteDocument
 ---
 
 ***example:***
 
-***from searchium import fvs***
+***import searchium***
 
-***client = fvs.get_client("your_allocation_id", "your_url")***
+***searchium.init("your_allocation_id", "your_url")***
 
-***dataset_id = 'your_dataset_id'***
+***dataset_id = 'your_dataset_uuid'***
 
-***client.load_dataset(dataset_id)***
+***searchium.create_dataset(dataset_id)***
 
-***client.search(dataset_id, query, 1)***
+***searchium.add_chunk(dataset_id: str, [{"document_id": str=doc_id, "vector": List[float]=embedding, "metadata": dict=metadata}])***
 
-***client.unload_dataset(dataset_id)***
+***searchium.train_dataset(dataset_id)***
+
+***searchium.load_dataset(dataset_id)***
+
+***searchium.search(dataset_id: str, query: List[List[float]], topk: int = 5)***
+
+***searchium.unload_dataset(dataset_id)***
```

