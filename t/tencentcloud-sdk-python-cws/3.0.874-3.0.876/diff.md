# Comparing `tmp/tencentcloud-sdk-python-cws-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-cws-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cws-3.0.874.tar", last modified: Mon Apr 17 00:27:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cws-3.0.876.tar", last modified: Wed Apr 19 00:23:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cws-3.0.874.tar` & `tencentcloud-sdk-python-cws-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/
--rw-r--r--   0 root         (0) root         (0)     1228 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55263 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/models.py
--rw-r--r--   0 root         (0) root         (0)    18517 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/cws_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:27:02.000000 tencentcloud-sdk-python-cws-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55263 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/models.py
+-rw-r--r--   0 root         (0) root         (0)    18517 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/cws_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:23:27.000000 tencentcloud-sdk-python-cws-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cws-3.0.874/README.rst` & `tencentcloud-sdk-python-cws-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cws-3.0.876/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.874'
+__version__ = '3.0.876'
```

### Comparing `tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/errorcodes.py` & `tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/models.py` & `tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.874/tencentcloud/cws/v20180312/cws_client.py` & `tencentcloud-sdk-python-cws-3.0.876/tencentcloud/cws/v20180312/cws_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cws-3.0.874/tencentcloud_sdk_python_cws.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cws-3.0.876/tencentcloud_sdk_python_cws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cws
-Version: 3.0.874
+Version: 3.0.876
 Summary: Tencent Cloud Cws SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cws-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-cws-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cws
-Version: 3.0.874
+Version: 3.0.876
 Summary: Tencent Cloud Cws SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cws-3.0.874/setup.py` & `tencentcloud-sdk-python-cws-3.0.876/setup.py`

 * *Files identical despite different names*

