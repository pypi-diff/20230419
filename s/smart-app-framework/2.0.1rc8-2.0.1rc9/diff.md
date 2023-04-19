# Comparing `tmp/smart_app_framework-2.0.1rc8-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.0.1rc9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 300398 bytes, number of entries: 330
+Zip file size: 300573 bytes, number of entries: 330
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -48,15 +48,15 @@
 -rw-r--r--  2.0 unx     2413 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/ceph_adapter.py
 -rw-r--r--  2.0 unx      114 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/ceph_exception.py
 -rw-r--r--  2.0 unx     1265 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/ceph_io.py
 -rw-r--r--  2.0 unx     4325 b- defN 80-Jan-01 00:00 core/db_adapter/db_adapter.py
 -rw-r--r--  2.0 unx      223 b- defN 80-Jan-01 00:00 core/db_adapter/error.py
 -rw-r--r--  2.0 unx     3004 b- defN 80-Jan-01 00:00 core/db_adapter/ignite_adapter.py
 -rw-r--r--  2.0 unx     3041 b- defN 80-Jan-01 00:00 core/db_adapter/ignite_thread_adapter.py
--rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 core/db_adapter/memory_adapter.py
+-rw-r--r--  2.0 unx     1455 b- defN 80-Jan-01 00:00 core/db_adapter/memory_adapter.py
 -rw-r--r--  2.0 unx     1201 b- defN 80-Jan-01 00:00 core/db_adapter/os_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/descriptions/__init__.py
 -rw-r--r--  2.0 unx     1155 b- defN 80-Jan-01 00:00 core/descriptions/descriptions.py
 -rw-r--r--  2.0 unx     1662 b- defN 80-Jan-01 00:00 core/descriptions/descriptions_items.py
 -rw-r--r--  2.0 unx      626 b- defN 80-Jan-01 00:00 core/descriptions/smart_updatable_descriptions_items.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/logging/__init__.py
 -rw-r--r--  2.0 unx      568 b- defN 80-Jan-01 00:00 core/logging/logger_constants.py
@@ -322,11 +322,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     1504 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10421 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc8.dist-info/WHEEL
-?rw-r--r--  2.0 unx    31832 b- defN 16-Jan-01 00:00 smart_app_framework-2.0.1rc8.dist-info/RECORD
-330 files, 974223 bytes uncompressed, 248550 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx    10421 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc9.dist-info/WHEEL
+?rw-r--r--  2.0 unx    31832 b- defN 16-Jan-01 00:00 smart_app_framework-2.0.1rc9.dist-info/RECORD
+330 files, 974648 bytes uncompressed, 248725 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -975,17 +975,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc8.dist-info/METADATA
+Filename: smart_app_framework-2.0.1rc9.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc8.dist-info/WHEEL
+Filename: smart_app_framework-2.0.1rc9.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc8.dist-info/RECORD
+Filename: smart_app_framework-2.0.1rc9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## core/db_adapter/memory_adapter.py

```diff
@@ -1,16 +1,26 @@
-from core.db_adapter import error
 from core.db_adapter.db_adapter import AsyncDBAdapter
+from copy import copy
+from cachetools import TTLCache
+from core.db_adapter import error
 
 
 class MemoryAdapter(AsyncDBAdapter):
+    IS_ASYNC = True
+    MEM_CACHE_SIZE = 250 * 1024 * 1024
+    TTL = 12 * 60 * 60
 
     def __init__(self, config=None):
         super(AsyncDBAdapter, self).__init__(config)
-        self.memory_storage = {}
+        config = self.config or {}
+        self.init_params = copy(config.get("init_params", {}))
+        self.init_params["getsizeof"] = len
+        self.init_params.setdefault("maxsize", self.MEM_CACHE_SIZE)
+        self.init_params.setdefault("ttl", self.TTL)
+        self.memory_storage = TTLCache(**self.init_params)
 
     async def _glob(self, path, pattern):
         raise error.NotSupportedOperation
 
     async def _path_exists(self, path):
         raise error.NotSupportedOperation
```

## Comparing `smart_app_framework-2.0.1rc8.dist-info/METADATA` & `smart_app_framework-2.0.1rc9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.0.1rc8
+Version: 2.0.1rc9
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.10
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.0.1rc8.dist-info/RECORD` & `smart_app_framework-2.0.1rc9.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 core/db_adapter/ceph/ceph_adapter.py,sha256=hK8GB5pFaNEZ5hopJ2V_2ks4x7LktBcD5dkbdgPJ-vA,2413
 core/db_adapter/ceph/ceph_exception.py,sha256=UUFOfRdcUVbc-9wPUZVUjToRGSNI-kAbRWPqmf-tOqw,114
 core/db_adapter/ceph/ceph_io.py,sha256=fYKx67FBnj4GN5We6MbZ8zLzOBIbd6gDJtt8sUoEIxU,1265
 core/db_adapter/db_adapter.py,sha256=ibJxmTl0WtjHqft3OztIQiPlzRQoFHUoWYvlrTuIMxQ,4325
 core/db_adapter/error.py,sha256=bGYTrKT70VD-uD_oxErjnYUy9003kMdV8wXfSIbm860,223
 core/db_adapter/ignite_adapter.py,sha256=zzn3iKJJIgNEyV4MZAb0eifDkJi5cDF9X4prfCb3vxI,3004
 core/db_adapter/ignite_thread_adapter.py,sha256=du1xQ45aB5fz_r-NuFRbnqUORYitVmvR6ClqZuHE2GU,3041
-core/db_adapter/memory_adapter.py,sha256=WWBtNOORl7sdygjRG5QG6LjTIVcojQzVvS_jdVqi23c,1030
+core/db_adapter/memory_adapter.py,sha256=p58l07oT4SuyPJKSDZ20L8RjXfjC7V36pwwLnwQ7lm8,1455
 core/db_adapter/os_adapter.py,sha256=R_d35gZWNO6Tgj95h6nNf4jHX5cyj35WTQXys0NMNKY,1201
 core/descriptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/descriptions/descriptions.py,sha256=FGbN8EYbSm5FkIJDSrQgY7BJaKZjpn7sXxdWUzx3pIg,1155
 core/descriptions/descriptions_items.py,sha256=LWBTAOssEnFJKS94bsigV1vAzNSDoV_-OZEyh8cdavc,1662
 core/descriptions/smart_updatable_descriptions_items.py,sha256=997QG44D9DDyx9Kh7M_YHGzMNjTlAiMnsRT4kG4RO9g,626
 core/logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/logging/logger_constants.py,sha256=hn56NJa4uT94uZ56W7nVFxV8rJp2fczrBHJLhh2XFPM,568
@@ -321,10 +321,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=Xkum0YisA1jYcEh3MHIAfvJttmp3hwxnyhWK5UV12Pc,1504
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.0.1rc8.dist-info/METADATA,sha256=hGVmpZpgL6cZzdlogN4fv08dxm7ZOvMPnGPl3OgAxC0,10421
-smart_app_framework-2.0.1rc8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-smart_app_framework-2.0.1rc8.dist-info/RECORD,,
+smart_app_framework-2.0.1rc9.dist-info/METADATA,sha256=_sw8iOho61lpC1mMcFKwe1e-Ln173yh4YVq7Sqv_hp0,10421
+smart_app_framework-2.0.1rc9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+smart_app_framework-2.0.1rc9.dist-info/RECORD,,
```

