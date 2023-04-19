# Comparing `tmp/tencentcloud-sdk-python-ssm-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-ssm-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.875.tar", last modified: Tue Apr 18 00:53:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.876.tar", last modified: Wed Apr 19 00:37:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssm-3.0.875.tar` & `tencentcloud-sdk-python-ssm-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/
--rw-r--r--   0 root         (0) root         (0)    24513 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/ssm_client.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62817 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:53:35.000000 tencentcloud-sdk-python-ssm-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/
+-rw-r--r--   0 root         (0) root         (0)    24513 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/ssm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62817 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:37:13.000000 tencentcloud-sdk-python-ssm-3.0.876/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/README.rst` & `tencentcloud-sdk-python-ssm-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/ssm_client.py` & `tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/ssm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/errorcodes.py` & `tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/ssm/v20190923/models.py` & `tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/ssm/v20190923/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssm-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.876/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.875/setup.py` & `tencentcloud-sdk-python-ssm-3.0.876/setup.py`

 * *Files identical despite different names*
