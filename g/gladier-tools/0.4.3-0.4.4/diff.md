# Comparing `tmp/gladier-tools-0.4.3.tar.gz` & `tmp/gladier-tools-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-tools-0.4.3.tar", last modified: Thu Apr  6 18:58:48 2023, max compression
+gzip compressed data, was "gladier-tools-0.4.4.tar", last modified: Wed Apr 19 21:17:32 2023, max compression
```

## Comparing `gladier-tools-0.4.3.tar` & `gladier-tools-0.4.4.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.858952 gladier-tools-0.4.3/gladier_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.858952 gladier-tools-0.4.3/gladier_tools/globus/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/globus/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.858952 gladier-tools-0.4.3/gladier_tools/posix/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/asymmetric_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/asymmetric_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/https_download_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/posix/untar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.858952 gladier-tools-0.4.3/gladier_tools/publish/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/publish/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/publish/publishv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/gladier_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/gladier_tools/tests/posix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_gladier_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/posix/test_untar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/gladier_tools/tests/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/publish/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/tests/publish/test_publishv2.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/gladier_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:58:48.858952 gladier-tools-0.4.3/gladier_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-06 18:58:48.000000 gladier-tools-0.4.3/gladier_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-06 18:58:48.000000 gladier-tools-0.4.3/gladier_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:58:48.000000 gladier-tools-0.4.3/gladier_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 18:58:48.000000 gladier-tools-0.4.3/gladier_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 18:58:48.000000 gladier-tools-0.4.3/gladier_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-06 18:58:48.862953 gladier-tools-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-06 18:58:36.000000 gladier-tools-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/experimental/globus/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/globus/mkdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/globus/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/globus/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/asymmetric_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/asymmetric_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/https_download_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/untar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/publishv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_gladier_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_untar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/test_publishv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/setup.py
```

### Comparing `gladier-tools-0.4.3/LICENSE` & `gladier-tools-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/PKG-INFO` & `gladier-tools-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.4.3
+Version: 0.4.4
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.4.3/README.rst` & `gladier-tools-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/globus/transfer.py` & `gladier-tools-0.4.4/gladier_tools/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/asymmetric_decrypt.py` & `gladier-tools-0.4.4/gladier_tools/posix/asymmetric_decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/asymmetric_encrypt.py` & `gladier-tools-0.4.4/gladier_tools/posix/asymmetric_encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/decrypt.py` & `gladier-tools-0.4.4/gladier_tools/posix/decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/encrypt.py` & `gladier-tools-0.4.4/gladier_tools/posix/encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/https_download_file.py` & `gladier-tools-0.4.4/gladier_tools/posix/https_download_file.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/shell_cmd.py` & `gladier-tools-0.4.4/gladier_tools/posix/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/tar.py` & `gladier-tools-0.4.4/gladier_tools/posix/tar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/posix/untar.py` & `gladier-tools-0.4.4/gladier_tools/posix/untar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/publish/publish.py` & `gladier-tools-0.4.4/gladier_tools/publish/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,17 +112,15 @@
     flow_definition = {
         'Comment': 'Publish metadata to Globus Search, with data from the result.',
         'StartAt': 'PublishGatherMetadata',
         'States': {
             'PublishGatherMetadata': {
                 'Comment': 'Say something to start the conversation',
                 'Type': 'Action',
-                'ActionUrl': 'https://automate.funcx.org',
-                'ActionScope': 'https://auth.globus.org/scopes/'
-                               'b3db7e59-a6f1-4947-95c2-59d6b7a70f8c/action_all',
+                'ActionUrl': 'https://compute2.dev.funcx.org/fxap',
                 'ExceptionOnActionFailure': False,
                 'Parameters': {
                     'tasks': [{
                         'endpoint.$': '$.input.funcx_endpoint_non_compute',
                         'function.$': '$.input.publish_gather_metadata_funcx_id',
                         'payload.$': '$.input.pilot',
                     }]
@@ -131,25 +129,25 @@
                 'WaitTime': 60,
                 'Next': 'PublishTransfer',
             },
             'PublishTransfer': {
                 'Comment': 'Transfer files for publication',
                 'Type': 'Action',
                 'ActionUrl': 'https://actions.automate.globus.org/transfer/transfer',
-                'InputPath': '$.PublishGatherMetadata.details.result[0].transfer',
+                'InputPath': '$.PublishGatherMetadata.details.results[0].output.transfer',
                 'ResultPath': '$.PublishTransfer',
                 'WaitTime': 600,
                 'Next': 'PublishIngest',
             },
             'PublishIngest': {
                 'Comment': 'Ingest the search document',
                 'Type': 'Action',
                 'ActionUrl': 'https://actions.globus.org/search/ingest',
                 'ExceptionOnActionFailure': False,
-                'InputPath': '$.PublishGatherMetadata.details.result[0].search',
+                'InputPath': '$.PublishGatherMetadata.details.results[0].output.search',
                 'ResultPath': '$.PublishIngest',
                 'WaitTime': 300,
                 'End': True
             },
         }
     }
```

### Comparing `gladier-tools-0.4.3/gladier_tools/publish/publishv2.py` & `gladier-tools-0.4.4/gladier_tools/publish/publishv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,28 +236,32 @@
     Publishv2 allows for specifying a file or folder on a Globus Collection, and "publishing" the
     data. Publication consists of first gathering metadata on the file or folder, cataloguing the
     metadata with Globus Search, and transferring the file or folder to a Globus Collection. Additional
     metadata may be provided for the ingest step, and several options exist for modifying what
     metadata is automatically gathered.
 
     Dependencies:
-        None!
+
+    * None!
+
     Optional Dependencies:
+
     * puremagic -- Better mimetype detection
     * datacite -- Validation of Datacite (dc) metadata
 
     FuncX Functions:
 
-    Publishv2 uses one function called "publishv2_gather_metadata". For using custom generated metadata from another
+    Publishv2 uses one function called 'publishv2_gather_metadata'. For using custom generated metadata from another
     function, it can be handy to generate the entire 'publishv2_gather_metadata' input block and pass it as flow input
     instead, which can be done via the following:
 
     .. code-block::
+
         @generate_flow_definition(modifiers={
-            'publishv2_gather_metadata': {'payload': '$.MyCustomPayload.details.result[0]'},
+            'publishv2_gather_metadata': {'payload': '$.MyCustomPayload.details.results[0].output'},
         })
 
     This tool nests input under the 'publishv2' keyword. An example is below:
 
     .. code-block::
 
         'publishv2': {
@@ -307,17 +311,15 @@
     flow_definition = {
         "Comment": "Publish metadata to Globus Search, with data from the result.",
         "StartAt": "Publishv2GatherMetadata",
         "States": {
             "Publishv2GatherMetadata": {
                 "Comment": "Generate search metadata and a transfer document",
                 "Type": "Action",
-                "ActionUrl": "https://automate.funcx.org",
-                "ActionScope": "https://auth.globus.org/scopes/"
-                "b3db7e59-a6f1-4947-95c2-59d6b7a70f8c/action_all",
+                "ActionUrl": "https://compute2.dev.funcx.org/fxap",
                 "ExceptionOnActionFailure": True,
                 "Parameters": {
                     "tasks": [
                         {
                             "endpoint.$": "$.input.funcx_endpoint_non_compute",
                             "function.$": "$.input.publishv2_gather_metadata_funcx_id",
                             "payload.$": "$.input.publishv2",
@@ -348,15 +350,15 @@
                 ],
                 "Default": "Publishv2SkipTransfer",
             },
             "Publishv2Transfer": {
                 "Comment": "Transfer files for publication",
                 "Type": "Action",
                 "ActionUrl": "https://actions.automate.globus.org/transfer/transfer",
-                "InputPath": "$.Publishv2GatherMetadata.details.result[0].transfer",
+                "InputPath": "$.Publishv2GatherMetadata.details.results[0].output.transfer",
                 "ResultPath": "$.Publishv2Transfer",
                 "WaitTime": 600,
                 "Next": "Publishv2ChoiceIngest",
             },
             "Publishv2SkipTransfer": {
                 "Comment": "The ingest step has been skipped",
                 "Type": "Pass",
@@ -382,15 +384,15 @@
                 ],
                 "Default": "Publishv2SkipIngest",
             },
             "Publishv2Ingest": {
                 "Comment": "Ingest the search document",
                 "Type": "Action",
                 "ActionUrl": "https://actions.globus.org/search/ingest",
-                "InputPath": "$.Publishv2GatherMetadata.details.result[0].search",
+                "InputPath": "$.Publishv2GatherMetadata.details.results[0].output.search",
                 "ResultPath": "$.Publishv2Ingest",
                 "WaitTime": 300,
                 "Next": "Publishv2Done",
             },
             "Publishv2SkipIngest": {
                 "Comment": "The ingest step has been skipped",
                 "Type": "Pass",
```

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_decrypt.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_encrypt.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_gladier_tools.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_gladier_tools.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_shell_cmd.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_tar.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_tar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/posix/test_untar.py` & `gladier-tools-0.4.4/gladier_tools/tests/posix/test_untar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/publish/test_publish.py` & `gladier-tools-0.4.4/gladier_tools/tests/publish/test_publish.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools/tests/publish/test_publishv2.py` & `gladier-tools-0.4.4/gladier_tools/tests/publish/test_publishv2.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.3/gladier_tools.egg-info/PKG-INFO` & `gladier-tools-0.4.4/gladier_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.4.3
+Version: 0.4.4
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.4.3/gladier_tools.egg-info/SOURCES.txt` & `gladier-tools-0.4.4/gladier_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 gladier_tools/__init__.py
 gladier_tools/version.py
 gladier_tools.egg-info/PKG-INFO
 gladier_tools.egg-info/SOURCES.txt
 gladier_tools.egg-info/dependency_links.txt
 gladier_tools.egg-info/requires.txt
 gladier_tools.egg-info/top_level.txt
+gladier_tools/experimental/__init__.py
+gladier_tools/experimental/base.py
+gladier_tools/experimental/globus/__init__.py
+gladier_tools/experimental/globus/mkdir.py
 gladier_tools/globus/__init__.py
 gladier_tools/globus/transfer.py
 gladier_tools/posix/__init__.py
 gladier_tools/posix/asymmetric_decrypt.py
 gladier_tools/posix/asymmetric_encrypt.py
 gladier_tools/posix/decrypt.py
 gladier_tools/posix/encrypt.py
```

### Comparing `gladier-tools-0.4.3/setup.py` & `gladier-tools-0.4.4/setup.py`

 * *Files identical despite different names*

