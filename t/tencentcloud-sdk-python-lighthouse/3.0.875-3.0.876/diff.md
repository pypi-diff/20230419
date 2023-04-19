# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.875.tar", last modified: Tue Apr 18 00:45:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.876.tar", last modified: Wed Apr 19 00:31:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.875.tar` & `tencentcloud-sdk-python-lighthouse-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    23217 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88751 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229680 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:45:15.000000 tencentcloud-sdk-python-lighthouse-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    23217 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    88751 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230506 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-19 00:31:08.000000 tencentcloud-sdk-python-lighthouse-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:31:09.000000 tencentcloud-sdk-python-lighthouse-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,16 +487,26 @@
         :type InternetMaxBandwidthOut: int
         :param InternetChargeType: 网络计费类型。
         :type InternetChargeType: str
         :param BundleSalesState: 套餐售卖状态,取值:‘AVAILABLE’(可用) , ‘SOLD_OUT’(售罄)
         :type BundleSalesState: str
         :param BundleType: 套餐类型。
 取值范围：
-<li> GENERAL_BUNDLE：通用型</li><li> STORAGE_BUNDLE：存储型 </li>
+<li>STARTER_BUNDLE：入门型</li>
+<li>GENERAL_BUNDLE：通用型</li>
+<li>ENTERPRISE_BUNDLE：企业型</li>
+<li>STORAGE_BUNDLE：存储型</li>
+<li>EXCLUSIVE_BUNDLE：专属型</li>
+<li>HK_EXCLUSIVE_BUNDLE：香港专属型 </li>
+<li>CAREFREE_BUNDLE：无忧型</li>
+<li>BEFAST_BUNDLE：蜂驰型 </li>
         :type BundleType: str
+        :param BundleTypeDescription: 套餐类型描述信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BundleTypeDescription: str
         :param BundleDisplayLabel: 套餐展示标签.
 取值范围:
 "ACTIVITY": 活动套餐,
 "NORMAL": 普通套餐
 "CAREFREE": 无忧套餐
         :type BundleDisplayLabel: str
         """
@@ -509,14 +519,15 @@
         self.SupportWindowsPlatform = None
         self.Price = None
         self.CPU = None
         self.InternetMaxBandwidthOut = None
         self.InternetChargeType = None
         self.BundleSalesState = None
         self.BundleType = None
+        self.BundleTypeDescription = None
         self.BundleDisplayLabel = None
 
 
     def _deserialize(self, params):
         self.BundleId = params.get("BundleId")
         self.Memory = params.get("Memory")
         self.SystemDiskType = params.get("SystemDiskType")
@@ -528,14 +539,15 @@
             self.Price = Price()
             self.Price._deserialize(params.get("Price"))
         self.CPU = params.get("CPU")
         self.InternetMaxBandwidthOut = params.get("InternetMaxBandwidthOut")
         self.InternetChargeType = params.get("InternetChargeType")
         self.BundleSalesState = params.get("BundleSalesState")
         self.BundleType = params.get("BundleType")
+        self.BundleTypeDescription = params.get("BundleTypeDescription")
         self.BundleDisplayLabel = params.get("BundleDisplayLabel")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2507,14 +2519,23 @@
 必选：否
 <li>zone</li>按照【可用区】进行过滤。
 类型：String
 必选：否
 <li>instance-state</li>按照【实例状态】进行过滤。
 类型：String
 必选：否
+<li>tag-key</li>按照【标签键】进行过滤。
+类型：String
+必选：否
+<li>tag-value</li>按照【标签值】进行过滤。
+类型：String
+必选：否
+<li> tag:tag-key</li>按照【标签键值对】进行过滤。 tag-key使用具体的标签键进行替换。
+类型：String
+必选：否
 每次请求的 Filters 的上限为 10，Filter.Values 的上限为 100。参数不支持同时指定 InstanceIds 和 Filters。
         :type Filters: list of Filter
         :param Offset: 偏移量，默认为 0。关于`Offset`的更进一步介绍请参考 API [简介](https://cloud.tencent.com/document/product/1207/47578)中的相关小节。
         :type Offset: int
         :param Limit: 返回数量，默认为 20，最大值为 100。关于`Limit`的更进一步介绍请参考 API [简介](https://cloud.tencent.com/document/product/1207/47578)中的相关小节。
         :type Limit: int
         """
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.876/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.876/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.875/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.876/setup.py`

 * *Files identical despite different names*

