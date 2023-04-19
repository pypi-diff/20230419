# Comparing `tmp/dynamobase-0.2.2.tar.gz` & `tmp/dynamobase-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamobase-0.2.2.tar", last modified: Tue Feb 28 21:11:59 2023, max compression
+gzip compressed data, was "dynamobase-1.0.0.tar", last modified: Wed Apr 19 04:15:40 2023, max compression
```

## Comparing `dynamobase-0.2.2.tar` & `dynamobase-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-02-28 21:11:59.063331 dynamobase-0.2.2/
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     1066 2022-10-26 21:39:47.000000 dynamobase-0.2.2/LICENSE
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     6369 2023-02-28 21:11:59.063209 dynamobase-0.2.2/PKG-INFO
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     5833 2023-02-28 21:05:06.000000 dynamobase-0.2.2/README.md
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      675 2023-02-28 21:05:34.000000 dynamobase-0.2.2/pyproject.toml
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       38 2023-02-28 21:11:59.063375 dynamobase-0.2.2/setup.cfg
-drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-02-28 21:11:59.061700 dynamobase-0.2.2/src/
-drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-02-28 21:11:59.062540 dynamobase-0.2.2/src/DynamoBase.egg-info/
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     6369 2023-02-28 21:11:59.000000 dynamobase-0.2.2/src/DynamoBase.egg-info/PKG-INFO
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      442 2023-02-28 21:11:59.000000 dynamobase-0.2.2/src/DynamoBase.egg-info/SOURCES.txt
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)        1 2023-02-28 21:11:59.000000 dynamobase-0.2.2/src/DynamoBase.egg-info/dependency_links.txt
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       34 2023-02-28 21:11:59.000000 dynamobase-0.2.2/src/DynamoBase.egg-info/requires.txt
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       11 2023-02-28 21:11:59.000000 dynamobase-0.2.2/src/DynamoBase.egg-info/top_level.txt
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     4706 2023-02-28 21:03:17.000000 dynamobase-0.2.2/src/DynamoBase.py
-drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-02-28 21:11:59.062848 dynamobase-0.2.2/tests/
--rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      400 2022-10-27 03:26:22.000000 dynamobase-0.2.2/tests/test.py
+drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-04-19 04:15:40.903353 dynamobase-1.0.0/
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     1066 2022-10-26 21:39:47.000000 dynamobase-1.0.0/LICENSE
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     6809 2023-04-19 04:15:40.903197 dynamobase-1.0.0/PKG-INFO
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     6273 2023-04-19 04:13:51.000000 dynamobase-1.0.0/README.md
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      675 2023-04-19 04:14:29.000000 dynamobase-1.0.0/pyproject.toml
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       38 2023-04-19 04:15:40.903401 dynamobase-1.0.0/setup.cfg
+drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-04-19 04:15:40.901094 dynamobase-1.0.0/src/
+drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-04-19 04:15:40.902284 dynamobase-1.0.0/src/DynamoBase.egg-info/
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     6809 2023-04-19 04:15:40.000000 dynamobase-1.0.0/src/DynamoBase.egg-info/PKG-INFO
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      442 2023-04-19 04:15:40.000000 dynamobase-1.0.0/src/DynamoBase.egg-info/SOURCES.txt
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)        1 2023-04-19 04:15:40.000000 dynamobase-1.0.0/src/DynamoBase.egg-info/dependency_links.txt
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       34 2023-04-19 04:15:40.000000 dynamobase-1.0.0/src/DynamoBase.egg-info/requires.txt
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)       11 2023-04-19 04:15:40.000000 dynamobase-1.0.0/src/DynamoBase.egg-info/top_level.txt
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)     5833 2023-04-19 04:08:17.000000 dynamobase-1.0.0/src/DynamoBase.py
+drwxr-xr-x   0 jack.yang (573133226) TLC\Domain Users (1611651953)        0 2023-04-19 04:15:40.902655 dynamobase-1.0.0/tests/
+-rw-r--r--   0 jack.yang (573133226) TLC\Domain Users (1611651953)      400 2022-10-27 03:26:22.000000 dynamobase-1.0.0/tests/test.py
```

### Comparing `dynamobase-0.2.2/LICENSE` & `dynamobase-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamobase-0.2.2/PKG-INFO` & `dynamobase-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamobase
-Version: 0.2.2
+Version: 1.0.0
 Summary: A Json Model that is the easiest way to query DynamoDB.
 Author-email: Jaguar <jack.v.yang@gmail.com>
 Project-URL: Homepage, https://github.com/jaguaryang/dynamo-base
 Project-URL: Bug Tracker, https://github.com/jaguaryang/dynamo-base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DynamoBase
 
 A lightweight JSON model that simplifies DynamoDB's obscure query operations. It retains all original parameters and supports DynamoDB versions and future upgrades.
 
