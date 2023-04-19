# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.875.tar", last modified: Tue Apr 18 01:00:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.876.tar", last modified: Wed Apr 19 00:41:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.875.tar` & `tencentcloud-sdk-python-tke-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   176385 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19361 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   638897 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 01:00:03.000000 tencentcloud-sdk-python-tke-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   177308 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19361 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   640464 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:41:06.000000 tencentcloud-sdk-python-tke-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.875/README.rst` & `tencentcloud-sdk-python-tke-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4162,14 +4162,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def UpdateClusterKubeconfig(self, request):
+        """对集群的Kubeconfig信息进行更新
+
+        :param request: Request instance for UpdateClusterKubeconfig.
+        :type request: :class:`tencentcloud.tke.v20180525.models.UpdateClusterKubeconfigRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.UpdateClusterKubeconfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateClusterKubeconfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateClusterKubeconfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def UpdateClusterVersion(self, request):
         """升级集群 Master 组件到指定版本
 
         :param request: Request instance for UpdateClusterVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateClusterVersionRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.UpdateClusterVersionResponse`
```

### Comparing `tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.875/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.876/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17412,14 +17412,64 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpdateClusterKubeconfigRequest(AbstractModel):
+    """UpdateClusterKubeconfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param SubAccounts: 子账户Uin列表，传空默认为调用此接口的SubUin
+        :type SubAccounts: list of str
+        """
+        self.ClusterId = None
+        self.SubAccounts = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.SubAccounts = params.get("SubAccounts")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateClusterKubeconfigResponse(AbstractModel):
+    """UpdateClusterKubeconfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UpdatedSubAccounts: 已更新的子账户Uin列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdatedSubAccounts: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.UpdatedSubAccounts = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.UpdatedSubAccounts = params.get("UpdatedSubAccounts")
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateClusterVersionRequest(AbstractModel):
     """UpdateClusterVersion请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tke-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.875/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.876/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.875/setup.py` & `tencentcloud-sdk-python-tke-3.0.876/setup.py`

 * *Files identical despite different names*

