# Comparing `tmp/alibabacloud_cloudauth-intl20220809-1.0.7.tar.gz` & `tmp/alibabacloud_cloudauth-intl20220809-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-1.0.7.tar", last modified: Fri Jan 13 08:07:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-1.0.8.tar", last modified: Wed Apr 19 04:26:21 2023, max compression
```

## Comparing `alibabacloud_cloudauth-intl20220809-1.0.7.tar` & `alibabacloud_cloudauth-intl20220809-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      246 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14298 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/client.py
--rw-r--r--   0 root         (0) root         (0)    20732 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-01-13 08:07:06.000000 alibabacloud_cloudauth-intl20220809-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15320 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/client.py
+-rw-r--r--   0 root         (0) root         (0)    22196 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-04-19 04:26:21.000000 alibabacloud_cloudauth-intl20220809-1.0.8/setup.py
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/LICENSE` & `alibabacloud_cloudauth-intl20220809-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth-intl20220809
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/README-CN.md` & `alibabacloud_cloudauth-intl20220809-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/README.md` & `alibabacloud_cloudauth-intl20220809-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/client.py` & `alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,36 +216,46 @@
     def initialize_with_options(
         self,
         request: cloudauth_intl_20220809_models.InitializeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_intl_20220809_models.InitializeResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.crop):
+            query['Crop'] = request.crop
         if not UtilClient.is_unset(request.doc_type):
             query['DocType'] = request.doc_type
         if not UtilClient.is_unset(request.face_picture_base_64):
             query['FacePictureBase64'] = request.face_picture_base_64
         if not UtilClient.is_unset(request.face_picture_url):
             query['FacePictureUrl'] = request.face_picture_url
         if not UtilClient.is_unset(request.flow_type):
             query['FlowType'] = request.flow_type
+        if not UtilClient.is_unset(request.id_face_quality):
+            query['IdFaceQuality'] = request.id_face_quality
+        if not UtilClient.is_unset(request.id_spoof):
+            query['IdSpoof'] = request.id_spoof
         if not UtilClient.is_unset(request.merchant_biz_id):
             query['MerchantBizId'] = request.merchant_biz_id
         if not UtilClient.is_unset(request.merchant_user_id):
             query['MerchantUserId'] = request.merchant_user_id
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
+        if not UtilClient.is_unset(request.ocr):
+            query['Ocr'] = request.ocr
         if not UtilClient.is_unset(request.operation_mode):
             query['OperationMode'] = request.operation_mode
         if not UtilClient.is_unset(request.pages):
             query['Pages'] = request.pages
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.product_config):
             query['ProductConfig'] = request.product_config
+        if not UtilClient.is_unset(request.return_url):
+            query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_code):
             query['SceneCode'] = request.scene_code
         if not UtilClient.is_unset(request.service_level):
             query['ServiceLevel'] = request.service_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -268,36 +278,46 @@
     async def initialize_with_options_async(
         self,
         request: cloudauth_intl_20220809_models.InitializeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_intl_20220809_models.InitializeResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.crop):
+            query['Crop'] = request.crop
         if not UtilClient.is_unset(request.doc_type):
             query['DocType'] = request.doc_type
         if not UtilClient.is_unset(request.face_picture_base_64):
             query['FacePictureBase64'] = request.face_picture_base_64
         if not UtilClient.is_unset(request.face_picture_url):
             query['FacePictureUrl'] = request.face_picture_url
         if not UtilClient.is_unset(request.flow_type):
             query['FlowType'] = request.flow_type
+        if not UtilClient.is_unset(request.id_face_quality):
+            query['IdFaceQuality'] = request.id_face_quality
+        if not UtilClient.is_unset(request.id_spoof):
+            query['IdSpoof'] = request.id_spoof
         if not UtilClient.is_unset(request.merchant_biz_id):
             query['MerchantBizId'] = request.merchant_biz_id
         if not UtilClient.is_unset(request.merchant_user_id):
             query['MerchantUserId'] = request.merchant_user_id
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
+        if not UtilClient.is_unset(request.ocr):
+            query['Ocr'] = request.ocr
         if not UtilClient.is_unset(request.operation_mode):
             query['OperationMode'] = request.operation_mode
         if not UtilClient.is_unset(request.pages):
             query['Pages'] = request.pages
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.product_config):
             query['ProductConfig'] = request.product_config
+        if not UtilClient.is_unset(request.return_url):
+            query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_code):
             query['SceneCode'] = request.scene_code
         if not UtilClient.is_unset(request.service_level):
             query['ServiceLevel'] = request.service_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809/models.py` & `alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -390,140 +390,176 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class InitializeRequest(TeaModel):
     def __init__(
         self,
+        crop: str = None,
         doc_type: str = None,
         face_picture_base_64: str = None,
         face_picture_url: str = None,
         flow_type: str = None,
+        id_face_quality: str = None,
+        id_spoof: str = None,
         merchant_biz_id: str = None,
         merchant_user_id: str = None,
         meta_info: str = None,
+        ocr: str = None,
         operation_mode: str = None,
         pages: str = None,
         product_code: str = None,
         product_config: str = None,
+        return_url: str = None,
         scene_code: str = None,
         service_level: str = None,
     ):
