# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.876.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.877.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.876.tar", last modified: Wed Apr 19 00:24:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.877.tar", last modified: Wed Apr 19 09:12:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.876.tar` & `tencentcloud-sdk-python-domain-3.0.877.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)    25103 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75209 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:24:44.000000 tencentcloud-sdk-python-domain-3.0.876/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)    25103 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75209 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:12:54.000000 tencentcloud-sdk-python-domain-3.0.877/setup.cfg
```

### Comparing `tencentcloud-sdk-python-domain-3.0.876/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.877/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.876
+Version: 3.0.877
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.876/README.rst` & `tencentcloud-sdk-python-domain-3.0.877/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.876/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.877/tencentcloud/domain/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.876/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.877/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.876/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.877/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.876
+Version: 3.0.877
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.876/setup.py` & `tencentcloud-sdk-python-domain-3.0.877/setup.py`

 * *Files identical despite different names*

