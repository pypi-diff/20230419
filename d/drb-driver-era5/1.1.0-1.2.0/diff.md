# Comparing `tmp/drb-driver-era5-1.1.0.tar.gz` & `tmp/drb-driver-era5-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-era5-1.1.0.tar", last modified: Tue Dec 27 17:11:29 2022, max compression
+gzip compressed data, was "drb-driver-era5-1.2.0.tar", last modified: Wed Apr 19 15:15:58 2023, max compression
```

## Comparing `drb-driver-era5-1.1.0.tar` & `drb-driver-era5-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8903 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8441 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.689616 drb-driver-era5-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.689616 drb-driver-era5-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/drb/drivers/era5/
--rw-rw-rw-   0 root         (0) root         (0)      770 2022-12-27 16:40:19.000000 drb-driver-era5-1.1.0/drb/drivers/era5/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/drb/drivers/era5/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    28703 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/drb/drivers/era5/era5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.693616 drb-driver-era5-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       53 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/drb/exceptions/era5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.689616 drb-driver-era5-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.693616 drb-driver-era5-1.1.0/drb/topics/era5/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/drb/topics/era5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/drb/topics/era5/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8903 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-27 17:11:29.000000 drb-driver-era5-1.1.0/drb_driver_era5.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-12-21 10:25:00.000000 drb-driver-era5-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-27 17:11:29.697616 drb-driver-era5-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-20 19:41:15.000000 drb-driver-era5-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.182903 drb-driver-era5-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 15:09:53.000000 drb-driver-era5-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8994 2023-04-19 15:15:58.182903 drb-driver-era5-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8441 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.166902 drb-driver-era5-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.166902 drb-driver-era5-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.190903 drb-driver-era5-1.2.0/drb/drivers/era5/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2022-12-27 16:40:19.000000 drb-driver-era5-1.2.0/drb/drivers/era5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 15:15:58.190903 drb-driver-era5-1.2.0/drb/drivers/era5/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    27883 2023-04-19 09:06:19.000000 drb-driver-era5-1.2.0/drb/drivers/era5/era5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.174903 drb-driver-era5-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/drb/exceptions/era5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.166902 drb-driver-era5-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.174903 drb-driver-era5-1.2.0/drb/topics/era5/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/drb/topics/era5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-19 15:14:24.000000 drb-driver-era5-1.2.0/drb/topics/era5/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.178902 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8994 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:15:57.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 15:15:58.000000 drb-driver-era5-1.2.0/drb_driver_era5.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-19 09:06:19.000000 drb-driver-era5-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-19 15:15:58.190903 drb-driver-era5-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-19 09:06:19.000000 drb-driver-era5-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:15:58.182903 drb-driver-era5-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/tests/test_data_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/tests/test_dataset_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     6913 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/tests/test_predicate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/tests/test_service_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-04-19 09:06:19.000000 drb-driver-era5-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-20 19:41:15.000000 drb-driver-era5-1.2.0/versioneer.py
```

### Comparing `drb-driver-era5-1.1.0/PKG-INFO` & `drb-driver-era5-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-era5
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB era5 OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/era5
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/era5
+Project-URL: Source, https://gitlab.com/drb-python/impl/era5
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # ERA5 driver
  Climate reanalysis produced by ECMWF driver.
 
 # Nodes
 ### Era5ServiceNode
 Represents the Climate Data Store (CDS) service. This node allows to parse dataset of
@@ -246,9 +247,7 @@
 ```
 pip install drb-driver-era5
 ```
 
 
 
 
-
-
```

### Comparing `drb-driver-era5-1.1.0/README.md` & `drb-driver-era5-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-era5-1.1.0/drb/drivers/era5/__init__.py` & `drb-driver-era5-1.2.0/drb/drivers/era5/__init__.py`

 * *Files identical despite different names*

### Comparing `drb-driver-era5-1.1.0/drb/drivers/era5/era5.py` & `drb-driver-era5-1.2.0/drb/drivers/era5/era5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import abc
 from enum import Enum
 from urllib.parse import urlparse
 
