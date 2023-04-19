# Comparing `tmp/rapyuta_io-1.8.0.tar.gz` & `tmp/rapyuta_io-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta_io-1.8.0.tar", last modified: Tue Feb  7 10:51:37 2023, max compression
+gzip compressed data, was "rapyuta_io-1.9.0.tar", last modified: Wed Apr 19 06:25:49 2023, max compression
```

## Comparing `rapyuta_io-1.8.0.tar` & `rapyuta_io-1.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:37.257159 rapyuta_io-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-02-07 10:51:37.257159 rapyuta_io-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:37.253159 rapyuta_io-1.8.0/rapyuta_io/
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:37.257159 rapyuta_io-1.8.0/rapyuta_io/clients/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    26896 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/buildoperation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10159 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/catalog_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/common_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    12216 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/core_api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    12817 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)    63737 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    16229 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    10302 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/organization.py
--rw-r--r--   0 runner    (1001) docker     (122)    44448 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/package.py
--rw-r--r--   0 runner    (1001) docker     (122)    11829 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/paramserver.py
--rw-r--r--   0 runner    (1001) docker     (122)    15478 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/persistent_volumes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     6413 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/provision_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/rip_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    29923 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     9233 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/clients/static_route.py
--rw-r--r--   0 runner    (1001) docker     (122)    80364 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/rio_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:37.257159 rapyuta_io-1.8.0/rapyuta_io/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     2615 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/objdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/object_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/partials.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/pollers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2473 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     4245 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/rapyuta_io/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 10:51:37.253159 rapyuta_io-1.8.0/rapyuta_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-02-07 10:51:37.000000 rapyuta_io-1.8.0/rapyuta_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-02-07 10:51:37.000000 rapyuta_io-1.8.0/rapyuta_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 10:51:37.000000 rapyuta_io-1.8.0/rapyuta_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-07 10:51:37.000000 rapyuta_io-1.8.0/rapyuta_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-07 10:51:37.000000 rapyuta_io-1.8.0/rapyuta_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 10:51:37.257159 rapyuta_io-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-02-07 10:51:06.000000 rapyuta_io-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:49.528375 rapyuta_io-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-04-19 06:25:49.528375 rapyuta_io-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:49.520375 rapyuta_io-1.9.0/rapyuta_io/
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:49.528375 rapyuta_io-1.9.0/rapyuta_io/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26896 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/buildoperation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10159 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/catalog_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12216 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/core_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12817 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63737 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5609 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16225 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10302 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12445 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/organization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44448 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13999 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/paramserver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15478 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/persistent_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6413 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/provision_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/rip_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29923 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6588 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9233 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/clients/static_route.py
+-rw-r--r--   0 runner    (1001) docker     (122)    81618 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/rio_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:49.528375 rapyuta_io-1.9.0/rapyuta_io/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2615 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/objdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/object_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/partials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/pollers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2473 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4245 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/rapyuta_io/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 06:25:49.524375 rapyuta_io-1.9.0/rapyuta_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-04-19 06:25:49.000000 rapyuta_io-1.9.0/rapyuta_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-04-19 06:25:49.000000 rapyuta_io-1.9.0/rapyuta_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 06:25:49.000000 rapyuta_io-1.9.0/rapyuta_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-19 06:25:49.000000 rapyuta_io-1.9.0/rapyuta_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-19 06:25:49.000000 rapyuta_io-1.9.0/rapyuta_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 06:25:49.528375 rapyuta_io-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-04-19 06:25:24.000000 rapyuta_io-1.9.0/setup.py
```

### Comparing `rapyuta_io-1.8.0/LICENSE` & `rapyuta_io-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/PKG-INFO` & `rapyuta_io-1.9.0/rapyuta_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapyuta_io
-Version: 1.8.0
+Name: rapyuta-io
+Version: 1.9.0
 Summary: Rapyuta.io Python SDK
 Home-page: UNKNOWN
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `rapyuta_io-1.8.0/README.md` & `rapyuta_io-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/__init__.py` & `rapyuta_io-1.9.0/rapyuta_io/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     BuildOptions
 from .clients.buildoperation import BuildOperation, BuildOperationInfo
 from .clients.project import Project
 from .clients.secret import Secret, SecretConfigSourceSSHAuth, SecretConfigDocker, \
     SecretConfigSourceBasicAuth
 from .clients.rosbag import UploadOptions
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/api_client.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/api_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/build.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/build.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/buildoperation.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/buildoperation.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/catalog_client.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/catalog_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/core_api_client.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/core_api_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/deployment.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/device.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/device.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/device_manager.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/device_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # encoding: utf-8
 from __future__ import absolute_import
+
 from enum import Enum
 
 from rapyuta_io.clients.device import Device, DeviceStatus
-from rapyuta_io.utils import RestClient, to_objdict
+from rapyuta_io.utils import RestClient
 from rapyuta_io.utils.rest_client import HttpMethod
 from rapyuta_io.utils.settings import DEVICE_API_PATH, DEVICE_SELECTION_API_PATH, PARAMETERS_API_PATH, \
-    DEVICE_API_ADD_DEVICE_PATH
+    DEVICE_API_ADD_DEVICE_PATH, DAEMONS_PATH
 from rapyuta_io.utils.utils import create_auth_header, prepend_bearer_to_auth_token, get_api_response_data, \
     validate_list_of_strings
 
 
 class DeviceArch(str, Enum):
     """
     DeviceArch enumeration represents supported device architectures.
@@ -115,7 +116,13 @@
         response = RestClient(url).method(HttpMethod.POST).headers(headers).execute(payload=device._serialize())
         return get_api_response_data(response, parse_full=True)
 
     def delete_device(self, device_id):
         url = self._device_api_host + DEVICE_API_PATH + device_id
         headers = create_auth_header(self._auth_token, self._project)
         return RestClient(url).method(HttpMethod.DELETE).headers(headers).execute()
+
+    def patch_daemons(self, device_id, payload):
+        url = self._device_api_host + DEVICE_API_PATH + device_id + DAEMONS_PATH
+        headers = create_auth_header(self._auth_token, self._project)
+        response = RestClient(url).method(HttpMethod.PATCH).headers(headers).execute(payload=payload)
+        return get_api_response_data(response, parse_full=True)
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/metrics.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,38 +185,38 @@
     :vartype from_datetime: :py:class:`~datetime.datetime`
     :ivar to_datetime: end time of querying metrics
     :vartype to_datetime: :py:class:`~datetime.datetime`
     :ivar step_interval: time interval to group data
     :vartype step_interval: :py:class:`~rapyuta_io.clients.metrics.StepInterval`
     :ivar ~.metrics: list of metrics
     :vartype ~.metrics: list(:py:class:`~rapyuta_io.clients.metrics.MetricOperation`)
-    :ivar tags: key pair of tags (must include project_id and organization_id)
+    :ivar tags: key pair of tags (must include tenant_id and organization_id)
     :vartype tags: dict
     :ivar sort: ordering to sort the metrics
     :vartype sort: :py:class:`~rapyuta_io.clients.metrics.SortOrder`
     :ivar groupby: list of tags to group data
     :vartype groupby: list(str)
 
     :param from_datetime: start time of querying metrics
     :type from_datetime: :py:class:`~datetime.datetime`
     :param to_datetime: end time of querying metrics
     :type to_datetime: :py:class:`~datetime.datetime`
     :param step_interval: time interval to group data
     :type step_interval: :py:class:`~rapyuta_io.clients.metrics.StepInterval`
     :param metrics: list of metrics
     :type metrics: list(:py:class:`~rapyuta_io.clients.metrics.MetricOperation`)
-    :param tags: key pair of tags (must include project_id and organization_id)
+    :param tags: key pair of tags (must include tenant_id and organization_id)
     :type tags: dict
     :param sort: ordering to sort the metrics
     :type sort: :py:class:`~rapyuta_io.clients.metrics.SortOrder`
     :param groupby: list of tags to group data
     :type groupby: list(str)
     """
 
-    PROJECT_ID_TAG = 'project_id'
+    TENANT_ID_TAG = 'tenant_id'
     ORGANIZATION_ID_TAG = 'organization_id'
 
     def __init__(self, from_datetime, to_datetime, step_interval, metrics, tags=None, sort=None, groupby=None):
         self.validate(from_datetime, to_datetime, step_interval, metrics, tags, sort, groupby)
         self.from_datetime = from_datetime
         self.to_datetime = to_datetime
         self.step_interval = step_interval
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/model.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/native_network.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/native_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rapyuta_io.utils import RestClient
 from rapyuta_io.utils.error import InvalidParameterException, OperationNotAllowedError, ParameterMissingException
 from rapyuta_io.utils.rest_client import HttpMethod
 from rapyuta_io.utils.utils import create_auth_header, get_api_response_data
 from rapyuta_io.utils.object_converter import ObjBase, enum_field, nested_field
 from rapyuta_io.utils.partials import PartialMixin
 import six
-
+from rapyuta_io.clients.common_models import Limits
 
 class NativeNetwork(PartialMixin, ObjBase):
     """
     NativeNetwork represents native network. \n
     Variables marked as (full-only) are only available on a full object. Use `refresh()` to convert a
     partial object into a full one.
 
@@ -192,123 +192,64 @@
 
 
 class Parameters(ObjBase):
     """
     Parameters represents Native Network Parameters
 
     :ivar limits: Values corresponding to limits of the parameters
-    :vartype limits: :py:class:`~rapyuta_io.clients.native_network.NativeNetworkLimits`
+    :vartype limits: :py:class:`~rapyuta_io.clients.common_models.Limits`
     :ivar device_id: device_id of device on which the native network is deployed.
     :vartype device_id: str
     :ivar network_interface: network interface to which native network is binded.
     :vartype network_interface: str
     :ivar restart_policy: restart policy of native network.
     :vartype restart_policy: enum :py:class:`~rapyuta_io.clients.package.RestartPolicy`
 
     :param limits: Values corresponding to limits of the parameters
-    :type limits: :py:class:`~rapyuta_io.clients.native_network.NativeNetworkLimits`
+    :type limits: :py:class:`~rapyuta_io.clients.common_models.Limits`
     :param device: device on which the native network is deployed.
     :type device: :py:class:`~rapyuta_io.clients.device.Device`
     :param network_interface: network interface to which native network is binded.
     :type network_interface: str
     :param restart_policy: restart policy of native network.
     :type restart_policy: enum :py:class:`~rapyuta_io.clients.package.RestartPolicy`
     """
 
     def __init__(self, limits=None, device=None, network_interface=None, restart_policy=None):
-        self.validate(limits, device, network_interface, restart_policy)
+        self.validate(device, network_interface, restart_policy)
         self.limits = limits
         self.device_id = device and device.uuid
         self.network_interface = network_interface
         self.restart_policy = restart_policy
 
     @staticmethod
-    def validate(limits, device, network_interface, restart_policy):
-        if device is None:
-            if not isinstance(limits, _Limits):
-                raise InvalidParameterException('limits must be one of '
-                                                'rapyuta_io.clients.native_network.NativeNetworkLimits')
-            return
-        if not isinstance(device, rapyuta_io.clients.device.Device):
-            raise InvalidParameterException('device must be of type rapyuta_io.clients.device.Device')
-        if not device.get('uuid'):
-            raise InvalidParameterException('uuid field must be present in rapyuta_io.clients.device.Device object')
-        if not device.get('ip_interfaces'):
-            raise InvalidParameterException(
-                'ip_interfaces field must be present in rapyuta_io.clients.device.Device object')
-        ip_interfaces = device.ip_interfaces or {}
-        if network_interface not in list(ip_interfaces.keys()):
-            raise InvalidParameterException('NETWORK_INTERFACE should be in {}'.format(list(ip_interfaces.keys())))
-        if restart_policy is not None and (
-                restart_policy not in list(rapyuta_io.clients.package.RestartPolicy.__members__.values())):
-            raise InvalidParameterException('RestartPolicy must be one of rapyuta_io.clients.package.RestartPolicy')
+    def validate(device, network_interface, restart_policy):
+        if device:
+            if not isinstance(device, rapyuta_io.clients.device.Device):
+                raise InvalidParameterException('device must be of type rapyuta_io.clients.device.Device')
+            if not device.get('uuid'):
+                raise InvalidParameterException('uuid field must be present in rapyuta_io.clients.device.Device object')
+            if not device.get('ip_interfaces'):
+                raise InvalidParameterException(
+                    'ip_interfaces field must be present in rapyuta_io.clients.device.Device object')
+            ip_interfaces = device.ip_interfaces or {}
+            if network_interface not in list(ip_interfaces.keys()):
+                raise InvalidParameterException('NETWORK_INTERFACE should be in {}'.format(list(ip_interfaces.keys())))
+            if restart_policy is not None and (
+                    restart_policy not in list(rapyuta_io.clients.package.RestartPolicy.__members__.values())):
+                raise InvalidParameterException('RestartPolicy must be one of rapyuta_io.clients.package.RestartPolicy')
 
     def get_deserialize_map(self):
         return {
-            'limits': nested_field('limits', _Limits),
+            'limits': nested_field('limits', Limits),
             'device_id': 'device_id',
             'network_interface': 'NETWORK_INTERFACE',
             'restart_policy': enum_field('restart_policy', rapyuta_io.clients.package.RestartPolicy),
         }
 
     def get_serialize_map(self):
         return {
             'limits': 'limits',
             'device_id': 'device_id',
             'NETWORK_INTERFACE': 'network_interface',
             'restart_policy': 'restart_policy'
         }
-
-
-class _Limits(ObjBase):
-    """
-    Limits represents cpu, memory details of the parameter
-
-    :ivar cpu: cpu
-    :vartype cpu: Union [float, integer]
-    :ivar memory: memory
-    :vartype memory: integer
-
-    :param cpu: cpu
-    :type cpu: Union [float, integer]
-    :param memory: memory
-    :type memory: integer
-    """
-
-    def __init__(self, cpu, memory):
-        self.validate(cpu, memory)
-        self.cpu = cpu
-        self.memory = memory
-
-    @staticmethod
-    def validate(cpu, memory):
-        if (not isinstance(cpu, float) and not isinstance(cpu, six.integer_types)) or cpu <= 0:
-            raise InvalidParameterException('cpu must be a positive float or integer')
-        if not isinstance(memory, six.integer_types) or memory <= 0:
-            raise InvalidParameterException('memory must be a positive integer')
-
-    def get_deserialize_map(self):
-        return {
-            'cpu': 'cpu',
-            'memory': 'memory'
-        }
-
-    def get_serialize_map(self):
-        return {
-            'cpu': 'cpu',
-            'memory': 'memory'
-        }
-
-
-class NativeNetworkLimits(object):
-    """
-    NativeNetworkLimits may be one of: \n
-    NativeNetworkLimits.X_SMALL (cpu: 0.5core, memory: 2GB) \n
-    NativeNetworkLimits.SMALL (cpu: 1core, memory: 4GB) \n
-    NativeNetworkLimits.MEDIUM (cpu: 2cores, memory: 8GB) \n
-    NativeNetworkLimits.LARGE (cpu: 4cores, memory: 16GB) \n
-    """
-
-    X_SMALL = _Limits(0.5, 2048)
-    SMALL = _Limits(1, 4096)
-    MEDIUM = _Limits(2, 8192)
-    LARGE = _Limits(4, 16384)
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/organization.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/organization.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/package.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/package.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/paramserver.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/paramserver.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 
     def __str__(self):
         return str(self.value)
 
     File = 'FileNode'
     Value = 'ValueNode'
     Attribute = 'AttributeNode'
-
+    Folder = 'FolderNode'
 
 class _ParamserverClient:
     """
     Internal client for paramserver. Not for public use.
     """
     yaml_content_type = 'text/yaml'
+    json_content_type = 'application/json'
     default_binary_content_type = "application/octet-stream"
 
     def __init__(self, auth_token, project, core_api_host):
         self._auth_token = auth_token
         self._headers = create_auth_header(prepend_bearer_to_auth_token(auth_token), project)
         self._core_api_host = core_api_host
 
@@ -46,17 +47,18 @@
 
     @staticmethod
     def get_md5_checksum(data):
         md5_hash = hashlib.md5()
         md5_hash.update(data)
         return md5_hash.hexdigest()
 
-    def create_file(self, tree_path, filedata, retry_limit=0):
+    def create_file(self, tree_path, filedata, retry_limit=0, content_type=None):
+        content_type = content_type if content_type else self.yaml_content_type
         url = self._core_api_host + PARAMSERVER_API_TREE_PATH + tree_path
-        payload = {'type': _Node.File, 'data': filedata, 'contentType': self.yaml_content_type}
+        payload = {'type': _Node.File, 'data': filedata, 'contentType': content_type}
         response = RestClient(url).method(HttpMethod.PUT).headers(self._headers).retry(retry_limit).execute(payload)
         return get_api_response_data(response, parse_full=True)
 
     def create_binary_file(self, tree_path, file_path, retry_limit=0):
         url = self._core_api_host + PARAMSERVER_API_FILENODE_PATH + tree_path
         content_type = self.default_binary_content_type
         headers = self._headers.copy()
@@ -78,14 +80,20 @@
 
     def create_value(self, tree_path, retry_limit=0):
         url = self._core_api_host + PARAMSERVER_API_TREE_PATH + tree_path
         payload = {'type': _Node.Value}
         response = RestClient(url).method(HttpMethod.PUT).headers(self._headers).retry(retry_limit).execute(payload)
         return get_api_response_data(response, parse_full=True)
 
+    def create_folder(self, tree_path, retry_limit=0):
+        url = self._core_api_host + PARAMSERVER_API_TREE_PATH + tree_path
+        payload = {'type': _Node.Folder}
+        response = RestClient(url).method(HttpMethod.PUT).headers(self._headers).retry(retry_limit).execute(payload)
+        return get_api_response_data(response, parse_full=True)
+
     def create_attribute(self, tree_path, retry_limit=0):
         url = self._core_api_host + PARAMSERVER_API_TREE_PATH + tree_path
         payload = {'type': _Node.Attribute}
         response = RestClient(url).method(HttpMethod.PUT).headers(self._headers).retry(retry_limit).execute(payload)
         return get_api_response_data(response, parse_full=True)
 
     def create_tree(self, tree_name, delete_existing, retry_limit=0):
@@ -122,36 +130,62 @@
                 dir_futures[future] = (new_tree_path, level + 1)
             elif not in_attribute_dir:  # ignore files in attribute directories
                 file_name = os.path.basename(full_path)
                 if file_name.endswith('.yaml'):
                     with open(full_path, 'r') as f:
                         data = f.read()
                     future = executor.submit(self.create_file, new_tree_path, data)
+                elif file_name.endswith('.json'):
+                    with open(full_path, 'r') as f:
+                        data = f.read()
+                    future = executor.submit(self.create_file, new_tree_path, data, content_type=self.json_content_type)
                 else:
                     future = executor.submit(self.create_binary_file, new_tree_path, full_path)
                 file_futures[future] = new_tree_path
         return dir_futures, file_futures
 
-    def upload_configurations(self, rootdir, tree_names, delete_existing_trees):
-        self.validate_args(rootdir, tree_names, delete_existing_trees)
+    def process_folder(self, executor, rootdir, tree_path, level, dir_futures, file_futures):
+        for name in listdir(join(rootdir, tree_path)):
+            full_path = join(rootdir, tree_path, name)
+            new_tree_path = join(tree_path, name)
+            if isdir(full_path):
+                future = executor.submit(self.create_folder, new_tree_path)
+                dir_futures[future] = (new_tree_path, level + 1)
+            else:
+                file_name = os.path.basename(full_path)
+                if file_name.endswith('.yaml'):
+                    with open(full_path, 'r') as f:
+                        data = f.read()
+                    future = executor.submit(self.create_file, new_tree_path, data)
+                elif file_name.endswith('.json'):
+                    with open(full_path, 'r') as f:
+                        data = f.read()
+                    future = executor.submit(self.create_file, new_tree_path, data, content_type=self.json_content_type)
+                else:
+                    future = executor.submit(self.create_binary_file, new_tree_path, full_path)
+                file_futures[future] = new_tree_path
+        return dir_futures, file_futures
+
+    def upload_configurations(self, rootdir, tree_names, delete_existing_trees, as_folder = False):
+        self.validate_args(rootdir, tree_names, delete_existing_trees, as_folder)
         with futures.ThreadPoolExecutor(max_workers=15) as executor:
             dir_futures = self.process_root_dir(executor, rootdir, tree_names, delete_existing_trees)
             file_futures = {}
             done = futures.wait(dir_futures, return_when=futures.FIRST_COMPLETED).done
             future = done.pop() if len(done) else None
             while future is not None:
                 tree_path, level = dir_futures[future]
                 del dir_futures[future]
                 exc = future.exception()
                 if exc is not None:
                     exc.tree_path = tree_path
                     raise exc
 
-                dir_futures, file_futures = self.process_dir(executor, rootdir, tree_path, level, dir_futures,
-                                                             file_futures)
+                processor_func = self.process_dir if not as_folder else self.process_folder
+                dir_futures, file_futures = processor_func(executor, rootdir, tree_path, level, dir_futures, file_futures)
                 done = futures.wait(dir_futures, return_when=futures.FIRST_COMPLETED).done
                 future = done.pop() if len(done) else None
 
             for future in futures.as_completed(file_futures):
                 exc = future.exception()
                 if exc is not None:
                     exc.tree_path = file_futures[future]
@@ -204,22 +238,23 @@
         response = RestClient(blob['signedUrl']).method(HttpMethod.GET).execute()
         path = os.path.join(blob_temp_dir, str(blob['ID']))
         with open(path, 'wb') as f:
             for chunk in response.iter_content(1024 * 1024):
                 f.write(chunk)
 
     @staticmethod
-    def validate_args(rootdir, tree_names, delete_existing_trees):
+    def validate_args(rootdir, tree_names, delete_existing_trees, as_folder = False):
         if not isinstance(rootdir, six.string_types):
             raise InvalidParameterException('rootdir must be a string')
         if tree_names:
             validate_list_of_strings(tree_names, 'tree_names')
         if not isinstance(delete_existing_trees, bool):
             raise InvalidParameterException('delete_existing_trees must be a boolean')
-
+        if not isinstance(as_folder, bool):
+            raise InvalidParameterException('as_folder must be a boolean')
     def download_configurations(self, rootdir, tree_names, delete_existing_trees):
         self.validate_args(rootdir, tree_names, delete_existing_trees)
         self._safe_makedirs(rootdir)
 
         try:
             url = self._core_api_host + PARAMSERVER_API_TREE_PATH.rstrip('/')
             response = RestClient(url).method(HttpMethod.GET).headers(self._headers).retry(0).execute()
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/persistent_volumes.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/persistent_volumes.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/plan.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/plan.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/project.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/project.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/provision_client.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/provision_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/rip_client.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/rip_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/rosbag.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/rosbag.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/routed_network.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/routed_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rapyuta_io.utils import ObjDict
 from rapyuta_io.utils import RestClient
 from rapyuta_io.utils import to_objdict
 from rapyuta_io.utils.rest_client import HttpMethod
 from rapyuta_io.utils.utils import create_auth_header, get_api_response_data
 from rapyuta_io.utils.error import InvalidParameterException
 from rapyuta_io.utils.partials import PartialMixin
-
+from rapyuta_io.clients.common_models import Limits
 
 class RoutedNetwork(PartialMixin, ObjDict):
     """
     RoutedNetwork represents Routed Network. \n
     Variables marked as (full-only) are only available on a full object. Use `refresh()` to convert a
     partial object into a full one.
 
@@ -143,55 +143,11 @@
     :ivar limits: Values corresponding to limits of the parameters
     :vartype limits: :py:class:`~rapyuta_io.clients.routed_network.RoutedNetworkLimits`
 
     :param limits: Values corresponding to limits of the parameters
     :type limits: :py:class:`~rapyuta_io.clients.routed_network.RoutedNetworkLimits`
     """
 
-    def __init__(self, limits):
-        self.validate(limits)
+    def __init__(self, limits = None):
         super(ObjDict, self).__init__(limits=limits)
 
-    @staticmethod
-    def validate(limits):
-        if not isinstance(limits, _Limits):
-            raise InvalidParameterException('limits must be one of '
-                                            'rapyuta_io.clients.routed_network.RoutedNetworkLimits')
-
-
-class _Limits(ObjDict):
-    """
-    Limits represents cpu, memory details of the parameter
-
-    :ivar cpu: cpu
-    :vartype cpu: Union [float, integer]
-    :ivar memory: memory
-    :vartype memory: integer
-
-    :param cpu: cpu
-    :type cpu: Union [float, integer]
-    :param memory: memory
-    :type memory: integer
-    """
-
-    def __init__(self, cpu, memory):
-        self.validate(cpu, memory)
-        super(ObjDict, self).__init__(cpu=cpu, memory=memory)
-
-    @staticmethod
-    def validate(cpu, memory):
-        if (not isinstance(cpu, float) and not isinstance(cpu, six.integer_types)) or cpu <= 0:
-            raise InvalidParameterException('cpu must be a positive float or integer')
-        if not isinstance(memory, six.integer_types) or memory <= 0:
-            raise InvalidParameterException('memory must be a positive integer')
-
 
-class RoutedNetworkLimits(object):
-    """
-    RoutedNetworkLimits may be one of: \n
-    RoutedNetworkLimits.SMALL (cpu: 1core, memory: 4GB) \n
-    RoutedNetworkLimits.MEDIUM (cpu: 2cores, memory: 8GB) \n
-    RoutedNetworkLimits.LARGE (cpu: 4cores, memory: 16GB) \n
-    """
-    SMALL = _Limits(1, 4096)
-    MEDIUM = _Limits(2, 8192)
-    LARGE = _Limits(4, 16384)
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/secret.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/clients/static_route.py` & `rapyuta_io-1.9.0/rapyuta_io/clients/static_route.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/rio_client.py` & `rapyuta_io-1.9.0/rapyuta_io/rio_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # encoding: utf-8
 from __future__ import absolute_import
+
 import json
 import os
 
+import six
+
 from rapyuta_io.clients import DeviceManagerClient, _ParamserverClient
+from rapyuta_io.clients.build import Build, BuildStatus
 from rapyuta_io.clients.catalog_client import CatalogClient
 from rapyuta_io.clients.core_api_client import CoreAPIClient
 from rapyuta_io.clients.deployment import Deployment
 from rapyuta_io.clients.device import Device
+from rapyuta_io.clients.metrics import QueryMetricsRequest, MetricOperation, MetricFunction, QueryMetricsResponse, \
+    ListMetricsRequest, ListTagKeysRequest, \
+    Metric, Tags, ListTagValuesRequest
 from rapyuta_io.clients.native_network import NativeNetwork
-from rapyuta_io.clients.organization import Organization
 from rapyuta_io.clients.package import Package
-from rapyuta_io.clients.project import Project
-from rapyuta_io.clients.secret import Secret
+from rapyuta_io.clients.package import Runtime, ROSDistro, RestartPolicy
 from rapyuta_io.clients.persistent_volumes import VolumeInstance
+from rapyuta_io.clients.project import Project
 from rapyuta_io.clients.rip_client import RIPClient
-from rapyuta_io.clients.routed_network import RoutedNetwork, Parameters
-from rapyuta_io.clients.build import Build, BuildStatus
 from rapyuta_io.clients.rosbag import ROSBagJob, ROSBagJobStatus, ROSBagBlob, ROSBagBlobStatus
-from rapyuta_io.clients.metrics import QueryMetricsRequest, StepInterval, SortOrder, \
-    MetricOperation, MetricFunction, QueryMetricsResponse, ListMetricsRequest, ListTagKeysRequest, \
-    Metric, Tags, ListTagValuesRequest
+from rapyuta_io.clients.routed_network import RoutedNetwork, Parameters
+from rapyuta_io.clients.secret import Secret
+from rapyuta_io.utils import InvalidAuthTokenException, InvalidParameterException
 from rapyuta_io.utils import to_objdict
 from rapyuta_io.utils.settings import VOLUME_PACKAGE_ID, default_host_config
-from rapyuta_io.utils import InvalidAuthTokenException, InvalidParameterException
-from rapyuta_io.clients.package import Runtime, ROSDistro, RestartPolicy
 from rapyuta_io.utils.utils import get_api_response_data, valid_list_elements
-from rapyuta_io.utils.partials import PartialMixin
-import six
 
 
 class Client(object):
     """
     Client class provides access to device, package, volume and deployment classes.
 
     """
@@ -452,14 +452,41 @@
         >>> client = Client(auth_token='auth_token', project='project_guid')
         >>> client.delete_device('device-id')
         """
         if not device_id or not isinstance(device_id, six.string_types):
             raise InvalidParameterException('device_id needs to be a non empty string')
         return self._dmClient.delete_device(device_id)
 
+    def toggle_features(self, device_id, features):
+        """
+        Patch a device on rapyuta.io platform.
+
+        :param device_id: Device ID
+        :type device_id: str
+        :param features: A tuple of featues and their states
+        :type features: list<tuple>
+
+        Following example demonstrates how to toggle features a device.
+
+            >>> from rapyuta_io import Client
+            >>> client = Client(auth_token='auth_token', project='project_guid')
+            >>> client.toggle_features('device-id', [('vpn', True), ('tracing', False)])
+        """
+        if not device_id or not isinstance(device_id, six.string_types):
+            raise InvalidParameterException('device_id needs to be a non empty string')
+        if not features or not (isinstance(features, list) or isinstance(features, tuple)):
+            raise InvalidParameterException('features needs to be a list or tuple')
+
+        data = {}
+        for entry in features:
+            feature, state = entry
+            data[feature] = state
+
+        return self._dmClient.patch_daemons(device_id, data)
+
     def create_package_from_manifest(self, manifest_filepath, retry_limit=0):
         """
         Create package from a manifest file
 
         :param manifest_filepath: File path of the manifest
         :type manifest_filepath: string
         :param retry_limit: No of retry attempts to be carried out if any failures occurs\
@@ -532,24 +559,26 @@
             >>> from rapyuta_io import Client
             >>> client = Client(auth_token='auth_token', project='project_guid')
             >>> package_details = client.create_package(manifest)
 
         """
         return self._catalog_client.create_package(manifest, retry_limit)
 
-    def upload_configurations(self, rootdir, tree_names=None, delete_existing_trees=False):
+    def upload_configurations(self, rootdir, tree_names=None, delete_existing_trees=False, as_folder=False):
         """
         Traverses rootdir and uploads configurations following the same directory structure.
 
         :param rootdir: Path to directory containing configurations
         :type rootdir: str
         :param tree_names: List of specific configuration trees to upload. If None, all trees under rootdir are uploaded
         :type tree_names: list[str], optional
         :param delete_existing_trees: For each tree to upload, delete existing tree at the server. Defaults to False
         :type delete_existing_trees: bool, optional
+        :param as_folder: For each tree to upload, upload as an folder hierarchy
+        :as_folder: bool, optional
 
         Following example demonstrates how to use upload_configurations and handle errors.
 
             >>> from rapyuta_io import Client
             >>> from rapyuta_io.utils.error import BadRequestError, InternalServerError
             >>> client = Client(auth_token='auth_token', project='project_guid')
             >>> try:
@@ -558,15 +587,15 @@
             ...                                  delete_existing_trees=True)
             ... except (BadRequestError, InternalServerError) as e:
             ...     print 'failed API request', e.tree_path, e
             ... except (IOError, OSError) as e:
             ...     print 'failed file/directory read', e
 
         """
-        return self._paramserver_client.upload_configurations(rootdir, tree_names, delete_existing_trees)
+        return self._paramserver_client.upload_configurations(rootdir, tree_names, delete_existing_trees, as_folder)
 
     def download_configurations(self, rootdir, tree_names=None, delete_existing_trees=False):
         """
         Download all configurations to rootdir following the same directory structure. If rootdir does not exist, it is
         created.
 
         :param rootdir: Path to directory to store downloaded configurations
@@ -1596,15 +1625,14 @@
             >>> native_network = NativeNetwork('native_network_name', Runtime.CLOUD, ROSDistro.KINETIC,
             ...                                  parameters=parameters)
             >>> native_network = client.create_native_network(native_network)
         """
         if not isinstance(native_network, NativeNetwork):
             raise InvalidParameterException("native_network must be non-empty and of type "
                                             "rapyuta_io.clients.native_network.NativeNetwork")
-
         native_network_response = self._catalog_client.create_native_network(native_network)
         return self.get_native_network(native_network_response['guid'])
 
     def delete_native_network(self, network_guid):
 
         """
         Delete a native network using its network_guid
@@ -1653,25 +1681,31 @@
 
         """
         if not isinstance(query_metrics_request, QueryMetricsRequest):
             raise InvalidParameterException('metrics_query_request must be '
                                             'of type rapyuta_io.clients.metrics.MetricsQueryRequest')
 
         default_tags = {}
-        if not query_metrics_request.tags.get(query_metrics_request.PROJECT_ID_TAG):
+        if not query_metrics_request.tags.get(query_metrics_request.TENANT_ID_TAG):
             project = self._core_api_client._project
             if not project:
                 raise InvalidParameterException('Either set project on client using client.set_project(), or '
-                                                'set {} in tags'.format(query_metrics_request.PROJECT_ID_TAG))
-            default_tags[query_metrics_request.PROJECT_ID_TAG] = project
+                                                'set {} in tags'.format(query_metrics_request.TENANT_ID_TAG))
+            default_tags[query_metrics_request.TENANT_ID_TAG] = {
+                "operator": "eq",
+                "value": project
+            }
 
         if not query_metrics_request.tags.get(query_metrics_request.ORGANIZATION_ID_TAG):
             user = self._core_api_client.get_user()
             organization_guid = user.organization.guid
-            default_tags[query_metrics_request.ORGANIZATION_ID_TAG] = organization_guid
+            default_tags[query_metrics_request.ORGANIZATION_ID_TAG] = {
+                "operator": "eq",
+                "value": organization_guid
+            }
 
         query_metrics_request.tags.update(default_tags)
 
         response = self._core_api_client.query_metrics(query_metrics_request)
         return QueryMetricsResponse.deserialize(response)
 
     def list_metrics(self, list_metrics_request):
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/constants.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/constants.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/error.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/error.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/objdict.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/objdict.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/object_converter.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/object_converter.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/partials.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/partials.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/pollers.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/pollers.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/query_builder.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/rest_client.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/settings.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Paramserver APIs
 PARAMSERVER_API_BASE_PATH = '/api/paramserver/'
 PARAMSERVER_API_TREE_PATH = PARAMSERVER_API_BASE_PATH + 'tree/'
 PARAMSERVER_API_TREEBLOBS_PATH = PARAMSERVER_API_BASE_PATH + 'treeblobs'
 PARAMSERVER_API_FILENODE_PATH = PARAMSERVER_API_BASE_PATH + 'filenode/'
 # Device selection API host Config
 SHARED_URL_PATH = '/logs/sharedurl'
+DAEMONS_PATH = '/daemons'
 DEVICE_API_BASE_PATH = '/api/device-manager/v0/'
 DEVICE_PATH = 'device/'
 DEVICE_API_PATH = DEVICE_API_BASE_PATH + 'devices/'
 DEVICE_SELECTION_API_PATH = DEVICE_API_BASE_PATH + 'selection/query/'
 DEVICE_CONFIG_VAR_API_PATH = DEVICE_API_BASE_PATH + 'config_variables/'
 DEVICE_COMMAND_API_PATH = DEVICE_API_BASE_PATH + 'cmd/'
 DEVICE_TOPIC_API_PATH = DEVICE_API_BASE_PATH + 'topics/'
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io/utils/utils.py` & `rapyuta_io-1.9.0/rapyuta_io/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/rapyuta_io.egg-info/PKG-INFO` & `rapyuta_io-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapyuta-io
-Version: 1.8.0
+Name: rapyuta_io
+Version: 1.9.0
 Summary: Rapyuta.io Python SDK
 Home-page: UNKNOWN
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `rapyuta_io-1.8.0/rapyuta_io.egg-info/SOURCES.txt` & `rapyuta_io-1.9.0/rapyuta_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapyuta_io-1.8.0/setup.py` & `rapyuta_io-1.9.0/setup.py`

 * *Files identical despite different names*

