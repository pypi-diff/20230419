# Comparing `tmp/oianalytics-0.5.1b5.tar.gz` & `tmp/oianalytics-0.5.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oianalytics-0.5.1b5.tar", max compression
+gzip compressed data, was "oianalytics-0.5.2b1.tar", max compression
```

## Comparing `oianalytics-0.5.1b5.tar` & `oianalytics-0.5.2b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.1b5/LICENSE
--rw-r--r--   0        0        0       94 2023-03-29 14:38:22.274778 oianalytics-0.5.1b5/oianalytics/__init__.py
--rw-r--r--   0        0        0       99 2023-03-15 14:01:49.113825 oianalytics-0.5.1b5/oianalytics/api/__init__.py
--rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.1b5/oianalytics/api/_credentials.py
--rw-r--r--   0        0        0     1342 2023-03-27 09:27:50.327205 oianalytics-0.5.1b5/oianalytics/api/_dataframes/__init__.py
--rw-r--r--   0        0        0     7272 2023-03-15 14:02:23.748123 oianalytics-0.5.1b5/oianalytics/api/_dataframes/assets.py
--rw-r--r--   0        0        0    40776 2023-03-27 09:27:20.569819 oianalytics-0.5.1b5/oianalytics/api/_dataframes/batches.py
--rw-r--r--   0        0        0    41468 2023-03-23 09:30:42.424602 oianalytics-0.5.1b5/oianalytics/api/_dataframes/data.py
--rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.1b5/oianalytics/api/_dataframes/events.py
--rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.1b5/oianalytics/api/_dataframes/files.py
--rw-r--r--   0        0        0     4250 2023-03-15 14:01:49.114990 oianalytics-0.5.1b5/oianalytics/api/_dataframes/users.py
--rw-r--r--   0        0        0      123 2023-03-15 14:02:23.748433 oianalytics-0.5.1b5/oianalytics/api/endpoints/__init__.py
--rw-r--r--   0        0        0     1552 2023-03-15 14:02:23.748497 oianalytics-0.5.1b5/oianalytics/api/endpoints/assets.py
--rw-r--r--   0        0        0     8316 2023-03-27 08:38:08.115045 oianalytics-0.5.1b5/oianalytics/api/endpoints/batches.py
--rw-r--r--   0        0        0    13020 2023-03-23 08:37:14.720021 oianalytics-0.5.1b5/oianalytics/api/endpoints/data.py
--rw-r--r--   0        0        0     2600 2023-03-15 14:01:49.115412 oianalytics-0.5.1b5/oianalytics/api/endpoints/events.py
--rw-r--r--   0        0        0     3159 2023-03-15 14:01:49.115505 oianalytics-0.5.1b5/oianalytics/api/endpoints/files.py
--rw-r--r--   0        0        0     1199 2023-03-15 14:01:49.115585 oianalytics-0.5.1b5/oianalytics/api/endpoints/users.py
--rw-r--r--   0        0        0     5881 2023-03-15 14:02:23.748714 oianalytics-0.5.1b5/oianalytics/api/utils.py
--rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.1b5/oianalytics/models/__init__.py
--rw-r--r--   0        0        0    39198 2023-03-29 14:38:03.806530 oianalytics-0.5.1b5/oianalytics/models/_dtos.py
--rw-r--r--   0        0        0      346 2023-03-15 14:02:23.748985 oianalytics-0.5.1b5/oianalytics/models/_queries/__init__.py
--rw-r--r--   0        0        0     1938 2023-03-15 14:02:23.749074 oianalytics-0.5.1b5/oianalytics/models/_queries/files.py
--rw-r--r--   0        0        0      711 2023-03-15 14:01:49.116301 oianalytics-0.5.1b5/oianalytics/models/_queries/instances.py
--rw-r--r--   0        0        0    10106 2023-03-15 14:01:49.116403 oianalytics-0.5.1b5/oianalytics/models/_queries/single_observation.py
--rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.1b5/oianalytics/models/_template_resources/__init__.py
--rw-r--r--   0        0        0     2796 2023-03-15 14:02:23.749203 oianalytics-0.5.1b5/oianalytics/models/_template_resources/file_processing_template.py
--rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.1b5/oianalytics/models/_template_resources/free_from_api_template.py
--rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.1b5/oianalytics/models/_template_resources/single_observation_template.py
--rw-r--r--   0        0        0    30641 2023-03-15 14:02:23.749371 oianalytics-0.5.1b5/oianalytics/models/outputs.py
--rw-r--r--   0        0        0      992 2023-03-15 14:01:49.117047 oianalytics-0.5.1b5/oianalytics/models/templates.py
--rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.1b5/oianalytics/models/testing/__init__.py
--rw-r--r--   0        0        0    31789 2023-03-15 14:01:49.117353 oianalytics-0.5.1b5/oianalytics/models/testing/_mocking.py
--rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.1b5/oianalytics/models/testing/_tests_setup.py
--rw-r--r--   0        0        0     2791 2023-03-15 14:01:49.117545 oianalytics-0.5.1b5/oianalytics/models/testing/file_processing.py
--rw-r--r--   0        0        0     2645 2023-03-15 14:01:49.117632 oianalytics-0.5.1b5/oianalytics/models/testing/free_from_api.py
--rw-r--r--   0        0        0     6985 2023-03-15 14:01:49.117720 oianalytics-0.5.1b5/oianalytics/models/testing/single_observation.py
--rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.1b5/oianalytics/models/utils.py
--rw-r--r--   0        0        0      471 2023-03-29 14:38:10.510129 oianalytics-0.5.1b5/pyproject.toml
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 oianalytics-0.5.1b5/PKG-INFO
+-rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.2b1/LICENSE
+-rw-r--r--   0        0        0       94 2023-04-19 09:25:30.486603 oianalytics-0.5.2b1/oianalytics/__init__.py
+-rw-r--r--   0        0        0       99 2023-03-15 14:01:49.113825 oianalytics-0.5.2b1/oianalytics/api/__init__.py
+-rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.2b1/oianalytics/api/_credentials.py
+-rw-r--r--   0        0        0     1342 2023-04-18 12:32:43.993044 oianalytics-0.5.2b1/oianalytics/api/_dataframes/__init__.py
+-rw-r--r--   0        0        0     7272 2023-04-18 12:32:43.960505 oianalytics-0.5.2b1/oianalytics/api/_dataframes/assets.py
+-rw-r--r--   0        0        0    40776 2023-04-18 12:32:43.993542 oianalytics-0.5.2b1/oianalytics/api/_dataframes/batches.py
+-rw-r--r--   0        0        0    41468 2023-04-18 12:32:43.986986 oianalytics-0.5.2b1/oianalytics/api/_dataframes/data.py
+-rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.2b1/oianalytics/api/_dataframes/events.py
+-rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.2b1/oianalytics/api/_dataframes/files.py
+-rw-r--r--   0        0        0     4250 2023-03-15 14:01:49.114990 oianalytics-0.5.2b1/oianalytics/api/_dataframes/users.py
+-rw-r--r--   0        0        0      123 2023-04-18 12:32:43.960591 oianalytics-0.5.2b1/oianalytics/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-18 12:32:43.960652 oianalytics-0.5.2b1/oianalytics/api/endpoints/assets.py
+-rw-r--r--   0        0        0     8316 2023-04-18 12:32:43.993820 oianalytics-0.5.2b1/oianalytics/api/endpoints/batches.py
+-rw-r--r--   0        0        0    13020 2023-04-18 12:32:43.987317 oianalytics-0.5.2b1/oianalytics/api/endpoints/data.py
+-rw-r--r--   0        0        0     2600 2023-03-15 14:01:49.115412 oianalytics-0.5.2b1/oianalytics/api/endpoints/events.py
+-rw-r--r--   0        0        0     3159 2023-04-19 09:24:50.987573 oianalytics-0.5.2b1/oianalytics/api/endpoints/files.py
+-rw-r--r--   0        0        0     1199 2023-03-15 14:01:49.115585 oianalytics-0.5.2b1/oianalytics/api/endpoints/users.py
+-rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.2b1/oianalytics/api/utils.py
+-rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.2b1/oianalytics/models/__init__.py
+-rw-r--r--   0        0        0    39198 2023-04-18 12:32:44.003683 oianalytics-0.5.2b1/oianalytics/models/_dtos.py
+-rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.2b1/oianalytics/models/_queries/__init__.py
+-rw-r--r--   0        0        0     1943 2023-04-19 09:25:06.769232 oianalytics-0.5.2b1/oianalytics/models/_queries/files.py
+-rw-r--r--   0        0        0      711 2023-03-15 14:01:49.116301 oianalytics-0.5.2b1/oianalytics/models/_queries/instances.py
+-rw-r--r--   0        0        0    10106 2023-03-15 14:01:49.116403 oianalytics-0.5.2b1/oianalytics/models/_queries/single_observation.py
+-rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.2b1/oianalytics/models/_template_resources/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.2b1/oianalytics/models/_template_resources/file_processing_template.py
+-rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.2b1/oianalytics/models/_template_resources/free_from_api_template.py
+-rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.2b1/oianalytics/models/_template_resources/single_observation_template.py
+-rw-r--r--   0        0        0    30641 2023-04-18 12:32:43.976382 oianalytics-0.5.2b1/oianalytics/models/outputs.py
+-rw-r--r--   0        0        0      992 2023-03-15 14:01:49.117047 oianalytics-0.5.2b1/oianalytics/models/templates.py
+-rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.2b1/oianalytics/models/testing/__init__.py
+-rw-r--r--   0        0        0    31789 2023-03-15 14:01:49.117353 oianalytics-0.5.2b1/oianalytics/models/testing/_mocking.py
+-rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.2b1/oianalytics/models/testing/_tests_setup.py
+-rw-r--r--   0        0        0     2791 2023-03-15 14:01:49.117545 oianalytics-0.5.2b1/oianalytics/models/testing/file_processing.py
+-rw-r--r--   0        0        0     2645 2023-03-15 14:01:49.117632 oianalytics-0.5.2b1/oianalytics/models/testing/free_from_api.py
+-rw-r--r--   0        0        0     6985 2023-03-15 14:01:49.117720 oianalytics-0.5.2b1/oianalytics/models/testing/single_observation.py
+-rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.2b1/oianalytics/models/utils.py
+-rw-r--r--   0        0        0      471 2023-04-19 09:25:35.141034 oianalytics-0.5.2b1/pyproject.toml
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 oianalytics-0.5.2b1/PKG-INFO
```

### Comparing `oianalytics-0.5.1b5/LICENSE` & `oianalytics-0.5.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_credentials.py` & `oianalytics-0.5.2b1/oianalytics/api/_credentials.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/__init__.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/assets.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/batches.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/data.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/events.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/files.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/_dataframes/users.py` & `oianalytics-0.5.2b1/oianalytics/api/_dataframes/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/assets.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/batches.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/data.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/events.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/files.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/endpoints/users.py` & `oianalytics-0.5.2b1/oianalytics/api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/api/utils.py` & `oianalytics-0.5.2b1/oianalytics/api/utils.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_dtos.py` & `oianalytics-0.5.2b1/oianalytics/models/_dtos.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_queries/files.py` & `oianalytics-0.5.2b1/oianalytics/models/_queries/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,8 +51,8 @@
         url=url,
         files={"file": (file_name, file_content)},
         **api_credentials.auth_kwargs,
     )
 
     # Output
     response.raise_for_status()