+import keyring
+from deprecated.classic import deprecated
 from drb.core import Predicate, DrbNode, ParsedPath, DrbFactory
 from drb.drivers.http import DrbHttpNode
 from drb.exceptions.core import DrbException, \
     DrbNotImplementationException, DrbFactoryException
 from drb.nodes.abstract_node import AbstractNode
 from drb.topics import resolver
-from drb.utils.keyringconnection import kr_check, kr_get_auth
-from requests.auth import AuthBase
-from typing import Optional, List, Union, Any, Dict, Tuple
+from requests.auth import AuthBase, HTTPBasicAuth
+from typing import List, Union, Any
 import cdsapi
 
 list_predefined_variables_era5_land = [
     '10m_u_component_of_wind', '10m_v_component_of_wind',
     '2m_dewpoint_temperature',
     '2m_temperature', 'evaporation_from_bare_soil',
     'evaporation_from_open_water_surfaces_excluding_oceans',
@@ -436,81 +437,62 @@
 
 
 class Era5ServiceNodeCommon(AbstractNode, abc.ABC):
     def __init__(self, parent: DrbNode):
         super().__init__()
 
         self._path = None
-        self._parent = parent
+        self.parent = parent
+        self.namespace_uri = 'ERA5'
+        self._available_impl.clear()
 
     @property
     def path(self) -> ParsedPath:
         if self._path is None:
             if self._parent is None:
                 self._path = ParsedPath(f'/{self.name}')
             else:
                 self._path = self.parent.path / self.name
         return self._path
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return 'ERA5'
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbNotImplementationException(
             f"Era5ServiceNodeCommon doesn't implement {impl}")
 
     def get_predicate_allowed(self):
         return None
 
     @property
     @abc.abstractmethod
     def client_cds(self):
         raise NotImplementedError
 
-    def close(self) -> None:
-        pass
+    def __setitem__(self, key, value):
+        raise NotImplementedError
 
+    def __delitem__(self, key):
+        raise NotImplementedError
 
-class Era5ServiceNode(Era5ServiceNodeCommon):
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return {}
 
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        raise DrbException(f'No attribute ({name}:{namespace_uri}) found!')
+class Era5ServiceNode(Era5ServiceNodeCommon):
 
     def __init__(self, path='https://cds.climate.copernicus.eu/api/v2',
                  auth: Union[AuthBase, str] = None):
         super().__init__(None)
         self._children = None
 
         self._path = path.replace('+era5', '') if '+era5' in path else path
+        self.name = self._path
         if len(self._path) == 0:
             self._path = 'https://cds.climate.copernicus.eu/api/v2'
         self._auth = auth
 
         self._cds = None
 
     @property
-    def name(self) -> str:
-        return self._path
-
-    @property
     def path(self) -> ParsedPath:
         return ParsedPath(self._path)
 
     @property
     def client_cds(self):
         if self._cds is None:
             key = None
@@ -527,18 +509,29 @@
                     url=self._path, verify=True)
         return self._cds
 
     @property
     def auth(self) -> Union[AuthBase, str]:
         if self._auth is not None:
             return self._auth
-        if kr_check(self._path):
-            return kr_get_auth(self._path)
+        if self._auth is None:
+            credential = keyring.get_credential(
+                service_name=self.path.path,
+                username=None
+            )
+            if credential is not None:
+                self._auth = HTTPBasicAuth(
+                    credential.username,
+                    credential.password
+                )
+        return self._auth
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
 
             for enum_data_set in DataSetERA5:
                 self._children.append(Era5NodeDataSet(self, enum_data_set))
 
@@ -546,44 +539,33 @@
 
 
 class Era5NodeDataSet(Era5ServiceNodeCommon):
 
     def __init__(self, parent: Era5ServiceNode, dataset_enum: DataSetERA5):
         super().__init__(parent)
 
-        self._name = dataset_enum.name
+        self.name = dataset_enum.name
         self._children_name = dataset_enum.children
         self._children = None
