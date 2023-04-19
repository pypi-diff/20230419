# Comparing `tmp/alibabacloud_hologram20220601-1.0.0.tar.gz` & `tmp/alibabacloud_hologram20220601-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.0.tar", last modified: Thu Apr 13 10:58:37 2023, max compression
+gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.1.tar", last modified: Wed Apr 19 07:17:57 2023, max compression
```

## Comparing `alibabacloud_hologram20220601-1.0.0.tar` & `alibabacloud_hologram20220601-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25012 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/client.py
--rw-r--r--   0 root         (0) root         (0)    49882 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      447 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-04-13 10:58:37.000000 alibabacloud_hologram20220601-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25012 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/client.py
+-rw-r--r--   0 root         (0) root         (0)    49882 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-04-19 07:17:57.000000 alibabacloud_hologram20220601-1.0.1/setup.py
```

### Comparing `alibabacloud_hologram20220601-1.0.0/LICENSE` & `alibabacloud_hologram20220601-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.0/PKG-INFO` & `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_hologram20220601
-Version: 1.0.0
+Name: alibabacloud-hologram20220601
+Version: 1.0.1
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.0/README-CN.md` & `alibabacloud_hologram20220601-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.0/README.md` & `alibabacloud_hologram20220601-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/client.py` & `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601/models.py` & `alibabacloud_hologram20220601-1.0.1/alibabacloud_hologram20220601/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.0/alibabacloud_hologram20220601.egg-info/PKG-INFO` & `alibabacloud_hologram20220601-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-hologram20220601
-Version: 1.0.0
+Name: alibabacloud_hologram20220601
+Version: 1.0.1
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.0/setup.py` & `alibabacloud_hologram20220601-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hologram20220601.
 
-Created on 13/04/2023
+Created on 19/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hologram20220601"
 NAME = "alibabacloud_hologram20220601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Hologres (20220601) SDK Library for Python"
```