+        self.crop = crop
         self.doc_type = doc_type
         self.face_picture_base_64 = face_picture_base_64
         self.face_picture_url = face_picture_url
         self.flow_type = flow_type
+        self.id_face_quality = id_face_quality
+        self.id_spoof = id_spoof
         self.merchant_biz_id = merchant_biz_id
         self.merchant_user_id = merchant_user_id
         self.meta_info = meta_info
+        self.ocr = ocr
         self.operation_mode = operation_mode
         self.pages = pages
         self.product_code = product_code
         self.product_config = product_config
+        self.return_url = return_url
         self.scene_code = scene_code
         self.service_level = service_level
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.crop is not None:
+            result['Crop'] = self.crop
         if self.doc_type is not None:
             result['DocType'] = self.doc_type
         if self.face_picture_base_64 is not None:
             result['FacePictureBase64'] = self.face_picture_base_64
         if self.face_picture_url is not None:
             result['FacePictureUrl'] = self.face_picture_url
         if self.flow_type is not None:
             result['FlowType'] = self.flow_type
+        if self.id_face_quality is not None:
+            result['IdFaceQuality'] = self.id_face_quality
+        if self.id_spoof is not None:
+            result['IdSpoof'] = self.id_spoof
         if self.merchant_biz_id is not None:
             result['MerchantBizId'] = self.merchant_biz_id
         if self.merchant_user_id is not None:
             result['MerchantUserId'] = self.merchant_user_id
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
+        if self.ocr is not None:
+            result['Ocr'] = self.ocr
         if self.operation_mode is not None:
             result['OperationMode'] = self.operation_mode
         if self.pages is not None:
             result['Pages'] = self.pages
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
         if self.product_config is not None:
             result['ProductConfig'] = self.product_config
+        if self.return_url is not None:
+            result['ReturnUrl'] = self.return_url
         if self.scene_code is not None:
             result['SceneCode'] = self.scene_code
         if self.service_level is not None:
             result['ServiceLevel'] = self.service_level
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Crop') is not None:
+            self.crop = m.get('Crop')
         if m.get('DocType') is not None:
             self.doc_type = m.get('DocType')
         if m.get('FacePictureBase64') is not None:
             self.face_picture_base_64 = m.get('FacePictureBase64')
         if m.get('FacePictureUrl') is not None:
             self.face_picture_url = m.get('FacePictureUrl')
         if m.get('FlowType') is not None:
             self.flow_type = m.get('FlowType')
+        if m.get('IdFaceQuality') is not None:
+            self.id_face_quality = m.get('IdFaceQuality')
+        if m.get('IdSpoof') is not None:
+            self.id_spoof = m.get('IdSpoof')
         if m.get('MerchantBizId') is not None:
             self.merchant_biz_id = m.get('MerchantBizId')
         if m.get('MerchantUserId') is not None:
             self.merchant_user_id = m.get('MerchantUserId')
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
+        if m.get('Ocr') is not None:
+            self.ocr = m.get('Ocr')
         if m.get('OperationMode') is not None:
             self.operation_mode = m.get('OperationMode')
         if m.get('Pages') is not None:
             self.pages = m.get('Pages')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
         if m.get('ProductConfig') is not None:
             self.product_config = m.get('ProductConfig')
+        if m.get('ReturnUrl') is not None:
+            self.return_url = m.get('ReturnUrl')
         if m.get('SceneCode') is not None:
             self.scene_code = m.get('SceneCode')
         if m.get('ServiceLevel') is not None:
             self.service_level = m.get('ServiceLevel')
         return self
 
 
 class InitializeResponseBodyResult(TeaModel):
     def __init__(
         self,
         client_cfg: str = None,
         transaction_id: str = None,
+        transaction_url: str = None,
     ):
         self.client_cfg = client_cfg
         self.transaction_id = transaction_id
+        self.transaction_url = transaction_url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.client_cfg is not None:
             result['ClientCfg'] = self.client_cfg
         if self.transaction_id is not None:
             result['TransactionId'] = self.transaction_id
+        if self.transaction_url is not None:
+            result['TransactionUrl'] = self.transaction_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientCfg') is not None:
             self.client_cfg = m.get('ClientCfg')
         if m.get('TransactionId') is not None:
             self.transaction_id = m.get('TransactionId')
+        if m.get('TransactionUrl') is not None:
+            self.transaction_url = m.get('TransactionUrl')
         return self
 
 
 class InitializeResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-1.0.8/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth-intl20220809
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.0.7/setup.py` & `alibabacloud_cloudauth-intl20220809-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth-intl20220809.
 
-Created on 13/01/2023
+Created on 19/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth_intl20220809"
 NAME = "alibabacloud_cloudauth-intl20220809" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python"
```

