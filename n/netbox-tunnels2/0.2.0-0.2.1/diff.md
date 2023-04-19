# Comparing `tmp/netbox-tunnels2-0.2.0.tar.gz` & `tmp/netbox-tunnels2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-tunnels2-0.2.0.tar", last modified: Wed Apr 19 12:51:24 2023, max compression
+gzip compressed data, was "netbox-tunnels2-0.2.1.tar", last modified: Wed Apr 19 17:07:46 2023, max compression
```

## Comparing `netbox-tunnels2-0.2.0.tar` & `netbox-tunnels2-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.193063 netbox-tunnels2-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/docs/img/tunnel-info.png
--rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/docs/img/tunnel-list.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/netbox_tunnels2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/netbox_tunnels2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/netbox_tunnels2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 12:51:24.000000 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-19 12:51:24.000000 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:51:24.000000 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 12:51:24.000000 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 12:51:24.000000 netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 12:51:24.201063 netbox-tunnels2-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:51:24.197063 netbox-tunnels2-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 12:51:13.000000 netbox-tunnels2-0.2.0/tests/test_netbox_tunnels_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.586333 netbox-tunnels2-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/docs/img/tunnel-info.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/docs/img/tunnel-list.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/tests/test_netbox_tunnels_plugin.py
```

### Comparing `netbox-tunnels2-0.2.0/CONTRIBUTING.md` & `netbox-tunnels2-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/LICENSE` & `netbox-tunnels2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/PKG-INFO` & `netbox-tunnels2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,15 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.0     |
+|   NetBox 3.4   |      0.2.1     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.0/README.md` & `netbox-tunnels2-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.0     |
+|   NetBox 3.4   |      0.2.1     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.0/docs/img/tunnel-info.png` & `netbox-tunnels2-0.2.1/docs/img/tunnel-info.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/docs/img/tunnel-list.png` & `netbox-tunnels2-0.2.1/docs/img/tunnel-list.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/__init__.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/api/serializers.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/api/views.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/filtersets.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/forms.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/graphql.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/migrations/0001_initial.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/models.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/models.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/navigation.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/tables.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/urls.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2/views.py` & `netbox-tunnels2-0.2.1/netbox_tunnels2/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/PKG-INFO` & `netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,15 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.0     |
+|   NetBox 3.4   |      0.2.1     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.0/netbox_tunnels2.egg-info/SOURCES.txt` & `netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,9 +27,12 @@
 netbox_tunnels2.egg-info/top_level.txt
 netbox_tunnels2/api/__init__.py
 netbox_tunnels2/api/serializers.py
 netbox_tunnels2/api/urls.py
 netbox_tunnels2/api/views.py
 netbox_tunnels2/migrations/0001_initial.py
 netbox_tunnels2/migrations/__init__.py
+netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
 tests/__init__.py
 tests/test_netbox_tunnels_plugin.py
```

### Comparing `netbox-tunnels2-0.2.0/pyproject.toml` & `netbox-tunnels2-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-tunnels2"
-version = "0.2.0"
+version = "0.2.1"
 description = "Provides the ability track IP Tunnels."
 readme = "README.md"
 authors = [{ name = "Robert Lynch", email = "robertlynch3@users.noreply.github.com" }]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/robertlynch3/netbox-tunnels2"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `netbox-tunnels2-0.2.0/setup.cfg` & `netbox-tunnels2-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [gh-actions]
 python = 
 	3.10: py310
 	3.9: py39
 	3.8: py38, format, lint, build
 
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `netbox-tunnels2-0.2.0/setup.py` & `netbox-tunnels2-0.2.1/setup.py`

 * *Files identical despite different names*

