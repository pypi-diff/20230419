# Comparing `tmp/privateai_client-1.0.4.tar.gz` & `tmp/privateai_client-1.0.5.tar.gz`

## Comparing `privateai_client-1.0.4.tar` & `privateai_client-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.4/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/README.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/objects.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 privateai_client-1.0.4/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0    32957 2020-02-02 00:00:00.000000 privateai_client-1.0.4/tests/test_request_objects.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 privateai_client-1.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.0.4/LICENSE
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 privateai_client-1.0.4/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 privateai_client-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 privateai_client-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.5/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 privateai_client-1.0.5/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0    32963 2020-02-02 00:00:00.000000 privateai_client-1.0.5/tests/test_request_objects.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 privateai_client-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.0.5/LICENSE
+-rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 privateai_client-1.0.5/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 privateai_client-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 privateai_client-1.0.5/PKG-INFO
```

### Comparing `privateai_client-1.0.4/.pytest_cache/v/cache/nodeids` & `privateai_client-1.0.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.4/src/privateai_client/objects.py` & `privateai_client-1.0.5/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.4/src/privateai_client/pai_client.py` & `privateai_client-1.0.5/src/privateai_client/pai_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.4/src/privateai_client/components/pai_requests.py` & `privateai_client-1.0.5/src/privateai_client/components/pai_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,9 @@
     def process_files_uri(self, request_object):
         return self.make_request(self.request_type, self.uris.process_files_uri, request_object)
     
     def process_files_base64(self, request_object):
         return self.make_request(self.request_type, self.uris.process_files_base64, request_object)
     
     def bleep(self, request_object):
-        return self.make_request(self.request_type, self.uris.bleep, request_object)
+        return self.make_request(self.request_type, self.uris.bleep, request_object)
+
```

### Comparing `privateai_client-1.0.4/src/privateai_client/components/pai_responses.py` & `privateai_client-1.0.5/src/privateai_client/components/pai_responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,8 +117,9 @@
 class BleepResponse(BaseResponse):
 
     def __init__(self, response_object: Response = None):
         super(BleepResponse, self).__init__(response_object, True)
     
     @property
     def bleeped_file(self):
-        return self.get_attribute_entries("bleeped_file")
+        return self.get_attribute_entries("bleeped_file")
+
```

### Comparing `privateai_client-1.0.4/src/privateai_client/components/pai_uris.py` & `privateai_client-1.0.5/src/privateai_client/components/pai_uris.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,9 @@
         return self._create_uri(self.pai_uri, self.api_version, "process", "files", "base64")
 
     @property
     def version(self):
         return self._create_uri(self.pai_uri, "")
 
     def _create_uri(self, *args):
-        return "/".join([x.strip("/") for x in args])
+        return "/".join([x.strip("/") for x in args])
+
```

### Comparing `privateai_client-1.0.4/src/privateai_client/components/request_objects.py` & `privateai_client-1.0.5/src/privateai_client/components/request_objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.4/tests/test_request_objects.py` & `privateai_client-1.0.5/tests/test_request_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,8 +638,9 @@
     assert error_msg in str(excinfo.value)
 
 def test_bleep_request_to_dict():
     file=File(data="test", content_type="image/jpg")
     timestamps=[Timestamp(start=0.0, end=1.0)]
     bleep_request = BleepRequest(file=file, timestamps=timestamps).to_dict()
     assert bleep_request["file"]["data"] == 'test'
