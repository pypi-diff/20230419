# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.875.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.875.tar", last modified: Tue Apr 18 00:48:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.876.tar", last modified: Wed Apr 19 00:34:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.875.tar` & `tencentcloud-sdk-python-postgres-3.0.876.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    81533 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   268844 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:48:23.000000 tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    81533 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270908 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 00:34:46.000000 tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/README.rst` & `tencentcloud-sdk-python-postgres-3.0.876/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,54 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BackupDownloadRestriction(AbstractModel):
+    """备份下载限制信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RestrictionType: 备份文件下载限制类型，NONE 无限制，内外网都可以下载；INTRANET 只允许内网下载；CUSTOMIZE 自定义限制下载的vpc或ip。
+        :type RestrictionType: str
+        :param VpcRestrictionEffect: vpc限制效力，ALLOW 允许；DENY 拒绝。
+        :type VpcRestrictionEffect: str
+        :param VpcIdSet: 允许或拒绝下载备份文件的vpcId列表。
+        :type VpcIdSet: list of str
+        :param IpRestrictionEffect: ip限制效力，ALLOW 允许；DENY 拒绝。
+        :type IpRestrictionEffect: str
+        :param IpSet: 允许或拒绝下载备份文件的ip列表。
+        :type IpSet: list of str
+        """
+        self.RestrictionType = None
+        self.VpcRestrictionEffect = None
+        self.VpcIdSet = None
+        self.IpRestrictionEffect = None
+        self.IpSet = None
+
+
+    def _deserialize(self, params):
+        self.RestrictionType = params.get("RestrictionType")
+        self.VpcRestrictionEffect = params.get("VpcRestrictionEffect")
+        self.VpcIdSet = params.get("VpcIdSet")
+        self.IpRestrictionEffect = params.get("IpRestrictionEffect")
+        self.IpSet = params.get("IpSet")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BackupPlan(AbstractModel):
     """备份计划
 
     """
 
     def __init__(self):
         r"""
@@ -2281,26 +2321,32 @@
         :type DBInstanceId: str
         :param BackupType: 备份类型，目前支持：LogBackup，BaseBackup。
         :type BackupType: str
         :param BackupId: 备份的唯一ID。
         :type BackupId: str
         :param URLExpireTime: 链接的有效时间，默认为12小时。
         :type URLExpireTime: int
+        :param BackupDownloadRestriction: 备份下载限制
+        :type BackupDownloadRestriction: :class:`tencentcloud.postgres.v20170312.models.BackupDownloadRestriction`
         """
         self.DBInstanceId = None
         self.BackupType = None
         self.BackupId = None
         self.URLExpireTime = None
+        self.BackupDownloadRestriction = None
 
 
     def _deserialize(self, params):
         self.DBInstanceId = params.get("DBInstanceId")
         self.BackupType = params.get("BackupType")
         self.BackupId = params.get("BackupId")
         self.URLExpireTime = params.get("URLExpireTime")
+        if params.get("BackupDownloadRestriction") is not None:
+            self.BackupDownloadRestriction = BackupDownloadRestriction()
+            self.BackupDownloadRestriction._deserialize(params.get("BackupDownloadRestriction"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.876/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/setup.py` & `tencentcloud-sdk-python-postgres-3.0.876/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.875/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.876/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.875
+Version: 3.0.876
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

