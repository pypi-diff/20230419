# Comparing `tmp/pai_thin_client-1.0.0.tar.gz` & `tmp/pai_thin_client-1.0.1.tar.gz`

## Comparing `pai_thin_client-1.0.0.tar` & `pai_thin_client-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/objects.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/pai_client.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/components/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/components/pai_requests.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/components/pai_responses.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/components/pai_uris.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/src/paiclient/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    32957 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/tests/test_request_objects.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/LICENSE
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 pai_thin_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/objects.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/pai_client.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/components/__init__.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/components/pai_requests.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/components/pai_responses.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/components/pai_uris.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/src/paiclient/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    32957 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/tests/test_request_objects.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9418 2020-02-02 00:00:00.000000 pai_thin_client-1.0.1/PKG-INFO
```

### Comparing `pai_thin_client-1.0.0/.pytest_cache/v/cache/nodeids` & `pai_thin_client-1.0.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/objects.py` & `pai_thin_client-1.0.1/src/paiclient/objects.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/pai_client.py` & `pai_thin_client-1.0.1/src/paiclient/pai_client.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/components/pai_requests.py` & `pai_thin_client-1.0.1/src/paiclient/components/pai_requests.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/components/pai_responses.py` & `pai_thin_client-1.0.1/src/paiclient/components/pai_responses.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/components/pai_uris.py` & `pai_thin_client-1.0.1/src/paiclient/components/pai_uris.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/src/paiclient/components/request_objects.py` & `pai_thin_client-1.0.1/src/paiclient/components/request_objects.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/tests/test_request_objects.py` & `pai_thin_client-1.0.1/tests/test_request_objects.py`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/LICENSE` & `pai_thin_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pai_thin_client-1.0.0/README.md` & `pai_thin_client-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# pai-thin-client
+# pai_thin_client
 
 A client for communicating with the Private Ai de-identication api. This document provides information about how to best use the client. For more information, see Private Ai's [API Documentation.][1]
 
 ### Quick Links
 1. [Installation](#installation)
 2. [Quick Start](#quick-start)
 3. [Working with the Client](#client)
 4. [Request Objects](#request-objects)
 5. [Sample Use](#sample-use)
 
 ### Installation <a name=installation></a>
 
 ```
-pip install paiclient
+pip install pai_thin_client
 ```
 
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
-from paiclient import PAIClient
-from paiclient import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client import request_objects
 
 schema = "http"
 host = "localhost"
 port = "8080"
 
 client = PAIClient(schema=schema, host=host, port=port)
 
@@ -46,15 +46,15 @@
 
 #### Initializing the Client
 
 the PAI client requires a scheme, host and optional port to initialize.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from paiclient import PAIClient
+from pai_thin_client import PAIClient
 scheme = 'http'
 host = 'localhost'
 port= '8080'
 client = PAIClient(scheme, host, port)
  
 client.ping()
 ```
@@ -90,15 +90,15 @@
 ```
 ["This is [NAME_1]'s sample dictionary request"]
 ```
 
 or using built-in request objects:
 
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "This is John Smith's sample process text object request"
 text_request_object =  request_objects.process_text_obj(text=[sample_text])
 
 response = client.process_text(text_request_object)
 response.processed_text
 ```
@@ -107,27 +107,27 @@
 ["This is [NAME_1]'s sample process text object request"]
 ```
 
 
 ### Request Objects <a name=request-objects></a>
 Request objects are a simple way of creating request bodies without the tediousness of writing dictionaries. Every post request (as listed in the [Private-Ai documentation][1]) has its own request own request object. 
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_obj = request_objects.file_url_obj(uri='path/to/file.jpg')
 sample_obj.uri
 ```
 Output:
 ```
 'path/to/file.jpg'
 ```
 
 Additionally there are request objects for each nested dictionary of a request:
 ```python 
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "This is John Smith's sample process text object request where names won't be removed"
 
 # sub-dictionary of entity_detection
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['NAME', 'NAME_GIVEN', 'NAME_FAMILY'])
 
 # sub-dictionary of a process text request
@@ -157,15 +157,15 @@
                "content_type": "application/pdf"}
 
 sample_file_obj2 = request_objects.file_obj.fromdict(sample_dict)
 ```
 
 Request objects also can be formatted as dictionaries:
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "Sample text."
 # Create the nested request objects
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['HIPAA'])
 sample_entity_detection = request_objects.entity_detection_obj(entity_types=[sample_entity_type_selector])
 # Create the request object
 sample_request = request_objects.process_text_obj(text=[sample_text], entity_detection=sample_entity_detection)
@@ -182,16 +182,16 @@
  'processed_text': {'type': 'MARKER', 'pattern': '[UNIQUE_NUMBERED_ENTITY_TYPE]'}
 }
 ```
 
 ### Sample Use <a name=sample-use></a>
 #### Processing a directory of files
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import os
 import logging
 
 file_dir = "/path/to/file/directory"
 client = PAIClient("http", "localhost", "8080")
 for file_name in os.listdir(file_dir):
     filepath = os.path.join(file_dir, file_name)
@@ -201,16 +201,16 @@
     # NOTE this method of file processing requires the container to have an the input and output directories mounted
     resp = client.process_files_uri(req_obj)
     if not resp.ok:
         logging.error(f"response for file {file_name} returned with {resp.status_code}")
 ```
 #### Processing a Base64 file
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
@@ -233,16 +233,16 @@
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.processed_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
 #### Bleep an audio file
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
```

