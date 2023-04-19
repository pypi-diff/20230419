# Comparing `tmp/zalo_sdk-0.1.3-py3-none-any.whl.zip` & `tmp/zalo_sdk-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 6995 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1440 b- defN 23-Apr-14 16:58 zalo_sdk/BaseClient.py
+Zip file size: 9050 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1512 b- defN 23-Apr-19 02:06 zalo_sdk/BaseClient.py
 -rw-r--r--  2.0 unx     2228 b- defN 23-Apr-14 16:45 zalo_sdk/Exception.py
 -rw-r--r--  2.0 unx       34 b- defN 23-Apr-14 16:59 zalo_sdk/__init__.py
--rw-r--r--  2.0 unx     5654 b- defN 23-Apr-14 16:59 zalo_sdk/oa/Client.py
--rw-r--r--  2.0 unx     2228 b- defN 23-Apr-14 16:45 zalo_sdk/oa/ZaloOAException.py
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-14 16:58 zalo_sdk/oa/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Apr-14 17:02 zalo_sdk-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1462 b- defN 23-Apr-14 17:02 zalo_sdk-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 17:02 zalo_sdk-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 17:02 zalo_sdk-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      865 b- defN 23-Apr-14 17:02 zalo_sdk-0.1.3.dist-info/RECORD
-11 files, 15147 bytes uncompressed, 5535 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx     5394 b- defN 23-Apr-19 02:06 zalo_sdk/oa/Client.py
+-rw-r--r--  2.0 unx     5414 b- defN 23-Apr-19 02:06 zalo_sdk/oa/ZaloMessage.py
+-rw-r--r--  2.0 unx     2426 b- defN 23-Apr-19 02:06 zalo_sdk/oa/ZaloOAException.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-19 02:06 zalo_sdk/oa/__init__.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Apr-19 02:09 zalo_sdk-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-19 02:09 zalo_sdk-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 02:09 zalo_sdk-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-19 02:09 zalo_sdk-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      948 b- defN 23-Apr-19 02:09 zalo_sdk-0.1.4.dist-info/RECORD
+12 files, 21021 bytes uncompressed, 7462 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: zalo_sdk/__init__.py
 Comment: 
 
 Filename: zalo_sdk/oa/Client.py
 Comment: 
 
+Filename: zalo_sdk/oa/ZaloMessage.py
+Comment: 
+
 Filename: zalo_sdk/oa/ZaloOAException.py
 Comment: 
 
 Filename: zalo_sdk/oa/__init__.py
 Comment: 
 
-Filename: zalo_sdk-0.1.3.dist-info/LICENSE
+Filename: zalo_sdk-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: zalo_sdk-0.1.3.dist-info/METADATA
+Filename: zalo_sdk-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: zalo_sdk-0.1.3.dist-info/WHEEL
+Filename: zalo_sdk-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: zalo_sdk-0.1.3.dist-info/top_level.txt
+Filename: zalo_sdk-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: zalo_sdk-0.1.3.dist-info/RECORD
+Filename: zalo_sdk-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zalo_sdk/BaseClient.py

```diff
@@ -19,19 +19,20 @@
     def access_token(self):
         return self._access_token
 
     @access_token.setter
     def access_token(self, token):
         self._access_token = token
 
-    def send_request(self, method, url, body):
+    def send_request(self, method: str, url: str, body: dict, xtra_headers: str = {}):
         if method == "POST":
             headers = {
                 'Content-Type': "application/json",
-                'access_token': self._access_token
+                'access_token': self._access_token,
+                **xtra_headers
             }
             response = requests.post(
                 url,
                 json=body,
                 headers=headers)
         elif method == "GET":
             headers = {
```

## zalo_sdk/oa/Client.py

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2023, TNT International Trading Corp.
 # All rights reserved.
 
 import datetime
 import requests
 import urllib.parse
 from zalo_sdk import BaseClient
-from zalo_sdk.oa import ZaloOAException
+import zalo_sdk.oa
 
 
 class Client(BaseClient):
     def __init__(self, app_id, secret_key):
         super(BaseClient)
         self.app_id = app_id
         self.secret_key = secret_key
