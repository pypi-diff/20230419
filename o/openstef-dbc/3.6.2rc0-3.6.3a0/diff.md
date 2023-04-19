# Comparing `tmp/openstef_dbc-3.6.2rc0.tar.gz` & `tmp/openstef_dbc-3.6.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.2rc0.tar", last modified: Mon Apr  3 09:08:11 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.3a0.tar", last modified: Wed Apr 19 13:44:50 2023, max compression
```

## Comparing `openstef_dbc-3.6.2rc0.tar` & `openstef_dbc-3.6.3a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.600072 openstef_dbc-3.6.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-03 09:08:11.600072 openstef_dbc-3.6.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.596072 openstef_dbc-3.6.2rc0/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.596072 openstef_dbc-3.6.2rc0/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.596072 openstef_dbc-3.6.2rc0/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.600072 openstef_dbc-3.6.2rc0/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:08:11.596072 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-03 09:08:11.000000 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-03 09:08:11.000000 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 09:08:11.000000 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-03 09:08:11.000000 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-03 09:08:11.000000 openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-03 09:08:11.600072 openstef_dbc-3.6.2rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-03 09:07:59.000000 openstef_dbc-3.6.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.286216 openstef_dbc-3.6.3a0/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.286216 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/setup.py
```

### Comparing `openstef_dbc-3.6.2rc0/LICENSE` & `openstef_dbc-3.6.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/PKG-INFO` & `openstef_dbc-3.6.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.2rc0
+Version: 3.6.3a0
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.2rc0/README.md` & `openstef_dbc-3.6.3a0/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/__init__.py` & `openstef_dbc-3.6.3a0/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.3a0/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/database.py` & `openstef_dbc-3.6.3a0/openstef_dbc/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,26 +33,31 @@
     _splitting = Splitting()
     _predictions = Predictions()
     _model_input = ModelInput()
     _systems = Systems()
 
     # write methods
     write_weather_data = _write.write_weather_data
+    write_realised_power_measurements = _write.write_realised_power_measurements
     write_realised_pvdata = _write.write_realised_pvdata
     write_kpi = _write.write_kpi
     write_forecast = _write.write_forecast
     write_apx_market_data = _write.write_apx_market_data
     write_sjv_load_profiles = _write.write_sjv_load_profiles
     write_windturbine_powercurves = _write.write_windturbine_powercurves
     write_energy_splitting_coefficients = _write.write_energy_splitting_coefficients
+
     # prediction job methods
     get_prediction_jobs_solar = _prediction_job.get_prediction_jobs_solar
     get_prediction_jobs_wind = _prediction_job.get_prediction_jobs_wind
     get_prediction_jobs = _prediction_job.get_prediction_jobs
     get_prediction_job = _prediction_job.get_prediction_job
+    get_pids_for_api_key = _prediction_job.get_pids_for_api_key
+    get_ean_for_pid = _prediction_job.get_ean_for_pid
+
     # weather methods
     get_weather_forecast_locations = _weather.get_weather_forecast_locations
     get_weather_data = _weather.get_weather_data
     get_datetime_last_stored_knmi_weatherdata = (
         _weather.get_datetime_last_stored_knmi_weatherdata
     )
     # predictor methods
@@ -66,26 +71,31 @@
     # splitting methods
     get_wind_ref = _splitting.get_wind_ref
     get_energy_split_coefs = _splitting.get_energy_split_coefs
     get_input_energy_splitting = _splitting.get_input_energy_splitting
     # predictions methods
     get_predicted_load = _predictions.get_predicted_load
     get_predicted_load_tahead = _predictions.get_predicted_load_tahead
+    get_prediction_including_components = (
+        _predictions.get_prediction_including_components
+    )
+    get_forecast_quality = _predictions.get_forecast_quality
     # model input methods
     get_model_input = _model_input.get_model_input
     get_wind_input = _model_input.get_wind_input
     get_power_curve = _model_input.get_power_curve
     get_solar_input = _model_input.get_solar_input
     # systems methods
     get_systems_near_location = _systems.get_systems_near_location
     get_systems_by_pid = _systems.get_systems_by_pid
     get_pv_systems_with_incorrect_location = (
         _systems.get_pv_systems_with_incorrect_location
     )
     get_random_pv_systems = _systems.get_random_pv_systems
