# Comparing `tmp/vmware-aria-operations-integration-sdk-lib-0.7.1.tar.gz` & `tmp/vmware-aria-operations-integration-sdk-lib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.1.tar", last modified: Sat Mar  4 23:41:55 2023, max compression
+gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.2.tar", last modified: Wed Apr 19 11:59:02 2023, max compression
```

## Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1.tar` & `vmware-aria-operations-integration-sdk-lib-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.476044 vmware-aria-operations-integration-sdk-lib-0.7.1/
--rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/LICENSE
--rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/NOTICE
--rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-03-04 23:41:55.476514 vmware-aria-operations-integration-sdk-lib-0.7.1/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     2038 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/README.md
--rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-01-11 16:15:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/pyproject.toml
--rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-03-04 23:41:55.479187 vmware-aria-operations-integration-sdk-lib-0.7.1/setup.cfg
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.411062 vmware-aria-operations-integration-sdk-lib-0.7.1/src/
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.417837 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/__init__.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.436130 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/
--rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     3522 2023-02-01 19:20:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/adapter_instance.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2948 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/adapter_logging.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2910 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/data.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.459015 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    12336 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/adapter_definition.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/assertions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     7217 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/attribute.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     9414 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/credential_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/exceptions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    11446 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/group.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6393 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/object_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6437 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/parameter.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/units.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2449 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17112 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/object.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1183 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/pipe_utils.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    13941 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     9803 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/suite_api_client.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     4133 2023-02-24 14:06:04.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/timer.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.467898 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/
--rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-03-04 23:41:55.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-03-04 23:41:55.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-03-04 23:41:55.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-03-04 23:41:55.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-03-04 23:41:55.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-03-04 23:41:55.475324 vmware-aria-operations-integration-sdk-lib-0.7.1/tests/
--rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_collect_result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_object_key.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_result.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.313619 vmware-aria-operations-integration-sdk-lib-0.7.2/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/LICENSE
+-rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/NOTICE
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-04-19 11:59:02.314088 vmware-aria-operations-integration-sdk-lib-0.7.2/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2038 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/README.md
+-rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-01-11 16:15:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/pyproject.toml
+-rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-04-19 11:59:02.316345 vmware-aria-operations-integration-sdk-lib-0.7.2/setup.cfg
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:01.948565 vmware-aria-operations-integration-sdk-lib-0.7.2/src/
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:01.956125 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/__init__.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.163673 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/
+-rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3522 2023-02-01 19:20:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_instance.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2948 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_logging.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2910 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/data.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.269973 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12336 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/adapter_definition.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/assertions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     7217 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/attribute.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     9414 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/credential_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/exceptions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    11446 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/group.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     6393 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/object_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     6437 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/parameter.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/units.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2449 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17112 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/object.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1183 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/pipe_utils.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    13941 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    13784 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/suite_api_client.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     4259 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/timer.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.291415 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.312456 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_collect_result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_object_key.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_result.py
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/LICENSE` & `vmware-aria-operations-integration-sdk-lib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.1
+Version: 0.7.2
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/README.md` & `vmware-aria-operations-integration-sdk-lib-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/setup.cfg` & `vmware-aria-operations-integration-sdk-lib-0.7.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vmware-aria-operations-integration-sdk-lib
-version = 0.7.1
+version = 0.7.2
 author = VMware, Inc.
 author_email = krokos@vmware.com
 description = Object model for interacting with the VMware Aria Operations Containerized API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vmware/vmware-aria-operations-integration-sdk
 project_urls =
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/adapter_instance.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_instance.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/adapter_logging.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_logging.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/data.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/data.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/adapter_definition.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/adapter_definition.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/assertions.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/assertions.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/attribute.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/attribute.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/credential_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/credential_type.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/group.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/group.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/object_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/object_type.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/parameter.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/parameter.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/definition/units.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/units.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/event.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/event.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/object.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/object.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/pipe_utils.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/pipe_utils.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/result.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/aria/ops/timer.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,42 +14,46 @@
     timers: List[Tuple[str, float, float]] = []
 
     def __init__(self, logger: Logger, name: str) -> None:
         self.logger = logger
         self.name = name
 
     def __enter__(self) -> Timer:
-        self.logger.info(self.name)
+        self.logger.info(f"Starting '{self.name}'")
         self.start_time = time()
         return self
 
     def __aenter__(self) -> Timer:
-        self.logger.info(self.name)
+        self.logger.info(f"Starting '{self.name}'")
         self.start_time = time()
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_value: Optional[BaseException] = None,
         traceback: Optional[TracebackType] = None,
     ) -> None:
         end_time = time()
         self.timers.append((self.name, self.start_time, end_time))
-        self.logger.info(f"finished {self.name} in {end_time - self.start_time:.2}s")
+        self.logger.info(
+            f"Finished '{self.name}' in {_to_time(end_time - self.start_time)}"
+        )
 
     def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_value: Optional[BaseException] = None,
         traceback: Optional[TracebackType] = None,
     ) -> None:
         end_time = time()
         self.timers.append((self.name, self.start_time, end_time))
-        self.logger.info(f"finished {self.name} in {end_time - self.start_time:.2}s")
+        self.logger.info(
+            f"Finished '{self.name}' in {_to_time(end_time - self.start_time)}"
+        )
 
     @classmethod
     def graph(cls) -> str:
         headers = ["Operation", "Time"]
         full_headers = []
         width = 88
         time_min = time()
@@ -108,15 +112,15 @@
     return f"{hl[:-1]}\n"
 
 
 def _graph_timespan(start: float, end: float, graph_width: int) -> str:
     line = ""
 
     def in_range(x_coord: float) -> bool:
-        return start <= x_coord < end
+        return start <= x_coord < end or x_coord - 1 < start <= x_coord
 
     for x in range(graph_width):
         if in_range(x - 1) and in_range(x) and in_range(x + 1):
             line += "─"
         elif in_range(x - 1) and in_range(x):
             line += "╼"
         elif in_range(x) and in_range(x + 1):
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.1
+Version: 0.7.2
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt` & `vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_collect_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_collect_result.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_object_key.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_object_key.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.1/tests/test_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_result.py`

 * *Files identical despite different names*

