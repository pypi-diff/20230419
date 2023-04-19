# Comparing `tmp/drb-driver-webdav-1.1.0.tar.gz` & `tmp/drb-driver-webdav-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-webdav-1.1.0.tar", last modified: Mon Dec 19 15:10:48 2022, max compression
+gzip compressed data, was "drb-driver-webdav-1.2.0.tar", last modified: Wed Apr 19 07:00:28 2023, max compression
```

## Comparing `drb-driver-webdav-1.1.0.tar` & `drb-driver-webdav-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3019 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2523 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.891722 drb-driver-webdav-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.891722 drb-driver-webdav-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/drb/drivers/webdav/
--rw-rw-rw-   0 root         (0) root         (0)      263 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/drb/drivers/webdav/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/drb/drivers/webdav/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/drb/drivers/webdav/utility_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     8269 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/drb/drivers/webdav/webdav.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.891722 drb-driver-webdav-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.891722 drb-driver-webdav-1.1.0/drb/topics/webdav/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/drb/topics/webdav/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2022-12-19 14:34:16.000000 drb-driver-webdav-1.1.0/drb/topics/webdav/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3019 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       99 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-19 15:10:48.000000 drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      214 2022-12-19 15:10:48.895722 drb-driver-webdav-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1208 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-19 14:29:16.000000 drb-driver-webdav-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.941200 drb-driver-webdav-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:06:22.000000 drb-driver-webdav-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-04-19 07:00:28.941200 drb-driver-webdav-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.925200 drb-driver-webdav-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.925200 drb-driver-webdav-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.941200 drb-driver-webdav-1.2.0/drb/drivers/webdav/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/drb/drivers/webdav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 07:00:28.941200 drb-driver-webdav-1.2.0/drb/drivers/webdav/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/drb/drivers/webdav/utility_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     8222 2023-04-18 07:54:31.000000 drb-driver-webdav-1.2.0/drb/drivers/webdav/webdav.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.925200 drb-driver-webdav-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.933200 drb-driver-webdav-1.2.0/drb/topics/webdav/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/drb/topics/webdav/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-04-19 06:59:38.000000 drb-driver-webdav-1.2.0/drb/topics/webdav/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.937200 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      616 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 07:00:28.000000 drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-17 14:13:41.000000 drb-driver-webdav-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-17 14:13:41.000000 drb-driver-webdav-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-19 07:00:28.941200 drb-driver-webdav-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-17 14:13:41.000000 drb-driver-webdav-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:00:28.937200 drb-driver-webdav-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2023-04-17 15:19:23.000000 drb-driver-webdav-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2023-04-18 07:54:31.000000 drb-driver-webdav-1.2.0/tests/test_webdav.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-19 14:29:16.000000 drb-driver-webdav-1.2.0/versioneer.py
```

### Comparing `drb-driver-webdav-1.1.0/PKG-INFO` & `drb-driver-webdav-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-webdav
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB Web-based Distributed Authoring and Versioning driver
-Home-page: https://gitlab.com/drb-python/impl/webdav
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/webdav
+Project-URL: Source, https://gitlab.com/drb-python/impl/webdav
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WebDav Implementation
 This drb-driver-webdav module implements the webdav protocol access with DRB data model.
 
 ## WebDav Factory and WebDav Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -70,8 +71,7 @@
 ## Limitations
 
 None
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/webdav
-
```

### Comparing `drb-driver-webdav-1.1.0/README.md` & `drb-driver-webdav-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-webdav-1.1.0/drb/drivers/webdav/webdav.py` & `drb-driver-webdav-1.2.0/drb/drivers/webdav/webdav.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import io
 from typing import Any, Optional, List, Dict, Tuple
 
+import keyring
+from deprecated.classic import deprecated
 from drb.core import DrbFactory, DrbNode, ParsedPath
 from drb.exceptions.core import DrbException, DrbNotImplementationException
 from drb.nodes.abstract_node import AbstractNode
 
 from requests.auth import AuthBase, HTTPBasicAuth
 from webdav3.client import Client
 from webdav3.urn import Urn