@@ -18,17 +18,18 @@
     def isAccessTokenExpired(self):
         return self.expire_at != 0 and self.expire_at < datetime.datetime.utcnow().timestamp()
         # If expire_at == 0, skip the check
 
     def check_zalo_error(self, response):
         if "error" in response and response["error"] != 0:
             if "message" in response:
-                raise ZaloOAException(response["error"], response["message"])
-            else:
-                raise ZaloOAException(response["error"])
+                if response["error"] == -216 and "expired" in response["message"]:
+                    raise zalo_sdk.oa.ZaloOAAuthTokenExpiredException(response["error"], response["message"])
+                raise zalo_sdk.oa.ZaloOAException(response["error"], response["message"])
+            raise zalo_sdk.oa.ZaloOAException.ZaloOAException(response["error"])
 
     def request_authoriation_code_url(self, callback_url, challenge_string=None):
         """
         Get the URL to request the authorization code.
 
         Official Documentation: https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-1-xac-thuc-voi-giao-thuc-oauth/lay-oa-access-token-tu-oa-refresh-token-post-4970
         """
@@ -42,18 +43,19 @@
             params['state'] = challenge_string
 
         auth_url = parsed_url._replace(query=urllib.parse.urlencode(params))
         return auth_url.geturl()
 
     def check_and_set_token(self, zalo_response):
         if 'refresh_token' not in zalo_response:
-            raise ZaloException(-1,
-                                "'refresh_token' not found in the response")
+            raise zalo_sdk.oa.ZaloOAException(-1,
+                                  "'refresh_token' not found in the response")
         if 'access_token' not in zalo_response:
-            raise ZaloException(-1, "'access_token' not found in the response")
+            raise zalo_sdk.oa.ZaloOAException(-1,
+                                  "'access_token' not found in the response")
 
         expire_in = int(zalo_response.get("expires_in", 0))
         expire_at = datetime.datetime.now()+datetime.timedelta(seconds=expire_in)
         self.refresh_token = zalo_response['refresh_token']
         self.access_token = zalo_response['access_token']
         self.expire_at = int(expire_at.timestamp())
 
@@ -98,48 +100,26 @@
 
         zalo_response = response.json()
         self.check_zalo_error(zalo_response)
         self.check_and_set_token(zalo_response)
 
         return self.access_token, self.refresh_token, self.expire_at
 
-    def send_message_to_user(self, user_id, message):
-        body = {
-            "recipient": {
-                "user_id": user_id
-            },
-            "message": {
-                "text": message
-            }
-        }
-        response = self.send_request(
-            "POST", "https://openapi.zalo.me/v2.0/oa/message", body)
-        self.check_http_error(response)
-
-        zalo_response = response.json()
-        self.check_zalo_error(zalo_response)
-
-        return zalo_response
-
-    def send_response_to_user(self, message_id, message):
-        body = {
-            "recipient": {
-                "message_id": message_id
-            },
-            "message": {
-                "text": message
-            }
-        }
+    def send_message(self, recipient, body=None, action=None):
+        msg_obj = zalo_sdk.oa.ZaloMessage(
+            recipient=recipient,
+            message_body=body,
+            action=action
+        )
         response = self.send_request(
-            "POST", "https://openapi.zalo.me/v2.0/oa/message", body)
+            "POST", "https://openapi.zalo.me/v2.0/oa/message", msg_obj.toDict())
         self.check_http_error(response)
 
         zalo_response = response.json()
         self.check_zalo_error(zalo_response)
-
         return zalo_response
 
     def get_free_response_quota(self, message_id):
         body = {
             "message_id": message_id
         }
         response = self.send_request(
@@ -159,8 +139,8 @@
             "GET", "https://openapi.zalo.me/v2.0/oa/getprofile", params
         )
         self.check_http_error(response)
 
         zalo_response = response.json()
         self.check_zalo_error(zalo_response)
 
-        return zalo_response
+        return zalo_response
```

## zalo_sdk/oa/ZaloOAException.py

```diff
@@ -45,7 +45,14 @@
         return self._msg
 
     def errCodeToStr(self) -> str:
         if self._code in ZaloOAException.ERROR_CODE_TO_STR:
             return ZaloOAException.ERROR_CODE_TO_STR[self._code]
 
         return "Unknown error"
