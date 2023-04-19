# Comparing `tmp/tencentcloud-sdk-python-live-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.875.tar", last modified: Tue Apr 18 00:45:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.876.tar", last modified: Wed Apr 19 00:31:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.875.tar` & `tencentcloud-sdk-python-live-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   136457 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   421069 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:45:22.000000 tencentcloud-sdk-python-live-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   136457 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   421867 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:31:16.000000 tencentcloud-sdk-python-live-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.875/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.876/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.875/README.rst` & `tencentcloud-sdk-python-live-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.875/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.876/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,40 +521,45 @@
         :param PornCensorshipNotifyUrl: 鉴黄回调 URL。
         :type PornCensorshipNotifyUrl: str
         :param CallbackKey: 回调的鉴权 key。
         :type CallbackKey: str
         :param PushExceptionNotifyUrl: 推流异常回调 URL。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PushExceptionNotifyUrl: str
+        :param AudioAuditNotifyUrl: 音频审核回调 URL。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AudioAuditNotifyUrl: str
         """
         self.TemplateId = None
         self.TemplateName = None
         self.Description = None
         self.StreamBeginNotifyUrl = None
         self.StreamMixNotifyUrl = None
         self.StreamEndNotifyUrl = None
         self.RecordNotifyUrl = None
         self.SnapshotNotifyUrl = None
         self.PornCensorshipNotifyUrl = None
         self.CallbackKey = None
         self.PushExceptionNotifyUrl = None
+        self.AudioAuditNotifyUrl = None
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.TemplateName = params.get("TemplateName")
         self.Description = params.get("Description")
         self.StreamBeginNotifyUrl = params.get("StreamBeginNotifyUrl")
         self.StreamMixNotifyUrl = params.get("StreamMixNotifyUrl")
         self.StreamEndNotifyUrl = params.get("StreamEndNotifyUrl")
         self.RecordNotifyUrl = params.get("RecordNotifyUrl")
         self.SnapshotNotifyUrl = params.get("SnapshotNotifyUrl")
         self.PornCensorshipNotifyUrl = params.get("PornCensorshipNotifyUrl")
         self.CallbackKey = params.get("CallbackKey")
         self.PushExceptionNotifyUrl = params.get("PushExceptionNotifyUrl")
+        self.AudioAuditNotifyUrl = params.get("AudioAuditNotifyUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8600,34 +8605,47 @@
 0: 未使用。
 1: 使用中。
 2: 已过期。
 3: 已冻结。
 4: 已耗尽。
 5: 已退款
         :type Status: int
+        :param WillRenew: 是否自动续购。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WillRenew: int
+        :param RenewalResult: 续购状态。
+1 ：续购成功。
+0 ：尚未续购。
+<0  : 续购失败。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RenewalResult: int
         """
         self.Id = None
         self.Total = None
         self.Used = None
         self.Left = None
         self.BuyTime = None
         self.ExpireTime = None
         self.Type = None
         self.Status = None
+        self.WillRenew = None
+        self.RenewalResult = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Total = params.get("Total")
         self.Used = params.get("Used")
         self.Left = params.get("Left")
         self.BuyTime = params.get("BuyTime")
         self.ExpireTime = params.get("ExpireTime")
         self.Type = params.get("Type")
         self.Status = params.get("Status")
+        self.WillRenew = params.get("WillRenew")
+        self.RenewalResult = params.get("RenewalResult")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.875/setup.py` & `tencentcloud-sdk-python-live-3.0.876/setup.py`

 * *Files identical despite different names*

