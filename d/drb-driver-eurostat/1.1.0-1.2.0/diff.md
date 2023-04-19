# Comparing `tmp/drb-driver-eurostat-1.1.0.tar.gz` & `tmp/drb-driver-eurostat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-eurostat-1.1.0.tar", last modified: Thu Jan  5 10:09:51 2023, max compression
+gzip compressed data, was "drb-driver-eurostat-1.2.0.tar", last modified: Wed Apr 19 08:56:03 2023, max compression
```

## Comparing `drb-driver-eurostat-1.1.0.tar` & `drb-driver-eurostat-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4876 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.826168 drb-driver-eurostat-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.826168 drb-driver-eurostat-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/drb/drivers/eurostat/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/drb/drivers/eurostat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/drb/drivers/eurostat/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    13195 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/drb/drivers/eurostat/drb_impl_eurostat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.826168 drb-driver-eurostat-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.826168 drb-driver-eurostat-1.1.0/drb/topics/eurostat/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-05 09:30:57.000000 drb-driver-eurostat-1.1.0/drb/topics/eurostat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-05 09:30:57.000000 drb-driver-eurostat-1.1.0/drb/topics/eurostat/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4876 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      502 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-05 10:09:51.000000 drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-05 10:09:51.834168 drb-driver-eurostat-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-07-26 08:19:16.000000 drb-driver-eurostat-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:18:31.000000 drb-driver-eurostat-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4328 2023-04-18 14:40:36.000000 drb-driver-eurostat-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.522622 drb-driver-eurostat-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.522622 drb-driver-eurostat-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/drb/drivers/eurostat/
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-18 15:06:34.000000 drb-driver-eurostat-1.2.0/drb/drivers/eurostat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/drb/drivers/eurostat/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11953 2023-04-18 15:06:34.000000 drb-driver-eurostat-1.2.0/drb/drivers/eurostat/eurostat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.522622 drb-driver-eurostat-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.530622 drb-driver-eurostat-1.2.0/drb/topics/eurostat/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-05 09:30:57.000000 drb-driver-eurostat-1.2.0/drb/topics/eurostat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-19 08:55:08.000000 drb-driver-eurostat-1.2.0/drb/topics/eurostat/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.530622 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 08:56:03.000000 drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-18 14:40:36.000000 drb-driver-eurostat-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-18 14:40:36.000000 drb-driver-eurostat-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 14:40:36.000000 drb-driver-eurostat-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:56:03.534622 drb-driver-eurostat-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-04-18 15:06:34.000000 drb-driver-eurostat-1.2.0/tests/test_driver_topic_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2023-04-18 15:45:28.000000 drb-driver-eurostat-1.2.0/tests/test_eurostat_data_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-04-18 15:45:28.000000 drb-driver-eurostat-1.2.0/tests/test_eurostat_row_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2023-04-18 15:45:28.000000 drb-driver-eurostat-1.2.0/tests/test_eurostat_service_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2023-04-18 15:45:28.000000 drb-driver-eurostat-1.2.0/tests/test_eurostat_value_node.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-01-04 10:58:40.000000 drb-driver-eurostat-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2022-07-26 08:19:16.000000 drb-driver-eurostat-1.2.0/versioneer.py
```

### Comparing `drb-driver-eurostat-1.1.0/PKG-INFO` & `drb-driver-eurostat-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-eurostat
-Version: 1.1.0
-Summary: DRB Eurostat implementation
-Home-page: https://gitlab.com/drb-python/impl/eurostat
+Version: 1.2.0
+Summary: DRB Eurostat Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/eurostat
 Project-URL: Source, https://gitlab.com/drb-python/impl/eurostat
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # EurostatNode Implementation
 This drb-impl-eurostat module implements access to Eurostat data with DRB data model.
 
 ## Eurostat Factory
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -62,15 +62,15 @@
 
 ```python
 from drb.drivers.eurostat import DrbEurostatFactory
 
 factory = DrbEurostatFactory()
 service = factory.create('eurostat://')
 
-tables = service.get_attribute('tables')
+tables = service @ 'tables'
 search = 'crimes'
 for table in tables:
     if search in table[0].lower():
         print(table)
 ```
 
 Output :
@@ -123,8 +123,7 @@
 5582   NR  ICCS050211    UKN02  434.0   443.0  476.0
 5583   NR  ICCS050211    UKN03  454.0   525.0  549.0
 5584   NR  ICCS050211    UKN04  358.0   340.0  336.0
 5585   NR  ICCS050211    UKN05  630.0   643.0  608.0
 
 [5586 rows x 6 columns]
 ```
-
```

### Comparing `drb-driver-eurostat-1.1.0/README.md` & `drb-driver-eurostat-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ```python
 from drb.drivers.eurostat import DrbEurostatFactory
 
 factory = DrbEurostatFactory()
 service = factory.create('eurostat://')
 
-tables = service.get_attribute('tables')
+tables = service @ 'tables'
 search = 'crimes'
 for table in tables:
     if search in table[0].lower():
         print(table)
 ```
 
 Output :
```

### Comparing `drb-driver-eurostat-1.1.0/drb_driver_eurostat.egg-info/PKG-INFO` & `drb-driver-eurostat-1.2.0/drb_driver_eurostat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-eurostat
-Version: 1.1.0
-Summary: DRB Eurostat implementation
-Home-page: https://gitlab.com/drb-python/impl/eurostat
+Version: 1.2.0
+Summary: DRB Eurostat Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/eurostat
 Project-URL: Source, https://gitlab.com/drb-python/impl/eurostat
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # EurostatNode Implementation
 This drb-impl-eurostat module implements access to Eurostat data with DRB data model.
 
 ## Eurostat Factory
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -62,15 +62,15 @@
 
 ```python
 from drb.drivers.eurostat import DrbEurostatFactory
 
 factory = DrbEurostatFactory()
 service = factory.create('eurostat://')
 
-tables = service.get_attribute('tables')
+tables = service @ 'tables'
 search = 'crimes'
 for table in tables:
     if search in table[0].lower():
         print(table)
 ```
 
 Output :
@@ -123,8 +123,7 @@
 5582   NR  ICCS050211    UKN02  434.0   443.0  476.0
 5583   NR  ICCS050211    UKN03  454.0   525.0  549.0
 5584   NR  ICCS050211    UKN04  358.0   340.0  336.0
 5585   NR  ICCS050211    UKN05  630.0   643.0  608.0
 
 [5586 rows x 6 columns]
 ```
-
```

### Comparing `drb-driver-eurostat-1.1.0/versioneer.py` & `drb-driver-eurostat-1.2.0/versioneer.py`

 * *Files identical despite different names*

