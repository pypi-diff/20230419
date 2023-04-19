# Comparing `tmp/tencentcloud-sdk-python-mgobe-3.0.876.tar.gz` & `tmp/tencentcloud-sdk-python-mgobe-3.0.877.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.876.tar", last modified: Wed Apr 19 00:31:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.877.tar", last modified: Wed Apr 19 09:21:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mgobe-3.0.876.tar` & `tencentcloud-sdk-python-mgobe-3.0.877.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)    34005 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/
--rw-r--r--   0 root         (0) root         (0)     8244 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)    34111 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20430 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:31:55.000000 tencentcloud-sdk-python-mgobe-3.0.876/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34005 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/
+-rw-r--r--   0 root         (0) root         (0)     8244 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34111 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20430 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:21:39.000000 tencentcloud-sdk-python-mgobe-3.0.877/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.876
+Version: 3.0.877
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/README.rst` & `tencentcloud-sdk-python-mgobe-3.0.877/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20190929/models.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20190929/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/mgobe/v20201014/models.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/mgobe/v20201014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mgobe-3.0.877/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.876'
+__version__ = '3.0.877'
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.877/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.876
+Version: 3.0.877
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.876/setup.py` & `tencentcloud-sdk-python-mgobe-3.0.877/setup.py`

 * *Files identical despite different names*