+    get_api_key_for_system = _systems.get_api_key_for_system
 
     def __init__(self, config):
         """Construct the DataBase singleton.
 
         Initialize the datainterface and api. WARNING: this is a singleton class when
         calling multiple times with a config argument no new configuration will be
         applied.
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.3a0/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.3a0/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.3a0/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.3a0/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/prediction_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 #
 # SPDX-License-Identifier: MPL-2.0
 
 import json
 from typing import List, Optional, Union
 from pydantic import ValidationError
+import pandas as pd
+
 from openstef.data_classes.prediction_job import PredictionJobDataClass
 
 from openstef_dbc.data_interface import _DataInterface
 from openstef_dbc.log import logging
 from openstef_dbc.services.systems import Systems
 
 
@@ -189,14 +191,61 @@
         return self._add_description_to_prediction_jobs([prediction_job])[0]
 
     def _add_quantiles_to_prediction_job(
         self, prediction_job: PredictionJobDataClass
     ) -> PredictionJobDataClass:
         return self._add_quantiles_to_prediction_jobs([prediction_job])[0]
 
+    def get_pids_for_api_key(self, api_key: str) -> list[int]:
+        """Get all pids that belong to a given API key.
+
+        Args:
+            api_key (str): The API key
+
+        Returns:
+            list[int]: dList of pids
+        """
+        bind_params = {"apiKey": api_key}
+        query = """
+            SELECT
+                p.id 
+            FROM `customersApiKeys` as cak 
+            LEFT JOIN `customers` as cu ON cak.cid = cu.id 
+            LEFT JOIN `customers_predictions` as cp ON cu.id = cp.customer_id 
+            LEFT JOIN `predictions` as p ON p.id = cp.prediction_id 
+            WHERE cak.api_key = %(apiKey)s 
+        """
+        result = _DataInterface.get_instance().exec_sql_query(query, bind_params)
+        if isinstance(result, pd.DataFrame) and result.empty:
+            return []
+        else:
+            return result["id"].to_list()
+
+    def get_ean_for_pid(self, pid: int) -> str:
+        """Get EAN that is connectec to a prediction
+
+        Args:
+            pid (int): The prediction ID
+
+        Returns:
+            str: The corresponding EAN code
+        """
+        bind_params = {"pid": pid}
+        query = """
+            SELECT
+                p.ean 
+            FROM `predictions` as p  
+            WHERE p.id = %(pid)s 
+        """
+        result = _DataInterface.get_instance().exec_sql_query(query, bind_params)
+        if isinstance(result, pd.DataFrame) and result.empty:
+            return []
+        else:
+            return result["ean"].to_list()
+
     @classmethod
     def _add_quantiles_to_prediction_jobs(
         cls, prediction_jobs: List[PredictionJobDataClass]
     ) -> List[PredictionJobDataClass]:
         prediction_job_ids = [pj["id"] for pj in prediction_jobs]
         prediction_jobs_ids_str = ", ".join([f"'{p}'" for p in prediction_job_ids])
 
@@ -276,14 +325,15 @@
 
         if limit:
             limit_clause = f"LIMIT {limit}"
 
         query = f"""
             SELECT
                 p.id, 
+                p.ean,
                 p.name,
                 p.forecast_type, 
                 p.model, 
                 p.horizon_minutes, 
                 p.resolution_minutes,
                 p.train_components,
                 min(s.lat) as lat,
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/predictions.py`

 * *Files 26% similar despite different names*

```diff
@@ -67,14 +67,140 @@
         # Return result
         if not result.empty:
             # Shifting is needed to output the same as with the old influx client
             return parse_influx_result(result).shift(-15, freq="T")
         else:
             return pd.Series()
 
