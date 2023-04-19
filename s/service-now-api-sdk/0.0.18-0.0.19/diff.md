# Comparing `tmp/service_now_api_sdk-0.0.18.tar.gz` & `tmp/service_now_api_sdk-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_now_api_sdk-0.0.18.tar", max compression
+gzip compressed data, was "service_now_api_sdk-0.0.19.tar", max compression
```

## Comparing `service_now_api_sdk-0.0.18.tar` & `service_now_api_sdk-0.0.19.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-04-19 14:40:58.045647 service_now_api_sdk-0.0.18/LICENSE
--rw-r--r--   0        0        0     6427 2023-04-19 14:44:48.295647 service_now_api_sdk-0.0.18/README.md
--rw-r--r--   0        0        0      565 2023-04-19 14:46:11.185647 service_now_api_sdk-0.0.18/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/__init__.py
--rw-r--r--   0        0        0       43 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/exceptions.py
--rw-r--r--   0        0        0      140 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-19 14:44:23.995647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/attachments/client.py
--rw-r--r--   0        0        0      227 2023-04-19 14:30:26.705647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
--rw-r--r--   0        0        0     2874 2023-04-19 14:44:48.295647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/helpers/client.py
--rw-r--r--   0        0        0    10869 2023-04-19 14:30:26.705647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
--rw-r--r--   0        0        0        0 2023-04-19 14:20:40.875647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/table/__init__.py
--rw-r--r--   0        0        0    15486 2023-04-19 14:44:23.995647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/table/client.py
--rw-r--r--   0        0        0      818 2023-04-19 14:30:26.715647 service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/table/exceptions.py
--rw-r--r--   0        0        0      255 2023-04-19 14:44:48.295647 service_now_api_sdk-0.0.18/service_now_api_sdk/settings.py
--rw-r--r--   0        0        0     6771 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/LICENSE
+-rw-r--r--   0        0        0     6564 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/README.md
+-rw-r--r--   0        0        0      565 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/exceptions.py
+-rw-r--r--   0        0        0      140 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/client.py
+-rw-r--r--   0        0        0      227 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/client.py
+-rw-r--r--   0        0        0    10869 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/__init__.py
+-rw-r--r--   0        0        0    15486 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/client.py
+-rw-r--r--   0        0        0      818 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/exceptions.py
+-rw-r--r--   0        0        0      255 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/settings.py
+-rw-r--r--   0        0        0     6906 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.19/PKG-INFO
```

### Comparing `service_now_api_sdk-0.0.18/LICENSE` & `service_now_api_sdk-0.0.19/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Guilherme Laércio da Silva
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `service_now_api_sdk-0.0.18/README.md` & `service_now_api_sdk-0.0.19/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# service_now_api_sdk
+# ServiceNow API SDK
 [![PyPI Latest Release](https://img.shields.io/pypi/v/service-now-api-sdk.svg)](https://pypi.org/project/service-now-api-sdk/)
-[![Downloads](https://pepy.tech/badge/service-now-api-sdk/month)](https://pepy.tech/project/service-now-api-sdk)
 
-Interact with ServiceNow functionalities within your python application, includes the ability to perform create, read, update, and delete (CRUD) operations on existing tables, insert data into, retrieve information from and submit tickets.
+Check out our [GitHub Repository](https://github.com/guilhermelaercio/service_now_api_sdk)!
+
+Check out [ServiceNow REST API documentation](https://docs.servicenow.com/en-US/bundle/sandiego-application-development/page/build/applications/concept/api-rest.html).
+
+Interact with ServiceNow functionalities for your python application, includes the ability to perform create, read, update, and delete (CRUD) operations on existing tables, insert data into, retrieve information from and submit tickets.
 ## Installation
 ```sh
-# or PyPI
 pip install service-now-api-sdk
 ```
 
 # Environment variables
 To use service-now-api-sdk library, you need set four environment variables:
 ```dotenv
 # ---DOTENV EXAMPLE---
```

### Comparing `service_now_api_sdk-0.0.18/pyproject.toml` & `service_now_api_sdk-0.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "service_now_api_sdk"
-version = "0.0.18"
+version = "0.0.19"
 description = "Service Now API SDK is used to facilitate integrations, automations and also code reuse"
 authors = [
     "Guilherme Laercio da Silva <guilhermelaerciodasilva@gmail.com>",
     "Stone People Analytic <systems-techpeople@stone.com.br>"
 ]
 readme = "README.md"
```

### Comparing `service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/attachments/client.py` & `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/helpers/client.py` & `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py` & `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/table/client.py` & `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.18/service_now_api_sdk/sdk/servicenow/table/exceptions.py` & `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.18/PKG-INFO` & `service_now_api_sdk-0.0.19/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: service-now-api-sdk
-Version: 0.0.18
+Version: 0.0.19
 Summary: Service Now API SDK is used to facilitate integrations, automations and also code reuse
 Author: Guilherme Laercio da Silva
 Author-email: guilhermelaerciodasilva@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
-# service_now_api_sdk
+# ServiceNow API SDK
 [![PyPI Latest Release](https://img.shields.io/pypi/v/service-now-api-sdk.svg)](https://pypi.org/project/service-now-api-sdk/)
-[![Downloads](https://pepy.tech/badge/service-now-api-sdk/month)](https://pepy.tech/project/service-now-api-sdk)
 
-Interact with ServiceNow functionalities within your python application, includes the ability to perform create, read, update, and delete (CRUD) operations on existing tables, insert data into, retrieve information from and submit tickets.
+Check out our [GitHub Repository](https://github.com/guilhermelaercio/service_now_api_sdk)!
+
+Check out [ServiceNow REST API documentation](https://docs.servicenow.com/en-US/bundle/sandiego-application-development/page/build/applications/concept/api-rest.html).
+
+Interact with ServiceNow functionalities for your python application, includes the ability to perform create, read, update, and delete (CRUD) operations on existing tables, insert data into, retrieve information from and submit tickets.
 ## Installation
 ```sh
-# or PyPI
 pip install service-now-api-sdk
 ```
 
 # Environment variables
 To use service-now-api-sdk library, you need set four environment variables:
 ```dotenv
 # ---DOTENV EXAMPLE---
```

