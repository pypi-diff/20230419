# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.875.tar", last modified: Tue Apr 18 00:28:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.876.tar", last modified: Wed Apr 19 00:21:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.875.tar` & `tencentcloud-sdk-python-ckafka-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3206 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   457296 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    67457 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:28:23.000000 tencentcloud-sdk-python-ckafka-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   458707 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    68390 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-19 00:21:39.000000 tencentcloud-sdk-python-ckafka-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:21:40.000000 tencentcloud-sdk-python-ckafka-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.875'
+__version__ = '3.0.876'
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10705,14 +10705,65 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RenewCkafkaInstanceRequest(AbstractModel):
+    """RenewCkafkaInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例id
+        :type InstanceId: str
+        :param TimeSpan: 续费时长, 默认为1, 单位是月
+        :type TimeSpan: int
+        """
+        self.InstanceId = None
+        self.TimeSpan = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.TimeSpan = params.get("TimeSpan")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RenewCkafkaInstanceResponse(AbstractModel):
+    """RenewCkafkaInstance接口出参bigDealIds
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BigDealId: 订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BigDealId: str
+        :param DealName: 子订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealName: str
+        """
+        self.BigDealId = None
+        self.DealName = None
+
+
+    def _deserialize(self, params):
+        self.BigDealId = params.get("BigDealId")
+        self.DealName = params.get("DealName")
+
+
 class ReplaceParam(AbstractModel):
     """数据处理——Value处理参数——替换参数
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.876/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1725,14 +1725,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RenewCkafkaInstance(self, request):
+        """续费Ckafka实例, 目前只支持国内站包年包月实例续费
+
+        :param request: Request instance for RenewCkafkaInstance.
+        :type request: :class:`tencentcloud.ckafka.v20190819.models.RenewCkafkaInstanceRequest`
+        :rtype: :class:`tencentcloud.ckafka.v20190819.models.RenewCkafkaInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RenewCkafkaInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.RenewCkafkaInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SendMessage(self, request):
         """通过HTTP接入层发送消息
 
         :param request: Request instance for SendMessage.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.SendMessageRequest`
         :rtype: :class:`tencentcloud.ckafka.v20190819.models.SendMessageResponse`
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.876/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.875/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.876/setup.py`

 * *Files identical despite different names*