### Comparing `pai_thin_client-1.0.0/pyproject.toml` & `pai_thin_client-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "pai-thin-client"
-version = "1.0.0"
+name = "pai_thin_client"
+version = "1.0.1"
 authors = [
   { name="Adam Guiducci", email="adam.guiducci@private-ai.com" },
 ]
 description = "A thin client for communicating with the Private Ai de-identication api."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/privateai/pai-thin-client/"
-"Bug Tracker" = "https://github.com/privateai/pai-thin-client/issues"
+"Homepage" = "https://github.com/privateai/pai_thin_client/"
+"Bug Tracker" = "https://github.com/privateai/pai_thin_client/issues"
```

### Comparing `pai_thin_client-1.0.0/PKG-INFO` & `pai_thin_client-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
-Name: pai-thin-client
-Version: 1.0.0
+Name: pai_thin_client
+Version: 1.0.1
 Summary: A thin client for communicating with the Private Ai de-identication api.
-Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
-Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
+Project-URL: Homepage, https://github.com/privateai/pai_thin_client/
+Project-URL: Bug Tracker, https://github.com/privateai/pai_thin_client/issues
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# pai-thin-client
+# pai_thin_client
 
 A client for communicating with the Private Ai de-identication api. This document provides information about how to best use the client. For more information, see Private Ai's [API Documentation.][1]
 
 ### Quick Links
 1. [Installation](#installation)
 2. [Quick Start](#quick-start)
 3. [Working with the Client](#client)
 4. [Request Objects](#request-objects)
 5. [Sample Use](#sample-use)
 
 ### Installation <a name=installation></a>
 
 ```
-pip install paiclient
+pip install pai_thin_client
 ```
 
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
-from paiclient import PAIClient
-from paiclient import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client import request_objects
 
 schema = "http"
 host = "localhost"
 port = "8080"
 
 client = PAIClient(schema=schema, host=host, port=port)
 
@@ -60,15 +60,15 @@
 
 #### Initializing the Client
 
 the PAI client requires a scheme, host and optional port to initialize.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from paiclient import PAIClient
+from pai_thin_client import PAIClient
 scheme = 'http'
 host = 'localhost'
 port= '8080'
 client = PAIClient(scheme, host, port)
  
 client.ping()
 ```
@@ -104,15 +104,15 @@
 ```
 ["This is [NAME_1]'s sample dictionary request"]
 ```
 
 or using built-in request objects:
 
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "This is John Smith's sample process text object request"
 text_request_object =  request_objects.process_text_obj(text=[sample_text])
 
 response = client.process_text(text_request_object)
 response.processed_text
 ```
@@ -121,27 +121,27 @@
 ["This is [NAME_1]'s sample process text object request"]
 ```
 
 
 ### Request Objects <a name=request-objects></a>
 Request objects are a simple way of creating request bodies without the tediousness of writing dictionaries. Every post request (as listed in the [Private-Ai documentation][1]) has its own request own request object. 
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_obj = request_objects.file_url_obj(uri='path/to/file.jpg')
 sample_obj.uri
 ```
 Output:
 ```
 'path/to/file.jpg'
 ```
 
 Additionally there are request objects for each nested dictionary of a request:
 ```python 
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "This is John Smith's sample process text object request where names won't be removed"
 
 # sub-dictionary of entity_detection
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['NAME', 'NAME_GIVEN', 'NAME_FAMILY'])
 
 # sub-dictionary of a process text request
@@ -171,15 +171,15 @@
                "content_type": "application/pdf"}
 
 sample_file_obj2 = request_objects.file_obj.fromdict(sample_dict)
 ```
 
 Request objects also can be formatted as dictionaries:
 ```python
-from paiclient import request_objects
+from pai_thin_client import request_objects
 
 sample_text = "Sample text."
 # Create the nested request objects
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['HIPAA'])
 sample_entity_detection = request_objects.entity_detection_obj(entity_types=[sample_entity_type_selector])
 # Create the request object
 sample_request = request_objects.process_text_obj(text=[sample_text], entity_detection=sample_entity_detection)
@@ -196,16 +196,16 @@
  'processed_text': {'type': 'MARKER', 'pattern': '[UNIQUE_NUMBERED_ENTITY_TYPE]'}
 }
 ```
 
 ### Sample Use <a name=sample-use></a>
 #### Processing a directory of files
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import os
 import logging
 
 file_dir = "/path/to/file/directory"
 client = PAIClient("http", "localhost", "8080")
 for file_name in os.listdir(file_dir):
     filepath = os.path.join(file_dir, file_name)
@@ -215,16 +215,16 @@
     # NOTE this method of file processing requires the container to have an the input and output directories mounted
     resp = client.process_files_uri(req_obj)
     if not resp.ok:
         logging.error(f"response for file {file_name} returned with {resp.status_code}")
 ```
 #### Processing a Base64 file
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
@@ -247,16 +247,16 @@
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.processed_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
 #### Bleep an audio file
 ```python
-from paiclient import PAIClient
-from paiclient.objects import request_objects
+from pai_thin_client import PAIClient
+from pai_thin_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
```

