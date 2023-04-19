# Comparing `tmp/aliendev_api-0.1.0.tar.gz` & `tmp/aliendev_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliendev_api-0.1.0.tar", max compression
+gzip compressed data, was "aliendev_api-0.1.1.tar", max compression
```

## Comparing `aliendev_api-0.1.0.tar` & `aliendev_api-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435969 aliendev_api-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 17:45:56.435917 aliendev_api-0.1.0/aliendev_api/__init__.py
--rw-r--r--   0        0        0      824 2023-04-19 13:51:07.507395 aliendev_api-0.1.0/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0      479 2023-04-19 18:47:44.244132 aliendev_api-0.1.0/aliendev_api/config/mongo.py
--rw-r--r--   0        0        0     1355 2023-04-19 18:49:13.198039 aliendev_api-0.1.0/aliendev_api/main.py
--rw-r--r--   0        0        0      358 2023-04-19 13:21:11.067455 aliendev_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 aliendev_api-0.1.0/setup.py
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 aliendev_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 19:50:51.111602 aliendev_api-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 19:50:51.111602 aliendev_api-0.1.1/aliendev_api/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-19 19:50:51.111602 aliendev_api-0.1.1/aliendev_api/config/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0      479 2023-04-19 19:50:51.111602 aliendev_api-0.1.1/aliendev_api/config/mongo.py
+-rw-r--r--   0        0        0     2325 2023-04-19 19:50:51.111602 aliendev_api-0.1.1/aliendev_api/main.py
+-rw-r--r--   0        0        0      379 2023-04-19 19:50:51.115602 aliendev_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 aliendev_api-0.1.1/PKG-INFO
```

### Comparing `aliendev_api-0.1.0/aliendev_api/config/__pycache__/mongo.cpython-311.pyc` & `aliendev_api-0.1.1/aliendev_api/config/__pycache__/mongo.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5af13f64 (Wed Apr 19 13:49:14 2023 UTC)
+moddate:  0x50374064 (Wed Apr 19 18:47:44 2023 UTC)
 files sz: 479
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `aliendev_api-0.1.0/aliendev_api/main.py` & `aliendev_api-0.1.1/aliendev_api/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,77 @@
 from bson.objectid import ObjectId
 from aliendev_api.config import mongo
+from pydantic import BaseModel, Field
+from enum import Enum
 
 def _case(param: str):
     splitter = param.lower().replace(" ", "-")
     return splitter
 
 
 method_name = ["GET", "POST", "PUT", "DELETE"]
 
+class ParamType(Enum):
+    param = 'Param'
+    body = 'Body'
+
+class ParamData(BaseModel):
+    key: str = Field(..., example="name")
+    data_type: str = Field(..., example="string|int|any")
+    required: bool
+
 
 class ApiGateway:
     def __init__(self, username, title) -> None:
         self.username = username
         self.title = title
         self.stack_name = _case(title)
         self.endpoint = []
 
-    def addMethod(self, method, prefix):
+    def addMethod(self, method, prefix, param_type:ParamType, data:ParamData):
+        """
+        Args:
+            method (string): "GET|POST|PUT|DELETE"
+            prefix (string): "/test-get"
+            param_type (ParamType): "param|body"
+            data (ParamData): [
+                        {
+                        "key": "name",
+                        "data_type": "string",
+                        "required": true
+                        },
+                        {
+                        "key": "age",
+                        "data_type": "int",
+                        "required": false
+                        }
+                    ]
+        """
         if method in method_name:
             endpoint = {
                 "method": method,
-                "prefix": prefix
+                "prefix": prefix,
+                "param_type":param_type,
+                "data":data
             }
             self.endpoint.append(endpoint)
 
     def build(self):
         objId = ObjectId()
         result_data = {
             "_id": str(objId),
             "username": self.username,
             "title": self.title,
             "stack_name": self.stack_name,
             "endpoint": self.endpoint
         }
         client, db = mongo.connect()
         with client:
-            finder = db['gateway'].find_one({"$and":[{"username":self.username},{"stack_name":self.stack_name}]})
+            finder = db['gateway'].find_one(
+                {"$and": [{"username": self.username}, {"stack_name": self.stack_name}]})
             if finder:
-                newvalues = { "$set": { "endpoint": self.endpoint } }
-                db['gateway'].update_one({"_id":finder['_id']},newvalues)
+                newvalues = {"$set": {"endpoint": self.endpoint}}
+                db['gateway'].update_one({"_id": finder['_id']}, newvalues)
             else:
                 db['gateway'].insert_one(result_data)
-                
+
         return result_data
```

