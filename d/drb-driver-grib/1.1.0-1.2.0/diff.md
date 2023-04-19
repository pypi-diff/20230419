# Comparing `tmp/drb-driver-grib-1.1.0.tar.gz` & `tmp/drb-driver-grib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-grib-1.1.0.tar", last modified: Mon Dec 19 16:59:49 2022, max compression
+gzip compressed data, was "drb-driver-grib-1.2.0.tar", last modified: Wed Apr 19 15:39:24 2023, max compression
```

## Comparing `drb-driver-grib-1.1.0.tar` & `drb-driver-grib-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2338 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1760 2022-12-19 14:52:25.000000 drb-driver-grib-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.239997 drb-driver-grib-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.239997 drb-driver-grib-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.251997 drb-driver-grib-1.1.0/drb/drivers/grib/
--rw-rw-rw-   0 root         (0) root         (0)      495 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/drivers/grib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-19 16:59:49.251997 drb-driver-grib-1.1.0/drb/drivers/grib/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/drivers/grib/grib_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4960 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/drivers/grib/grib_node.py
--rw-rw-rw-   0 root         (0) root         (0)     4704 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/drivers/grib/grib_node_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      186 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/exceptions/grib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.239997 drb-driver-grib-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/drb/topics/grib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/topics/grib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/drb/topics/grib/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2338 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      113 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-19 16:59:49.000000 drb-driver-grib-1.1.0/drb_driver_grib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-12-19 14:34:50.000000 drb-driver-grib-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 16:59:49.247997 drb-driver-grib-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1320 2022-12-19 14:52:25.000000 drb-driver-grib-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 14:20:07.000000 drb-driver-grib-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.119938 drb-driver-grib-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-30 09:50:20.000000 drb-driver-grib-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-19 15:39:24.119938 drb-driver-grib-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2022-12-19 14:52:25.000000 drb-driver-grib-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.099938 drb-driver-grib-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.099938 drb-driver-grib-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.123938 drb-driver-grib-1.2.0/drb/drivers/grib/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/drb/drivers/grib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 15:39:24.123938 drb-driver-grib-1.2.0/drb/drivers/grib/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/drb/drivers/grib/grib_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/drb/drivers/grib/grib_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4712 2023-01-30 10:23:31.000000 drb-driver-grib-1.2.0/drb/drivers/grib/grib_node_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.111938 drb-driver-grib-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/drb/exceptions/grib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.099938 drb-driver-grib-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.111938 drb-driver-grib-1.2.0/drb/topics/grib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/drb/topics/grib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-19 15:37:52.000000 drb-driver-grib-1.2.0/drb/topics/grib/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.115938 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:39:23.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 15:39:24.000000 drb-driver-grib-1.2.0/drb_driver_grib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-19 15:39:24.123938 drb-driver-grib-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:39:24.119938 drb-driver-grib-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/tests/test_drb_grib_coord.py
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2023-03-21 12:01:31.000000 drb-driver-grib-1.2.0/tests/test_drb_grib_dims.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/tests/test_drb_grib_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/tests/test_drb_grib_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3354 2023-04-19 15:25:01.000000 drb-driver-grib-1.2.0/tests/test_drb_grib_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 14:20:07.000000 drb-driver-grib-1.2.0/versioneer.py
```

### Comparing `drb-driver-grib-1.1.0/PKG-INFO` & `drb-driver-grib-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-grib
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB GRIB driver
-Home-page: https://gitlab.com/drb-python/impl/grib
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/grib
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/grib
 Project-URL: Source, https://gitlab.com/drb-python/impl/grib
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # GRIB driver
 This drb-driver-grib module implements grib format access with DRB data model. It is able to navigates among the grib contents.
 
 ## GRIB Factory and GRIB Node
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -42,9 +41,7 @@
 
 This module depends on cfgrib
 
 See installation of cfgrib, on https://pypi.org/project/cfgrib/
 If you install it by pip install you need to install the ECMWF ecCodes library.
 See https://confluence.ecmwf.int/display/ECC/ecCodes+installation.
 
-
-
```

### Comparing `drb-driver-grib-1.1.0/README.md` & `drb-driver-grib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-grib-1.1.0/drb/drivers/grib/grib_node_factory.py` & `drb-driver-grib-1.2.0/drb/drivers/grib/grib_node_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             self._root_dataset = xarray.open_dataset(
                 self._filename,
                 engine="cfgrib")
         else:
             raise DrbGribNobeException('Unsupported parent '
                                        f'{type(self.base_node).__name__}'
-                                       ' for DrbNetcdfRootNode')
+                                       ' for DrbGribNode')
 
     @property
     def parent(self) -> Optional[DrbNode]:
         return self.base_node.parent
 
     @property
     def path(self) -> ParsedPath:
@@ -120,15 +120,15 @@
     def has_impl(self, impl: type) -> bool:
         if impl == xarray.Dataset:
             return True
         return self.base_node.has_impl(impl)
 
     def get_impl(self, impl: type, **kwargs) -> Any:
         if impl == xarray.Dataset:
-            return True
+            return self._root_dataset
         return self.base_node.get_impl(impl)
 
     def close(self):
         if self._root_dataset is not None:
             self._root_dataset.close()
         if self.temp_file and self._filename is not None:
             os.remove(self._filename)
```

### Comparing `drb-driver-grib-1.1.0/drb_driver_grib.egg-info/PKG-INFO` & `drb-driver-grib-1.2.0/drb_driver_grib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-grib
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB GRIB driver
-Home-page: https://gitlab.com/drb-python/impl/grib
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/grib
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/grib
 Project-URL: Source, https://gitlab.com/drb-python/impl/grib
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # GRIB driver
 This drb-driver-grib module implements grib format access with DRB data model. It is able to navigates among the grib contents.
 
 ## GRIB Factory and GRIB Node
 The module implements the basic factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -42,9 +41,7 @@
 
 This module depends on cfgrib
 
 See installation of cfgrib, on https://pypi.org/project/cfgrib/
 If you install it by pip install you need to install the ECMWF ecCodes library.
 See https://confluence.ecmwf.int/display/ECC/ecCodes+installation.
 
-
-
```

### Comparing `drb-driver-grib-1.1.0/versioneer.py` & `drb-driver-grib-1.2.0/versioneer.py`

 * *Files identical despite different names*

