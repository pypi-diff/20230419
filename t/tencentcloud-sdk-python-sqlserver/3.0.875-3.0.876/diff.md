# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.875.tar", last modified: Tue Apr 18 00:50:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.876.tar", last modified: Wed Apr 19 00:36:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.875.tar` & `tencentcloud-sdk-python-sqlserver-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   101706 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   325396 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:50:12.000000 tencentcloud-sdk-python-sqlserver-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   104555 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334850 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:36:44.000000 tencentcloud-sdk-python-sqlserver-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -873,14 +873,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDBInstancesAttribute(self, request):
+        """本接口（DescribeDBInstancesAttribute）用于查询实例附属属性
+
+        :param request: Request instance for DescribeDBInstancesAttribute.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBInstancesAttributeRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBInstancesAttributeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDBInstancesAttribute", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDBInstancesAttributeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDBSecurityGroups(self, request):
         """本接口(DescribeDBSecurityGroups)用于查询实例的安全组详情。
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBSecurityGroupsRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBSecurityGroupsResponse`
 
@@ -1402,14 +1425,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeXEvents(self, request):
+        """本接口（DescribeXEvents）用于查询扩展事件列表。
+
+        :param request: Request instance for DescribeXEvents.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeXEventsRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeXEventsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeXEvents", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeXEventsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeZones(self, request):
         """本接口 (DescribeZones) 用于查询当前可售卖的可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeZonesRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeZonesResponse`
 
