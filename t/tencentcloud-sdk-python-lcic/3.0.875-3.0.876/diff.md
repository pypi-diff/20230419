# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.875.tar", last modified: Tue Apr 18 00:45:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.876.tar", last modified: Wed Apr 19 00:31:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.875.tar` & `tencentcloud-sdk-python-lcic-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127771 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    43349 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-18 00:45:07.000000 tencentcloud-sdk-python-lcic-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:45:08.000000 tencentcloud-sdk-python-lcic-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135371 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    46709 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/README.rst` & `tencentcloud-sdk-python-lcic-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1270,14 +1270,59 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteSupervisorRequest(AbstractModel):
+    """DeleteSupervisor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 应用ID
+        :type SdkAppId: int
+        :param Users: 用户ID列表
+        :type Users: list of str
+        """
+        self.SdkAppId = None
+        self.Users = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.Users = params.get("Users")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteSupervisorResponse(AbstractModel):
+    """DeleteSupervisor返回参数结构体
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
 class DescribeAnswerListRequest(AbstractModel):
     """DescribeAnswerList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1664,14 +1709,93 @@
                 obj = DocumentInfo()
                 obj._deserialize(item)
                 self.Documents.append(obj)
         self.Total = params.get("Total")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDocumentsRequest(AbstractModel):
