# Comparing `tmp/mdf_connect_client-0.4.0a3.tar.gz` & `tmp/mdf_connect_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mdf_connect_client-0.4.0a3.tar", last modified: Wed Jan 12 03:13:30 2022, max compression
+gzip compressed data, was "mdf_connect_client-0.4.1.tar", last modified: Wed Apr 19 19:57:29 2023, max compression
```

## Comparing `mdf_connect_client-0.4.0a3.tar` & `mdf_connect_client-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 bengal1    (502) staff       (20)        0 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/
--rw-r--r--   0 bengal1    (502) staff       (20)      679 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/PKG-INFO
--rw-r--r--   0 bengal1    (502) staff       (20)     2435 2021-01-05 17:55:51.000000 mdf_connect_client-0.4.0a3/README.md
-drwxr-xr-x   0 bengal1    (502) staff       (20)        0 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client/
--rw-r--r--   0 bengal1    (502) staff       (20)       98 2021-01-05 17:55:51.000000 mdf_connect_client-0.4.0a3/mdf_connect_client/__init__.py
--rw-r--r--   0 bengal1    (502) staff       (20)    65554 2022-01-12 03:10:22.000000 mdf_connect_client-0.4.0a3/mdf_connect_client/mdfcc.py
--rw-r--r--   0 bengal1    (502) staff       (20)       75 2022-01-12 03:11:35.000000 mdf_connect_client-0.4.0a3/mdf_connect_client/version.py
-drwxr-xr-x   0 bengal1    (502) staff       (20)        0 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/
--rw-r--r--   0 bengal1    (502) staff       (20)      679 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/PKG-INFO
--rw-r--r--   0 bengal1    (502) staff       (20)      326 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/SOURCES.txt
--rw-r--r--   0 bengal1    (502) staff       (20)        1 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/dependency_links.txt
--rw-r--r--   0 bengal1    (502) staff       (20)       80 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/requires.txt
--rw-r--r--   0 bengal1    (502) staff       (20)       19 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/top_level.txt
--rw-r--r--   0 bengal1    (502) staff       (20)      121 2022-01-12 03:13:30.000000 mdf_connect_client-0.4.0a3/setup.cfg
--rw-r--r--   0 bengal1    (502) staff       (20)     1220 2022-01-11 21:51:18.000000 mdf_connect_client-0.4.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:29.879039 mdf_connect_client-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-19 19:57:29.879039 mdf_connect_client-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:29.879039 mdf_connect_client-0.4.1/mdf_connect_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/mdf_connect_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65812 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/mdf_connect_client/mdfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/mdf_connect_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:29.879039 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-19 19:57:29.000000 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-19 19:57:29.000000 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:29.000000 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 19:57:29.000000 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 19:57:29.000000 mdf_connect_client-0.4.1/mdf_connect_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 19:57:29.879039 mdf_connect_client-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-19 19:57:18.000000 mdf_connect_client-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mdf_connect_client-0.4.0a3/PKG-INFO` & `mdf_connect_client-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdf_connect_client
-Version: 0.4.0a3
+Version: 0.4.1
 Summary: Materials Data Facility Connect Client
 Home-page: https://github.com/materials-data-facility/connect_client
 License: Apache License, Version 2.0
-Description: The MDF Connect Client is the Python client to easily submit datasets to MDF Connect.
 Keywords: MDF,Materials Data Facility,materials science,utility,Connect Client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: NOTICE