-    assert bleep_request["timestamps"][0]["start"] == 0
+    assert bleep_request["timestamps"][0]["start"] == 0
+
```

### Comparing `privateai_client-1.0.4/LICENSE` & `privateai_client-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-1.0.4/README.md` & `privateai_client-1.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# paiclient
+# privateai_client
 
 A client for communicating with the Private Ai de-identication api. This document provides information about how to best use the client. For more information, see Private Ai's [API Documentation.][1]
 
 ### Quick Links
 1. [Installation](#installation)
 2. [Quick Start](#quick-start)
 3. [Working with the Client](#client)
 4. [Request Objects](#request-objects)
 5. [Sample Use](#sample-use)
 
 ### Installation <a name=installation></a>
 
 ```
-pip install pai_thin_client
+pip install privateai_client
 ```
 
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
-from pai_thin_client import PAIClient
-from pai_thin_client import request_objects
+from privateai_client import PAIClient
+from privateai_client import request_objects
 
 schema = "http"
 host = "localhost"
 port = "8080"
 
 client = PAIClient(schema=schema, host=host, port=port)
 
@@ -46,15 +46,15 @@
 
 #### Initializing the Client
 
 the PAI client requires a scheme, host and optional port to initialize.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from pai_thin_client import PAIClient
+from privateai_client import PAIClient
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
 sample_obj = request_objects.file_url_obj(uri='path/to/file.jpg')
 sample_obj.uri
 ```
 Output:
 ```
 'path/to/file.jpg'
 ```
 
 Additionally there are request objects for each nested dictionary of a request:
 ```python 
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
@@ -266,8 +266,45 @@
 if not resp.ok:
     logging.error(f"response for file {file_name} returned with {resp.status_code}")
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.bleeped_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
+
+#### Working with structured data
+When deidentifying smaller strings of structured data, more accuracte results can be achieved by passing in the whole column as a string (including the header) and a delimiter. For example, making a request row by row for a column named SSN will return data identified as PHONE_NUMBER, even when the header is included
+
+```python
+# Working with data frames
+import pandas as pd
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
+
+client = PAIClient("http", "localhost", "8080")
+data_frame = pd.DataFrame(
+    {
+        "Name": [
+            "Braund, Mr. Owen Harris",
+            "Allen, Mr. William Henry",
+            "Bonnell, Miss. Elizabeth",
+        ],
+        "Age": [22, 35, 58],
+        "Sex": ["male", "male", "female"],
+    }
+)
+print(data_frame)
+text_req = request_objects.process_text_obj(text=[])
+for column in data_frame.columns:
+    text_req.text.append(f"{column}:{' | '.join([str(row) for row in data_frame[column]])}")
+
+resp = client.process_text(text_req)
+redacted_data = dict()
+for row in resp.processed_text:
+    data = row.split(':',1)
+    redacted_data[data[0]] = data[1].split(' | ')
+redacted_data_frame = pd.DataFrame(redacted_data)
+print(redacted_data_frame)
+```
+
+
 [1]:https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

### Comparing `privateai_client-1.0.4/pyproject.toml` & `privateai_client-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "privateai_client"
-version = "1.0.4"
+version = "1.0.5"
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
 "Homepage" = "https://github.com/privateai/pai-thin-client/"
-"Bug Tracker" = "https://github.com/privateai/pai-thin-client/issues"
+"Bug Tracker" = "https://github.com/privateai/pai-thin-client/issues"
```

### Comparing `privateai_client-1.0.4/PKG-INFO` & `privateai_client-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: privateai_client
-Version: 1.0.4
+Version: 1.0.5
 Summary: A thin client for communicating with the Private Ai de-identication api.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# paiclient
+# privateai_client
 
 A client for communicating with the Private Ai de-identication api. This document provides information about how to best use the client. For more information, see Private Ai's [API Documentation.][1]
 
 ### Quick Links
 1. [Installation](#installation)
 2. [Quick Start](#quick-start)
 3. [Working with the Client](#client)
 4. [Request Objects](#request-objects)
 5. [Sample Use](#sample-use)
 
 ### Installation <a name=installation></a>
 
 ```
-pip install pai_thin_client
+pip install privateai_client
 ```
 
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
-from pai_thin_client import PAIClient
-from pai_thin_client import request_objects
+from privateai_client import PAIClient
+from privateai_client import request_objects
 
 schema = "http"
 host = "localhost"
 port = "8080"
 
 client = PAIClient(schema=schema, host=host, port=port)
 
@@ -60,15 +60,15 @@
 
 #### Initializing the Client
 
 the PAI client requires a scheme, host and optional port to initialize.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from pai_thin_client import PAIClient
+from privateai_client import PAIClient
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
 sample_obj = request_objects.file_url_obj(uri='path/to/file.jpg')
 sample_obj.uri
 ```
 Output:
 ```
 'path/to/file.jpg'
 ```
 
 Additionally there are request objects for each nested dictionary of a request:
 ```python 
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import request_objects
+from privateai_client import request_objects
 
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
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
-from pai_thin_client import PAIClient
-from pai_thin_client.objects import request_objects
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
 import base64
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
@@ -280,8 +280,45 @@
 if not resp.ok:
     logging.error(f"response for file {file_name} returned with {resp.status_code}")
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.bleeped_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
+
+#### Working with structured data
+When deidentifying smaller strings of structured data, more accuracte results can be achieved by passing in the whole column as a string (including the header) and a delimiter. For example, making a request row by row for a column named SSN will return data identified as PHONE_NUMBER, even when the header is included
+
+```python
+# Working with data frames
+import pandas as pd
+from privateai_client import PAIClient
+from privateai_client.objects import request_objects
+
+client = PAIClient("http", "localhost", "8080")
+data_frame = pd.DataFrame(
+    {
+        "Name": [
+            "Braund, Mr. Owen Harris",
+            "Allen, Mr. William Henry",
+            "Bonnell, Miss. Elizabeth",
+        ],
+        "Age": [22, 35, 58],
+        "Sex": ["male", "male", "female"],
+    }
+)
+print(data_frame)
+text_req = request_objects.process_text_obj(text=[])
+for column in data_frame.columns:
+    text_req.text.append(f"{column}:{' | '.join([str(row) for row in data_frame[column]])}")
+
+resp = client.process_text(text_req)
+redacted_data = dict()
+for row in resp.processed_text:
+    data = row.split(':',1)
+    redacted_data[data[0]] = data[1].split(' | ')
+redacted_data_frame = pd.DataFrame(redacted_data)
+print(redacted_data_frame)
+```
+
+
 [1]:https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