+# What can be done:
+
+1. Query condition is JSON format
+2. No need to consider complex expressions no matter query or update
+3. Column names can be any reserved keywords
+4. Return result correctly returns int, float, number types
+5. New function get_first can get the frist item by GSI/LSI
+
+# What can't be done:
+<del>Create, modify, and drop DynamoDB tables</del>
+
 # Install
 
 ```
 pip install dynamobase
 ```
 
 # Use
@@ -29,22 +40,20 @@
 ```
 from DynamoBase import DynamoBase
 
 DynamoBase.table_region = "ap-southeast-2"
 DynamoBase.table_name = "users"
 DynamoBase.session = ... # if you need specific settings like aws profile, credentials etc.
 
-# scan
-data = DynamoBase.scan(IndexName="ix_name")
-
 # get a single item
 user = DynamoBase.get_item(query={"first_name": "Jackson"})
 print(user)
 
 # get a list of items, IndexName is optional
+# query relate to KeyConditions, filter relate to FilterExpression
 user = DynamoBase.get_items(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
 # get the first item, IndexName is optional
 user = DynamoBase.get_first(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
@@ -164,14 +173,15 @@
 ## get_item
 
 ### parameters
 
 | Name  | Type | Example     | description                              |
 | ----- | ---- | ----------- | ---------------------------------------- |
 | query | dict | {"id": 123} | query must be primary key (and sort key) |
+| filter | dict | {"id": 123} | any fields and any values |
 
 ### return: Dict or None
 
 ## get_items
 
 ### parameters: The parameters supported by `get_items` and `get_first` are as follows:
```

### Comparing `dynamobase-0.2.2/README.md` & `dynamobase-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # DynamoBase
 
 A lightweight JSON model that simplifies DynamoDB's obscure query operations. It retains all original parameters and supports DynamoDB versions and future upgrades.
 
+# What can be done:
+
+1. Query condition is JSON format
+2. No need to consider complex expressions no matter query or update
+3. Column names can be any reserved keywords
+4. Return result correctly returns int, float, number types
+5. New function get_first can get the frist item by GSI/LSI
+
+# What can't be done:
+<del>Create, modify, and drop DynamoDB tables</del>
+
 # Install
 
 ```
 pip install dynamobase
 ```
 
 # Use
@@ -15,22 +26,20 @@
 ```
 from DynamoBase import DynamoBase
 
 DynamoBase.table_region = "ap-southeast-2"
 DynamoBase.table_name = "users"
 DynamoBase.session = ... # if you need specific settings like aws profile, credentials etc.
 
-# scan
-data = DynamoBase.scan(IndexName="ix_name")
-
 # get a single item
 user = DynamoBase.get_item(query={"first_name": "Jackson"})
 print(user)
 
 # get a list of items, IndexName is optional
+# query relate to KeyConditions, filter relate to FilterExpression
 user = DynamoBase.get_items(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
 # get the first item, IndexName is optional
 user = DynamoBase.get_first(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
@@ -150,14 +159,15 @@
 ## get_item
 
 ### parameters
 
 | Name  | Type | Example     | description                              |
 | ----- | ---- | ----------- | ---------------------------------------- |
 | query | dict | {"id": 123} | query must be primary key (and sort key) |
+| filter | dict | {"id": 123} | any fields and any values |
 
 ### return: Dict or None
 
 ## get_items
 
 ### parameters: The parameters supported by `get_items` and `get_first` are as follows:
```

### Comparing `dynamobase-0.2.2/pyproject.toml` & `dynamobase-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamobase"
-version = "0.2.2"
+version = "1.0.0"
 authors = [
   { name="Jaguar", email="jack.v.yang@gmail.com" },
 ]
 description = "A Json Model that is the easiest way to query DynamoDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `dynamobase-0.2.2/src/DynamoBase.egg-info/PKG-INFO` & `dynamobase-1.0.0/src/DynamoBase.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamobase
-Version: 0.2.2
+Version: 1.0.0
 Summary: A Json Model that is the easiest way to query DynamoDB.
 Author-email: Jaguar <jack.v.yang@gmail.com>
 Project-URL: Homepage, https://github.com/jaguaryang/dynamo-base
 Project-URL: Bug Tracker, https://github.com/jaguaryang/dynamo-base/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DynamoBase
 
 A lightweight JSON model that simplifies DynamoDB's obscure query operations. It retains all original parameters and supports DynamoDB versions and future upgrades.
 
+# What can be done:
+
+1. Query condition is JSON format
+2. No need to consider complex expressions no matter query or update
+3. Column names can be any reserved keywords
+4. Return result correctly returns int, float, number types
+5. New function get_first can get the frist item by GSI/LSI
+
+# What can't be done:
+<del>Create, modify, and drop DynamoDB tables</del>
+
 # Install
 
 ```
 pip install dynamobase
 ```
 
 # Use