@@ -2323,14 +2369,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def StartInstanceXEvent(self, request):
+        """本接口（StartInstanceXEvent）用于开启、关闭扩展事件。
+
+        :param request: Request instance for StartInstanceXEvent.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartInstanceXEventRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.StartInstanceXEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartInstanceXEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartInstanceXEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def StartMigrationCheck(self, request):
         """本接口（StartMigrationCheck）的作用是启动一个迁移前的校验任务，适用于迁移源的类型为TencentDB for SQLServer 的迁移方式
 
         :param request: Request instance for StartMigrationCheck.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartMigrationCheckRequest`
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3686,14 +3686,87 @@
             for item in params.get("InterInstanceSet"):
                 obj = InterInstance()
                 obj._deserialize(item)
                 self.InterInstanceSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDBInstancesAttributeRequest(AbstractModel):
+    """DescribeDBInstancesAttribute请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        """
+        self.InstanceId = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDBInstancesAttributeResponse(AbstractModel):
+    """DescribeDBInstancesAttribute返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param RegularBackupEnable: 定期备份状态 enable-开启，disable-关闭
+        :type RegularBackupEnable: str
+        :param RegularBackupSaveDays: 定期备份保留天数 [90 - 3650]天
+        :type RegularBackupSaveDays: int
+        :param RegularBackupStrategy: 定期备份策略 years-每年，quarters-每季度，months-每月
+        :type RegularBackupStrategy: str
+        :param RegularBackupCounts: 定期备份保留个数
+        :type RegularBackupCounts: int
+        :param RegularBackupStartTime: 定期备份开始日期，格式-YYYY-MM-DD 默认当前日期
+        :type RegularBackupStartTime: str
+        :param BlockedThreshold: 阻塞进程阈值，单位毫秒
+        :type BlockedThreshold: int
+        :param EventSaveDays: 慢SQL、阻塞、死锁扩展事件文件保留时长
+        :type EventSaveDays: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceId = None
+        self.RegularBackupEnable = None
+        self.RegularBackupSaveDays = None
+        self.RegularBackupStrategy = None
+        self.RegularBackupCounts = None
+        self.RegularBackupStartTime = None
+        self.BlockedThreshold = None
+        self.EventSaveDays = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.RegularBackupEnable = params.get("RegularBackupEnable")
+        self.RegularBackupSaveDays = params.get("RegularBackupSaveDays")
+        self.RegularBackupStrategy = params.get("RegularBackupStrategy")
+        self.RegularBackupCounts = params.get("RegularBackupCounts")
+        self.RegularBackupStartTime = params.get("RegularBackupStartTime")
+        self.BlockedThreshold = params.get("BlockedThreshold")
+        self.EventSaveDays = params.get("EventSaveDays")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDBInstancesRequest(AbstractModel):
     """DescribeDBInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5339,14 +5412,88 @@
         self.TmpSecretKey = params.get("TmpSecretKey")
         self.XCosSecurityToken = params.get("XCosSecurityToken")
         self.StartTime = params.get("StartTime")
         self.ExpiredTime = params.get("ExpiredTime")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeXEventsRequest(AbstractModel):
+    """DescribeXEvents请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param EventType: 事件类型，slow-慢SQL事件，blocked-阻塞事件，deadlock-死锁事件
+        :type EventType: str
+        :param StartTime: 扩展文件生成开始时间
+        :type StartTime: str
+        :param EndTime: 扩展文件生成结束时间
+        :type EndTime: str
+        :param Offset: 分页返回，页编号，默认值为第0页
+        :type Offset: int
+        :param Limit: 分页返回，每页返回的数目，取值为1~100，默认值为20
+        :type Limit: int
+        """
+        self.InstanceId = None
+        self.EventType = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.EventType = params.get("EventType")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeXEventsResponse(AbstractModel):
+    """DescribeXEvents返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Events: 扩展事件列表
+        :type Events: list of Events
+        :param TotalCount: 扩展事件总数量
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Events = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Events") is not None:
+            self.Events = []
+            for item in params.get("Events"):
+                obj = Events()
+                obj._deserialize(item)
+                self.Events.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeZonesRequest(AbstractModel):
     """DescribeZones请求参数结构体
 
     """
 
 
 class DescribeZonesResponse(AbstractModel):
@@ -5420,14 +5567,98 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class EventConfig(AbstractModel):
+    """设置实例扩展事件阈值
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventType: 事件类型，slow-设置慢SQL阈值，blocked-设置阻塞、死锁阈值
+        :type EventType: str
+        :param Threshold: 阈值，单位毫秒。0表示关闭，大于0表示开启
+        :type Threshold: int
+        """
+        self.EventType = None
+        self.Threshold = None
+
+
+    def _deserialize(self, params):
+        self.EventType = params.get("EventType")
+        self.Threshold = params.get("Threshold")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class Events(AbstractModel):
+    """实例扩展事件详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: ID
+        :type Id: int
+        :param FileName: 扩展事件文件名称
+        :type FileName: str
+        :param Size: 扩展事件文件大小
+        :type Size: int
+        :param EventType: 事件类型，slow-慢SQL事件，blocked-阻塞事件，deadlock-死锁事件
+        :type EventType: str
+        :param Status: 事件记录状态，1-成功，2-失败
+        :type Status: int
+        :param StartTime: 扩展文件生成开始时间
+        :type StartTime: str
+        :param EndTime: 扩展文件生成开始时间
+        :type EndTime: str
+        :param InternalAddr: 内网下载地址
+        :type InternalAddr: str
+        :param ExternalAddr: 外网下载地址
+        :type ExternalAddr: str
+        """
+        self.Id = None
+        self.FileName = None
+        self.Size = None
+        self.EventType = None
+        self.Status = None
+        self.StartTime = None
+        self.EndTime = None
+        self.InternalAddr = None
+        self.ExternalAddr = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.FileName = params.get("FileName")
+        self.Size = params.get("Size")
+        self.EventType = params.get("EventType")
+        self.Status = params.get("Status")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.InternalAddr = params.get("InternalAddr")
+        self.ExternalAddr = params.get("ExternalAddr")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FileAction(AbstractModel):
     """允许动作信息
 
     """
 
     def __init__(self):
         r"""
@@ -8962,14 +9193,64 @@
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
+class StartInstanceXEventRequest(AbstractModel):
+    """StartInstanceXEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param EventConfig: 开启、关闭扩展事件
+        :type EventConfig: list of EventConfig
+        """
+        self.InstanceId = None
+        self.EventConfig = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        if params.get("EventConfig") is not None:
+            self.EventConfig = []
+            for item in params.get("EventConfig"):
+                obj = EventConfig()
+                obj._deserialize(item)
+                self.EventConfig.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StartInstanceXEventResponse(AbstractModel):
+    """StartInstanceXEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class StartMigrationCheckRequest(AbstractModel):
     """StartMigrationCheck请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.876/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.876/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.875/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.876/setup.py`

 * *Files identical despite different names*