+
+The MDF Connect Client is the Python client to easily submit datasets to MDF Connect.
```

### Comparing `mdf_connect_client-0.4.0a3/README.md` & `mdf_connect_client-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # MDF Connect Client
-[![PyPI](https://img.shields.io/pypi/v/mdf_connect_client.svg)](https://pypi.python.org/pypi/mdf-connect-client) [![Build Status](https://travis-ci.org/materials-data-facility/connect_client.svg?branch=master)](https://travis-ci.org/materials-data-facility/connect_client) [![Coverage Status](https://coveralls.io/repos/github/materials-data-facility/connect_client/badge.svg?branch=master)](https://coveralls.io/github/materials-data-facility/connect_client?branch=master) [![Read the Docs](https://readthedocs.org/projects/mdf-connect-client/badge/?version=master)](http://mdf-connect-client.readthedocs.io/en/master/)
+[![PyPI](https://img.shields.io/pypi/v/mdf_connect_client.svg)](https://pypi.python.org/pypi/mdf-connect-client) 
+[![Coverage Status](https://coveralls.io/repos/github/materials-data-facility/connect_client/badge.svg?branch=master)](https://coveralls.io/github/materials-data-facility/connect_client?branch=master)
+![GHA](https://github.com/materials-data-facility/connect_client/actions/workflows/testing-work.yml/badge.svg)
 
 The MDF Connect Client is the Python client to easily submit datasets to MDF Connect.
 
 # Installation
 
 ```
 pip install mdf_connect_client
@@ -13,15 +15,15 @@
 ```
 git clone https://github.com/materials-data-facility/connect_client.git
 cd connect_client
 pip install -e .
 ```
 
 # Documentation and examples
-Documentation is available on [Read the Docs](https://mdf-connect-client.readthedocs.io/) and [GitHub](https://github.com/materials-data-facility/connect_client/tree/master/docs/). Examples and tutorials are provided as Jupyter notebooks, which can optionally be run interactively with [Jupyter](http://jupyter.org/).
+Documentation is available on [Read the Docs](https://mdf-connect-client.readthedocs.io/) and [GitHub](https://github.com/materials-data-facility/connect_client/tree/master/docs/). [Examples and tutorials](https://github.com/materials-data-facility/connect_client/tree/master/docs/tutorials) are provided as Jupyter notebooks, which can optionally be run interactively with [Jupyter](http://jupyter.org/).
 
 
 # Requirements
 * The Connect Client requires Python 3.5 or greater.
 * To submit data to MDF Connect, you must have an account recognized by Globus Auth (including Google, ORCiD, many academic institutions, or a [free Globus ID](https://www.globusid.org/create)), and be a member of the [MDF Connect Convert Globus Group](https://app.globus.org/groups/cc192dca-3751-11e8-90c1-0a7c735d220a).
```

### Comparing `mdf_connect_client-0.4.0a3/mdf_connect_client/mdfcc.py` & `mdf_connect_client-0.4.1/mdf_connect_client/mdfcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import globus_sdk
 import mdf_toolbox
 from nameparser import HumanName
 import requests
 
 from .version import __version__
 
-CONNECT_SERVICE_LOC = "https://publish.materialsdatafacility.org"
-CONNECT_DEV_LOC = "https://publish-dev.materialsdatafacility.org"
+CONNECT_SERVICE_LOC = "https://api.materialsdatafacility.org"
+CONNECT_DEV_LOC = "https://f6avec0img.execute-api.us-east-1.amazonaws.com/test"
 CONNECT_EXTRACT_ROUTE = "/submit"
 CONNECT_STATUS_ROUTE = "/status/"
 CONNECT_ALL_STATUS_ROUTE = "/submissions/"
 CONNECT_CURATION_ROUTE = "/curate/"
 CONNECT_ALL_CURATION_ROUTE = "/curation/"
 CONNECT_MD_UPDATE_ROUTE = "/update/"
 CURATION_SUMMARY_STR = ("{source_id} by {submitter}\nWaiting since {waiting_since}"
@@ -524,28 +524,28 @@
         """
         self.mdf["source_name"] = source_name
 
     def clear_source_name(self):
         """Remove a previously set source_name."""
         self.mdf.pop("source_name", None)
 
-    def set_update_metadata_only(self, metadata_only):
-        """Make this submission an update on the metadata only of a previous submission.
+    def set_incremental_update(self, source_id):
+        """Make this submission an incremental update of a previous submission.
         Incremental updates use the same submission metadata, except for whatever you
-        specify in the new submission. For example, if you submit an metadata only update
+        specify in the new submission. For example, if you submit an incremental update
         and only include a ``data_source``, the submission will run as if you copied the
         DC block and other metadata into the submission, but with the new ``data_source``.
 
         Note:
             You must still set ``update=True`` when submitting an incremental update.
 
         Arguments:
-            metadata_only (boolean): If true then flow performs an update on the metadata only
+            source_id (str): The ``source_id`` of the previous submission to update.
         """
-        self.update_metadata_only = metadata_only
+        self.incremental_update = source_id
 
     def add_data_destination(self, data_destination):
         """Add a data destination to your submission.
         Note that this method is cumulative, so calls do not overwrite previous ones.
 
         Arguments:
             data_destination (str or list of str): The destination for the data.
@@ -663,16 +663,14 @@
             "dc": self.dc,
             "data_sources": self.data_sources,
             "test": self.test,
             "update": self.update
         }
         if self.mdf:
             submission["mdf"] = self.mdf
-        else:
-            submission["mdf"] = {}
         if self.mrr:
             submission["mrr"] = self.mrr
         if self.custom:
             submission["custom"] = self.custom
         if self.projects:
             submission["projects"] = self.projects
         if self.data_destinations:
@@ -691,15 +689,16 @@
             submission["links"] = self.links
         if self.curation:
             submission["curation"] = self.curation
         if self.no_extract:
             submission["no_extract"] = self.no_extract
         if self.dataset_acl:
             submission["dataset_acl"] = self.dataset_acl
-        submission["update_metadata_only"] = self.update_metadata_only
+        if self.incremental_update:
+            submission["incremental_update"] = self.incremental_update
         return submission
 
     def reset_submission(self):
         """Reset and clear metadata from your submission.
 
         Warning:
             **This action cannot be undone.**
@@ -718,15 +717,15 @@
 
         self.projects = {}
 
         self.set_custom_block({})
         self.set_extraction_config({})
         self.set_curation(False)
         self.set_passthrough(False)
-        self.set_update_metadata_only(False)
+        self.set_incremental_update(False)
 
         self.clear_data_sources()
         self.clear_external_uri()
         self.clear_data_destinations()
         self.clear_index()
         self.clear_services()
         self.clear_tags()
@@ -779,15 +778,15 @@
                               " Set update=True to resubmit it")
                 }
             self.update = update
             submission = self.get_submission()
 
         # Check for required data
         if ((not submission["dc"] or not submission["data_sources"])
-                and not submission["update_metadata_only"]):
+                and not submission["incremental_update"]):
             return {
                 'source_id': None,
                 'success': False,
                 'error': "You must populate the dc and data blocks before submission."
             }
         # Validate JSON
         try:
@@ -797,21 +796,21 @@
                 'source_id': None,
                 'success': False,
                 'error': "The submission JSON is invalid: {}".format(repr(e))
             }
 
         # Make the request
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.post(self.service_loc+self.extract_route,
                             json=submission, headers=headers)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.post(self.service_loc+self.extract_route,
                                 json=submission, headers=headers)
 
         # Check for success
         error = None
         try:
             json_res = res.json()
@@ -864,35 +863,35 @@
         metadata_update.pop("update", None)
         metadata_update.pop("data_destinations", None)
         metadata_update.pop("index", None)
         metadata_update.pop("extraction_config", None)
         metadata_update.pop("services", None)
         metadata_update.pop("curation", None)
         metadata_update.pop("no_extract", None)
-        metadata_update.pop("update_metadata_only", None)
+        metadata_update.pop("incremental_update", None)
 
         # Validate JSON
         try:
             json.dumps(metadata_update, allow_nan=False)
         except Exception as e:
             return {
                 'source_id': None,
                 'success': False,
                 'error': "The metadata update JSON is invalid: {}".format(repr(e))
             }
 
         # Make the request
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.post(self.service_loc+self.md_update_route+source_id,
                             json=metadata_update, headers=headers)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.post(self.service_loc+self.md_update_route+source_id,
                                 json=metadata_update, headers=headers)
 
         # Check for success
         error = None
         try:
             json_res = res.json()
@@ -942,21 +941,21 @@
         Returns:
             If ``raw`` is ``True``, *dict*: The full status result.
         """
         if not source_id and not self.source_id:
             print("Error: No dataset submitted")
             return None
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.get(self.service_loc+self.status_route+(source_id or self.source_id),
                            headers=headers)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.get(self.service_loc+self.status_route+(source_id or self.source_id),
                                headers=headers)
 
         try:
             json_res = res.json()
         except Exception as e:
             if raw:
@@ -967,28 +966,28 @@
                 }
             elif res.status_code < 300:
                 print("Error decoding {} response: {}".format(res.status_code, res.content))
             else:
                 print("Error {}. MDF Connect may be experiencing technical"
                       " difficulties.".format(res.status_code))
         else:
-            if json_res["status"] == 'ACTIVE':
+            if json_res.get("status", {}).get("active"):
                 active_msg = "This submission is still processing."
             else:
                 active_msg = "This submission is no longer processing."
             if raw:
                 json_res["status_code"] = res.status_code
                 return json_res
             elif res.status_code >= 300:
                 print("Error {} fetching status: {}".format(res.status_code,
                                                             json_res.get("error", json_res)))
             elif short:
                 print("{}: {}".format((source_id or self.source_id), active_msg))
             else:
-                print("\n{}\n{}\n".format(json_res["display_status"], active_msg))
+                print("\n{}\n{}\n".format(json_res["status"]["status_message"], active_msg))
 
     def check_all_submissions(self, verbose=False, active_only=False, include_tests=True,
                               newer_than_date=None, older_than_date=None, raw=False,
                               filters=None, _admin_code=None):
         """Check the status of all of your submissions.
 
         Arguments:
@@ -1076,24 +1075,24 @@
                 raise ValueError("newer_than_date must be before older_than_date")
         if newer_than_date:
             filters.append(("submission_time", ">=", newer_than_date.isoformat("T") + "Z"))
         if older_than_date:
             filters.append(("submission_time", "<=", older_than_date.isoformat("T") + "Z"))
 
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         body = {
             "filters": filters
         }
         url = self.service_loc + self.all_status_route + (_admin_code or "")
         res = requests.post(url, headers=headers, json=body)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.post(url, headers=headers, json=body)
 
         try:
             json_res = res.json()
         except Exception as e:
             if raw:
                 return {
@@ -1166,20 +1165,20 @@
                     For direct human consumption, ``False`` is recommended.
                     **Default:** ``False``
 
         Returns:
             if raw is ``True``, *dict*: The full task results.
         """
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.get(self.service_loc+self.curation_route+source_id, headers=headers)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.get(self.service_loc+self.curation_route+source_id, headers=headers)
 
         try:
             json_res = res.json()
         except Exception as e:
             if raw:
                 return {
@@ -1236,21 +1235,21 @@
                     Only MDF Connect administrators are allowed to use these codes.
                     **Default:** ``None``, the only valid value for non-admins.
 
         Returns:
             if raw is ``True``, *dict*: The full task results.
         """
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.get(self.service_loc+self.all_curation_route+(_admin_code or ""),
                            headers=headers)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.get(self.service_loc+self.all_curation_route+(_admin_code or ""),
                                headers=headers)
         try:
             json_res = res.json()
         except Exception as e:
             if raw:
                 return {
@@ -1380,21 +1379,21 @@
 
         # Submit verdict
         command = {
             "action": verdict,
             "reason": reason
         }
         headers = {}
-        self.__authorizer.set_authorization_header(headers)
+        headers["Authorization"] = self.__authorizer.get_authorization_header()
         res = requests.post(self.service_loc+self.curation_route+source_id, headers=headers,
                             json=command)
         # Handle first 401/403 by regenerating auth headers
         if res.status_code == 401 or res.status_code == 403:
             self.__authorizer.handle_missing_authorization()
-            self.__authorizer.set_authorization_header(headers)
+            headers["Authorization"] = self.__authorizer.get_authorization_header()
             res = requests.get(self.service_loc+self.curation_route+source_id, headers=headers,
                                json=command)
 
         try:
             json_res = res.json()
         except Exception as e:
             if raw:
```

### Comparing `mdf_connect_client-0.4.0a3/mdf_connect_client.egg-info/PKG-INFO` & `mdf_connect_client-0.4.1/mdf_connect_client.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdf-connect-client
-Version: 0.4.0a3
+Version: 0.4.1
 Summary: Materials Data Facility Connect Client
 Home-page: https://github.com/materials-data-facility/connect_client
 License: Apache License, Version 2.0
-Description: The MDF Connect Client is the Python client to easily submit datasets to MDF Connect.
 Keywords: MDF,Materials Data Facility,materials science,utility,Connect Client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: NOTICE
+
+The MDF Connect Client is the Python client to easily submit datasets to MDF Connect.
```

### Comparing `mdf_connect_client-0.4.0a3/setup.py` & `mdf_connect_client-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     name='mdf_connect_client',
     version=version,
     packages=['mdf_connect_client'],
     description='Materials Data Facility Connect Client',
     long_description=("The MDF Connect Client is the Python client to easily submit"
                       " datasets to MDF Connect."),
     install_requires=[
-        "mdf-toolbox==0.5.8-alpha.2",
-        "jsonschema>=3.2.0",
+        "mdf-toolbox>=0.6.0",
         "nameparser>=1.0.4",
         "requests>=2.18.4"
     ],
     python_requires=">=3.5",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
```