-        self._attributes = None
         self._list_product_type = dataset_enum.list_product_type
 
         self._predicate_class = dataset_enum.predicate_class
+        self.__init_attributes()
 
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {
-                ('product_type', None): [v for v in self._list_product_type]}
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        try:
-            return self.attributes[name, namespace_uri]
-        except KeyError:
-            raise DrbException(f'No attribute ({name}:{namespace_uri}) found!')
+    def __init_attributes(self):
+        if self._list_product_type is not None:
+            self @= ('product_type', [v for v in self._list_product_type])
 
     @property
     def client_cds(self):
         return self.parent.client_cds
 
     @property
-    def name(self) -> str:
-        return self._name
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
             for child_name in self._children_name:
                 self._children.append(EraNode(self, child_name))
         return self._children
 
@@ -609,32 +591,28 @@
         return self._predicate_class
 
 
 class EraNode(Era5ServiceNodeCommon):
 
     def __init__(self, parent: Era5ServiceNode, name: str):
         super().__init__(parent)
-        self._name = name
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self.parent.attributes
+        self.name = name
+        self.__init_attributes()
 
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        return self.parent.get_attribute(name, namespace_uri)
+    def __init_attributes(self):
+        for k, v in self.parent.attributes:
+            self @= (k, self.parent.attributes[(k, v)])
 
     @property
     def client_cds(self):
         return self.parent.client_cds
 
     @property
-    def name(self) -> str:
-        return self._name
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         return []
 
     def __getitem__(self, item):
         dict_request = {}
         if isinstance(item, dict):
             dict_request = item
@@ -643,58 +621,44 @@
         if 'variable' not in dict_request.keys():
             dict_request['variable'] = self.name
         return self.parent.execute_request(dict_request)
 
 
 class EraNodeData(Era5ServiceNodeCommon):
 
+    def __init__(self, parent: Era5ServiceNode, res):
+        super().__init__(parent)
+        self._parent = parent
+        self.value = res
+        self._child = None
+
+        parsed_uri = urlparse(res['location'])
+        self.name = str(parsed_uri.path).split('/')[-1]
+        self.__init_attributes()
+
+    def __init_attributes(self):
+        for k, v in self.value.items():
+            self @= (k, v)
+
     @property
     def client_cds(self):
         return self.parent.client_cds
 
     @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {(k, None): v for k, v in self._res.items()}
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        try:
-            return self.attributes[name, namespace_uri]
-        except KeyError:
-            raise DrbException(f'No attribute ({name}:{namespace_uri}) found!')
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._child is None:
             url = self._res['location']
             node = DrbHttpNode(url)
 
             self._child = resolver.create(node)
 
         return [self._child]
 
-    def __init__(self, parent: Era5ServiceNode, res):
-        super().__init__(parent)
-        self._parent = parent
-        self._res = res
-        self._attributes = None
-        self._child = None
-
-        parsed_uri = urlparse(res['location'])
-        self._name = str(parsed_uri.path).split('/')[-1]
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def value(self) -> Optional[Any]:
-        return self._res
-
 
 class DataSetERA5(Enum):
     ERA5_LAND = (
         'reanalysis-era5-land',
         list_predefined_variables_era5_land,
         None,
         Era5PredicateEra5Land)
```

### Comparing `drb-driver-era5-1.1.0/drb_driver_era5.egg-info/PKG-INFO` & `drb-driver-era5-1.2.0/drb_driver_era5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-era5
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB era5 OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/era5
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/era5
+Project-URL: Source, https://gitlab.com/drb-python/impl/era5
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # ERA5 driver
  Climate reanalysis produced by ECMWF driver.
 
 # Nodes
 ### Era5ServiceNode
 Represents the Climate Data Store (CDS) service. This node allows to parse dataset of
@@ -246,9 +247,7 @@
 ```
 pip install drb-driver-era5
 ```
 
 
 
 
-
-
```

### Comparing `drb-driver-era5-1.1.0/versioneer.py` & `drb-driver-era5-1.2.0/versioneer.py`

 * *Files identical despite different names*