+
+class ZaloOAAuthTokenExpiredException(ZaloOAException):
+    """
+    Auth token expired expcetion. When we get this exception, we should
+    refresh the auth token to get a new one.
+    """
+    pass
```

## zalo_sdk/oa/__init__.py

```diff
@@ -1,2 +1,3 @@
-from .Client import Client
-from .ZaloOAException import ZaloOAException
+from .Client import *
+from .ZaloOAException import *
+from .ZaloMessage import *
```

## Comparing `zalo_sdk-0.1.3.dist-info/LICENSE` & `zalo_sdk-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zalo_sdk-0.1.3.dist-info/METADATA` & `zalo_sdk-0.1.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Zalo SDK
 Home-page: https://github.com/connext-biz/zalo_integration
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
@@ -25,8 +25,25 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 License-File: LICENSE
 
-# zalo_integration
+# Zalo Integration SDK
+
+This is a work in progress project. **Use at your own risk!**
+
+At this point, this library only support Official Account APIs.
+
+If you found any problems, please create an issue to track it, or feel free to open a PR.
+
+## Installation
+
+`pip install zalo_sdk`
+
+
+## Documentation
+
+The code is its own document.
+
+(I'm kidding, I'll add documentation later)
```

## Comparing `zalo_sdk-0.1.3.dist-info/RECORD` & `zalo_sdk-0.1.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-zalo_sdk/BaseClient.py,sha256=V_jZ9PoSJHkhG5DFSuDT_eo9_YjA1zK-Lus6u09CRxs,1440
+zalo_sdk/BaseClient.py,sha256=YyeOwkyUBrhAiRFsYwd93SF4QrAlGHsgxgdrPxotRUs,1512
 zalo_sdk/Exception.py,sha256=XUze9ukyscBA3ExHek4qisrsUigpSl6mHinrXghaUOk,2228
 zalo_sdk/__init__.py,sha256=eMIRVZSpFkWrKuSRsC_og-vZDGPaGs760mMWttqWIZ0,34
-zalo_sdk/oa/Client.py,sha256=YGN3ZbqacHUlSRo1USmuy77jOhfjDfl5xEOk2UjOmho,5654
-zalo_sdk/oa/ZaloOAException.py,sha256=XUze9ukyscBA3ExHek4qisrsUigpSl6mHinrXghaUOk,2228
-zalo_sdk/oa/__init__.py,sha256=SOKR_iSAUE1o0Ios4zdddv1gMFeD2Z4fti1GLkmVr2w,71
-zalo_sdk-0.1.3.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
-zalo_sdk-0.1.3.dist-info/METADATA,sha256=9F8xp87Vf5F32PSFNpalyWijJX8wymNMo1I2ObQ4dYY,1462
-zalo_sdk-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zalo_sdk-0.1.3.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
-zalo_sdk-0.1.3.dist-info/RECORD,,
+zalo_sdk/oa/Client.py,sha256=7YHmO8on1wyQZHVOwkorUPm3mmWZY74uu-cUnVIOC8M,5394
+zalo_sdk/oa/ZaloMessage.py,sha256=vn27DhP953EtXYfnPhvufSeqEXhVwGiuzE8wvPcU-Ik,5414
+zalo_sdk/oa/ZaloOAException.py,sha256=Jt3njqkWqPiW_mazGZoCmSicpMl9Nrtj9SZJie2BRoI,2426
+zalo_sdk/oa/__init__.py,sha256=c44yA-pbHfH-T9_-3zMeFAMLP2_mMzG0O3r18tJhnok,79
+zalo_sdk-0.1.4.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
+zalo_sdk-0.1.4.dist-info/METADATA,sha256=KSDgzFnESgzoAk7A4Xkb6HrhEUpn38hev7qHcZqW6s8,1821
+zalo_sdk-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zalo_sdk-0.1.4.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
+zalo_sdk-0.1.4.dist-info/RECORD,,
```

