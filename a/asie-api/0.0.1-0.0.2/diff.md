# Comparing `tmp/asie_api-0.0.1-py3-none-any.whl.zip` & `tmp/asie_api-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3008 bytes, number of entries: 8
+Zip file size: 3112 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       75 b- defN 23-Mar-16 07:34 asie_api/__init__.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Mar-16 13:21 asie_api/client.py
+-rw-rw-rw-  2.0 fat     2033 b- defN 23-Apr-19 02:11 asie_api/client.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-16 07:05 data_api/__init__.py
 -rw-rw-rw-  2.0 fat     1209 b- defN 23-Mar-16 07:14 data_api/client.py
--rw-rw-rw-  2.0 fat      146 b- defN 23-Apr-19 01:26 asie_api-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 01:26 asie_api-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-19 01:26 asie_api-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      599 b- defN 23-Apr-19 01:26 asie_api-0.0.1.dist-info/RECORD
-8 files, 3733 bytes uncompressed, 1962 bytes compressed:  47.4%
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-19 02:14 asie_api-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 02:14 asie_api-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-19 02:14 asie_api-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      599 b- defN 23-Apr-19 02:14 asie_api-0.0.2.dist-info/RECORD
+8 files, 4140 bytes uncompressed, 2066 bytes compressed:  50.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: data_api/__init__.py
 Comment: 
 
 Filename: data_api/client.py
 Comment: 
 
-Filename: asie_api-0.0.1.dist-info/METADATA
+Filename: asie_api-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: asie_api-0.0.1.dist-info/WHEEL
+Filename: asie_api-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: asie_api-0.0.1.dist-info/top_level.txt
+Filename: asie_api-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: asie_api-0.0.1.dist-info/RECORD
+Filename: asie_api-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asie_api/client.py

```diff
@@ -6,44 +6,57 @@
 import pandas as pd
 import json
 import requests as rq
 
 class DataApi:
 
     __token = ''
+    __host = 'www.asieai.com/quant'
+    __router = '/php/bar_pro.php'
     __http_url = 'http://www.asieai.com/quant/php/bar_pro.php'
     __uid = 'data_share'
 
-    def __init__(self, token='', uid='data_share', timeout=120):
+    def __init__(self, token='', uid='data_share', timeout=120, host=None, router=None):
         """
         Parameters
         ----------
         token: str
             API接口的接入密钥字符串，用于用户的认证
         """
         self.__token = token
         self.__timeout = timeout
         self.__uid = uid
+        if host or router:
+            self.set_url(host, router)
     
     def set_token(self, token):
         """
         Parameters
         ----------
         token: str
             API接口的接入密钥字符串，用于用户的认证
         """
         self.__token = token
 
-    def query(self, api_name, fields='', **kwargs):
+    def set_url(self, host, router=None):
+        if host:
+            self.__host = host    
+        if router:
+            self.__router = router
+
+        self.__http_url = 'http://' + self.__host + self.__router
+
+    def query(self, api_name=None, ent_name=None, fields='', **kwargs):
         req_params = {
             'api': api_name,
+            'ent': ent_name,
             'tok': self.__token,
             'uid': self.__uid,
             'col': fields,
-            'params': kwargs
+            **kwargs
         }
 
         res = rq.post(self.__http_url, json=req_params, timeout=self.__timeout)
 
         if not res:
             return pd.DataFrame()
         try:
```

## Comparing `asie_api-0.0.1.dist-info/RECORD` & `asie_api-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 asie_api/__init__.py,sha256=8NJczHyYSk2UQduAVWLcszdN2IKznDfOJXbjmfN0DVo,75
-asie_api/client.py,sha256=DoKOP17CmbZXIJeN8BtB_4hz8bFWGGXDJydS9KTTKAM,1603
+asie_api/client.py,sha256=Is2ienW4hT-TVB1ZToZ3SVAFoaSmi09K8S3nkoU_srg,2033
 data_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_api/client.py,sha256=tQ8AnkH49pIoh8yOenRUxE1cM-qKha1qDCjDvPG6Eow,1209
-asie_api-0.0.1.dist-info/METADATA,sha256=KXGBEawb4TflAEoRKlTXo_yAaZbA4OseGVVkacl7woo,146
-asie_api-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-asie_api-0.0.1.dist-info/top_level.txt,sha256=n1zX4TlQgKmxYxLGUo0EijT4iA_l_ekYyz_QYpK_jBE,9
-asie_api-0.0.1.dist-info/RECORD,,
+asie_api-0.0.2.dist-info/METADATA,sha256=gxJKcrYgCZFNuCGUA11bm5yqnXgncIpIVk1aaNB67Hs,123
+asie_api-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+asie_api-0.0.2.dist-info/top_level.txt,sha256=n1zX4TlQgKmxYxLGUo0EijT4iA_l_ekYyz_QYpK_jBE,9
+asie_api-0.0.2.dist-info/RECORD,,
```

