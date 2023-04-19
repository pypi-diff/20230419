# Comparing `tmp/drb-driver-netcdf-1.1.1.tar.gz` & `tmp/drb-driver-netcdf-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-netcdf-1.1.1.tar", last modified: Wed Dec 21 10:22:58 2022, max compression
+gzip compressed data, was "drb-driver-netcdf-1.2.0.tar", last modified: Wed Apr 19 08:20:50 2023, max compression
```

## Comparing `drb-driver-netcdf-1.1.1.tar` & `drb-driver-netcdf-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.406580 drb-driver-netcdf-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2618 2022-12-21 10:22:58.406580 drb-driver-netcdf-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2030 2022-12-19 14:52:00.000000 drb-driver-netcdf-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.402580 drb-driver-netcdf-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.402580 drb-driver-netcdf-1.1.1/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.414580 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/
--rw-rw-rw-   0 root         (0) root         (0)      725 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-21 10:22:58.414580 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_common.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_dimension_node.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_group_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_list_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_node_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_variable_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.406580 drb-driver-netcdf-1.1.1/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/exceptions/netcdf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.402580 drb-driver-netcdf-1.1.1/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.406580 drb-driver-netcdf-1.1.1/drb/topics/netcdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/drb/topics/netcdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2022-12-21 09:45:48.000000 drb-driver-netcdf-1.1.1/drb/topics/netcdf/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 10:22:58.406580 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2618 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      709 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       99 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-21 10:22:58.000000 drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      214 2022-12-21 10:22:58.414580 drb-driver-netcdf-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1357 2022-12-19 14:52:00.000000 drb-driver-netcdf-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 12:41:04.000000 drb-driver-netcdf-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2022-12-19 14:52:00.000000 drb-driver-netcdf-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.921820 drb-driver-netcdf-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.917820 drb-driver-netcdf-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11690 2023-04-18 15:24:17.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf_node_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.929820 drb-driver-netcdf-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/exceptions/netcdf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.921820 drb-driver-netcdf-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.929820 drb-driver-netcdf-1.2.0/drb/topics/netcdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/topics/netcdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-04-19 08:19:37.000000 drb-driver-netcdf-1.2.0/drb/topics/netcdf/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.933820 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     3823 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_temporary_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/versioneer.py
```

### Comparing `drb-driver-netcdf-1.1.1/PKG-INFO` & `drb-driver-netcdf-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-netcdf
-Version: 1.1.1
-Summary: DRB NetCDF driver
-Home-page: https://gitlab.com/drb-python/impl/netcdf
+Version: 1.2.0
+Summary: DRB NetCDF Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/netcdf
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/netcdf
 Project-URL: Source, https://gitlab.com/drb-python/impl/netcdf
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Netcdf driver
 This drb-driver-netcdf module implements netcdf format access with DRB data model. It is able to navigates among the netcdf contents.
 
 ## Netcdf Factory and Netcdf Node
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -48,9 +47,7 @@
 ## Using this module
 To include this module into your project, the `drb-driver-netcdf` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 ```commandline
 pip install drb-driver-netcdf
 ```
 
 
-
-
```

### Comparing `drb-driver-netcdf-1.1.1/README.md` & `drb-driver-netcdf-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.1.1/drb/drivers/netcdf/netcdf_node_factory.py` & `drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf_node_factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.1.1/drb_driver_netcdf.egg-info/PKG-INFO` & `drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-netcdf
-Version: 1.1.1
-Summary: DRB NetCDF driver
-Home-page: https://gitlab.com/drb-python/impl/netcdf
+Version: 1.2.0
+Summary: DRB NetCDF Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/netcdf
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/netcdf
 Project-URL: Source, https://gitlab.com/drb-python/impl/netcdf
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Netcdf driver
 This drb-driver-netcdf module implements netcdf format access with DRB data model. It is able to navigates among the netcdf contents.
 
 ## Netcdf Factory and Netcdf Node
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -48,9 +47,7 @@
 ## Using this module
 To include this module into your project, the `drb-driver-netcdf` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 ```commandline
 pip install drb-driver-netcdf
 ```
 
 
-
-
```

### Comparing `drb-driver-netcdf-1.1.1/versioneer.py` & `drb-driver-netcdf-1.2.0/versioneer.py`

 * *Files identical despite different names*