@@ -112,66 +114,88 @@
                          verbose mode is off.
 
     """
 
     def __init__(self, webdav_hostname: str, auth: AuthBase = None, **kwargs):
         super().__init__()
         if '+webdav' in webdav_hostname:
-            webdav_hostname = webdav_hostname.replace('+webdav', '')
-        if '+dav' in webdav_hostname:
-            webdav_hostname = webdav_hostname.replace('+dav', '')
+            self.webdav_hostname = webdav_hostname.replace('+webdav', '')
+        elif '+dav' in webdav_hostname:
+            self.webdav_hostname = webdav_hostname.replace('+dav', '')
+        else:
+            self.webdav_hostname = webdav_hostname
         if 'options' in kwargs.keys():
             self.options = kwargs.get('options')
         else:
             self.options = {
                 'webdav_hostname': webdav_hostname,
                 'webdav_root': kwargs.get('webdav_root', None),
                 'webdav_recv_speed': kwargs.get('webdav_recv_speed', None),
                 'webdav_send_speed': kwargs.get('webdav_send_speed', None),
                 'webdav_timeout': kwargs.get('webdav_timeout', 30),
                 'webdav_verbose': kwargs.get('webdav_verbose', False),
             }
-        self._attributes: Dict[Tuple[str, str], Any] = kwargs.get(
-            'attributes',
-            None
-        )
         self._children: List[DrbNode] = None
-        self._parent: DrbNode = kwargs.get('parent', None)
+        self.parent = kwargs.get('parent', None)
         self._path: DrbNode = kwargs.get('path', None)
         if self.parent:
             self.webdav = self.parent.webdav
         else:
             self.webdav = None
-        self.auth = auth
+        self._auth = auth
+        self._available_impl.append(io.BytesIO)
+        self.__init_attr(
+            kwargs.get(
+                'attributes',
+                None
+            )
+        )
+        self.name = self @ 'name'
 
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        self.webdav = WebdavConnection(self.options, self.auth)
-        if self._attributes is None:
-            self._attributes = self.webdav.info(self.path.path)
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if name in self.attributes.keys() and namespace_uri is None:
-            return self.attributes[name]
-        raise DrbException(f'Attribute not found name: {name}, '
-                           f'namespace: {namespace_uri}')
+    def __setitem__(self, key, value):
+        raise NotImplementedError
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
+    def __delitem__(self, key):
+        raise NotImplementedError
+
+    def __init_attr(self, attrs: dict = None):
+        if attrs is not None:
+            for e in attrs.keys():
+                if attrs[e] is None:
+                    self @= (e, -1)
+                else:
+                    self @= (e, attrs[e])
+        else:
+            self.webdav = WebdavConnection(self.options, self.auth)
+            self.__init_attr(self.webdav.info(self.path.path))
 
     @property
     def path(self) -> ParsedPath:
-        self.webdav = WebdavConnection(self.options, self.auth)
+        self.webdav = WebdavConnection(self.options, self._auth)
         if self._path is None:
             self._path = self.webdav.root
         return ParsedPath(self._path)
 
     @property
+    def auth(self) -> AuthBase:
+        if self._auth is None:
+            credential = keyring.get_credential(
+                service_name=self.webdav_hostname,
+                username=None
+            )
+            if credential is not None:
+                self._auth = HTTPBasicAuth(
+                    credential.username,
+                    credential.password
+                )
+        return self._auth
+
+    @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         self.webdav = WebdavConnection(self.options, self.auth)
         if self._children is None:
             self._children = []
             children_attributes = self.webdav.list(
                 self.path.path,
                 get_info=True
@@ -182,49 +206,24 @@
                     options=self.options,
                     parent=self,
                     path=attribute.get('path')
                 )
                 self._children.append(child)
         return self._children
 
-    def close(self) -> None:
-        pass
-
-    @property
-    def name(self) -> str:
-        return self.get_attribute('name')
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    def has_impl(self, impl: type) -> bool:
-        return issubclass(io.BytesIO, impl)
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         self.webdav = WebdavConnection(self.options, self.auth)
-        if self.has_impl(impl) and self.attributes.get('size') is not None:
+        if self.has_impl(impl) and int(self @ 'size') >= 0:
             return Download(
                 self.path.path,
                 self.webdav,
             )
         raise DrbNotImplementationException(
             f'no {impl} implementation found')
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is None:
-                return len(self.children) > 0
-            return name in list(map(lambda x: x.name, self.children))
-        return False
-
 
 class DrbWebdavFactory(DrbFactory):
 
     def _create(self, node: DrbNode) -> DrbNode:
         if isinstance(node, DrbWebdavNode):
             return node
         uri = node.path.name
```

### Comparing `drb-driver-webdav-1.1.0/drb_driver_webdav.egg-info/PKG-INFO` & `drb-driver-webdav-1.2.0/drb_driver_webdav.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-webdav
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB Web-based Distributed Authoring and Versioning driver
-Home-page: https://gitlab.com/drb-python/impl/webdav
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/webdav
+Project-URL: Source, https://gitlab.com/drb-python/impl/webdav
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WebDav Implementation
 This drb-driver-webdav module implements the webdav protocol access with DRB data model.
 
 ## WebDav Factory and WebDav Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -70,8 +71,7 @@
 ## Limitations
 
 None
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/webdav
-
```

### Comparing `drb-driver-webdav-1.1.0/versioneer.py` & `drb-driver-webdav-1.2.0/versioneer.py`

 * *Files identical despite different names*

