# Comparing `tmp/kachery_cloud-0.4.1.tar.gz` & `tmp/kachery_cloud-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kachery_cloud-0.4.1.tar", last modified: Thu Mar 16 12:41:54 2023, max compression
+gzip compressed data, was "kachery_cloud-0.4.2.tar", last modified: Wed Apr 19 18:49:38 2023, max compression
```

## Comparing `kachery_cloud-0.4.1.tar` & `kachery_cloud-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)      465 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     5235 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-03-16 12:41:54.986690 kachery_cloud-0.4.1/bin/
--rwxrwxr-x   0 magland   (1000) magland   (1000)       95 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud
--rwxrwxr-x   0 magland   (1000) magland   (1000)       45 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-cat
--rwxrwxr-x   0 magland   (1000) magland   (1000)       41 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-init
--rwxrwxr-x   0 magland   (1000) magland   (1000)       46 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-link
--rwxrwxr-x   0 magland   (1000) magland   (1000)       46 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-load
--rwxrwxr-x   0 magland   (1000) magland   (1000)       51 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-load-info
--rwxrwxr-x   0 magland   (1000) magland   (1000)       62 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-request-file-experimental
--rwxrwxr-x   0 magland   (1000) magland   (1000)       67 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-share-local-files-experimental
--rwxrwxr-x   0 magland   (1000) magland   (1000)       47 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-store
--rwxrwxr-x   0 magland   (1000) magland   (1000)       53 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/bin/kachery-cloud-store-local
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/kachery_cloud/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1465 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/TemporaryDirectory.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      881 2023-03-13 11:55:03.000000 kachery_cloud-0.4.1/kachery_cloud/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     6265 2023-03-13 11:50:50.000000 kachery_cloud-0.4.1/kachery_cloud/_client_keys.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1002 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_fs_operations.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1100 2023-03-13 14:45:16.000000 kachery_cloud-0.4.1/kachery_cloud/_get_kachery_gateway_url.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      707 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_get_local_client_config.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      843 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_json_stringify_deterministic.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1058 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_kachery_gateway_request.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1258 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_load_github_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2391 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_safe_pickle.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2348 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_serialize.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      217 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_sha1_of_dict.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      136 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/_sha1_of_string.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      442 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/cat_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2168 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/cli.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3615 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/core.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      141 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/get_client_id.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2258 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/get_kachery_cloud_dir.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2634 2023-03-13 11:52:26.000000 kachery_cloud-0.4.1/kachery_cloud/init.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1102 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/link_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1276 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/load_bytes.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    10508 2023-03-14 14:36:25.000000 kachery_cloud-0.4.1/kachery_cloud/load_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2878 2023-03-13 11:53:03.000000 kachery_cloud-0.4.1/kachery_cloud/mutable_local.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3185 2023-03-14 14:37:32.000000 kachery_cloud-0.4.1/kachery_cloud/request_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3462 2023-03-16 11:38:17.000000 kachery_cloud-0.4.1/kachery_cloud/store_file.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3835 2023-03-16 11:38:06.000000 kachery_cloud-0.4.1/kachery_cloud/store_file_local.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/kachery_cloud/zenodo_upload/
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/zenodo_upload/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     5225 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/kachery_cloud/zenodo_upload/zenodo_upload.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/kachery_cloud.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      465 2023-03-16 12:41:54.000000 kachery_cloud-0.4.1/kachery_cloud.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     1409 2023-03-16 12:41:54.000000 kachery_cloud-0.4.1/kachery_cloud.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-03-16 12:41:54.000000 kachery_cloud-0.4.1/kachery_cloud.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       71 2023-03-16 12:41:54.000000 kachery_cloud-0.4.1/kachery_cloud.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       14 2023-03-16 12:41:54.000000 kachery_cloud-0.4.1/kachery_cloud.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      490 2023-03-16 12:41:54.990690 kachery_cloud-0.4.1/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      722 2023-03-13 11:45:01.000000 kachery_cloud-0.4.1/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)      465 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5235 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-19 18:49:38.786195 kachery_cloud-0.4.2/bin/
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       95 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       45 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-cat
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       41 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-init
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       46 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-link
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       46 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-load
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       51 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-load-info
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       62 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-request-file-experimental
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       67 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-share-local-files-experimental
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       47 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-store
+-rwxrwxr-x   0 magland   (1000) magland   (1000)       53 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/bin/kachery-cloud-store-local
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/kachery_cloud/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1465 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/TemporaryDirectory.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      881 2023-03-13 11:55:03.000000 kachery_cloud-0.4.2/kachery_cloud/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     6265 2023-03-13 11:50:50.000000 kachery_cloud-0.4.2/kachery_cloud/_client_keys.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1002 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_fs_operations.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1100 2023-03-13 14:45:16.000000 kachery_cloud-0.4.2/kachery_cloud/_get_kachery_gateway_url.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      707 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_get_local_client_config.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      843 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_json_stringify_deterministic.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1058 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_kachery_gateway_request.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1258 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_load_github_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2391 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_safe_pickle.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2348 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_serialize.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      217 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_sha1_of_dict.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      136 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/_sha1_of_string.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      442 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/cat_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2168 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/cli.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3615 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/core.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      141 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/get_client_id.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2258 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/get_kachery_cloud_dir.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2634 2023-03-13 11:52:26.000000 kachery_cloud-0.4.2/kachery_cloud/init.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1102 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/link_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1276 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/load_bytes.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    10584 2023-04-19 18:47:56.000000 kachery_cloud-0.4.2/kachery_cloud/load_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2878 2023-03-13 11:53:03.000000 kachery_cloud-0.4.2/kachery_cloud/mutable_local.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3185 2023-03-14 14:37:32.000000 kachery_cloud-0.4.2/kachery_cloud/request_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3462 2023-03-16 11:38:17.000000 kachery_cloud-0.4.2/kachery_cloud/store_file.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3835 2023-03-16 11:38:06.000000 kachery_cloud-0.4.2/kachery_cloud/store_file_local.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/kachery_cloud/zenodo_upload/
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/zenodo_upload/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5225 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/kachery_cloud/zenodo_upload/zenodo_upload.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/kachery_cloud.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      465 2023-04-19 18:49:38.000000 kachery_cloud-0.4.2/kachery_cloud.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1409 2023-04-19 18:49:38.000000 kachery_cloud-0.4.2/kachery_cloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-04-19 18:49:38.000000 kachery_cloud-0.4.2/kachery_cloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       71 2023-04-19 18:49:38.000000 kachery_cloud-0.4.2/kachery_cloud.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       14 2023-04-19 18:49:38.000000 kachery_cloud-0.4.2/kachery_cloud.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      490 2023-04-19 18:49:38.790195 kachery_cloud-0.4.2/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      722 2023-03-13 11:45:01.000000 kachery_cloud-0.4.2/setup.py
```

### Comparing `kachery_cloud-0.4.1/LICENSE` & `kachery_cloud-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/README.md` & `kachery_cloud-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/TemporaryDirectory.py` & `kachery_cloud-0.4.2/kachery_cloud/TemporaryDirectory.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/__init__.py` & `kachery_cloud-0.4.2/kachery_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_client_keys.py` & `kachery_cloud-0.4.2/kachery_cloud/_client_keys.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_fs_operations.py` & `kachery_cloud-0.4.2/kachery_cloud/_fs_operations.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_get_kachery_gateway_url.py` & `kachery_cloud-0.4.2/kachery_cloud/_get_kachery_gateway_url.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_get_local_client_config.py` & `kachery_cloud-0.4.2/kachery_cloud/_get_local_client_config.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_json_stringify_deterministic.py` & `kachery_cloud-0.4.2/kachery_cloud/_json_stringify_deterministic.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_kachery_gateway_request.py` & `kachery_cloud-0.4.2/kachery_cloud/_kachery_gateway_request.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_load_github_file.py` & `kachery_cloud-0.4.2/kachery_cloud/_load_github_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_safe_pickle.py` & `kachery_cloud-0.4.2/kachery_cloud/_safe_pickle.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/_serialize.py` & `kachery_cloud-0.4.2/kachery_cloud/_serialize.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/cli.py` & `kachery_cloud-0.4.2/kachery_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/core.py` & `kachery_cloud-0.4.2/kachery_cloud/core.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/get_kachery_cloud_dir.py` & `kachery_cloud-0.4.2/kachery_cloud/get_kachery_cloud_dir.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/init.py` & `kachery_cloud-0.4.2/kachery_cloud/init.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/link_file.py` & `kachery_cloud-0.4.2/kachery_cloud/link_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/load_bytes.py` & `kachery_cloud-0.4.2/kachery_cloud/load_bytes.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/load_file.py` & `kachery_cloud-0.4.2/kachery_cloud/load_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from multiprocessing.dummy import shutdown
 import os
 import shutil
 from typing import Union
 import requests
 import random
 import time
 