-    return response.json()
+    return response.status_code
```

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_queries/instances.py` & `oianalytics-0.5.2b1/oianalytics/models/_queries/instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_queries/single_observation.py` & `oianalytics-0.5.2b1/oianalytics/models/_queries/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_template_resources/file_processing_template.py` & `oianalytics-0.5.2b1/oianalytics/models/_template_resources/file_processing_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_template_resources/free_from_api_template.py` & `oianalytics-0.5.2b1/oianalytics/models/_template_resources/free_from_api_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/_template_resources/single_observation_template.py` & `oianalytics-0.5.2b1/oianalytics/models/_template_resources/single_observation_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/outputs.py` & `oianalytics-0.5.2b1/oianalytics/models/outputs.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/templates.py` & `oianalytics-0.5.2b1/oianalytics/models/templates.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/testing/_mocking.py` & `oianalytics-0.5.2b1/oianalytics/models/testing/_mocking.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/testing/_tests_setup.py` & `oianalytics-0.5.2b1/oianalytics/models/testing/_tests_setup.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/testing/file_processing.py` & `oianalytics-0.5.2b1/oianalytics/models/testing/file_processing.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/testing/free_from_api.py` & `oianalytics-0.5.2b1/oianalytics/models/testing/free_from_api.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/oianalytics/models/testing/single_observation.py` & `oianalytics-0.5.2b1/oianalytics/models/testing/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.1b5/PKG-INFO` & `oianalytics-0.5.2b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oianalytics
-Version: 0.5.1b5
+Version: 0.5.2b1
 Summary: Python tools for working with OIAnalytics
 License: EUPL-1.2
 Author: Optimistik SAS
 Author-email: arthur.martel@optimistik.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