+    """DescribeDocuments请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SchoolId: 学校id
+        :type SchoolId: int
+        :param Page: 分页查询当前页数，从1开始递增
+        :type Page: int
+        :param Limit: 每页数据量，最大1000
+        :type Limit: int
+        :param Permission: 课件权限。[0]：获取owner的私有课件；[1]：获取owner的公开课件; [0,1]：则获取owner的私有课件和公开课件；[2]：获取owner的私有课件和所有人(包括owner)的公开课件
+        :type Permission: list of int non-negative
+        :param Owner: 课件所有者的user_id，不填默认获取school_id下所有课件
+        :type Owner: str
+        :param Keyword: 课件名称搜索词
+        :type Keyword: str
+        :param DocumentId: 课件id列表，从列表中查询，忽略错误的id
+        :type DocumentId: list of str
+        """
+        self.SchoolId = None
+        self.Page = None
+        self.Limit = None
+        self.Permission = None
+        self.Owner = None
+        self.Keyword = None
+        self.DocumentId = None
+
+
+    def _deserialize(self, params):
+        self.SchoolId = params.get("SchoolId")
+        self.Page = params.get("Page")
+        self.Limit = params.get("Limit")
+        self.Permission = params.get("Permission")
+        self.Owner = params.get("Owner")
+        self.Keyword = params.get("Keyword")
+        self.DocumentId = params.get("DocumentId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDocumentsResponse(AbstractModel):
+    """DescribeDocuments返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 符合查询条件文档总数
+        :type Total: int
+        :param Documents: 文档信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Documents: list of DocumentInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Documents = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Documents") is not None:
+            self.Documents = []
+            for item in params.get("Documents"):
+                obj = DocumentInfo()
+                obj._deserialize(item)
+                self.Documents.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeGroupListRequest(AbstractModel):
     """DescribeGroupList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2369,14 +2493,26 @@
         :type DocumentType: str
         :param DocumentSize: 文档大小，单位：字节
 注意：此字段可能返回 null，表示取不到有效值。
         :type DocumentSize: int
         :param UpdateTime: 更新的UNIX时间戳
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: int
+        :param Pages: 课件页数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Pages: int
+        :param Width: 宽，仅在静态转码的课件有效
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Width: int
+        :param Height: 高，仅在静态转码的课件有效
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Height: int
+        :param Cover: 封面，仅转码的课件会生成封面
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Cover: str
         """
         self.DocumentId = None
         self.DocumentUrl = None
         self.DocumentName = None
         self.Owner = None
         self.SdkAppId = None
         self.Permission = None
@@ -2384,14 +2520,18 @@
         self.TranscodeType = None
         self.TranscodeProgress = None
         self.TranscodeState = None
         self.TranscodeInfo = None
         self.DocumentType = None
         self.DocumentSize = None
         self.UpdateTime = None
+        self.Pages = None
+        self.Width = None
+        self.Height = None
+        self.Cover = None
 
 
     def _deserialize(self, params):
         self.DocumentId = params.get("DocumentId")
         self.DocumentUrl = params.get("DocumentUrl")
         self.DocumentName = params.get("DocumentName")
         self.Owner = params.get("Owner")
@@ -2401,23 +2541,68 @@
         self.TranscodeType = params.get("TranscodeType")
         self.TranscodeProgress = params.get("TranscodeProgress")
         self.TranscodeState = params.get("TranscodeState")
         self.TranscodeInfo = params.get("TranscodeInfo")
         self.DocumentType = params.get("DocumentType")
         self.DocumentSize = params.get("DocumentSize")
         self.UpdateTime = params.get("UpdateTime")
+        self.Pages = params.get("Pages")
+        self.Width = params.get("Width")
+        self.Height = params.get("Height")
+        self.Cover = params.get("Cover")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class EndRoomRequest(AbstractModel):
+    """EndRoom请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RoomId: 房间ID。
+        :type RoomId: int
+        """
+        self.RoomId = None
+
+
+    def _deserialize(self, params):
+        self.RoomId = params.get("RoomId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EndRoomResponse(AbstractModel):
+    """EndRoom返回参数结构体
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
 class EventDataInfo(AbstractModel):
     """房间事件对应的信息。
 
     """
 
     def __init__(self):
         r"""
@@ -2972,14 +3157,24 @@
         :param Device: 用户设备平台信息。0:unknown  1:windows  2:mac  3:android  4:ios  5:web   6:h5   7:miniprogram （小程序）
         :type Device: int
         :param PerMemberMicCount: 每个成员上麦次数。
         :type PerMemberMicCount: int
         :param PerMemberMessageCount: 每个成员发送消息数量。
 
         :type PerMemberMessageCount: int
+        :param Role: 用户角色。0代表学生；1代表老师； 2助教；3巡课。
+        :type Role: int
+        :param GroupId: 上课班号
+        :type GroupId: str
+        :param SubGroupId: 子上课班号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubGroupId: list of str
+        :param Stage: 用户的上台状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Stage: int
         """
         self.UserId = None
         self.UserName = None
         self.PresentTime = None
         self.Camera = None
         self.Mic = None
         self.Silence = None
@@ -2989,14 +3184,18 @@
         self.LastQuitTimestamp = None
         self.Rewords = None
         self.IPAddress = None
         self.Location = None
         self.Device = None
         self.PerMemberMicCount = None
         self.PerMemberMessageCount = None
+        self.Role = None
+        self.GroupId = None
+        self.SubGroupId = None
+        self.Stage = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
         self.UserName = params.get("UserName")
         self.PresentTime = params.get("PresentTime")
         self.Camera = params.get("Camera")
@@ -3008,14 +3207,18 @@
         self.LastQuitTimestamp = params.get("LastQuitTimestamp")
         self.Rewords = params.get("Rewords")
         self.IPAddress = params.get("IPAddress")
         self.Location = params.get("Location")
         self.Device = params.get("Device")
         self.PerMemberMicCount = params.get("PerMemberMicCount")
         self.PerMemberMessageCount = params.get("PerMemberMessageCount")
+        self.Role = params.get("Role")
+        self.GroupId = params.get("GroupId")
+        self.SubGroupId = params.get("SubGroupId")
+        self.Stage = params.get("Stage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3769,14 +3972,55 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class StartRoomRequest(AbstractModel):
+    """StartRoom请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RoomId: 房间ID。
+        :type RoomId: int
+        """
+        self.RoomId = None
+
+
+    def _deserialize(self, params):
+        self.RoomId = params.get("RoomId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StartRoomResponse(AbstractModel):
+    """StartRoom返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteSupervisor(self, request):
+        """删除巡课
+
+        :param request: Request instance for DeleteSupervisor.
+        :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteSupervisorRequest`
+        :rtype: :class:`tencentcloud.lcic.v20220817.models.DeleteSupervisorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteSupervisor", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteSupervisorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeAnswerList(self, request):
         """获取房间答题详情
 
         :param request: Request instance for DescribeAnswerList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeAnswerListRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.DescribeAnswerListResponse`
 
@@ -574,14 +597,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDocuments(self, request):
+        """批量获取文档信息
+
+        :param request: Request instance for DescribeDocuments.
+        :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsRequest`
+        :rtype: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDocuments", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDocumentsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDocumentsByRoom(self, request):
         """此接口获取指定房间下课件列表
 
         :param request: Request instance for DescribeDocumentsByRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsByRoomRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsByRoomResponse`
 
@@ -804,14 +850,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def EndRoom(self, request):
+        """结束房间的直播
+
+        :param request: Request instance for EndRoom.
+        :type request: :class:`tencentcloud.lcic.v20220817.models.EndRoomRequest`
+        :rtype: :class:`tencentcloud.lcic.v20220817.models.EndRoomResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EndRoom", params, headers=headers)
+            response = json.loads(body)
+            model = models.EndRoomResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GetRoomEvent(self, request):
         """获取房间事件,仅在课堂结束1小时内有效。
 
         :param request: Request instance for GetRoomEvent.
         :type request: :class:`tencentcloud.lcic.v20220817.models.GetRoomEventRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.GetRoomEventResponse`
 
@@ -1101,14 +1170,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def StartRoom(self, request):
+        """开始房间的直播
+
+        :param request: Request instance for StartRoom.
+        :type request: :class:`tencentcloud.lcic.v20220817.models.StartRoomRequest`
+        :rtype: :class:`tencentcloud.lcic.v20220817.models.StartRoomResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartRoom", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartRoomResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UnbindDocumentFromRoom(self, request):
         """文档从房间解绑
 
         :param request: Request instance for UnbindDocumentFromRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.UnbindDocumentFromRoomRequest`
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.876/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.875/setup.py` & `tencentcloud-sdk-python-lcic-3.0.876/setup.py`

 * *Files identical despite different names*