@@ -40,14 +39,17 @@
             return fname
         resource_url = os.getenv('KACHERY_RESOURCE_URL', None)
         if resource_url is not None and do_request is not False:
             from .request_file import request_file
             while True:
                 # the timeout refers to how long we will wait for the file to upload before returning
                 rr = request_file(uri, resource_url=resource_url, timeout_sec=5, ignore_local=True, ignore_bucket=True)
+                if rr.errored:
+                    print(f'Error: {rr.error_message}')
+                    return None
                 if not rr.found:
                     return None
                 if rr.completed:
                     print('Downloading file')
                     return load_file(uri, dest=dest, do_request=False) # set do_request=False to avoid possibility of infinnite recursion
                 if rr.queued:
                     print('File queued for upload')
```

### Comparing `kachery_cloud-0.4.1/kachery_cloud/mutable_local.py` & `kachery_cloud-0.4.2/kachery_cloud/mutable_local.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/request_file.py` & `kachery_cloud-0.4.2/kachery_cloud/request_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/store_file.py` & `kachery_cloud-0.4.2/kachery_cloud/store_file.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/store_file_local.py` & `kachery_cloud-0.4.2/kachery_cloud/store_file_local.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud/zenodo_upload/zenodo_upload.py` & `kachery_cloud-0.4.2/kachery_cloud/zenodo_upload/zenodo_upload.py`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/kachery_cloud.egg-info/SOURCES.txt` & `kachery_cloud-0.4.2/kachery_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kachery_cloud-0.4.1/setup.py` & `kachery_cloud-0.4.2/setup.py`

 * *Files identical despite different names*

