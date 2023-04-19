# Comparing `tmp/mango-0.0.3.tar.gz` & `tmp/mango-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-0.0.3.tar", last modified: Tue Apr 18 12:58:01 2023, max compression
+gzip compressed data, was "mango-0.0.4.tar", last modified: Wed Apr 19 10:56:30 2023, max compression
```

## Comparing `mango-0.0.3.tar` & `mango-0.0.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-18 12:57:56.000000 mango-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 12:57:56.000000 mango-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 12:58:01.119768 mango-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 12:57:56.000000 mango-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 12:57:56.000000 mango-0.0.3/mango/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/email_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-18 12:57:56.000000 mango-0.0.3/mango/clients/google_cloud_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/config/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 12:57:56.000000 mango-0.0.3/mango/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-18 12:57:56.000000 mango-0.0.3/mango/config/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/data/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 12:57:56.000000 mango-0.0.3/mango/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-18 12:57:56.000000 mango-0.0.3/mango/data/ts_dataset.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-18 12:57:56.000000 mango-0.0.3/mango/images/images_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-18 12:57:56.000000 mango-0.0.3/mango/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/models/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-18 12:57:56.000000 mango-0.0.3/mango/models/neural_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-18 12:57:56.000000 mango-0.0.3/mango/plots/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-18 12:57:56.000000 mango-0.0.3/mango/processing/processing_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 12:57:56.000000 mango-0.0.3/mango/schemas/location.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-18 12:57:56.000000 mango-0.0.3/mango/shared/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.115768 mango-0.0.3/mango/table/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/pytups_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/pytups_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-18 12:57:56.000000 mango-0.0.3/mango/table/table_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/mango/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.119768 mango-0.0.3/mango/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/json_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_bad_type.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_bad_value.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/data/test_good.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_arcgis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_processing_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-18 12:57:56.000000 mango-0.0.3/mango/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:58:01.111768 mango-0.0.3/mango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 12:58:01.000000 mango-0.0.3/mango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:58:01.119768 mango-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 12:57:56.000000 mango-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-19 10:56:17.000000 mango-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 10:56:17.000000 mango-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 10:56:30.779928 mango-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 10:56:17.000000 mango-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 10:56:17.000000 mango-0.0.4/mango/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/email_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/google_cloud_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 10:56:17.000000 mango-0.0.4/mango/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-19 10:56:17.000000 mango-0.0.4/mango/config/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 10:56:17.000000 mango-0.0.4/mango/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-19 10:56:17.000000 mango-0.0.4/mango/data/ts_dataset.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-19 10:56:17.000000 mango-0.0.4/mango/images/images_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/neural_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-19 10:56:17.000000 mango-0.0.4/mango/plots/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/processing_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 10:56:17.000000 mango-0.0.4/mango/schemas/location.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/pytups_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/pytups_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/json_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_bad_type.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_bad_value.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_good.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_arcgis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_processing_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:56:30.779928 mango-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-19 10:56:17.000000 mango-0.0.4/setup.py
```

### Comparing `mango-0.0.3/LICENSE` & `mango-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/PKG-INFO` & `mango-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.3/mango/clients/arcgis.py` & `mango-0.0.4/mango/clients/arcgis.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/clients/email_downloader.py` & `mango-0.0.4/mango/clients/email_downloader.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/clients/email_sender.py` & `mango-0.0.4/mango/clients/email_sender.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/clients/google_cloud_storage.py` & `mango-0.0.4/mango/clients/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/config/base_config.py` & `mango-0.0.4/mango/config/base_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/data/ts_dataset.pkl` & `mango-0.0.4/mango/data/ts_dataset.pkl`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/images/images_functions.py` & `mango-0.0.4/mango/images/images_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/logging/chrono.py` & `mango-0.0.4/mango/logging/chrono.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import logging
 import time
 from .logger import get_basic_logger
 
 
 class Chrono:
     """
     Class to measure time
     """
 
-    basic_logger = get_basic_logger()
-
     def __init__(
-        self, name: str, silent: bool = False, precision: int = 2, logger=basic_logger
+        self, name: str, silent: bool = False, precision: int = 2, logger: str = "root"
     ):
         """
         Constructor of the class
 
         :param name: name of the chrono
         :param silent: if the chrono should be silent
         :param precision: number of decimals to round the time to
-        :param logger: logging logger object
+        :param str logger: the name of the logger to use. It defaults to root
         """
         self.silent = silent
         self.precision = precision
         self.start_time = {name: time.time()}
         self.end = {name: None}
-        self.logger = logger
+        self.logger = logging.getLogger(logger)
 
     def new(self, name: str):
         """
         Method to create a new chrono
 
         :param name: name of the chrono
         """
```

### Comparing `mango-0.0.3/mango/logging/decorators.py` & `mango-0.0.4/mango/logging/decorators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import time
 from functools import wraps
 import logging
 
-logger = logging.getLogger("root")
 
