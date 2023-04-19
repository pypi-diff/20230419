# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.875.tar", last modified: Tue Apr 18 01:01:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.876.tar", last modified: Wed Apr 19 00:42:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.875.tar` & `tencentcloud-sdk-python-tsf-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49509 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   190807 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   789423 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 01:01:13.000000 tencentcloud-sdk-python-tsf-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49509 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   192711 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   795624 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:42:10.000000 tencentcloud-sdk-python-tsf-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/README.rst` & `tencentcloud-sdk-python-tsf-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,14 +413,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateConfigWithDetailResp(self, request):
+        """创建配置项，返回详细信息
+
+        :param request: Request instance for CreateConfigWithDetailResp.
+        :type request: :class:`tencentcloud.tsf.v20180326.models.CreateConfigWithDetailRespRequest`
+        :rtype: :class:`tencentcloud.tsf.v20180326.models.CreateConfigWithDetailRespResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateConfigWithDetailResp", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateConfigWithDetailRespResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateContainGroup(self, request):
         """（已废弃，请使用 CreateGroup 和 DeployContainerGroup 创建和部署容器部署组）创建容器部署组
 
         :param request: Request instance for CreateContainGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateContainGroupRequest`
         :rtype: :class:`tencentcloud.tsf.v20180326.models.CreateContainGroupResponse`
 
@@ -457,14 +480,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateFileConfigWithDetailResp(self, request):
+        """创建文件配置项，返回详细信息
+
+        :param request: Request instance for CreateFileConfigWithDetailResp.
+        :type request: :class:`tencentcloud.tsf.v20180326.models.CreateFileConfigWithDetailRespRequest`
+        :rtype: :class:`tencentcloud.tsf.v20180326.models.CreateFileConfigWithDetailRespResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateFileConfigWithDetailResp", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateFileConfigWithDetailRespResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateGatewayApi(self, request):
         """批量导入API至api分组(也支持新建API到分组)
 
         :param request: Request instance for CreateGatewayApi.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateGatewayApiRequest`
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/tsf/v20180326/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3739,14 +3739,90 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = ConfigTemplate()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateConfigWithDetailRespRequest(AbstractModel):
+    """CreateConfigWithDetailResp请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ConfigName: 配置项名称
+        :type ConfigName: str
+        :param ConfigVersion: 配置项版本
+        :type ConfigVersion: str
+        :param ConfigValue: 配置项值
+        :type ConfigValue: str
+        :param ApplicationId: 应用ID
+        :type ApplicationId: str
+        :param ConfigVersionDesc: 配置项版本描述
+        :type ConfigVersionDesc: str
+        :param ConfigType: 配置项值类型
+        :type ConfigType: str
+        :param EncodeWithBase64: Base64编码的配置项
+        :type EncodeWithBase64: bool
+        :param ProgramIdList: 无
+        :type ProgramIdList: list of str
+        """
+        self.ConfigName = None
+        self.ConfigVersion = None
+        self.ConfigValue = None
+        self.ApplicationId = None
+        self.ConfigVersionDesc = None
+        self.ConfigType = None
+        self.EncodeWithBase64 = None
+        self.ProgramIdList = None
+
+
+    def _deserialize(self, params):
+        self.ConfigName = params.get("ConfigName")
+        self.ConfigVersion = params.get("ConfigVersion")
+        self.ConfigValue = params.get("ConfigValue")
+        self.ApplicationId = params.get("ApplicationId")
+        self.ConfigVersionDesc = params.get("ConfigVersionDesc")
+        self.ConfigType = params.get("ConfigType")
+        self.EncodeWithBase64 = params.get("EncodeWithBase64")
+        self.ProgramIdList = params.get("ProgramIdList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateConfigWithDetailRespResponse(AbstractModel):
+    """CreateConfigWithDetailResp返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 配置项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.tsf.v20180326.models.Config`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self.Result = Config()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class CreateContainGroupRequest(AbstractModel):
     """CreateContainGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3967,14 +4043,102 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class CreateFileConfigWithDetailRespRequest(AbstractModel):
+    """CreateFileConfigWithDetailResp请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ConfigName: 配置项名称
+        :type ConfigName: str
+        :param ConfigVersion: 配置项版本
+        :type ConfigVersion: str
+        :param ConfigFileName: 配置项文件名
+        :type ConfigFileName: str
+        :param ConfigFileValue: 配置项文件内容（原始内容编码需要 utf-8 格式，如果 ConfigFileCode 为 gbk，后台会进行转换）
+        :type ConfigFileValue: str
+        :param ApplicationId: 配置项关联应用ID
+        :type ApplicationId: str
+        :param ConfigFilePath: 发布路径
+        :type ConfigFilePath: str
+        :param ConfigVersionDesc: 配置项版本描述
+        :type ConfigVersionDesc: str
+        :param ConfigFileCode: 配置项文件编码，utf-8 或 gbk。注：如果选择 gbk，需要新版本 tsf-consul-template （公有云虚拟机需要使用 1.32 tsf-agent，容器需要从文档中获取最新的 tsf-consul-template-docker.tar.gz）的支持
+        :type ConfigFileCode: str
+        :param ConfigPostCmd: 后置命令
+        :type ConfigPostCmd: str
+        :param EncodeWithBase64: Base64编码的配置项
+        :type EncodeWithBase64: bool
+        :param ProgramIdList: 无
+        :type ProgramIdList: list of str
+        """
+        self.ConfigName = None
+        self.ConfigVersion = None
+        self.ConfigFileName = None
+        self.ConfigFileValue = None
+        self.ApplicationId = None
+        self.ConfigFilePath = None
+        self.ConfigVersionDesc = None
+        self.ConfigFileCode = None
+        self.ConfigPostCmd = None
+        self.EncodeWithBase64 = None
+        self.ProgramIdList = None
+
+
+    def _deserialize(self, params):
+        self.ConfigName = params.get("ConfigName")
+        self.ConfigVersion = params.get("ConfigVersion")
+        self.ConfigFileName = params.get("ConfigFileName")
+        self.ConfigFileValue = params.get("ConfigFileValue")
+        self.ApplicationId = params.get("ApplicationId")
+        self.ConfigFilePath = params.get("ConfigFilePath")
+        self.ConfigVersionDesc = params.get("ConfigVersionDesc")
+        self.ConfigFileCode = params.get("ConfigFileCode")
+        self.ConfigPostCmd = params.get("ConfigPostCmd")
+        self.EncodeWithBase64 = params.get("EncodeWithBase64")
+        self.ProgramIdList = params.get("ProgramIdList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateFileConfigWithDetailRespResponse(AbstractModel):
+    """CreateFileConfigWithDetailResp返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 文件配置项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.tsf.v20180326.models.FileConfig`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self.Result = FileConfig()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class CreateGatewayApiRequest(AbstractModel):
     """CreateGatewayApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.876/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.875/setup.py` & `tencentcloud-sdk-python-tsf-3.0.876/setup.py`

 * *Files identical despite different names*

