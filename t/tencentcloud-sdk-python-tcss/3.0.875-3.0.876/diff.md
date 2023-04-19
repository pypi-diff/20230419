# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.875.tar", last modified: Tue Apr 18 00:57:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.876.tar", last modified: Wed Apr 19 00:39:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.875.tar` & `tencentcloud-sdk-python-tcss-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1014997 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:57:49.000000 tencentcloud-sdk-python-tcss-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1015029 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:39:07.000000 tencentcloud-sdk-python-tcss-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/README.rst` & `tencentcloud-sdk-python-tcss-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.876/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16396,15 +16396,16 @@
 
     def __init__(self):
         r"""
         :param Limit: 需要返回的数量，默认为10，最大值为100
         :type Limit: int
         :param Offset: 偏移量，默认为0。
         :type Offset: int
-        :param Filters: 过滤参数,"Filters":[{"Name":"Status","Values":["2"]}]
+        :param Filters: 过滤参数
+InnerNetAlarmShow- int - 是否必填：1 - 内网告警展示 0 - 不展示
         :type Filters: list of RunTimeFilters
         :param Order: 升序降序,asc desc
         :type Order: str
         :param By: 排序字段
         :type By: str
         """
         self.Limit = None
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.876/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.875/setup.py` & `tencentcloud-sdk-python-tcss-3.0.876/setup.py`

 * *Files identical despite different names*