-
-def log_time(func):
+def log_time(logger: str = "root"):
     """
-    The log_time function is a decorator that wraps the function func.
-    It takes the arguments and keyword arguments passed to it, passes them on to func,
-    and returns what func returns. However, before doing so it logs a message with log.info()
-    describing what function is being called and how long it took to execute.
-
-    :param func: pass the function to be decorated
-    :return: the result of the call to func
-    :doc-author: baobab soluciones
+    The log_time functions is a decorator that can receive a logger name as a parameter and returns the actual
+    wraper for the function that is going to be executed
+
+    :param str logger: the name of the logger to use
+    :return: the log_decorator function
     """
+    logger = logging.getLogger(logger)
 
-    @wraps(func)
-    def wrapper(*args, **kwargs):
+    def log_decorator(func):
         """
-        The wrapper function is a decorator that wraps the function func.
+        The log_decorator function is a decorator that wraps the function func.
         It takes the arguments and keyword arguments passed to it, passes them on to func,
         and returns what func returns. However, before doing so it logs a message with log.info()
         describing what function is being called and how long it took to execute.
 
-        :param *args: pass a non-keyworded, variable-length argument list
-        :param **kwargs: catch all keyword arguments that are passed to the function
-        :return: The result of the function it wraps
+        :param func: pass the function to be decorated
+        :return: the result of the call to func
         :doc-author: baobab soluciones
         """
-        start = time.time()
-        result = func(*args, **kwargs)
-        duration = round(time.time() - start, 2)
-        logger.info(f"{func.__name__} took {duration} seconds")
-        return result
 
-    return wrapper
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            """
+            The wrapper function is a decorator that wraps the function func.
+            It takes the arguments and keyword arguments passed to it, passes them on to func,
+            and returns what func returns. However, before doing so it logs a message with log.info()
+            describing what function is being called and how long it took to execute.
+
+            :param *args: pass a non-keyworded, variable-length argument list
+            :param **kwargs: catch all keyword arguments that are passed to the function
+            :return: The result of the function it wraps
+            :doc-author: baobab soluciones
+            """
+            start = time.time()
+            result = func(*args, **kwargs)
+            duration = round(time.time() - start, 2)
+            logger.info(f"{func.__name__} took {duration} seconds")
+            return result
+
+        return wrapper
+
+    return log_decorator
```

### Comparing `mango-0.0.3/mango/logging/logger.py` & `mango-0.0.4/mango/logging/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 
 
-LOG_FORMAT = "%(asctime)s: %(levelname)s %(message)s"
+LOG_FORMAT = "%(asctime)s: %(levelname)s - %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def get_basic_logger(
     console=True,
     log_file=None,
     log_level=logging.INFO,
     log_format=LOG_FORMAT,
     date_format=DATE_FORMAT,
     logger_name="root",
-    clear=True
+    clear=True,
 ):
     """
     Create a basic logger to log messages in console and/or file.
 
     :param console: bool output log in python console.
     :param log_file: str path of the file where to write the log.
     :param log_level: minimal level of log to show (logging.DEBUG, INFO, WARNING...)
```

### Comparing `mango-0.0.3/mango/models/neural_networks.py` & `mango-0.0.4/mango/models/neural_networks.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/plots/plots.py` & `mango-0.0.4/mango/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/processing/__init__.py` & `mango-0.0.4/mango/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/processing/date_functions.py` & `mango-0.0.4/mango/processing/date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/processing/file_functions.py` & `mango-0.0.4/mango/processing/file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/processing/object_functions.py` & `mango-0.0.4/mango/processing/object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/processing/processing_time_series.py` & `mango-0.0.4/mango/processing/processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/shared/const.py` & `mango-0.0.4/mango/shared/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/shared/decorators.py` & `mango-0.0.4/mango/shared/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/table/pytups_table.py` & `mango-0.0.4/mango/table/pytups_table.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/table/pytups_tools.py` & `mango-0.0.4/mango/table/pytups_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/table/table_tools.py` & `mango-0.0.4/mango/table/table_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/const.py` & `mango-0.0.4/mango/tests/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/data/json_dataset.json` & `mango-0.0.4/mango/tests/data/json_dataset.json`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/data/test.xlsx` & `mango-0.0.4/mango/tests/data/test.xlsx`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_arcgis_client.py` & `mango-0.0.4/mango/tests/test_arcgis_client.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_config.py` & `mango-0.0.4/mango/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_date_functions.py` & `mango-0.0.4/mango/tests/test_date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_file_functions.py` & `mango-0.0.4/mango/tests/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_images.py` & `mango-0.0.4/mango/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_models.py` & `mango-0.0.4/mango/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_object_functions.py` & `mango-0.0.4/mango/tests/test_object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_processing_time_series.py` & `mango-0.0.4/mango/tests/test_processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_table.py` & `mango-0.0.4/mango/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_tools.py` & `mango-0.0.4/mango/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango/tests/test_validation.py` & `mango-0.0.4/mango/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/mango.egg-info/PKG-INFO` & `mango-0.0.4/mango.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.3/mango.egg-info/SOURCES.txt` & `mango-0.0.4/mango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-0.0.3/setup.py` & `mango-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "xlsxwriter",
     ],
 }
 
 
 setuptools.setup(
     name="mango",
-    version="0.0.3",
+    version="0.0.4",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Library with a collection of useful classes and methods to DRY",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/mango",
     packages=setuptools.find_packages(),
     classifiers=[
```

