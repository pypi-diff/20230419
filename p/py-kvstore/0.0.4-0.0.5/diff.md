# Comparing `tmp/py_kvstore-0.0.4.tar.gz` & `tmp/py_kvstore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_kvstore-0.0.4.tar", last modified: Tue Apr 18 05:44:11 2023, max compression
+gzip compressed data, was "py_kvstore-0.0.5.tar", last modified: Wed Apr 19 20:02:00 2023, max compression
```

## Comparing `py_kvstore-0.0.4.tar` & `py_kvstore-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/
--rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)       13 2023-04-18 03:31:33.000000 py_kvstore-0.0.4/README.md
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/py_kvstore/
--rw-r--r--   0 reece     (1000) reece     (1001)       78 2023-04-18 04:17:04.000000 py_kvstore-0.0.4/py_kvstore/__init__.py
--rw-r--r--   0 reece     (1000) reece     (1001)     6528 2023-04-18 05:41:02.000000 py_kvstore-0.0.4/py_kvstore/py_kvstore.py
--rw-r--r--   0 reece     (1000) reece     (1001)     1840 2023-04-18 04:20:33.000000 py_kvstore-0.0.4/py_kvstore/test.py
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/py_kvstore.egg-info/
--rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/SOURCES.txt
--rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/dependency_links.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-18 05:44:11.000000 py_kvstore-0.0.4/py_kvstore.egg-info/top_level.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-18 05:44:11.240211 py_kvstore-0.0.4/setup.cfg
--rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-18 05:44:09.000000 py_kvstore-0.0.4/setup.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 20:02:00.275770 py_kvstore-0.0.5/
+-rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-19 20:02:00.275770 py_kvstore-0.0.5/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)       13 2023-04-18 03:31:33.000000 py_kvstore-0.0.5/README.md
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 20:02:00.275770 py_kvstore-0.0.5/py_kvstore/
+-rw-r--r--   0 reece     (1000) reece     (1001)       78 2023-04-18 04:17:04.000000 py_kvstore-0.0.5/py_kvstore/__init__.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     7936 2023-04-19 20:01:41.000000 py_kvstore-0.0.5/py_kvstore/py_kvstore.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     3401 2023-04-19 20:00:40.000000 py_kvstore-0.0.5/py_kvstore/test.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 20:02:00.275770 py_kvstore-0.0.5/py_kvstore.egg-info/
+-rw-r--r--   0 reece     (1000) reece     (1001)      662 2023-04-19 20:02:00.000000 py_kvstore-0.0.5/py_kvstore.egg-info/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-19 20:02:00.000000 py_kvstore-0.0.5/py_kvstore.egg-info/SOURCES.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-19 20:02:00.000000 py_kvstore-0.0.5/py_kvstore.egg-info/dependency_links.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-19 20:02:00.000000 py_kvstore-0.0.5/py_kvstore.egg-info/top_level.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-19 20:02:00.275770 py_kvstore-0.0.5/setup.cfg
+-rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-19 19:32:59.000000 py_kvstore-0.0.5/setup.py
```

### Comparing `py_kvstore-0.0.4/PKG-INFO` & `py_kvstore-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_kvstore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `py_kvstore-0.0.4/py_kvstore/py_kvstore.py` & `py_kvstore-0.0.5/py_kvstore/py_kvstore.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,48 +3,78 @@
 # if no timeout is specified, set it as -1.
 
 import json
 import os
 import re as regex
 import time
 from dataclasses import dataclass
+from enum import Enum
 from typing import Any, Optional
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 
 
+class StoreType(Enum):
+    PAIR = "pair"
+    HASHSET = "hashset"
+
+    def __str__(self):
+        return self.value
+
+
 @dataclass
 class Pair:
     value: Any
     timeout: int
+    store_type: str = str(StoreType.PAIR)
 
     def toJSON(self):
-        return {"value": self.value, "timeout": self.timeout}
+        return {
+            "value": self.value,
+            "timeout": self.timeout,
+            "ttl_seconds": (
+                -1 if self.timeout == -1 else self.timeout - int(time.time())
+            ),
+        }
 
     @staticmethod
     def fromJSON(json: dict):
         return Pair(json["value"], json["timeout"])
 
 
 @dataclass
 class HashSet(Pair):
     value: dict[str, Any]
     timeout: int
+    store_type: str = str(StoreType.HASHSET)
 
 
 class KVStore:
     # TODO: Specify in memory or on the disk (slower, but better for large data sets)
-    def __init__(self, name: Optional[str] = None, dump_dir=None):
+    def __init__(self, name: Optional[str] = None, dump_dir: str = ""):
         self.name = name
         self.store: dict[str, Pair] = {}
 
         self.dump_dir = current_dir
-        if dump_dir is not None:
+        if len(dump_dir) > 0:
             self.dump_dir = dump_dir
 
+    def get_dump_dir(self):
+        return self.dump_dir
+
+    def get_dump_file(self):
+        return os.path.join(self.dump_dir, f"{self.name}.json")
+
+    def __check_type(self, key: str, store_type: StoreType):
+        if self.store[key].store_type != str(store_type):
+            raise Exception(f"Key {key} is not a {store_type}")
+
+    def __value_not_expired(self, value: Pair | HashSet):
+        return value.timeout == -1 or value.timeout > int(time.time())
+
     def set(self, key: str, value: Any, timeout: int = -1):
         """
         -1: no timeout
         0: delete key time
         > 0: timeout in seconds (epoch)
         """
         if len(key) == 0:
@@ -63,15 +93,19 @@
     # hash set and hash get
     # You can only set the expire time on creation?
     def hset(self, key: str, field: str, value: Any, timeout: int = -1):
         self.delete_expired_data_if_applicable(key)
 
         if key not in self.store:
             # timeout can only be set on creation
-            self.store[key] = HashSet({}, timeout)
+            current_time = int(time.time())
+            self.store[key] = HashSet({}, current_time + timeout)
+        else:
+            if self.store[key].store_type != "hashset":
+                raise Exception(f"Key {key} is not a hashset")
 
         # grab the current hset
         hset = self.store[key].value
         hset[field] = value
         # reset the store value
         self.store[key].value = hset
 
@@ -85,118 +119,133 @@
         self.delete_expired_data_if_applicable(key)
         if key not in self.store:
             return None
 
         if field not in self.store[key].value:
             return None
 
+        self.__check_type(key, StoreType.HASHSET)
+
         return self.store[key].value[field]
 
     def incr(self, key: str, amount: int = 1) -> int:
         """Returns the new value"""
         if key not in self.store:
             self.set(key, amount)
             return amount
 
-        # what if key value is not an int?
+        self.__check_type(key, StoreType.PAIR)
+
         if not isinstance(self.store[key].value, int):
             raise Exception(f"key:{key}'s value is not an int")
 
         self.store[key].value += amount
         return self.store[key].value
 
     def get(self, key) -> Any | None:
         self.delete_expired_data_if_applicable(key)
 
         if key in self.store:
+            self.__check_type(key, StoreType.PAIR)
+
             return self.store[key].value
         return None
 
     def get_keys(self, search_regex: str = "") -> list[str]:
         search_regex = search_regex.replace("*", ".+")
         self.delete_all_expired_data()
         if len(search_regex) == 0:
             return list(self.store.keys())
         else:
             return [k for k in self.store.keys() if regex.match(search_regex, k)]
 
-    def delete(self, *keys) -> bool:
+    def delete(self, keys: str | list[str]) -> bool:
+        if isinstance(keys, str):
+            keys = [keys]
+
         for key in keys:
             if key in self.store:
                 del self.store[key]
             else:
                 return False
         return True
 
     def clear(self):
-        self.store = {}
+        self.store.clear()
 
     def ttl(self, key) -> int:
         self.delete_expired_data_if_applicable(key)
         if key in self.store:
             p = self.store[key]
             return p.timeout
         return -2
 
     def dbg(self):
         self.delete_all_expired_data()
         print("dbg", self.name, self.dump_dir, self.store)
 
     def delete_all_expired_data(self):
-        current_time = int(time.time())
         self.store = {
-            k: v
-            for k, v in self.store.items()
-            if v.timeout >= current_time or v.timeout == -1
+            k: v for k, v in self.store.items() if self.__value_not_expired(v)
         }
 
-    def delete_expired_data_if_applicable(self, key: str) -> bool:
-        if key in self.store:
-            timeout = self.store[key].timeout
-            if timeout >= 0 and timeout < int(time.time()):
-                del self.store[key]
-                return True
-        return False
+    def delete_expired_data_if_applicable(self, keys: str | list[str]) -> int:
+        """
+        Returns an int of the number of keys removed
+        """
+        if isinstance(keys, str):
+            keys = [keys]
 
-    def dump(self):
-        file = os.path.join(self.dump_dir, f"{self.name}.json")
-        # print("Dumping to file", file)
+        found = 0
+        for k in keys:
+            if k in self.store:
+                timeout = self.store[k].timeout
+                if timeout >= 0 and timeout <= int(time.time()):
+                    del self.store[k]
+                    found += 1
+        return found
 
+    def dump(self):
+        file = self.get_dump_file()
         with open(file, "w") as f:
             json.dump(
                 self.store,
                 f,
                 default=lambda o: o.toJSON(),
             )
         self.delete_all_expired_data()
 
     def load(self):
         current_time = int(time.time())
 
-        file = os.path.join(self.dump_dir, f"{self.name}.json")
+        file = self.get_dump_file()
         if not os.path.isfile(file):
             return
 
         with open(file, "r") as f:
             pre_store = json.load(f)
 
         for key, value in pre_store.items():
             p = Pair.fromJSON(value)
-            if p.timeout <= current_time and p.timeout != -1:
-                continue
-            self.store[key] = p
+            if self.__value_not_expired(p):
+                self.store[key] = p
 
     # def __del__(self):
     #     # on close of program, dump the data to a file
     #     # print("Garbage Collection: Dumping to file for storage")
     #     self.dump()
 
     def __str__(self):
+        self.delete_all_expired_data()
         return f"Name: {self.name}, Store Keys Amount: {len(self.store)}"
 
+    def to_json(self) -> dict:
+        self.delete_all_expired_data()
+        return json.loads(json.dumps(self.store, default=lambda o: o.toJSON()))
+
 
 def main():
     kv1 = KVStore(name="transactions")
 
     if True:
         kv1.set("dict", {"test": "other value"})
         kv1.set("list", [])
```

### Comparing `py_kvstore-0.0.4/py_kvstore.egg-info/PKG-INFO` & `py_kvstore-0.0.5/py_kvstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-kvstore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `py_kvstore-0.0.4/setup.py` & `py_kvstore-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # pip install twine
 # python setup.py bdist
 # twine upload -r py_kvstore dist/*
 
 setup(
     name="py_kvstore",
-    version="0.0.4",
+    version="0.0.5",
     description="A key value store",
     url="https://github.com/Reecepbcups/py_kvstore",
     author="Reece Willims",
     author_email="reecepbcups@gmail.com",
     license="Apache 2.0",
     packages=["py_kvstore"],
     install_requires=[],
```

