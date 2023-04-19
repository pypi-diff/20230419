# Comparing `tmp/hubmap-sdk-1.0.2.tar.gz` & `tmp/hubmap-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubmap-sdk-1.0.2.tar", last modified: Tue Jun 28 19:44:18 2022, max compression
+gzip compressed data, was "hubmap-sdk-1.0.3.tar", last modified: Wed Apr 19 14:53:02 2023, max compression
```

## Comparing `hubmap-sdk-1.0.2.tar` & `hubmap-sdk-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-06-28 19:44:18.795196 hubmap-sdk-1.0.2/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     3879 2022-06-28 19:44:18.795196 hubmap-sdk-1.0.2/PKG-INFO
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     2862 2022-06-28 18:00:56.000000 hubmap-sdk-1.0.2/README.md
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-06-28 19:44:18.795196 hubmap-sdk-1.0.2/hubmap_sdk/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      345 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/__init__.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)        0 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/client.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      208 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/collection.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      206 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/dataset.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      204 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/donor.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      180 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/entity.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)    19164 2022-06-28 18:02:08.000000 hubmap-sdk-1.0.2/hubmap_sdk/entitysdk.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      205 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/sample.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     3720 2022-06-28 18:02:08.000000 hubmap-sdk-1.0.2/hubmap_sdk/sdk_helper.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     2548 2022-06-28 18:17:55.000000 hubmap-sdk-1.0.2/hubmap_sdk/searchsdk.py
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      205 2022-05-16 14:49:27.000000 hubmap-sdk-1.0.2/hubmap_sdk/upload.py
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-06-28 19:44:18.795196 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     3879 2022-06-28 19:44:18.000000 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      434 2022-06-28 19:44:18.000000 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)        1 2022-06-28 19:44:18.000000 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       78 2022-06-28 19:44:18.000000 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/requires.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       11 2022-06-28 19:44:18.000000 hubmap-sdk-1.0.2/hubmap_sdk.egg-info/top_level.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       38 2022-06-28 19:44:18.795196 hubmap-sdk-1.0.2/setup.cfg
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      880 2022-06-28 19:18:49.000000 hubmap-sdk-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.201152 hubmap-sdk-1.0.3/hubmap_sdk/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/client.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/collection.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/donor.py
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/entity.py
+-rw-r--r--   0 root         (0) root         (0)    19599 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/entitysdk.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/sample.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/sdk_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/searchsdk.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/hubmap_sdk/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 14:53:02.000000 hubmap-sdk-1.0.3/hubmap_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 14:53:02.202153 hubmap-sdk-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-19 14:46:43.000000 hubmap-sdk-1.0.3/setup.py
```

### Comparing `hubmap-sdk-1.0.2/PKG-INFO` & `hubmap-sdk-1.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,67 @@
-Metadata-Version: 2.1
-Name: hubmap-sdk
-Version: 1.0.2
-Summary: Python Client Libary to use HuBMAP web services
-Home-page: UNKNOWN
-Author: Hubmap
-Author-email: api-developers@hubmapconsortium.org
-License: UNKNOWN
-Description: # hubmap-sdk
-        
-        ---
-        A Python interface to the various HuBMAP web services
-        
-        ### Overview
-        
-        The hubmap sdk is a client library that allows for easy integration of the API's associated with HuBMAP. 
-        
-        ### Using hubmap-sdk
-        
-        The hubmap-sdk library is available through PyPi via the command:
-        
-        ```bash
-        pip3 install hubmap-sdk
-        ```
-        hubmap-sdk requirements can be found [here](requirements.txt)
-        
-        ## Documentation
-        Documentation and examples can be found here
-        
-        * [hubmapsdk](https://software.docs.hubmapconsortium.org/sdk/hubmapsdk.html)
-        * [entitysdk](https://software.docs.hubmapconsortium.org/sdk/entitysdk.html)
-        * [searchsdk](https://software.docs.hubmapconsortium.org/sdk/searchsdk.html)
-        
-        ### Building and Publishing hubmap-sdk
-        
-        <a href="https://pypi.org/project/setuptools/">SetupTools</a> and <a href="https://pypi.org/project/wheel/">Wheel</a> is required to build the sdk distribution. <a href="https://pypi.org/project/twine/">Twine</a> is required to publish to Pypi
-        
-        Build the distribution directory with: 
-        
-        ```bash
-        python3 setup.py sdist bdist_wheel
-        ```
-        
-        from within the python-sdk project directory
-        
-        To publish, from inside the project directory, run:
-        
-        ```bash
-        twine upload dist/*
-        ```
-        
-        A prompt to enter login information to the hubmap Pypi account will appear
-        
-        
-        ### Files 
-        
-        This code contains:
-        
-        **collection.py** Contains the Collection class. This is used for creation and modification of Collection objects.
-        
-        **dataset.py** Contains the Dataset class. This is used for creation and modification of Dataset objects.
-        
-        **donor.py** Contains the Donor class. This is used for creation and modification of Donor objects.
-        
-        **entity.py** Contains the Entity class. This is the base class for the Donor, Dataset, Upload, Collection, and Sample classes
-        
-        **entitysdk.py** This file contains the primary methods used to interface with the Entity Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within entitysdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
-        
-        **sample.py** Contains the Sample class. This is used for creation and modification of Sample objects.
-        
-        **sdk_helper.py** This helper function contains various functions used frequently throughout the sdk. These include make_entity() and make_request()
-        
-        **searchsdk.py** This file contains the primary methods used to interface with the Search Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within searchsdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
-        
-        **upload.py** Contains the Upload class. This is used for creation and modification of Upload objects.
-        
-Keywords: HuBMAP Sdk,python
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# hubmap-sdk
+
+---
+A Python interface to the various HuBMAP web services
+
+### Overview
+
+The hubmap sdk is a client library that allows for easy integration of the API's associated with HuBMAP. 
+
+### Using hubmap-sdk
+
+The hubmap-sdk library is available through PyPi via the command:
+
+```bash
+pip3 install hubmap-sdk
+```
+hubmap-sdk requirements can be found [here](requirements.txt)
+
+## Documentation
+Documentation and examples can be found here
+
+* [hubmapsdk](https://software.docs.hubmapconsortium.org/sdk/hubmapsdk.html)
+* [entitysdk](https://software.docs.hubmapconsortium.org/sdk/entitysdk.html)
+* [searchsdk](https://software.docs.hubmapconsortium.org/sdk/searchsdk.html)
+
+### Building and Publishing hubmap-sdk
+
+<a href="https://pypi.org/project/setuptools/">SetupTools</a> and <a href="https://pypi.org/project/wheel/">Wheel</a> is required to build the sdk distribution. <a href="https://pypi.org/project/twine/">Twine</a> is required to publish to Pypi
+
+Build the distribution directory with: 
+
+```bash
+python3 setup.py sdist bdist_wheel
+```
+
+from within the python-sdk project directory
+
+To publish, from inside the project directory, run:
+
+```bash
+twine upload dist/*
+```
+
+A prompt to enter login information to the hubmap Pypi account will appear
+
+
+### Files 
+
+This code contains:
+
+**collection.py** Contains the Collection class. This is used for creation and modification of Collection objects.
+
+**dataset.py** Contains the Dataset class. This is used for creation and modification of Dataset objects.
+
+**donor.py** Contains the Donor class. This is used for creation and modification of Donor objects.
+
+**entity.py** Contains the Entity class. This is the base class for the Donor, Dataset, Upload, Collection, and Sample classes
+
+**entitysdk.py** This file contains the primary methods used to interface with the Entity Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within entitysdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
+
+**sample.py** Contains the Sample class. This is used for creation and modification of Sample objects.
+
+**sdk_helper.py** This helper function contains various functions used frequently throughout the sdk. These include make_entity() and make_request()
+
+**searchsdk.py** This file contains the primary methods used to interface with the Search Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within searchsdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
+
+**upload.py** Contains the Upload class. This is used for creation and modification of Upload objects.
```

#### html2text {}

```diff
@@ -1,11 +1,8 @@
-Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.2 Summary: Python Client
-Libary to use HuBMAP web services Home-page: UNKNOWN Author: Hubmap Author-
-email: api-developers@hubmapconsortium.org License: UNKNOWN Description: #
-hubmap-sdk --- A Python interface to the various HuBMAP web services ###
+# hubmap-sdk --- A Python interface to the various HuBMAP web services ###
 Overview The hubmap sdk is a client library that allows for easy integration of
 the API's associated with HuBMAP. ### Using hubmap-sdk The hubmap-sdk library
 is available through PyPi via the command: ```bash pip3 install hubmap-sdk ```
 hubmap-sdk requirements can be found [here](requirements.txt) ## Documentation
 Documentation and examples can be found here * [hubmapsdk](https://
 software.docs.hubmapconsortium.org/sdk/hubmapsdk.html) * [entitysdk](https://
 software.docs.hubmapconsortium.org/sdk/entitysdk.html) * [searchsdk](https://
@@ -30,12 +27,8 @@
 objects. **sdk_helper.py** This helper function contains various functions used
 frequently throughout the sdk. These include make_entity() and make_request()
 **searchsdk.py** This file contains the primary methods used to interface with
 the Search Api. These methods are part of the EntitySdk class. An instance of
 this class is needed to use the various methods in this class. For a detailed
 breakdown of the various methods within searchsdk.py, visit
 api.docs.hubmapconsortium.org **upload.py** Contains the Upload class. This is
-used for creation and modification of Upload objects. Keywords: HuBMAP
-Sdk,python Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+used for creation and modification of Upload objects.
```

### Comparing `hubmap-sdk-1.0.2/README.md` & `hubmap-sdk-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: hubmap-sdk
+Version: 1.0.3
+Summary: Python Client Libary to use HuBMAP web services
+Author: Hubmap
+Author-email: api-developers@hubmapconsortium.org
+Keywords: HuBMAP Sdk,python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hubmap-sdk
 
 ---
 A Python interface to the various HuBMAP web services
 
 ### Overview
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-# hubmap-sdk --- A Python interface to the various HuBMAP web services ###
-Overview The hubmap sdk is a client library that allows for easy integration of
-the API's associated with HuBMAP. ### Using hubmap-sdk The hubmap-sdk library
-is available through PyPi via the command: ```bash pip3 install hubmap-sdk ```
+Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.3 Summary: Python Client
+Libary to use HuBMAP web services Author: Hubmap Author-email: api-
+developers@hubmapconsortium.org Keywords: HuBMAP Sdk,python Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE # hubmap-sdk --
+- A Python interface to the various HuBMAP web services ### Overview The hubmap
+sdk is a client library that allows for easy integration of the API's
+associated with HuBMAP. ### Using hubmap-sdk The hubmap-sdk library is
+available through PyPi via the command: ```bash pip3 install hubmap-sdk ```
 hubmap-sdk requirements can be found [here](requirements.txt) ## Documentation
 Documentation and examples can be found here * [hubmapsdk](https://
 software.docs.hubmapconsortium.org/sdk/hubmapsdk.html) * [entitysdk](https://
 software.docs.hubmapconsortium.org/sdk/entitysdk.html) * [searchsdk](https://
 software.docs.hubmapconsortium.org/sdk/searchsdk.html) ### Building and
 Publishing hubmap-sdk SetupTools and Wheel is required to build the sdk
 distribution. Twine is required to publish to Pypi Build the distribution
```

### Comparing `hubmap-sdk-1.0.2/hubmap_sdk/entitysdk.py` & `hubmap-sdk-1.0.3/hubmap_sdk/entitysdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,7 +322,19 @@
     # Returns the provenance information in the form of a dictionary for a given dataset given by its id (HuBMAP ID, or
     # uuid).
     def get_prov_info_by_id(self, identifier):
         url = f"{self.entity_url}datasets/{identifier}/prov-info"
         arguments = "?format=json"
         output = sdk_helper.make_request('get', self, url, arguments)
         return output
+
+    # empty the entity cache for the given entity
+    def clear_cache(self, identifier):
+        url = f"{self.entity_url}flush-cache/{identifier}"
+        output = sdk_helper.make_request('delete', self, url)
+        return output
+
+    # empty the entire entity cache
+    def clear_all_cache(self):
+        url = f"{self.entity_url}flush-all-cache"
+        output = sdk_helper.make_request('delete', self, url)
+        return output
```

### Comparing `hubmap-sdk-1.0.2/hubmap_sdk/sdk_helper.py` & `hubmap-sdk-1.0.3/hubmap_sdk/sdk_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,38 +27,47 @@
             if instance.token is None:
                 if method_type == 'get':
                     r = requests.get(url + optional_argument)
                 if method_type == 'put':
                     r = requests.put(url + optional_argument)
                 if method_type == 'post':
                     r = requests.post(url + optional_argument)
+                if method_type == 'delete':
+                    r = requests.delete(url + optional_argument)
+
             else:
                 if method_type == 'get':
                     r = requests.get(url + optional_argument, headers=instance.header)
                 if method_type == 'put':
                     r = requests.put(url + optional_argument, headers=instance.header)
                 if method_type == 'post':
                     r = requests.post(url + optional_argument, headers=instance.header)
+                if method_type == 'delete':
+                    r = requests.delete(url + optional_argument, headers=instance.header)
         else:
             if not isinstance(data, dict):
                 raise Exception("Data given must be a dictionary")
             if instance.token is None:
                 if method_type == 'get':
                     r = requests.get(url + optional_argument, json=data)
                 if method_type == 'put':
                     r = requests.put(url + optional_argument, json=data)
                 if method_type == 'post':
                     r = requests.post(url + optional_argument, json=data)
+                if method_type == 'delete':
+                    r = requests.delete(url + optional_argument, json=data)
             else:
                 if method_type == 'get':
                     r = requests.get(url + optional_argument, headers=instance.header, json=data)
                 if method_type == 'put':
                     r = requests.put(url + optional_argument, headers=instance.header, json=data)
                 if method_type == 'post':
                     r = requests.post(url + optional_argument, headers=instance.header, json=data)
+                if method_type == 'delete':
+                    r = requests.delete(url + optional_argument, headers=instance.header, json=data)
     except Exception:
         raise HTTPException("Connection Error. Check that service url is correct in instance of Entity Class", 404)
     if r.status_code > 299:
         # if r.status_code == 401:
         #     raise Exception("401 Authorization Required. No Token or Invalid Token Given")
         try:
             error = r.json()['error']
```

### Comparing `hubmap-sdk-1.0.2/hubmap_sdk/searchsdk.py` & `hubmap-sdk-1.0.3/hubmap_sdk/searchsdk.py`

 * *Files identical despite different names*

### Comparing `hubmap-sdk-1.0.2/hubmap_sdk.egg-info/PKG-INFO` & `hubmap-sdk-1.0.3/hubmap_sdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 Metadata-Version: 2.1
 Name: hubmap-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Client Libary to use HuBMAP web services
-Home-page: UNKNOWN
 Author: Hubmap
 Author-email: api-developers@hubmapconsortium.org
-License: UNKNOWN
-Description: # hubmap-sdk
-        
-        ---
-        A Python interface to the various HuBMAP web services
-        
-        ### Overview
-        
-        The hubmap sdk is a client library that allows for easy integration of the API's associated with HuBMAP. 
-        
-        ### Using hubmap-sdk
-        
-        The hubmap-sdk library is available through PyPi via the command:
-        
-        ```bash
-        pip3 install hubmap-sdk
-        ```
-        hubmap-sdk requirements can be found [here](requirements.txt)
-        
-        ## Documentation
-        Documentation and examples can be found here
-        
-        * [hubmapsdk](https://software.docs.hubmapconsortium.org/sdk/hubmapsdk.html)
-        * [entitysdk](https://software.docs.hubmapconsortium.org/sdk/entitysdk.html)
-        * [searchsdk](https://software.docs.hubmapconsortium.org/sdk/searchsdk.html)
-        
-        ### Building and Publishing hubmap-sdk
-        
-        <a href="https://pypi.org/project/setuptools/">SetupTools</a> and <a href="https://pypi.org/project/wheel/">Wheel</a> is required to build the sdk distribution. <a href="https://pypi.org/project/twine/">Twine</a> is required to publish to Pypi
-        
-        Build the distribution directory with: 
-        
-        ```bash
-        python3 setup.py sdist bdist_wheel
-        ```
-        
-        from within the python-sdk project directory
-        
-        To publish, from inside the project directory, run:
-        
-        ```bash
-        twine upload dist/*
-        ```
-        
-        A prompt to enter login information to the hubmap Pypi account will appear
-        
-        
-        ### Files 
-        
-        This code contains:
-        
-        **collection.py** Contains the Collection class. This is used for creation and modification of Collection objects.
-        
-        **dataset.py** Contains the Dataset class. This is used for creation and modification of Dataset objects.
-        
-        **donor.py** Contains the Donor class. This is used for creation and modification of Donor objects.
-        
-        **entity.py** Contains the Entity class. This is the base class for the Donor, Dataset, Upload, Collection, and Sample classes
-        
-        **entitysdk.py** This file contains the primary methods used to interface with the Entity Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within entitysdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
-        
-        **sample.py** Contains the Sample class. This is used for creation and modification of Sample objects.
-        
-        **sdk_helper.py** This helper function contains various functions used frequently throughout the sdk. These include make_entity() and make_request()
-        
-        **searchsdk.py** This file contains the primary methods used to interface with the Search Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within searchsdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
-        
-        **upload.py** Contains the Upload class. This is used for creation and modification of Upload objects.
-        
 Keywords: HuBMAP Sdk,python
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# hubmap-sdk
+
+---
+A Python interface to the various HuBMAP web services
+
+### Overview
+
+The hubmap sdk is a client library that allows for easy integration of the API's associated with HuBMAP. 
+
+### Using hubmap-sdk
+
+The hubmap-sdk library is available through PyPi via the command:
+
+```bash
+pip3 install hubmap-sdk
+```
+hubmap-sdk requirements can be found [here](requirements.txt)
+
+## Documentation
+Documentation and examples can be found here
+
+* [hubmapsdk](https://software.docs.hubmapconsortium.org/sdk/hubmapsdk.html)
+* [entitysdk](https://software.docs.hubmapconsortium.org/sdk/entitysdk.html)
+* [searchsdk](https://software.docs.hubmapconsortium.org/sdk/searchsdk.html)
+
+### Building and Publishing hubmap-sdk
+
+<a href="https://pypi.org/project/setuptools/">SetupTools</a> and <a href="https://pypi.org/project/wheel/">Wheel</a> is required to build the sdk distribution. <a href="https://pypi.org/project/twine/">Twine</a> is required to publish to Pypi
+
+Build the distribution directory with: 
+
+```bash
+python3 setup.py sdist bdist_wheel
+```
+
+from within the python-sdk project directory
+
+To publish, from inside the project directory, run:
+
+```bash
+twine upload dist/*
+```
+
+A prompt to enter login information to the hubmap Pypi account will appear
+
+
+### Files 
+
+This code contains:
+
+**collection.py** Contains the Collection class. This is used for creation and modification of Collection objects.
+
+**dataset.py** Contains the Dataset class. This is used for creation and modification of Dataset objects.
+
+**donor.py** Contains the Donor class. This is used for creation and modification of Donor objects.
+
+**entity.py** Contains the Entity class. This is the base class for the Donor, Dataset, Upload, Collection, and Sample classes
+
+**entitysdk.py** This file contains the primary methods used to interface with the Entity Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within entitysdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
+
+**sample.py** Contains the Sample class. This is used for creation and modification of Sample objects.
+
+**sdk_helper.py** This helper function contains various functions used frequently throughout the sdk. These include make_entity() and make_request()
+
+**searchsdk.py** This file contains the primary methods used to interface with the Search Api. These methods are part of the EntitySdk class. An instance of this class is needed to use the various methods in this class. For a detailed breakdown of the various methods within searchsdk.py, visit <a href="https://api.docs.hubmapconsortium.org">api.docs.hubmapconsortium.org</a>  
+
+**upload.py** Contains the Upload class. This is used for creation and modification of Upload objects.
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.2 Summary: Python Client
-Libary to use HuBMAP web services Home-page: UNKNOWN Author: Hubmap Author-
-email: api-developers@hubmapconsortium.org License: UNKNOWN Description: #
-hubmap-sdk --- A Python interface to the various HuBMAP web services ###
-Overview The hubmap sdk is a client library that allows for easy integration of
-the API's associated with HuBMAP. ### Using hubmap-sdk The hubmap-sdk library
-is available through PyPi via the command: ```bash pip3 install hubmap-sdk ```
+Metadata-Version: 2.1 Name: hubmap-sdk Version: 1.0.3 Summary: Python Client
+Libary to use HuBMAP web services Author: Hubmap Author-email: api-
+developers@hubmapconsortium.org Keywords: HuBMAP Sdk,python Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE # hubmap-sdk --
+- A Python interface to the various HuBMAP web services ### Overview The hubmap
+sdk is a client library that allows for easy integration of the API's
+associated with HuBMAP. ### Using hubmap-sdk The hubmap-sdk library is
+available through PyPi via the command: ```bash pip3 install hubmap-sdk ```
 hubmap-sdk requirements can be found [here](requirements.txt) ## Documentation
 Documentation and examples can be found here * [hubmapsdk](https://
 software.docs.hubmapconsortium.org/sdk/hubmapsdk.html) * [entitysdk](https://
 software.docs.hubmapconsortium.org/sdk/entitysdk.html) * [searchsdk](https://
 software.docs.hubmapconsortium.org/sdk/searchsdk.html) ### Building and
 Publishing hubmap-sdk SetupTools and Wheel is required to build the sdk
 distribution. Twine is required to publish to Pypi Build the distribution
@@ -30,12 +33,8 @@
 objects. **sdk_helper.py** This helper function contains various functions used
 frequently throughout the sdk. These include make_entity() and make_request()
 **searchsdk.py** This file contains the primary methods used to interface with
 the Search Api. These methods are part of the EntitySdk class. An instance of
 this class is needed to use the various methods in this class. For a detailed
 breakdown of the various methods within searchsdk.py, visit
 api.docs.hubmapconsortium.org **upload.py** Contains the Upload class. This is
-used for creation and modification of Upload objects. Keywords: HuBMAP
-Sdk,python Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+used for creation and modification of Upload objects.
```

### Comparing `hubmap-sdk-1.0.2/setup.py` & `hubmap-sdk-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hubmap-sdk",
-    version="1.0.2",
+    version="1.0.3",
     author="Hubmap",
     author_email="api-developers@hubmapconsortium.org",
     description="Python Client Libary to use HuBMAP web services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['hubmap_sdk'],
     keywords=[
```