+    def get_forecast_quality(
+        self, pj: dict, start_time: datetime = None, end_time: datetime = None
+    ):
+        """Get forecast quality for historic load predictions for given pid.
+
+        Args:
+            pj (dict): Prediction job
+            start_time (datetime): Start time to retrieve the historic load prediction.
+            end_time (datetime): End time to retrieve the historic load prediction.
+
+        Returns:
+            pandas.Series: Quality column with the quality of the predicted values
+
+        """
+        if start_time is None:
+            start_time = datetime.utcnow()
+        if end_time is None:
+            end_time = datetime.utcnow() + timedelta(days=2)
+
+        bind_params = {
+            "pid": str(pj["id"]),
+            "_start": start_time.astimezone(pytz.UTC),
+            "_stop": end_time.astimezone(pytz.UTC),
+        }
+
+        query = f"""
+        from(bucket: "forecast_latest/autogen")
+            |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
+            |> filter(fn: (r) => 
+                r._measurement == "prediction")
+            |> filter(fn: (r) => 
+                r._field == "quality" )                 
+            |> filter(fn: (r) => r.pid == "{bind_params["pid"]}")
+        """
+
+        # Query the database
+        result = _DataInterface.get_instance().exec_influx_query(query, bind_params)
+
+        # For multiple Fields a list is returned.
+        if isinstance(result, list):
+            result = pd.concat(result)[["_value", "_field", "_time"]]
+
+        # Return result
+        if not result.empty:
+            # Shifting is needed to output the same as with the old influx client
+            return parse_influx_result(result, aggfunc="first").shift(-15, freq="T")
+        else:
+            return pd.Series()
+
+    def get_prediction_including_components(
+        self,
+        pj: dict,
+        start_time: datetime = None,
+        end_time: datetime = None,
+        quantiles: bool = False,
+    ):
+        """Get historic load predictions for given pid including component forecasts.
+
+        Args:
+            pj (dict): Prediction job
+            start_time (datetime): Start time  to retrieve the historic load prediction.
+            end_time (datetime): End timeto retrieve the historic load prediction.
+            quantiles: (boo): Indicates wheter quantiles should be retrieved as well.
+
+        Returns:
+            pandas.DataFrame: Dataframe with the total forecast,
+            the components forecasts and the quantiles if they are requested.
+
+        """
+        # Apply default parameters if none are provided
+        if start_time is None:
+            start_time = datetime.utcnow()
+        if end_time is None:
+            end_time = datetime.utcnow() + timedelta(days=2)
+
+        bind_params = {
+            "pid": str(pj["id"]),
+            "_start": start_time.astimezone(pytz.UTC),
+            "_stop": end_time.astimezone(pytz.UTC),
+        }
+        quantile_section = (
+            """or r._field == "quantile_P"""
+            + """" or r._field == "quantile_P""".join(
+                [f"{quantile * 100:02.0f}" for quantile in pj["quantiles"]]
+            )
+            + '"'
+        )
+
+        if quantiles:
+            query = f"""
+            from(bucket: "forecast_latest/autogen")
+                |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
+                |> filter(fn: (r) => 
+                    r._measurement == "prediction")
+                |> filter(fn: (r) => 
+                   r._field == "forecast" or r._field == "stdev" or r._field == "forecast_other" or r._field == "forecast_solar" or r._field == "forecast_wind_on_shore"{quantile_section})                 
+                |> filter(fn: (r) => r.pid == "{bind_params["pid"]}")
+                |> aggregateWindow(every: {pj["resolution_minutes"]}m, fn: mean)
+        """
+
+        else:
+            query = f"""
+                from(bucket: "forecast_latest/autogen")
+                    |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
+                    |> filter(fn: (r) => 
+                        r._measurement == "prediction")
+                    |> filter(fn: (r) => 
+                        r._field == "quality" or r._field == "forecast" or r._field == "stdev" or r._field == "forecast_other" or r._field == "forecast_solar" or r._field == "forecast_wind_on_shore")                 
+                    |> filter(fn: (r) => r.pid == "{bind_params["pid"]}")
+                    |> aggregateWindow(every: {pj["resolution_minutes"]}m, fn: mean)
+            """
+
+        # Query the database
+        result = _DataInterface.get_instance().exec_influx_query(query, bind_params)
+
+        # For multiple Fields a list is returned.
+        if isinstance(result, list):
+            result = pd.concat(result)[["_value", "_field", "_time"]]
+
+        # Return result
+        if not result.empty:
+            # Shifting is needed to output the same as with the old influx client
+            return parse_influx_result(result).shift(-15, freq="T")
+        else:
+            return pd.Series()
+
     def get_predicted_load_tahead(
         self,
         pj: dict,
         start_time: datetime = None,
         end_time: datetime = None,
         t_ahead: Union[List[str], str] = None,
         component: bool = False,
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/systems.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,7 +117,32 @@
             SELECT sid, qual, freq, lag
             FROM systems
             WHERE left(sid, 3) = 'pv_' AND autoupdate = %(autoupdate)s
             ORDER BY RAND() {limit_query}
         """
 
         return _DataInterface.get_instance().exec_sql_query(query, bind_params)
+
+    def get_api_key_for_system(self, sid: str) -> str:
+        """Get (sysetm) API key that is connected to a given system.
+
+        Args:
+            sid (str): The system ID
+
+        Returns:
+            str: The API key that is connected to the given system.
+        """
+        bind_params = {"system": sid}
+
+        query = """
+            SELECT 
+                sa.apiKey 
+            FROM `systems` as s 
+            LEFT JOIN `systemsApiKeys` as sa ON s.measurements_customer_api_key_id = sa.id 
+            WHERE s.sid = %(system)s;
+        """
+
+        result = _DataInterface.get_instance().exec_sql_query(query, bind_params)
+        if isinstance(result, pd.DataFrame) and result.empty:
+            return ""
+        else:
+            return result["apiKey"][0]
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/services/write.py` & `openstef_dbc-3.6.3a0/openstef_dbc/services/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,25 +80,19 @@
         # Write DataFrame to influx database
         # Find tag columns
         tag_columns = ["pid", "type", "customer"]
         # Specify field columns
         field_columns = [x for x in forecast.columns if x not in tag_columns]
 
         # Cast columns to correct type, as influx is extremely picky
-        casting_dict = {"prediction": float, "stdev": float, "created": int}
+        casting_dict = {"prediction": float, "stdev": float}
         for col, cast in casting_dict.items():
             if col in field_columns:
                 forecast = forecast.astype({col: cast})
 
-        # TEMPORARY FIX - do not store created, as data types are int on one
-        # shard, but str on another...
-        # FK 20230403
-        forecast = forecast.drop("created", axis=1)
-        # END TEMPORARY FIX
-
         result = _DataInterface.get_instance().exec_influx_write(
             forecast.copy(),
             database=dbname,
             measurement=influxtable,
             tag_columns=tag_columns,
             field_columns=field_columns,
             time_precision="s",
@@ -278,14 +272,49 @@
             )
             self.logger.info(
                 "Successfully written tags to database", tag_columns=tag_columns
             )
 
         return message
 
+    def write_realised_power_measurements(self, df: pd.DataFrame, sid: str):
+        """Method that writes measurement data to the influx database.
+
+        Args:
+            df: pd.DataFrame(index = "datetime", columns = ['output'])
+            sid: (str) String with system id of the measurement
+
+        Returns:
+            None
+        """
+        df["type"] = "measurement"
+        df["system"] = str(sid)
+        df["created"] = int(time.time())
+        df = df.astype({"output": np.float64})
+        # Write to influx database
+        result = _DataInterface.get_instance().exec_influx_write(
+            df,
+            database="realised",
+            measurement="power",
+            tag_columns=["system", "type"],
+            field_columns=["output", "created"],
+            time_precision="s",
+        )
+        if not result:
+            self.logger.error(
+                "Something wend wrong while writing measurement data to influx"
+            )
+            return
+
+        self.logger.info(
+            "Wrote measurement data for {} systems to influx".format(
+                df["system"].nunique()
+            )
+        )
+
     def write_realised_pvdata(self, df: pd.DataFrame, region: str) -> None:
         """Method that writes realised pv data to the influx database. This function
         also adds systems to the systems table in mysql if they do not yet excist.
 
         Args:
             df: pd.DataFrame(index = "datetime", columns = ['output','system'])
             region: (str) String with the pvdata.org region to which the systems in the df belong
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc/utils.py` & `openstef_dbc-3.6.3a0/openstef_dbc/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,22 @@
     datetime_start = datetime_index[0].to_pydatetime()
     datetime_end = datetime_index[-1].to_pydatetime()
 
     return datetime_start, datetime_end, datetime_index
 
 
 def parse_influx_result(
-    result: pd.DataFrame, aditional_indices: list[str] = None
+    result: pd.DataFrame, aditional_indices: list[str] = None, aggfunc="mean"
 ) -> pd.DataFrame:
     """Parse resulting DataFrame of flux query to a format we expect in the rest of the lib."""
     indices = ["_time"]
     if aditional_indices is not None:
         indices.extend(aditional_indices)
 
     result["_time"] = pd.to_datetime(result["_time"])
-    result = result.pivot_table(columns="_field", values="_value", index=indices)
+    result = result.pivot_table(
+        columns="_field", values="_value", index=indices, aggfunc=aggfunc
+    )
     result = result.reset_index().set_index("_time")
     result.index.name = "datetime"
     result.columns.name = ""
     return result
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.3a0/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.2rc0
+Version: 3.6.3a0
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.2rc0/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.3a0/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.2rc0/setup.py` & `openstef_dbc-3.6.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.2c",
+    version="3.6.3a",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

