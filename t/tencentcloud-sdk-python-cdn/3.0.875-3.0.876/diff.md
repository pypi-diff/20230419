# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.875.tar", last modified: Tue Apr 18 00:26:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.876.tar", last modified: Wed Apr 19 00:20:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.875.tar` & `tencentcloud-sdk-python-cdn-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21844 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   568035 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:26:59.000000 tencentcloud-sdk-python-cdn-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21844 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   568258 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:20:07.000000 tencentcloud-sdk-python-cdn-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/README.rst` & `tencentcloud-sdk-python-cdn-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.876/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7851,28 +7851,33 @@
         :type LogPath: str
         :param Area: 日志包对应加速区域
 mainland：境内
 overseas：境外
         :type Area: str
         :param LogName: 日志包文件名
         :type LogName: str
+        :param FileSize: 文件大小，单位: Byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileSize: int
         """
         self.StartTime = None
         self.EndTime = None
         self.LogPath = None
         self.Area = None
         self.LogName = None
+        self.FileSize = None
 
 
     def _deserialize(self, params):
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.LogPath = params.get("LogPath")
         self.Area = params.get("Area")
         self.LogName = params.get("LogName")
+        self.FileSize = params.get("FileSize")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.876/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.875/setup.py` & `tencentcloud-sdk-python-cdn-3.0.876/setup.py`

 * *Files identical despite different names*

