# Comparing `tmp/alibabacloud_cloudauth20221125-1.0.5.tar.gz` & `tmp/alibabacloud_cloudauth20221125-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20221125-1.0.5.tar", last modified: Mon Jan  9 02:57:16 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20221125-1.0.6.tar", last modified: Wed Apr 19 03:40:30 2023, max compression
```

## Comparing `alibabacloud_cloudauth20221125-1.0.5.tar` & `alibabacloud_cloudauth20221125-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      245 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11554 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/client.py
--rw-r--r--   0 root         (0) root         (0)    16762 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2023-01-09 02:57:16.000000 alibabacloud_cloudauth20221125-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11554 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/client.py
+-rw-r--r--   0 root         (0) root         (0)    17022 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-04-19 03:40:30.000000 alibabacloud_cloudauth20221125-1.0.6/setup.py
```

### Comparing `alibabacloud_cloudauth20221125-1.0.5/LICENSE` & `alibabacloud_cloudauth20221125-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20221125-1.0.5/PKG-INFO` & `alibabacloud_cloudauth20221125-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20221125
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud ID Verification (20221125) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20221125-1.0.5/README-CN.md` & `alibabacloud_cloudauth20221125-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20221125-1.0.5/README.md` & `alibabacloud_cloudauth20221125-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/client.py` & `alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125/models.py` & `alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,38 +79,44 @@
         return self
 
 
 class EntElementVerifyResponseBodyResult(TeaModel):
     def __init__(
         self,
         biz_code: str = None,
+        reason_code: str = None,
         status: str = None,
     ):
         self.biz_code = biz_code
+        self.reason_code = reason_code
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.biz_code is not None:
             result['BizCode'] = self.biz_code
+        if self.reason_code is not None:
+            result['ReasonCode'] = self.reason_code
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BizCode') is not None:
             self.biz_code = m.get('BizCode')
+        if m.get('ReasonCode') is not None:
+            self.reason_code = m.get('ReasonCode')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class EntElementVerifyResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_cloudauth20221125-1.0.5/alibabacloud_cloudauth20221125.egg-info/PKG-INFO` & `alibabacloud_cloudauth20221125-1.0.6/alibabacloud_cloudauth20221125.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20221125
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud ID Verification (20221125) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20221125-1.0.5/setup.py` & `alibabacloud_cloudauth20221125-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20221125.
 
-Created on 09/01/2023
+Created on 19/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20221125"
 NAME = "alibabacloud_cloudauth20221125" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20221125) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