@@ -29,22 +40,20 @@
 ```
 from DynamoBase import DynamoBase
 
 DynamoBase.table_region = "ap-southeast-2"
 DynamoBase.table_name = "users"
 DynamoBase.session = ... # if you need specific settings like aws profile, credentials etc.
 
-# scan
-data = DynamoBase.scan(IndexName="ix_name")
-
 # get a single item
 user = DynamoBase.get_item(query={"first_name": "Jackson"})
 print(user)
 
 # get a list of items, IndexName is optional
+# query relate to KeyConditions, filter relate to FilterExpression
 user = DynamoBase.get_items(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
 # get the first item, IndexName is optional
 user = DynamoBase.get_first(query={"first_name": "Jackson"}, IndexName='ix_name')
 print(user)
 
@@ -164,14 +173,15 @@
 ## get_item
 
 ### parameters
 
 | Name  | Type | Example     | description                              |
 | ----- | ---- | ----------- | ---------------------------------------- |
 | query | dict | {"id": 123} | query must be primary key (and sort key) |
+| filter | dict | {"id": 123} | any fields and any values |
 
 ### return: Dict or None
 
 ## get_items
 
 ### parameters: The parameters supported by `get_items` and `get_first` are as follows:
```

### Comparing `dynamobase-0.2.2/src/DynamoBase.py` & `dynamobase-1.0.0/src/DynamoBase.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,49 +4,76 @@
 
 class DynamoBase:
     table_region = "us-east-1"
     table_name = None
     session = boto3.Session()
 
     @classmethod
-    def scan(cls, **kwargs):
-        response = cls._table().scan(**kwargs)
-        res = json.loads(json.dumps(response["Items"]))
-        return res
-
-    @classmethod
     def get_item(cls, **kwargs):
         query = kwargs["query"]
         response = cls._table().get_item(Key=query)
         if "Item" not in response:
             return None
         res = json.loads(json.dumps(response["Item"]))
         return res
 
     @classmethod
     def get_items(cls, **kwargs):
-        query = kwargs["query"]
-        expression = cls._KeyConditionExpression(query)
         params = kwargs.copy()
-        params.pop("query", None)
         params.pop("TableName", None)
+        params.pop("ExpressionAttributeNames", None)
+        params.pop("ExpressionAttributeValues", None)
+        expression = {"ExpressionAttributeNames": {}, "ExpressionAttributeValues": {}}
+
+        # query
+        if "query" in kwargs:
+            params.pop("query", None)
+            exp = cls._KeyConditionExpression(kwargs["query"])
+            params["KeyConditionExpression"] = " and ".join(exp["Expression"])
+            expression["ExpressionAttributeNames"] = {
+                **expression["ExpressionAttributeNames"],
+                **exp["ExpressionAttributeNames"],
+            }
+            expression["ExpressionAttributeValues"] = {
+                **expression["ExpressionAttributeValues"],
+                **exp["ExpressionAttributeValues"],
+            }
+
+        # filter
+        if "filter" in kwargs:
+            params.pop("filter", None)
+            exp = cls._KeyConditionExpression(kwargs["filter"])
+            params["FilterExpression"] = " and ".join(exp["Expression"])
+            expression["ExpressionAttributeNames"] = {
+                **expression["ExpressionAttributeNames"],
+                **exp["ExpressionAttributeNames"],
+            }
+            expression["ExpressionAttributeValues"] = {
+                **expression["ExpressionAttributeValues"],
+                **exp["ExpressionAttributeValues"],
+            }
+
+        # Necessary for ProjectionExpression
         if "ExpressionAttributeNames" in kwargs:
             expression["ExpressionAttributeNames"] = {
                 **expression["ExpressionAttributeNames"],
                 **kwargs["ExpressionAttributeNames"],
             }
-        params.pop("KeyConditionExpression", None)
-        params.pop("ExpressionAttributeNames", None)
-        params.pop("ExpressionAttributeValues", None)
-        response = cls._table().query(
-            **params,
-            KeyConditionExpression=" and ".join(expression["Expression"]),
-            ExpressionAttributeNames=expression["ExpressionAttributeNames"],
-            ExpressionAttributeValues=expression["ExpressionAttributeValues"],
-        )
+
+        # Merge expression to params
+        if expression["ExpressionAttributeNames"]:
+            params["ExpressionAttributeNames"] = expression["ExpressionAttributeNames"]
+        if expression["ExpressionAttributeValues"]:
+            params["ExpressionAttributeValues"] = expression["ExpressionAttributeValues"]
+
+        if "query" in kwargs:
+            response = cls._table().query(**params)
+        else:
+            response = cls._table().scan(**params)
+
         res = json.loads(json.dumps(response["Items"]))
         return res
 
     @classmethod
     def get_first(cls, **kwargs):
         items = cls.get_items(**kwargs, Limit=1)
         return items[0] if items else None
```

