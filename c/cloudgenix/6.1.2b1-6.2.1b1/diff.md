# Comparing `tmp/cloudgenix-6.1.2b1.tar.gz` & `tmp/cloudgenix-6.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudgenix-6.1.2b1.tar", last modified: Tue Jan 24 02:40:26 2023, max compression
+gzip compressed data, was "dist/cloudgenix-6.2.1b1.tar", last modified: Wed Apr 19 19:25:34 2023, max compression
```

## Comparing `cloudgenix-6.1.2b1.tar` & `cloudgenix-6.2.1b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)     1077 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/LICENSE
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)     4791 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/PKG-INFO
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)     4147 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/README.md
-drwxr-xr-x   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix/
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)    66495 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/__init__.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)    14160 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/ca_bundle.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)   143769 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/delete_api.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)   358346 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/get_api.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)    48216 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/interactive.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)    17468 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/patch_api.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)   515287 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/post_api.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)   284796 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/put_api.py
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)     4468 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/cloudgenix/ws_api.py
-drwxr-xr-x   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)        0 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)     4791 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/PKG-INFO
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)      415 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/SOURCES.txt
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)        1 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/dependency_links.txt
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)       71 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/requires.txt
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)       11 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/cloudgenix.egg-info/top_level.txt
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)      262 2023-01-24 02:40:26.000000 cloudgenix-6.1.2b1/setup.cfg
--rw-r--r--   0 dishah   (1305937620) PALOALTONETWORK\Domain Users (192360288)      999 2023-01-24 02:35:40.000000 cloudgenix-6.1.2b1/setup.py
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/
+-rw-r--r--   0 dishah   (1305937620) 192360288     1077 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/LICENSE
+-rw-r--r--   0 dishah   (1305937620) 192360288     4859 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/PKG-INFO
+-rw-r--r--   0 dishah   (1305937620) 192360288     4215 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/README.md
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix/
+-rw-r--r--   0 dishah   (1305937620) 192360288    66495 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/__init__.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    14160 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/ca_bundle.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   146123 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/delete_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   370766 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/get_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    48216 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/interactive.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    17707 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/patch_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   530779 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/post_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   290322 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/put_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288     4468 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/ws_api.py
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/
+-rw-r--r--   0 dishah   (1305937620) 192360288     4859 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/PKG-INFO
+-rw-r--r--   0 dishah   (1305937620) 192360288      415 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/SOURCES.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288        1 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/dependency_links.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288       71 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/requires.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288       11 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/top_level.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288      262 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/setup.cfg
+-rw-r--r--   0 dishah   (1305937620) 192360288      999 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/setup.py
```

### Comparing `cloudgenix-6.1.2b1/LICENSE` & `cloudgenix-6.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.1.2b1/PKG-INFO` & `cloudgenix-6.2.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix
-Version: 6.1.2b1
+Version: 6.2.1b1
 Summary: Python2 and Python3 SDK for the CloudGenix AppFabric
 Home-page: https://github.com/CloudGenix/sdk-python
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.1.2b1
+# CloudGenix Python SDK v6.2.1b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
@@ -57,14 +57,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
 | **5.5.3** | **b1** | Support for June 2021 Controller release. |
```

### Comparing `cloudgenix-6.1.2b1/README.md` & `cloudgenix-6.2.1b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.1.2b1
+# CloudGenix Python SDK v6.2.1b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
@@ -39,14 +39,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
 | **5.5.3** | **b1** | Support for June 2021 Controller release. |
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/__init__.py` & `cloudgenix-6.2.1b1/cloudgenix/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
-**Version:** v6.1.2b1
+**Version:** v6.2.1b1
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017-2023 CloudGenix, Inc
 
 **License:** MIT
 
@@ -137,15 +137,15 @@
 """logging.getlogger object to enable debug printing via `cloudgenix.API.set_debug`"""
 
 if PYTHON36_FEATURES:
     ws_logger = logging.getLogger('websockets')
 
 
 # Version of SDK
-version = "6.1.2b1"
+version = "6.2.1b1"
 """SDK Version string"""
 __version__ = version
 
 # PyPI URL for checking for updates.
 update_info_url = "https://pypi.org/pypi/cloudgenix/json"
 """URL for checking for updates."""
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/ca_bundle.py` & `cloudgenix-6.2.1b1/cloudgenix/ca_bundle.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.1.2b1/cloudgenix/delete_api.py` & `cloudgenix-6.2.1b1/cloudgenix/delete_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,23 +76,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/apnprofiles/{}".format(api_version,
                                                                          tenant_id,
                                                                          apnprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def appdefs(self, appdef_id, tenant_id=None, api_version="v2.4"):
+    def appdefs(self, appdef_id, tenant_id=None, api_version="v2.5"):
         """
-        Delete a application definition (v2.4)
+        Delete an application definition (v2.5)
 
           **Parameters:**:
 
           - **appdef_id**: Application Definition ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -196,24 +196,24 @@
                                                                                            site_id,
                                                                                            element_id,
                                                                                            bgppeer_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def dhcpservers(self, site_id, dhcpserver_id, tenant_id=None, api_version="v2.1"):
+    def dhcpservers(self, site_id, dhcpserver_id, tenant_id=None, api_version="v2.2"):
         """
-        Delete DHCPServer for a Tenant on a site (v2.1)
+        Delete DHCPServer for a Tenant on a site (v2.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **dhcpserver_id**: DHCP Server ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -226,35 +226,63 @@
                                                                                   tenant_id,
                                                                                   site_id,
                                                                                   dhcpserver_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def dnsserviceprofiles(self, dnsserviceprofile_id, tenant_id=None, api_version="v2.0"):
+    def directoryservices(self, directoryservice_id, tenant_id=None, api_version="v2.0"):
         """
-        Delete a DNS service profile (v2.0)
+        DELETE Directoryservices API Function
 
           **Parameters:**:
 
-          - **dnsserviceprofile_id**: DNS Service Profile ID
+          - **directoryservice_id**: Directory Service ID
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
         elif not tenant_id:
             # No value for tenant_id.
             raise TypeError("tenant_id is required but not set or cached.")
         cur_ctlr = self._parent_class.controller
 
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/{}".format(api_version,
+                                                                               tenant_id,
+                                                                               directoryservice_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "delete")
+
+    def dnsserviceprofiles(self, dnsserviceprofile_id, tenant_id=None, api_version="v2.1"):
+        """
+        Delete a DNS service profile (v2.1)
+
+          **Parameters:**:
+
+          - **dnsserviceprofile_id**: DNS Service Profile ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.1)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
         url = str(cur_ctlr) + "/{}/api/tenants/{}/dnsserviceprofiles/{}".format(api_version,
                                                                                 tenant_id,
                                                                                 dnsserviceprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
@@ -290,15 +318,15 @@
         """
         Delete a DNS service config (v2.0)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
-          - **dnsservice_id**: DNS Service ID 
+          - **dnsservice_id**: DNS Service ID
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -760,25 +788,25 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/idps/{}".format(api_version,
                                                                   tenant_id,
                                                                   idp_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def interfaces(self, site_id, element_id, interface_id, tenant_id=None, api_version="v4.14"):
+    def interfaces(self, site_id, element_id, interface_id, tenant_id=None, api_version="v4.15"):
         """
-        Delete Cellular Interface (v4.14)
+        Delete Cellular Interface (v4.15)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
           - **interface_id**: Interface ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v4.14)
+          - **api_version**: API version to use (default v4.15)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -992,24 +1020,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ipsecprofiles/{}".format(api_version,
                                                                            tenant_id,
                                                                            ipsecprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def lannetworks(self, site_id, lannetwork_id, tenant_id=None, api_version="v3.1"):
+    def lannetworks(self, site_id, lannetwork_id, tenant_id=None, api_version="v3.2"):
         """
-        Delete an existing LAN (v3.1)
+        Delete an existing LAN (v3.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **lannetwork_id**: LAN Network ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1398,23 +1426,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkcontexts/{}".format(api_version,
                                                                              tenant_id,
                                                                              networkcontext_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id, tenant_id=None, api_version="v2.0"):
+    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete a Network Policy Global Prefix. (v2.0)
+        Delete a Network Policy Global Prefix. (v2.1)
 
           **Parameters:**:
 
           - **networkpolicyglobalprefix_id**: Network Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1426,24 +1454,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicyglobalprefixes/{}".format(api_version,
                                                                                          tenant_id,
                                                                                          networkpolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id, tenant_id=None, api_version="v2.1"):
+    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id, tenant_id=None, api_version="v2.2"):
         """
-        Delete network policy rule of tenant. (v2.1)
+        Delete network policy rule of tenant. (v2.2)
 
           **Parameters:**:
 
           - **networkpolicyset_id**: Network Policy Set ID
           - **networkpolicyrule_id**: Network Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1512,23 +1540,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicysetstacks/{}".format(api_version,
                                                                                     tenant_id,
                                                                                     networkpolicysetstack_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete a Security Policy V2 Local Prefix by tenant ID and its ID (v2.0)
+        Delete a Security Policy V2 Local Prefix by tenant ID and its ID (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyglobalprefix_id**: NGFW Security Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1568,24 +1596,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicylocalprefixes/{}".format(api_version,
                                                                                              tenant_id,
                                                                                              ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete an existing Security Policy V2 Rule under a policy set (v2.0)
+        Delete an existing Security Policy V2 Rule under a policy set (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyset_id**: NGFW Security Policy Set ID
           - **ngfwsecuritypolicyrule_id**: NGFW Security Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1800,23 +1828,23 @@
                                                                                     tenant_id,
                                                                                     site_id,
                                                                                     prefixfilter_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete a Priority Policy Global Prefix. (v2.0)
+        Delete a Priority Policy Global Prefix. (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyglobalprefix_id**: Priority Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1828,24 +1856,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicyglobalprefixes/{}".format(api_version,
                                                                                           tenant_id,
                                                                                           prioritypolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete priority policy rule of tenant. (v2.0)
+        Delete priority policy rule of tenant. (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyset_id**: Priority Policy Set ID
           - **prioritypolicyrule_id**: Priority Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2420,24 +2448,24 @@
                                                                                        tenant_id,
                                                                                        site_id,
                                                                                        natlocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id, tenant_id=None, api_version="v2.0"):
+    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete an existing Site Network Policy local prefix association (v2.0)
+        Delete an existing Site Network Policy local prefix association (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **networkpolicylocalprefix_id**: Network Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2450,24 +2478,24 @@
                                                                                                  tenant_id,
                                                                                                  site_id,
                                                                                                  networkpolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id, tenant_id=None, api_version="v2.0"):
+    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete an existing security policy v2 local prefix site association (v2.0)
+        Delete an existing security policy v2 local prefix site association (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **ngfwsecuritypolicylocalprefix_id**: NGFW Security Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2480,24 +2508,24 @@
                                                                                                       tenant_id,
                                                                                                       site_id,
                                                                                                       ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
-    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id, tenant_id=None, api_version="v2.0"):
+    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id, tenant_id=None, api_version="v2.1"):
         """
-        Delete an existing Site Priority Policy local prefix association (v2.0)
+        Delete an existing Site Priority Policy local prefix association (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **prioritypolicylocalprefix_id**: Priority Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2978,14 +3006,42 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/tenantpassageconfigs/{}".format(api_version,
                                                                                   tenant_id,
                                                                                   tenantpassageconfig_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "delete")
 
+    def useridagents(self, useridagent_id, tenant_id=None, api_version="v2.0"):
+        """
+        DELETE Useridagents API Function
+
+          **Parameters:**:
+
+          - **useridagent_id**: User Id Agent ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents/{}".format(api_version,
+                                                                          tenant_id,
+                                                                          useridagent_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "delete")
+
     def users(self, user_id, tenant_id=None, api_version="v2.0"):
         """
         Delete an user identity. (v2.0)
 
           **Parameters:**:
 
           - **user_id**: User ID
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/get_api.py` & `cloudgenix-6.2.1b1/cloudgenix/get_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,23 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/apnprofiles/{}".format(api_version,
                                                                              tenant_id,
                                                                              apnprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def appdefs(self, appdef_id=None, tenant_id=None, api_version="v2.4"):
+    def appdefs(self, appdef_id=None, tenant_id=None, api_version="v2.5"):
         """
-        Get all application definitions (v2.4)
+        Get all application definitions (v2.5)
 
           **Parameters:**:
 
           - **appdef_id**: (optional) Application Definition ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -843,24 +843,59 @@
                                                                                     tenant_id,
                                                                                     site_id,
                                                                                     demstatus_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def dhcpservers(self, site_id, dhcpserver_id=None, tenant_id=None, api_version="v2.1"):
+    def deviceidconfigs(self, site_id, deviceidconfig_id=None, tenant_id=None, api_version="v2.0"):
+        """
+        GET Deviceidconfigs API Function
+
+          **Parameters:**:
+
+          - **site_id**: Site ID
+          - **deviceidconfig_id**: (optional) Device Id Config ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        if not deviceidconfig_id:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/deviceidconfigs".format(api_version,
+                                                                                       tenant_id,
+                                                                                       site_id)
+        else:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/deviceidconfigs/{}".format(api_version,
+                                                                                          tenant_id,
+                                                                                          site_id,
+                                                                                          deviceidconfig_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
+    def dhcpservers(self, site_id, dhcpserver_id=None, tenant_id=None, api_version="v2.2"):
         """
-        Get all DHCPServers for a Tenant on a site (v2.1)
+        Get all DHCPServers for a Tenant on a site (v2.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **dhcpserver_id**: (optional) DHCP Server ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -878,35 +913,151 @@
                                                                                       tenant_id,
                                                                                       site_id,
                                                                                       dhcpserver_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def dnsserviceprofiles(self, dnsserviceprofile_id=None, tenant_id=None, api_version="v2.0"):
+    def directoryservices(self, tenant_id=None, api_version="v2.0"):
         """
-        Read all DNS service profiles (v2.0)
+        GET Directoryservices API Function
+
+          **Parameters:**:
+
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices".format(api_version,
+                                                                            tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
+    def directoryservices_status(self, tenant_id=None, api_version="v2.0"):
+        """
+        GET Directoryservices_Status API Function
 
           **Parameters:**:
 
-          - **dnsserviceprofile_id**: (optional) DNS Service Profile ID
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
         elif not tenant_id:
             # No value for tenant_id.
             raise TypeError("tenant_id is required but not set or cached.")
         cur_ctlr = self._parent_class.controller
 
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/status".format(api_version,
+                                                                                   tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
+    def directoryusergroups(self, directoryusergroup_id=None, tenant_id=None, api_version="v2.0"):
+        """
+        GET Directoryusergroups API Function
+
+          **Parameters:**:
+
+          - **directoryusergroup_id**: (optional) Directory User Group ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        if not directoryusergroup_id:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusergroups".format(api_version,
+                                                                                  tenant_id)
+        else:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusergroups/{}".format(api_version,
+                                                                                     tenant_id,
+                                                                                     directoryusergroup_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
+    def directoryusers(self, directoryuser_id=None, tenant_id=None, api_version="v2.0"):
+        """
+        GET Directoryusers API Function
+
+          **Parameters:**:
+
+          - **directoryuser_id**: (optional) Directory User ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        if not directoryuser_id:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusers".format(api_version,
+                                                                             tenant_id)
+        else:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusers/{}".format(api_version,
+                                                                                tenant_id,
+                                                                                directoryuser_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
+    def dnsserviceprofiles(self, dnsserviceprofile_id=None, tenant_id=None, api_version="v2.1"):
+        """
+        Read all DNS service profiles (v2.1)
+
+          **Parameters:**:
+
+          - **dnsserviceprofile_id**: (optional) DNS Service Profile ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.1)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
         if not dnsserviceprofile_id:
             url = str(cur_ctlr) + "/{}/api/tenants/{}/dnsserviceprofiles".format(api_version,
                                                                                  tenant_id)
         else:
             url = str(cur_ctlr) + "/{}/api/tenants/{}/dnsserviceprofiles/{}".format(api_version,
                                                                                     tenant_id,
                                                                                     dnsserviceprofile_id)
@@ -950,15 +1101,15 @@
         """
         Read all DNS service configs (v2.0)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
-          - **dnsservice_id**: (optional) DNS Service ID 
+          - **dnsservice_id**: (optional) DNS Service ID
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -980,14 +1131,44 @@
                                                                                                   site_id,
                                                                                                   element_id,
                                                                                                   dnsservice_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
+    def directoryservices_domainstatus(self, directoryservice_id, domainstatus_id, tenant_id=None, api_version="v2.0"):
+        """
+        GET Domainstatus_Directoryservices API Function
+
+          **Parameters:**:
+
+          - **directoryservice_id**: Directory Service ID
+          - **domainstatus_id**: Domain Status ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/{}/domainstatus/{}".format(api_version,
+                                                                                               tenant_id,
+                                                                                               directoryservice_id,
+                                                                                               domainstatus_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
     def element_bgppeers_status(self, site_id, element_id, bgppeer_id, tenant_id=None, api_version="v2.1"):
         """
         GET Element_Bgppeers_Status API Function
 
           **Parameters:**:
 
           - **site_id**: Site ID
@@ -1300,23 +1481,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/elements/{}/state".format(api_version,
                                                                             tenant_id,
                                                                             element_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def element_status(self, element_id, tenant_id=None, api_version="v2.1"):
+    def element_status(self, element_id, tenant_id=None, api_version="v2.2"):
         """
-        Get specific element status for a tenant (v2.1)
+        Get specific element status for a tenant (v2.2)
 
           **Parameters:**:
 
           - **element_id**: Element (Device) ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1616,22 +1797,22 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/elementusers/{}/password".format(api_version,
                                                                                    tenant_id,
                                                                                    elementuser_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def enterpriseprefixset(self, tenant_id=None, api_version="v2.0"):
+    def enterpriseprefixset(self, tenant_id=None, api_version="v2.1"):
         """
         GET Enterpriseprefixset API Function
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2175,25 +2356,25 @@
                                                                                                                              element_id,
                                                                                                                              interface_id,
                                                                                                                              multicastigmpmembership_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def interfaces(self, site_id, element_id, interface_id=None, tenant_id=None, api_version="v4.14"):
+    def interfaces(self, site_id, element_id, interface_id=None, tenant_id=None, api_version="v4.15"):
         """
-        Get all Cellular Interfaces (v4.14)
+        Get all Cellular Interfaces (v4.15)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
           - **interface_id**: (optional) Interface ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v4.14)
+          - **api_version**: API version to use (default v4.15)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -2539,24 +2720,24 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/ipsecprofiles/{}".format(api_version,
                                                                                tenant_id,
                                                                                ipsecprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def lannetworks(self, site_id, lannetwork_id=None, tenant_id=None, api_version="v3.1"):
+    def lannetworks(self, site_id, lannetwork_id=None, tenant_id=None, api_version="v3.2"):
         """
-        Get LAN networks (v3.1)
+        Get LAN networks (v3.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **lannetwork_id**: (optional) LAN Network ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3027,14 +3208,40 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/aggregates".format(api_version,
                                                                                    tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
+    def monitor_aiops_anomaly(self, tenant_id=None, api_version="v2.0"):
+        """
+        GET Monitor_Aiops_Anomaly API Function
+
+          **Parameters:**:
+
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/anomaly".format(api_version,
+                                                                                tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
     def monitor_aiops_forecast(self, tenant_id=None, api_version="v2.1"):
         """
         GET Monitor_Aiops_Forecast API Function
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
@@ -3105,14 +3312,42 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/object_stats".format(api_version,
                                                                                      tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
+    def monitor_application_qos_metrics(self, qos_metric_id, tenant_id=None, api_version="v2.0"):
+        """
+        GET Monitor_Application_Qos_Metrics API Function
+
+          **Parameters:**:
+
+          - **qos_metric_id**: QoS Metric ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/application/qos_metrics/{}".format(api_version,
+                                                                                             tenant_id,
+                                                                                             qos_metric_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
     def monitor_bulk_metrics(self, bulk_metric_id, tenant_id=None, api_version="v2.0"):
         """
         GET Monitor_Bulk_Metrics API Function
 
           **Parameters:**:
 
           - **bulk_metric_id**: Bulk Metric ID
@@ -3187,22 +3422,22 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/metrics/{}".format(api_version,
                                                                              tenant_id,
                                                                              metric_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def monitor_object_stats(self, tenant_id=None, api_version="v2.4"):
+    def monitor_object_stats(self, tenant_id=None, api_version="v2.5"):
         """
         GET Monitor_Object_Stats API Function
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3239,22 +3474,22 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/qos_metrics".format(api_version,
                                                                               tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def monitor_sys_metrics(self, tenant_id=None, api_version="v2.2"):
+    def monitor_sys_metrics(self, tenant_id=None, api_version="v2.3"):
         """
         GET Monitor_Sys_Metrics API Function
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.2)
+          - **api_version**: API version to use (default v2.3)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3936,23 +4171,23 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/networkcontexts/{}".format(api_version,
                                                                                  tenant_id,
                                                                                  networkcontext_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get all Network policy global prefixes. (v2.0)
+        Get all Network policy global prefixes. (v2.1)
 
           **Parameters:**:
 
           - **networkpolicyglobalprefix_id**: (optional) Network Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3968,24 +4203,24 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicyglobalprefixes/{}".format(api_version,
                                                                                              tenant_id,
                                                                                              networkpolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id=None, tenant_id=None, api_version="v2.1"):
+    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id=None, tenant_id=None, api_version="v2.2"):
         """
-        Get network policy rules of tenant (v2.1)
+        Get network policy rules of tenant (v2.2)
 
           **Parameters:**:
 
           - **networkpolicyset_id**: Network Policy Set ID
           - **networkpolicyrule_id**: (optional) Network Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -4095,23 +4330,23 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicysetstacks/{}".format(api_version,
                                                                                         tenant_id,
                                                                                         networkpolicysetstack_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get all Security Policy V2 Global Prefixes for a tenant (v2.0)
+        Get all Security Policy V2 Global Prefixes for a tenant (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyglobalprefix_id**: (optional) NGFW Security Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -4159,24 +4394,24 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicylocalprefixes/{}".format(api_version,
                                                                                                  tenant_id,
                                                                                                  ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id=None, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get all Security Policy V2 Rules under a policy set (v2.0)
+        Get all Security Policy V2 Rules under a policy set (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyset_id**: NGFW Security Policy Set ID
           - **ngfwsecuritypolicyrule_id**: (optional) NGFW Security Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -4630,23 +4865,23 @@
                                                                                         tenant_id,
                                                                                         site_id,
                                                                                         prefixfilter_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get all Priority policy prefixes. (v2.0)
+        Get all Priority policy prefixes. (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyglobalprefix_id**: (optional) Priority Policy Global Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -4662,24 +4897,24 @@
             url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicyglobalprefixes/{}".format(api_version,
                                                                                               tenant_id,
                                                                                               prioritypolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id=None, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get priority policy rules of tenant (v2.0)
+        Get priority policy rules of tenant (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyset_id**: Priority Policy Set ID
           - **prioritypolicyrule_id**: (optional) Priority Policy Rule ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -5766,24 +6001,24 @@
                                                                                            tenant_id,
                                                                                            site_id,
                                                                                            natlocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get site Network policy prefix associations (v2.0)
+        Get site Network policy prefix associations (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **networkpolicylocalprefix_id**: (optional) Network Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -5801,24 +6036,24 @@
                                                                                                      tenant_id,
                                                                                                      site_id,
                                                                                                      networkpolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get all security policy v2 local prefix site association for a site (v2.0)
+        Get all security policy v2 local prefix site association for a site (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **ngfwsecuritypolicylocalprefix_id**: (optional) NGFW Security Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -5836,24 +6071,24 @@
                                                                                                           tenant_id,
                                                                                                           site_id,
                                                                                                           ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id=None, tenant_id=None, api_version="v2.0"):
+    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id=None, tenant_id=None, api_version="v2.1"):
         """
-        Get site Priority policy prefix associations (v2.0)
+        Get site Priority policy prefix associations (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **prioritypolicylocalprefix_id**: (optional) Priority Policy Local Prefix ID
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -6828,22 +7063,22 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/tenantpassageconfigs".format(api_version,
                                                                                tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def tenants(self, tenant_id=None, api_version="v2.4"):
+    def tenants(self, tenant_id=None, api_version="v2.5"):
         """
-        Get tenant details for tenant id (v2.4)
+        Get tenant details for tenant id (v2.5)
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -6880,14 +7115,46 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/toolkitsessions".format(api_version,
                                                                           tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
+    def useridagents(self, useridagent_id=None, tenant_id=None, api_version="v2.0"):
+        """
+        GET Useridagents API Function
+
+          **Parameters:**:
+
+          - **useridagent_id**: (optional) User Id Agent ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        if not useridagent_id:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents".format(api_version,
+                                                                           tenant_id)
+        else:
+            url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents/{}".format(api_version,
+                                                                              tenant_id,
+                                                                              useridagent_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
     def users(self, user_id=None, tenant_id=None, api_version="v2.0"):
         """
         Get Users. (v2.0)
 
           **Parameters:**:
 
           - **user_id**: (optional) User ID
@@ -7394,14 +7661,17 @@
 
     aggregates_aiops_monitor = monitor_aiops_aggregates
     """ Backwards-compatibility alias of `aggregates_aiops_monitor` to `monitor_aiops_aggregates`"""
 
     aggregates_monitor = monitor_aggregates
     """ Backwards-compatibility alias of `aggregates_monitor` to `monitor_aggregates`"""
 
+    anomaly_aiops_monitor = monitor_aiops_anomaly
+    """ Backwards-compatibility alias of `anomaly_aiops_monitor` to `monitor_aiops_anomaly`"""
+
     anynetlinks_s = site_anynetlinks
     """ Backwards-compatibility alias of `anynetlinks_s` to `site_anynetlinks`"""
 
     anynetlinks_t = tenant_anynetlinks
     """ Backwards-compatibility alias of `anynetlinks_t` to `tenant_anynetlinks`"""
 
     api_versions_t = tenant_api_versions
@@ -7448,14 +7718,17 @@
 
     correlationevents_waninterfaces = wantinterfaces_correlationevents
     """ Backwards-compatibility alias of `correlationevents_waninterfaces` to `wantinterfaces_correlationevents`"""
 
     discoveredprefixes_bgppeers = bgppeers_discoveredprefixes
     """ Backwards-compatibility alias of `discoveredprefixes_bgppeers` to `bgppeers_discoveredprefixes`"""
 
+    domainstatus_directoryservices = directoryservices_domainstatus
+    """ Backwards-compatibility alias of `discoveredprefixes_bgppeers` to `bgppeers_discoveredprefixes`"""
+
     elementpassageconfigs_e = elementpassageconfigs
     """ Backwards-compatibility alias of `elementpassageconfigs_e` to `elementpassageconfigs`"""
 
     elementpassageconfigs_t = tenant_elementpassageconfigs
     """ Backwards-compatibility alias of `elementpassageconfigs_t` to `tenant_elementpassageconfigs`"""
 
     extensions_i = element_extensions
@@ -7565,14 +7838,17 @@
 
     prioritypolicylocalprefixes_s = site_prioritypolicylocalprefixes
     """ Backwards-compatibility alias of `prioritypolicylocalprefixes_s` to `site_prioritypolicylocalprefixes`"""
 
     prioritypolicylocalprefixes_t = tenant_prioritypolicylocalprefixes
     """ Backwards-compatibility alias of `prioritypolicylocalprefixes_t` to `tenant_prioritypolicylocalprefixes`"""
 
+    qos_metrics_application_monitor = monitor_application_qos_metrics
+    """ Backwards-compatibility alias of `qos_metrics_application_monitor` to `monitor_application_qos_metrics`"""
+
     qos_metrics_monitor = monitor_qos_metrics
     """ Backwards-compatibility alias of `qos_metrics_monitor` to `monitor_qos_metrics`"""
 
     reachableprefixes_bgppeers = bgppeers_reachableprefixes
     """ Backwards-compatibility alias of `reachableprefixes_bgppeers` to `bgppeers_reachableprefixes`"""
 
     revoked_certificates = certificates_revoked
@@ -7613,14 +7889,17 @@
 
     status_cellular_modules_e = element_cellular_modules_status
     """ Backwards-compatibility alias of `status_cellular_modules_e` to `element_cellular_modules_status`"""
 
     status_cellular_modules_m = machine_cellular_modules_status
     """ Backwards-compatibility alias of `status_cellular_modules_m` to `machine_cellular_modules_status`"""
 
+    status_directoryservices = directoryservices_status
+    """ Backwards-compatibility alias of `status_directoryservices` to `directoryservices_status`"""
+
     status_e = element_status
     """ Backwards-compatibility alias of `status_e` to `element_status`"""
 
     status_firmware_cellular_modules_e = element_cellular_modules_firmware_status
     """ Backwards-compatibility alias of `status_firmware_cellular_modules_e` to `element_cellular_modules_firmware_status`"""
 
     status_firmware_cellular_modules_m = machine_cellular_modules_firmware_status
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/interactive.py` & `cloudgenix-6.2.1b1/cloudgenix/interactive.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.1.2b1/cloudgenix/patch_api.py` & `cloudgenix-6.2.1b1/cloudgenix/patch_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,23 +161,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/operators/{}".format(api_version,
                                                                        tenant_id,
                                                                        operator_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "patch", data=data)
 
-    def tenants(self, data, tenant_id=None, api_version="v2.4"):
+    def tenants(self, data, tenant_id=None, api_version="v2.5"):
         """
-        Patch tenant (v2.4)
+        Patch tenant (v2.5)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to PATCH as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
            - **address:**           
                - **city:**  Type: string 
                - **country:**  Type: string 
                - **post_code:**  Type: string 
@@ -191,14 +191,15 @@
            - **disabled:**  Type: string 
            - **disabled_reason:**  Type: string 
            - **inactive:**  Type: string 
            - **inactive_reason:**  Type: string 
            - **ipv4_list:**           
                - **ipv4:**  Type: string 
            - **is_esp:**  Type: boolean 
+           - **is_pa_iot_security_license:**  Type: boolean 
            - **is_support:**  Type: boolean 
            - **name:**  Type: string 
            - **operator:**           
                - **addresses:**           
                    - **city:**  Type: string 
                    - **country:**  Type: string 
                    - **post_code:**  Type: string 
@@ -352,14 +353,18 @@
                - **salt:**  Type: string 
                - **security:**  Type: string 
            - **region:**  Type: string 
            - **sase_at:**  Type: string 
            - **telemetry_region:**  Type: string 
            - **tenant_id:**  Type: string 
            - **tsg_id:**  Type: string 
+           - **tsg_instances:**           
+               - **app_id:**  Type: string 
+               - **region:**  Type: string 
+               - **tenant_id:**  Type: string 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/post_api.py` & `cloudgenix-6.2.1b1/cloudgenix/post_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,44 @@
 
     Object to handle making Post requests via shared Requests Session.
     """
 
     # placeholder for parent class namespace
     _parent_class = None
 
+    def activeuserips_query(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Activeuserips_Query API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/activeuserips/query".format(api_version,
+                                                                              tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def anynetlinks_correlationevents_query(self, data, tenant_id=None, api_version="v2.1"):
         """
         POST Anynetlinks_Correlationevents_Query API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -160,23 +190,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/apnprofiles/query".format(api_version,
                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def appdefs(self, data, tenant_id=None, api_version="v2.4"):
+    def appdefs(self, data, tenant_id=None, api_version="v2.5"):
         """
-        Create a application definition (v2.4)
+        Create an application definition (v2.5)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
            - **abbreviation:**  Type: string 
            - **aggregate_flows:**  Type: boolean 
            - **app_type:**  Type: string 
            - **app_unreachability_detection:**  Type: boolean 
@@ -295,23 +325,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/appdefs/{}/overrides".format(api_version,
                                                                                tenant_id,
                                                                                appdef_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def appdefs_query(self, data, tenant_id=None, api_version="v2.4"):
+    def appdefs_query(self, data, tenant_id=None, api_version="v2.5"):
         """
-        Queries db for limit number of app defs that match query params. (v2.4)
+        Queries db for limit number of app defs that match query params. (v2.5)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -495,15 +525,15 @@
           - **bgppeer_id**: BGP Peer ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
           **Payload Attributes:** 
 
-           - **value:**  Type: string 
+           - **action:**  Type: string 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1120,27 +1150,60 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/demstatus/query".format(api_version,
                                                                           tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def dhcpservers(self, site_id, data, tenant_id=None, api_version="v2.1"):
+    def deviceidconfigs(self, site_id, data, tenant_id=None, api_version="v2.0"):
         """
-        Create a new dhcp server configuration for a subnet (v2.1)
+        POST Deviceidconfigs API Function
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/deviceidconfigs".format(api_version,
+                                                                                   tenant_id,
+                                                                                   site_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def dhcpservers(self, site_id, data, tenant_id=None, api_version="v2.2"):
+        """
+        Create a new dhcp server configuration for a subnet (v2.2)
+
+          **Parameters:**:
+
+          - **site_id**: Site ID
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
+           - **address_family:**  Type: string 
            - **broadcast_address:**  Type: string 
            - **custom_options:**           
                - **option_definition:**  Type: string 
                - **option_value:**  Type: string 
                - **vendor_class_identifier:**  Type: string 
            - **default_lease_time:**  Type: integer 
            - **description:**  Type: string 
@@ -1150,14 +1213,15 @@
            - **gateway:**  Type: string 
            - **ip_ranges:**           
                - **end_ip:**  Type: string 
                - **start_ip:**  Type: string 
            - **max_lease_time:**  Type: integer 
            - **network_context_id:**  Type: string 
            - **static_mappings:**           
+               - **client_duid:**  Type: string 
                - **ip_address:**  Type: string 
                - **mac:**  Type: string 
                - **name:**  Type: string 
            - **subnet:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
@@ -1174,26 +1238,116 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/dhcpservers".format(api_version,
                                                                                tenant_id,
                                                                                site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def dnsserviceprofiles(self, data, tenant_id=None, api_version="v2.0"):
+    def directoryservices(self, data, tenant_id=None, api_version="v2.0"):
         """
-        Create a new DNS service profile (v2.0)
+        POST Directoryservices API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
           **Payload Attributes:** 
 
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices".format(api_version,
+                                                                            tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def directoryusergroups_query(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Directoryusergroups_Query API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusergroups/query".format(api_version,
+                                                                                    tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def directoryusers_query(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Directoryusers_Query API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryusers/query".format(api_version,
+                                                                               tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def dnsserviceprofiles(self, data, tenant_id=None, api_version="v2.1"):
+        """
+        Create a new DNS service profile (v2.1)
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.1)
+
+          **Payload Attributes:** 
+
            - **authoritative_config:**           
                - **caa_records:**           
                    - **flags:**  Type: string 
                    - **name:**  Type: string 
                    - **tag:**  Type: string 
                    - **value:**  Type: string 
                - **cname_records:**           
@@ -1260,18 +1414,17 @@
            - **cache_config:**           
                - **cache_size:**  Type: integer 
                - **disable_negative_caching:**  Type: boolean 
                - **max_cache_ttl:**  Type: integer 
                - **min_cache_ttl:**  Type: integer 
                - **negative_cache_ttl:**  Type: integer 
            - **description:**  Type: string 
-           - **disabled:**  Type: boolean 
-           - **disabled_reason:**  Type: string 
            - **dns_forward_config:**           
                - **dns_servers:**           
+                   - **address_family:**  Type: string 
                    - **dnsserver_ip:**  Type: string 
                    - **dnsserver_port:**  Type: integer 
                    - **domain_names:**  [Type: string] 
                    - **forward_dnsservicerole_id:**  Type: string 
                    - **ip_prefix:**  Type: string 
                    - **source_port:**  Type: integer 
                - **max_source_port:**  Type: integer 
@@ -1320,22 +1473,18 @@
                - **domain_names:**  [Type: string] 
                - **ipv4_address:**  Type: string 
                - **ipv6_address:**  Type: string 
            - **edns_packet_max:**  Type: integer 
            - **enable_dns_loop_detection:**  Type: boolean 
            - **enable_dnssec_proxy:**  Type: boolean 
            - **enable_strict_domain_name:**  Type: boolean 
-           - **inactive:**  Type: boolean 
-           - **inactive_reason:**  Type: string 
            - **listen_dnsservicerole_id:**  Type: string 
            - **listen_port:**  Type: integer 
            - **name:**  Type: string 
-           - **region:**  Type: string 
            - **tags:**  [Type: string] 
-           - **tenant_id:**  Type: string 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -1346,23 +1495,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/dnsserviceprofiles".format(api_version,
                                                                              tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def dnsserviceprofiles_query(self, data, tenant_id=None, api_version="v2.0"):
+    def dnsserviceprofiles_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query DNS service profile based on parameters (v2.0)
+        Query DNS service profile based on parameters (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -2565,33 +2714,34 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/hubclusters/query".format(api_version,
                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def interfaces(self, site_id, element_id, data, tenant_id=None, api_version="v4.14"):
+    def interfaces(self, site_id, element_id, data, tenant_id=None, api_version="v4.15"):
         """
-        Create a Interface (v4.14)
+        Create a Interface (v4.15)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v4.14)
+          - **api_version**: API version to use (default v4.15)
 
           **Payload Attributes:** 
 
            - **admin_up:**  Type: boolean 
            - **attached_lan_networks:**           
                - **lan_network_id:**  Type: string 
                - **vlan_id:**  Type: integer 
            - **authentication_config:**           
+               - **fallback_retry_count:**  Type: integer 
                - **mode:**  Type: string 
                - **reauthentication_timeout:**  Type: integer 
            - **bound_interfaces:**  [Type: string] 
            - **bypass_pair:**           
                - **lan:**  Type: string 
                - **lan_state_propagation:**  Type: boolean 
                - **use_relay:**  Type: boolean 
@@ -2668,14 +2818,15 @@
                    - **name_servers:**  [Type: string] 
                    - **search:**  [Type: string] 
                - **routes:**           
                    - **destination:**  Type: string 
                    - **via:**  Type: string 
                - **static_config:**           
                    - **address:**  Type: string 
+                   - **enable_prefix_distribution:**  Type: boolean 
                - **type:**  Type: string 
            - **lldp_enabled:**  Type: boolean 
            - **mac_address:**  Type: string 
            - **mtu:**  Type: integer 
            - **multicast_config:**           
                - **igmp_version:**  Type: string 
                - **multicast_enabled:**  Type: boolean 
@@ -2688,14 +2839,15 @@
                    - **start:**  Type: string 
                - **nat_pool_id:**  Type: string 
            - **nat_port:**  Type: integer 
            - **nat_port_v6:**  Type: integer 
            - **nat_zone_id:**  Type: string 
            - **network_context_id:**  Type: string 
            - **parent:**  Type: string 
+           - **peer_bypasspair_wan_port_type:**  Type: string 
            - **poe_enabled:**  Type: boolean 
            - **power_usage_threshold:**  Type: integer 
            - **pppoe_config:**           
                - **host_uniq:**  Type: string 
                - **ip_address_type:**  Type: string 
                - **password:**  Type: string 
                - **reconnection_delay:**  Type: integer 
@@ -2829,23 +2981,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/interfaces/correlationevents/query".format(api_version,
                                                                                              tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def interfaces_query(self, data, tenant_id=None, api_version="v4.14"):
+    def interfaces_query(self, data, tenant_id=None, api_version="v4.15"):
         """
-        Queries db for limit number of interfaces that match query params. (v4.14)
+        Queries db for limit number of interfaces that match query params. (v4.15)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v4.14)
+          - **api_version**: API version to use (default v4.15)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -3596,24 +3748,24 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ipsecprofiles/query".format(api_version,
                                                                               tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def lannetworks(self, site_id, data, tenant_id=None, api_version="v3.1"):
+    def lannetworks(self, site_id, data, tenant_id=None, api_version="v3.2"):
         """
-        Create a new LAN (v3.1)
+        Create a new LAN (v3.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_config:**           
                - **default_routers:**  [Type: string] 
                - **dhcp_relay:**           
@@ -3645,14 +3797,17 @@
                    - **static_mappings:**           
                        - **ip_address:**  Type: string 
                        - **mac:**  Type: string 
                        - **name:**  Type: string 
                    - **subnet:**  Type: string 
                    - **tags:**  [Type: string] 
                - **prefixes:**  [Type: string] 
+           - **ipv6_config:**           
+               - **default_routers:**  [Type: string] 
+               - **prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **network_context_id:**  Type: string 
            - **scope:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
@@ -3668,23 +3823,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/lannetworks".format(api_version,
                                                                                tenant_id,
                                                                                site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def lannetworks_query(self, data, tenant_id=None, api_version="v3.1"):
+    def lannetworks_query(self, data, tenant_id=None, api_version="v3.2"):
         """
-        Query db for Site LAN networks that match query parameters (v3.1)
+        Query db for Site LAN networks that match query parameters (v3.2)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -4018,14 +4173,44 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aggregates".format(api_version,
                                                                              tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
+    def monitor_aggregates_application_qos(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Monitor_Aggregates_Application_Qos API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aggregates/application/qos".format(api_version,
+                                                                                             tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def monitor_aggregates_healthscore(self, data, tenant_id=None, api_version="v2.0"):
         """
         POST Monitor_Aggregates_Healthscore API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -4138,14 +4323,44 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/aggregates".format(api_version,
                                                                                    tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
+    def monitor_aiops_anomaly(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Monitor_Aiops_Anomaly API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/anomaly".format(api_version,
+                                                                                tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def monitor_aiops_forecast(self, data, tenant_id=None, api_version="v2.1"):
         """
         POST Monitor_Aiops_Forecast API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -4258,14 +4473,74 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/aiops/topn".format(api_version,
                                                                              tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
+    def monitor_application_qos_metrics(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Monitor_Application_Qos_Metrics API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/application/qos_metrics".format(api_version,
+                                                                                          tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def monitor_application_users(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Monitor_Application_Users API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.cdl_url
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/application/users".format(api_version,
+                                                                                    tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def monitor_bulk_metrics(self, data, tenant_id=None, api_version="v2.0"):
         """
         POST Monitor_Bulk_Metrics API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -4348,23 +4623,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/cellular_metrics/topn".format(api_version,
                                                                                         tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def monitor_flows(self, data, tenant_id=None, api_version="v3.6"):
+    def monitor_flows(self, data, tenant_id=None, api_version="v3.7"):
         """
         POST Monitor_Flows API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.6)
+          - **api_version**: API version to use (default v3.7)
 
           **Payload Attributes:** 
 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
@@ -4588,23 +4863,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/network_point_metrics_hs".format(api_version,
                                                                                            tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def monitor_object_stats(self, data, tenant_id=None, api_version="v2.4"):
+    def monitor_object_stats(self, data, tenant_id=None, api_version="v2.5"):
         """
         POST Monitor_Object_Stats API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
@@ -4648,23 +4923,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/qos_metrics".format(api_version,
                                                                               tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def monitor_sys_metrics(self, data, tenant_id=None, api_version="v2.2"):
+    def monitor_sys_metrics(self, data, tenant_id=None, api_version="v2.3"):
         """
         POST Monitor_Sys_Metrics API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.2)
+          - **api_version**: API version to use (default v2.3)
 
           **Payload Attributes:** 
 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
@@ -5510,14 +5785,15 @@
            - **destination_ports:**           
                - **from:**  Type: integer 
                - **to:**  Type: integer 
            - **destination_prefixes:**           
                - **description:**  Type: string 
                - **id:**  Type: string 
                - **ipv4_prefixes:**  [Type: string] 
+               - **ipv6_prefixes:**  [Type: string] 
                - **name:**  Type: string 
                - **tags:**  [Type: string] 
            - **destination_prefixes_id:**  Type: string 
            - **destination_zone:**           
                - **default_for_public_interfaces:**  Type: boolean 
                - **description:**  Type: string 
                - **disabled:**  Type: boolean 
@@ -5547,14 +5823,15 @@
            - **source_ports:**           
                - **from:**  Type: integer 
                - **to:**  Type: integer 
            - **source_prefixes:**           
                - **description:**  Type: string 
                - **id:**  Type: string 
                - **ipv4_prefixes:**  [Type: string] 
+               - **ipv6_prefixes:**  [Type: string] 
                - **name:**  Type: string 
                - **tags:**  [Type: string] 
            - **source_prefixes_id:**  Type: string 
            - **source_zone:**           
                - **default_for_public_interfaces:**  Type: boolean 
                - **description:**  Type: string 
                - **disabled:**  Type: boolean 
@@ -5663,14 +5940,15 @@
                - **destination_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
                - **destination_prefixes:**           
                    - **description:**  Type: string 
                    - **id:**  Type: string 
                    - **ipv4_prefixes:**  [Type: string] 
+                   - **ipv6_prefixes:**  [Type: string] 
                    - **name:**  Type: string 
                    - **tags:**  [Type: string] 
                - **destination_prefixes_id:**  Type: string 
                - **destination_zone:**           
                    - **default_for_public_interfaces:**  Type: boolean 
                    - **description:**  Type: string 
                    - **disabled:**  Type: boolean 
@@ -5701,14 +5979,15 @@
                - **source_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
                - **source_prefixes:**           
                    - **description:**  Type: string 
                    - **id:**  Type: string 
                    - **ipv4_prefixes:**  [Type: string] 
+                   - **ipv6_prefixes:**  [Type: string] 
                    - **name:**  Type: string 
                    - **tags:**  [Type: string] 
                - **source_prefixes_id:**  Type: string 
                - **source_zone:**           
                    - **default_for_public_interfaces:**  Type: boolean 
                    - **description:**  Type: string 
                    - **disabled:**  Type: boolean 
@@ -6006,28 +6285,29 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkcontexts/query".format(api_version,
                                                                                 tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def networkpolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.0"):
+    def networkpolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Create a new global prefix. (v2.0)
+        Create a new global prefix. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -6040,23 +6320,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicyglobalprefixes".format(api_version,
                                                                                       tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def networkpolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def networkpolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query Network Global Prefixes. (v2.0)
+        Query Network Global Prefixes. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -6084,23 +6364,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicyglobalprefixes/query".format(api_version,
                                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def networkpolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def networkpolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query site network prefix association. (v2.0)
+        Query site network prefix association. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -6128,24 +6408,24 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicylocalprefixes/query".format(api_version,
                                                                                            tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def networkpolicyrules(self, networkpolicyset_id, data, tenant_id=None, api_version="v2.1"):
+    def networkpolicyrules(self, networkpolicyset_id, data, tenant_id=None, api_version="v2.2"):
         """
-        Create a new NetworkPolicyRule (v2.1)
+        Create a new NetworkPolicyRule (v2.2)
 
           **Parameters:**:
 
           - **networkpolicyset_id**: Network Policy Set ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefixes_id:**  Type: string 
            - **enabled:**  Type: boolean 
@@ -6166,14 +6446,17 @@
                - **active_service_label_id:**  Type: string 
                - **active_service_label_type:**  Type: string 
                - **backup_service_label_id:**  Type: string 
                - **backup_service_label_type:**  Type: string 
                - **type:**  Type: string 
            - **source_prefixes_id:**  Type: string 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -6185,23 +6468,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicysets/{}/networkpolicyrules".format(api_version,
                                                                                                   tenant_id,
                                                                                                   networkpolicyset_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def networkpolicyrules_query(self, data, tenant_id=None, api_version="v2.1"):
+    def networkpolicyrules_query(self, data, tenant_id=None, api_version="v2.2"):
         """
-        Query Network policy rules. (v2.1)
+        Query Network policy rules. (v2.2)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefixes_id:**  Type: string 
            - **enabled:**  Type: boolean 
@@ -6223,14 +6506,17 @@
                - **active_service_label_id:**  Type: string 
                - **active_service_label_type:**  Type: string 
                - **backup_service_label_id:**  Type: string 
                - **backup_service_label_type:**  Type: string 
                - **type:**  Type: string 
            - **source_prefixes_id:**  Type: string 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -6544,28 +6830,29 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networks/bulk_config_state/query".format(api_version,
                                                                                            tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def ngfwsecuritypolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Create an Security Policy V2 Global Prefix (v2.0)
+        Create an Security Policy V2 Global Prefix (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -6578,28 +6865,29 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicyglobalprefixes".format(api_version,
                                                                                            tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def ngfwsecuritypolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query Security Policy V2 Global Prefixes of a tenant (v2.0)
+        Query Security Policy V2 Global Prefixes of a tenant (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -6645,23 +6933,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicylocalprefixes".format(api_version,
                                                                                           tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def ngfwsecuritypolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query security policy v2 local prefix site associations of a tenant (v2.0)
+        Query security policy v2 local prefix site associations of a tenant (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -6689,24 +6977,24 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicylocalprefixes/query".format(api_version,
                                                                                                 tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Create a Security Policy V2 Rule under a policy set (v2.0)
+        Create a Security Policy V2 Rule under a policy set (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyset_id**: NGFW Security Policy Set ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **action:**  Type: string 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefix_ids:**  [Type: string] 
@@ -6720,14 +7008,17 @@
                - **protocol:**  Type: integer 
                - **source_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
            - **source_prefix_ids:**  [Type: string] 
            - **source_zone_ids:**  [Type: string] 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -6739,45 +7030,47 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicysets/{}/ngfwsecuritypolicyrules".format(api_version,
                                                                                                             tenant_id,
                                                                                                             ngfwsecuritypolicyset_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def ngfwsecuritypolicyrules_query(self, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyrules_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query security policy v2 rules of a tenant (v2.0)
+        Query security policy v2 rules of a tenant (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **action:**  Type: string 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefix_ids:**  [Type: string] 
            - **destination_zone_ids:**  [Type: string] 
            - **enabled:**  Type: boolean 
            - **name:**  Type: string 
-           - **policyset_id:**  Type: string 
            - **services:**           
                - **destination_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
                - **protocol:**  Type: integer 
                - **source_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
            - **source_prefix_ids:**  [Type: string] 
            - **source_zone_ids:**  [Type: string] 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -7427,28 +7720,29 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/prefixfilters/query".format(api_version,
                                                                                        tenant_id,
                                                                                        site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def prioritypolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyglobalprefixes(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Create a new global prefix. (v2.0)
+        Create a new global prefix. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -7461,23 +7755,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicyglobalprefixes".format(api_version,
                                                                                        tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def prioritypolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyglobalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query Priority Global Prefixes. (v2.0)
+        Query Priority Global Prefixes. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -7505,23 +7799,23 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicyglobalprefixes/query".format(api_version,
                                                                                              tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def prioritypolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicylocalprefixes_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query site priority prefix association. (v2.0)
+        Query site priority prefix association. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -7549,24 +7843,24 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicylocalprefixes/query".format(api_version,
                                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def prioritypolicyrules(self, prioritypolicyset_id, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyrules(self, prioritypolicyset_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Create a new PriorityPolicyRule (v2.0)
+        Create a new PriorityPolicyRule (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyset_id**: Priority Policy Set ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefixes_id:**  Type: string 
            - **dscp:**           
@@ -7574,14 +7868,17 @@
            - **enabled:**  Type: boolean 
            - **name:**  Type: string 
            - **network_context_id:**  Type: string 
            - **order_number:**  Type: integer 
            - **priority_number:**  Type: integer 
            - **source_prefixes_id:**  Type: string 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -7593,23 +7890,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicysets/{}/prioritypolicyrules".format(api_version,
                                                                                                     tenant_id,
                                                                                                     prioritypolicyset_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def prioritypolicyrules_query(self, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyrules_query(self, data, tenant_id=None, api_version="v2.1"):
         """
-        Query Priority policy rules. (v2.0)
+        Query Priority policy rules. (v2.1)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -9376,24 +9673,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/ipfixlocalprefixes".format(api_version,
                                                                                       tenant_id,
                                                                                       site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def site_lannetworks_query(self, site_id, data, tenant_id=None, api_version="v3.1"):
+    def site_lannetworks_query(self, site_id, data, tenant_id=None, api_version="v3.2"):
         """
-        Query LAN networks that match query params (v3.1)
+        Query LAN networks that match query params (v3.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -9457,28 +9754,29 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/natlocalprefixes".format(api_version,
                                                                                     tenant_id,
                                                                                     site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def site_networkpolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.0"):
+    def site_networkpolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Create an association between site and Network local Prefix. (v2.0)
+        Create an association between site and Network local Prefix. (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -9492,28 +9790,29 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/networkpolicylocalprefixes".format(api_version,
                                                                                               tenant_id,
                                                                                               site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def site_ngfwsecuritypolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.0"):
+    def site_ngfwsecuritypolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Create a security policy V2 local prefix site association (v2.0)
+        Create a security policy V2 local prefix site association (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -9527,28 +9826,29 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/ngfwsecuritypolicylocalprefixes".format(api_version,
                                                                                                    tenant_id,
                                                                                                    site_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def site_prioritypolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.0"):
+    def site_prioritypolicylocalprefixes(self, site_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Create an association between site and Priority local Prefix. (v2.0)
+        Create an association between site and Priority local Prefix. (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -10251,23 +10551,23 @@
                                                                                             tenant_id,
                                                                                             site_id,
                                                                                             element_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
-    def status_query(self, data, tenant_id=None, api_version="v2.1"):
+    def status_query(self, data, tenant_id=None, api_version="v2.2"):
         """
-        Query and get element status objects for a tenant (v2.1)
+        Query and get element status objects for a tenant (v2.2)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
            - **aggregate:**           
                - **field:**  Type: string 
                - **operator:**  Type: string 
            - **dest_page:**  Type: integer 
@@ -10974,14 +11274,74 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/upgrade_status/query".format(api_version,
                                                                                tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
+    def useridagents(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Useridagents API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents".format(api_version,
+                                                                       tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def useridagents_query(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Useridagents_Query API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents/query".format(api_version,
+                                                                             tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def users(self, data, tenant_id=None, api_version="v2.0"):
         """
         Create an user identity. (v2.0)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -11665,14 +12025,17 @@
 
     aggregates_aiops_monitor = monitor_aiops_aggregates
     """ Backwards-compatibility alias of `aggregates_aiops_monitor` to `monitor_aiops_aggregates`"""
 
     aggregates_monitor = monitor_aggregates
     """ Backwards-compatibility alias of `aggregates_monitor` to `monitor_aggregates`"""
 
+    anomaly_aiops_monitor = monitor_aiops_anomaly
+    """ Backwards-compatibility alias of `anomaly_aiops_monitor` to `monitor_aiops_anomaly`"""
+
     anynetlinks_t = tenant_anynetlinks
     """ Backwards-compatibility alias of `anynetlinks_t` to `tenant_anynetlinks`"""
 
     bulk_metrics_monitor = monitor_bulk_metrics
     """ Backwards-compatibility alias of `bulk_metrics_monitor` to `monitor_bulk_metrics`"""
 
     cellular_metrics_monitor = monitor_cellular_metrics
@@ -11800,17 +12163,26 @@
 
     prioritypolicylocalprefixes_s = site_prioritypolicylocalprefixes
     """ Backwards-compatibility alias of `prioritypolicylocalprefixes_s` to `site_prioritypolicylocalprefixes`"""
 
     prioritypolicylocalprefixes_t = tenant_prioritypolicylocalprefixes
     """ Backwards-compatibility alias of `prioritypolicylocalprefixes_t` to `tenant_prioritypolicylocalprefixes`"""
 
+    qos_application_aggregates_monitor = monitor_aggregates_application_qos
+    """ Backwards-compatibility alias of `qos_application_aggregates_monitor` to `monitor_aggregates_application_qos`"""
+
+    qos_metrics_application_monitor = monitor_application_qos_metrics
+    """ Backwards-compatibility alias of `qos_metrics_application_monitor` to `monitor_application_qos_metrics`"""
+
     qos_metrics_monitor = monitor_qos_metrics
     """ Backwards-compatibility alias of `qos_metrics_monitor` to `monitor_qos_metrics`"""
 
+    query_activeuserips = activeuserips_query
+    """ Backwards-compatibility alias of `query_activeuserips` to `activeuserips_query`"""
+
     query_apnprofiles = apnprofiles_query
     """ Backwards-compatibility alias of `query_apnprofiles` to `apnprofiles_query`"""
 
     query_appdefs = appdefs_query
     """ Backwards-compatibility alias of `query_appdefs` to `appdefs_query`"""
 
     query_auditlog = auditlog_query
@@ -11857,14 +12229,20 @@
 
     query_current_status_software = software_current_status_query
     """ Backwards-compatibility alias of `query_current_status_software` to `software_current_status_query`"""
 
     query_demstatus = demstatus_query
     """ Backwards-compatibility alias of `query_demstatus` to `demstatus_query`"""
 
+    query_directoryusergroups = directoryusergroups_query
+    """ Backwards-compatibility alias of `query_directoryusergroups` to `directoryusergroups_query`"""
+
+    query_directoryusers = directoryusers_query
+    """ Backwards-compatibility alias of `query_directoryusers` to `directoryusers_query`"""
+
     query_dnsserviceprofiles = dnsserviceprofiles_query
     """ Backwards-compatibility alias of `query_dnsserviceprofiles` to `dnsserviceprofiles_query`"""
 
     query_dnsserviceroles = dnsserviceroles_query
     """ Backwards-compatibility alias of `query_dnsserviceroles` to `dnsserviceroles_query`"""
 
     query_dnsservices = dnsservices_query
@@ -12133,14 +12511,17 @@
 
     query_toolkitsessions = toolkitsessions_query
     """ Backwards-compatibility alias of `query_toolkitsessions` to `toolkitsessions_query`"""
 
     query_upgrade_status = upgrade_status_query
     """ Backwards-compatibility alias of `query_upgrade_status` to `upgrade_status_query`"""
 
+    query_useridagents = useridagents_query
+    """ Backwards-compatibility alias of `query_useridagents` to `useridagents_query`"""
+
     query_vpnlinks = vpnlinks_query
     """ Backwards-compatibility alias of `query_vpnlinks` to `vpnlinks_query`"""
 
     query_waninterfacelabels = waninterfacelabels_query
     """ Backwards-compatibility alias of `query_waninterfacelabels` to `waninterfacelabels_query`"""
 
     query_waninterfaces = waninterfaces_query
@@ -12184,14 +12565,17 @@
 
     topn_monitor = monitor_topn
     """ Backwards-compatibility alias of `topn_monitor` to `monitor_topn`"""
 
     topn_sys_metrics_monitor = monitor_sys_metrics_topn
     """ Backwards-compatibility alias of `topn_sys_metrics_monitor` to `monitor_sys_metrics_topn`"""
 
+    users_application_monitor = monitor_application_users
+    """ Backwards-compatibility alias of `users_application_monitor` to `monitor_application_users`"""
+
     wan_neighbor_multicast_aggregates_monitor = monitor_aggregates_multicast_wan_neighbor
     """ Backwards-compatibility alias of `wan_neighbor_multicast_aggregates_monitor` to `monitor_aggregates_multicast_wan_neighbor`"""
 
     elements_bulk_config_state_query = element_bulk_config_state_query
     """ Backwards-compatibility alias of `elements_bulk_config_state_query` to `element_bulk_config_state_query`"""
 
     elements_query = element_query
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/put_api.py` & `cloudgenix-6.2.1b1/cloudgenix/put_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,24 +88,24 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/apnprofiles/{}".format(api_version,
                                                                          tenant_id,
                                                                          apnprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def appdefs(self, appdef_id, data, tenant_id=None, api_version="v2.4"):
+    def appdefs(self, appdef_id, data, tenant_id=None, api_version="v2.5"):
         """
-        Update a application definition (v2.4)
+        Update an application definition (v2.5)
 
           **Parameters:**:
 
           - **appdef_id**: Application Definition ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
            - **abbreviation:**  Type: string 
            - **aggregate_flows:**  Type: boolean 
            - **app_type:**  Type: string 
            - **app_unreachability_detection:**  Type: boolean 
@@ -454,28 +454,63 @@
                                                                                                           element_id,
                                                                                                           cellular_module_id,
                                                                                                           sim_security_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def dhcpservers(self, site_id, dhcpserver_id, data, tenant_id=None, api_version="v2.1"):
+    def deviceidconfigs(self, site_id, deviceidconfig_id, data, tenant_id=None, api_version="v2.0"):
         """
-        Update an existing dhcp server configuration for a subnet (v2.1)
+        PUT Deviceidconfigs API Function
+
+          **Parameters:**:
+
+          - **site_id**: Site ID
+          - **deviceidconfig_id**: Device Id Config ID
+          - **data**: Dictionary containing data to PUT as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/sites/{}/deviceidconfigs/{}".format(api_version,
+                                                                                      tenant_id,
+                                                                                      site_id,
+                                                                                      deviceidconfig_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "put", data=data)
+
+    def dhcpservers(self, site_id, dhcpserver_id, data, tenant_id=None, api_version="v2.2"):
+        """
+        Update an existing dhcp server configuration for a subnet (v2.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **dhcpserver_id**: DHCP Server ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
+           - **address_family:**  Type: string 
            - **broadcast_address:**  Type: string 
            - **custom_options:**           
                - **option_definition:**  Type: string 
                - **option_value:**  Type: string 
                - **vendor_class_identifier:**  Type: string 
            - **default_lease_time:**  Type: integer 
            - **description:**  Type: string 
@@ -485,14 +520,15 @@
            - **gateway:**  Type: string 
            - **ip_ranges:**           
                - **end_ip:**  Type: string 
                - **start_ip:**  Type: string 
            - **max_lease_time:**  Type: integer 
            - **network_context_id:**  Type: string 
            - **static_mappings:**           
+               - **client_duid:**  Type: string 
                - **ip_address:**  Type: string 
                - **mac:**  Type: string 
                - **name:**  Type: string 
            - **subnet:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
@@ -510,27 +546,59 @@
                                                                                   tenant_id,
                                                                                   site_id,
                                                                                   dhcpserver_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def dnsserviceprofiles(self, dnsserviceprofile_id, data, tenant_id=None, api_version="v2.0"):
+    def directoryservices(self, directoryservice_id, data, tenant_id=None, api_version="v2.0"):
         """
-        Update a DNS service profile (v2.0)
+        PUT Directoryservices API Function
 
           **Parameters:**:
 
-          - **dnsserviceprofile_id**: DNS Service Profile ID
+          - **directoryservice_id**: Directory Service ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
           **Payload Attributes:** 
 
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/{}".format(api_version,
+                                                                               tenant_id,
+                                                                               directoryservice_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "put", data=data)
+
+    def dnsserviceprofiles(self, dnsserviceprofile_id, data, tenant_id=None, api_version="v2.1"):
+        """
+        Update a DNS service profile (v2.1)
+
+          **Parameters:**:
+
+          - **dnsserviceprofile_id**: DNS Service Profile ID
+          - **data**: Dictionary containing data to PUT as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.1)
+
+          **Payload Attributes:** 
+
            - **authoritative_config:**           
                - **caa_records:**           
                    - **flags:**  Type: string 
                    - **name:**  Type: string 
                    - **tag:**  Type: string 
                    - **value:**  Type: string 
                - **cname_records:**           
@@ -597,18 +665,17 @@
            - **cache_config:**           
                - **cache_size:**  Type: integer 
                - **disable_negative_caching:**  Type: boolean 
                - **max_cache_ttl:**  Type: integer 
                - **min_cache_ttl:**  Type: integer 
                - **negative_cache_ttl:**  Type: integer 
            - **description:**  Type: string 
-           - **disabled:**  Type: boolean 
-           - **disabled_reason:**  Type: string 
            - **dns_forward_config:**           
                - **dns_servers:**           
+                   - **address_family:**  Type: string 
                    - **dnsserver_ip:**  Type: string 
                    - **dnsserver_port:**  Type: integer 
                    - **domain_names:**  [Type: string] 
                    - **forward_dnsservicerole_id:**  Type: string 
                    - **ip_prefix:**  Type: string 
                    - **source_port:**  Type: integer 
                - **max_source_port:**  Type: integer 
@@ -657,22 +724,18 @@
                - **domain_names:**  [Type: string] 
                - **ipv4_address:**  Type: string 
                - **ipv6_address:**  Type: string 
            - **edns_packet_max:**  Type: integer 
            - **enable_dns_loop_detection:**  Type: boolean 
            - **enable_dnssec_proxy:**  Type: boolean 
            - **enable_strict_domain_name:**  Type: boolean 
-           - **inactive:**  Type: boolean 
-           - **inactive_reason:**  Type: string 
            - **listen_dnsservicerole_id:**  Type: string 
            - **listen_port:**  Type: integer 
            - **name:**  Type: string 
-           - **region:**  Type: string 
            - **tags:**  [Type: string] 
-           - **tenant_id:**  Type: string 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -727,15 +790,15 @@
         """
         Update a DNS service config (v2.0)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
-          - **dnsservice_id**: DNS Service ID 
+          - **dnsservice_id**: DNS Service ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.0)
 
           **Payload Attributes:** 
 
            - **cache_config:**           
@@ -1228,23 +1291,23 @@
                                                                                     tenant_id,
                                                                                     elementuser_id,
                                                                                     access_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def enterpriseprefixset(self, data, tenant_id=None, api_version="v2.0"):
+    def enterpriseprefixset(self, data, tenant_id=None, api_version="v2.1"):
         """
         PUT Enterpriseprefixset API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
@@ -1670,34 +1733,35 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/idps/{}".format(api_version,
                                                                   tenant_id,
                                                                   idp_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def interfaces(self, site_id, element_id, interface_id, data, tenant_id=None, api_version="v4.14"):
+    def interfaces(self, site_id, element_id, interface_id, data, tenant_id=None, api_version="v4.15"):
         """
-        Update a Cellular Interface (v4.14)
+        Update a Cellular Interface (v4.15)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **element_id**: Element (Device) ID
           - **interface_id**: Interface ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v4.14)
+          - **api_version**: API version to use (default v4.15)
 
           **Payload Attributes:** 
 
            - **admin_up:**  Type: boolean 
            - **attached_lan_networks:**           
                - **lan_network_id:**  Type: string 
                - **vlan_id:**  Type: integer 
            - **authentication_config:**           
+               - **fallback_retry_count:**  Type: integer 
                - **mode:**  Type: string 
                - **reauthentication_timeout:**  Type: integer 
            - **bound_interfaces:**  [Type: string] 
            - **bypass_pair:**           
                - **lan:**  Type: string 
                - **lan_state_propagation:**  Type: boolean 
                - **use_relay:**  Type: boolean 
@@ -1774,14 +1838,15 @@
                    - **name_servers:**  [Type: string] 
                    - **search:**  [Type: string] 
                - **routes:**           
                    - **destination:**  Type: string 
                    - **via:**  Type: string 
                - **static_config:**           
                    - **address:**  Type: string 
+                   - **enable_prefix_distribution:**  Type: boolean 
                - **type:**  Type: string 
            - **lldp_enabled:**  Type: boolean 
            - **mac_address:**  Type: string 
            - **mtu:**  Type: integer 
            - **multicast_config:**           
                - **igmp_version:**  Type: string 
                - **multicast_enabled:**  Type: boolean 
@@ -1794,14 +1859,15 @@
                    - **start:**  Type: string 
                - **nat_pool_id:**  Type: string 
            - **nat_port:**  Type: integer 
            - **nat_port_v6:**  Type: integer 
            - **nat_zone_id:**  Type: string 
            - **network_context_id:**  Type: string 
            - **parent:**  Type: string 
+           - **peer_bypasspair_wan_port_type:**  Type: string 
            - **poe_enabled:**  Type: boolean 
            - **power_usage_threshold:**  Type: integer 
            - **pppoe_config:**           
                - **host_uniq:**  Type: string 
                - **ip_address_type:**  Type: string 
                - **password:**  Type: string 
                - **reconnection_delay:**  Type: integer 
@@ -2268,25 +2334,25 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ipsecprofiles/{}".format(api_version,
                                                                            tenant_id,
                                                                            ipsecprofile_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def lannetworks(self, site_id, lannetwork_id, data, tenant_id=None, api_version="v3.1"):
+    def lannetworks(self, site_id, lannetwork_id, data, tenant_id=None, api_version="v3.2"):
         """
-        Update an existing LAN (v3.1)
+        Update an existing LAN (v3.2)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **lannetwork_id**: LAN Network ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v3.1)
+          - **api_version**: API version to use (default v3.2)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_config:**           
                - **default_routers:**  [Type: string] 
                - **dhcp_relay:**           
@@ -2318,14 +2384,17 @@
                    - **static_mappings:**           
                        - **ip_address:**  Type: string 
                        - **mac:**  Type: string 
                        - **name:**  Type: string 
                    - **subnet:**  Type: string 
                    - **tags:**  [Type: string] 
                - **prefixes:**  [Type: string] 
+           - **ipv6_config:**           
+               - **default_routers:**  [Type: string] 
+               - **prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **network_context_id:**  Type: string 
            - **scope:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
@@ -2751,14 +2820,15 @@
            - **destination_ports:**           
                - **from:**  Type: integer 
                - **to:**  Type: integer 
            - **destination_prefixes:**           
                - **description:**  Type: string 
                - **id:**  Type: string 
                - **ipv4_prefixes:**  [Type: string] 
+               - **ipv6_prefixes:**  [Type: string] 
                - **name:**  Type: string 
                - **tags:**  [Type: string] 
            - **destination_prefixes_id:**  Type: string 
            - **destination_zone:**           
                - **default_for_public_interfaces:**  Type: boolean 
                - **description:**  Type: string 
                - **disabled:**  Type: boolean 
@@ -2788,14 +2858,15 @@
            - **source_ports:**           
                - **from:**  Type: integer 
                - **to:**  Type: integer 
            - **source_prefixes:**           
                - **description:**  Type: string 
                - **id:**  Type: string 
                - **ipv4_prefixes:**  [Type: string] 
+               - **ipv6_prefixes:**  [Type: string] 
                - **name:**  Type: string 
                - **tags:**  [Type: string] 
            - **source_prefixes_id:**  Type: string 
            - **source_zone:**           
                - **default_for_public_interfaces:**  Type: boolean 
                - **description:**  Type: string 
                - **disabled:**  Type: boolean 
@@ -2862,14 +2933,15 @@
                - **destination_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
                - **destination_prefixes:**           
                    - **description:**  Type: string 
                    - **id:**  Type: string 
                    - **ipv4_prefixes:**  [Type: string] 
+                   - **ipv6_prefixes:**  [Type: string] 
                    - **name:**  Type: string 
                    - **tags:**  [Type: string] 
                - **destination_prefixes_id:**  Type: string 
                - **destination_zone:**           
                    - **default_for_public_interfaces:**  Type: boolean 
                    - **description:**  Type: string 
                    - **disabled:**  Type: boolean 
@@ -2900,14 +2972,15 @@
                - **source_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
                - **source_prefixes:**           
                    - **description:**  Type: string 
                    - **id:**  Type: string 
                    - **ipv4_prefixes:**  [Type: string] 
+                   - **ipv6_prefixes:**  [Type: string] 
                    - **name:**  Type: string 
                    - **tags:**  [Type: string] 
                - **source_prefixes_id:**  Type: string 
                - **source_zone:**           
                    - **default_for_public_interfaces:**  Type: boolean 
                    - **description:**  Type: string 
                    - **disabled:**  Type: boolean 
@@ -3056,29 +3129,30 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkcontexts/{}".format(api_version,
                                                                              tenant_id,
                                                                              networkcontext_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def networkpolicyglobalprefixes(self, networkpolicyglobalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update a Network global prefix. (v2.0)
+        Update a Network global prefix. (v2.1)
 
           **Parameters:**:
 
           - **networkpolicyglobalprefix_id**: Network Policy Global Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -3092,25 +3166,25 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicyglobalprefixes/{}".format(api_version,
                                                                                          tenant_id,
                                                                                          networkpolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id, data, tenant_id=None, api_version="v2.1"):
+    def networkpolicyrules(self, networkpolicyset_id, networkpolicyrule_id, data, tenant_id=None, api_version="v2.2"):
         """
-        Update network policy rule of tenant. (v2.1)
+        Update network policy rule of tenant. (v2.2)
 
           **Parameters:**:
 
           - **networkpolicyset_id**: Network Policy Set ID
           - **networkpolicyrule_id**: Network Policy Rule ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.1)
+          - **api_version**: API version to use (default v2.2)
 
           **Payload Attributes:** 
 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefixes_id:**  Type: string 
            - **enabled:**  Type: boolean 
@@ -3131,14 +3205,17 @@
                - **active_service_label_id:**  Type: string 
                - **active_service_label_type:**  Type: string 
                - **backup_service_label_id:**  Type: string 
                - **backup_service_label_type:**  Type: string 
                - **type:**  Type: string 
            - **source_prefixes_id:**  Type: string 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3335,29 +3412,30 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/networkpolicysetstacks/{}".format(api_version,
                                                                                     tenant_id,
                                                                                     networkpolicysetstack_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyglobalprefixes(self, ngfwsecuritypolicyglobalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update an existing Security Policy V2 Global Prefix (v2.0)
+        Update an existing Security Policy V2 Global Prefix (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyglobalprefix_id**: NGFW Security Policy Global Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -3406,25 +3484,25 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/ngfwsecuritypolicylocalprefixes/{}".format(api_version,
                                                                                              tenant_id,
                                                                                              ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id, data, tenant_id=None, api_version="v2.0"):
+    def ngfwsecuritypolicyrules(self, ngfwsecuritypolicyset_id, ngfwsecuritypolicyrule_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update an existing Security Policy V2 Rule under a policy set (v2.0)
+        Update an existing Security Policy V2 Rule under a policy set (v2.1)
 
           **Parameters:**:
 
           - **ngfwsecuritypolicyset_id**: NGFW Security Policy Set ID
           - **ngfwsecuritypolicyrule_id**: NGFW Security Policy Rule ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **action:**  Type: string 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefix_ids:**  [Type: string] 
@@ -3438,14 +3516,17 @@
                - **protocol:**  Type: integer 
                - **source_ports:**           
                    - **from:**  Type: integer 
                    - **to:**  Type: integer 
            - **source_prefix_ids:**  [Type: string] 
            - **source_zone_ids:**  [Type: string] 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -3789,29 +3870,30 @@
                                                                                     tenant_id,
                                                                                     site_id,
                                                                                     prefixfilter_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyglobalprefixes(self, prioritypolicyglobalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update a  Priority global prefix. (v2.0)
+        Update a  Priority global prefix. (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyglobalprefix_id**: Priority Policy Global Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **description:**  Type: string 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **name:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -3825,25 +3907,25 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicyglobalprefixes/{}".format(api_version,
                                                                                           tenant_id,
                                                                                           prioritypolicyglobalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id, data, tenant_id=None, api_version="v2.0"):
+    def prioritypolicyrules(self, prioritypolicyset_id, prioritypolicyrule_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update priority policy rule of tenant. (v2.0)
+        Update priority policy rule of tenant. (v2.1)
 
           **Parameters:**:
 
           - **prioritypolicyset_id**: Priority Policy Set ID
           - **prioritypolicyrule_id**: Priority Policy Rule ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **app_def_ids:**  [Type: string] 
            - **description:**  Type: string 
            - **destination_prefixes_id:**  Type: string 
            - **dscp:**           
@@ -3851,14 +3933,17 @@
            - **enabled:**  Type: boolean 
            - **name:**  Type: string 
            - **network_context_id:**  Type: string 
            - **order_number:**  Type: integer 
            - **priority_number:**  Type: integer 
            - **source_prefixes_id:**  Type: string 
            - **tags:**  [Type: string] 
+           - **user_or_group:**           
+               - **user_group_ids:**  [Type: string] 
+               - **user_ids:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -4792,29 +4877,30 @@
                                                                                        tenant_id,
                                                                                        site_id,
                                                                                        natlocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def site_networkpolicylocalprefixes(self, site_id, networkpolicylocalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update an existing Site Network policy local prefix (v2.0)
+        Update an existing Site Network policy local prefix (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **networkpolicylocalprefix_id**: Network Policy Local Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -4829,29 +4915,30 @@
                                                                                                  tenant_id,
                                                                                                  site_id,
                                                                                                  networkpolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def site_ngfwsecuritypolicylocalprefixes(self, site_id, ngfwsecuritypolicylocalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update an existing security policy V2 local prefix site association (v2.0)
+        Update an existing security policy V2 local prefix site association (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **ngfwsecuritypolicylocalprefix_id**: NGFW Security Policy Local Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -4866,29 +4953,30 @@
                                                                                                       tenant_id,
                                                                                                       site_id,
                                                                                                       ngfwsecuritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id, data, tenant_id=None, api_version="v2.0"):
+    def site_prioritypolicylocalprefixes(self, site_id, prioritypolicylocalprefix_id, data, tenant_id=None, api_version="v2.1"):
         """
-        Update an existing Site Priority policy local prefix (v2.0)
+        Update an existing Site Priority policy local prefix (v2.1)
 
           **Parameters:**:
 
           - **site_id**: Site ID
           - **prioritypolicylocalprefix_id**: Priority Policy Local Prefix ID
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
+          - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **ipv4_prefixes:**  [Type: string] 
+           - **ipv6_prefixes:**  [Type: string] 
            - **prefix_id:**  Type: string 
            - **tags:**  [Type: string] 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
@@ -5729,23 +5817,23 @@
         url = str(cur_ctlr) + "/{}/api/tenants/{}/prioritypolicylocalprefixes/{}".format(api_version,
                                                                                          tenant_id,
                                                                                          prioritypolicylocalprefix_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
-    def tenants(self, data, tenant_id=None, api_version="v2.4"):
+    def tenants(self, data, tenant_id=None, api_version="v2.5"):
         """
-        Update tenant (v2.4)
+        Update tenant (v2.5)
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to PUT as JSON
           - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.4)
+          - **api_version**: API version to use (default v2.5)
 
           **Payload Attributes:** 
 
            - **address:**           
                - **city:**  Type: string 
                - **country:**  Type: string 
                - **post_code:**  Type: string 
@@ -5759,14 +5847,15 @@
            - **disabled:**  Type: string 
            - **disabled_reason:**  Type: string 
            - **inactive:**  Type: string 
            - **inactive_reason:**  Type: string 
            - **ipv4_list:**           
                - **ipv4:**  Type: string 
            - **is_esp:**  Type: boolean 
+           - **is_pa_iot_security_license:**  Type: boolean 
            - **is_support:**  Type: boolean 
            - **name:**  Type: string 
            - **operator:**           
                - **addresses:**           
                    - **city:**  Type: string 
                    - **country:**  Type: string 
                    - **post_code:**  Type: string 
@@ -5916,16 +6005,22 @@
                    - **protocol:**           
                    - **region:**  Type: string 
                    - **template:**  Type: string 
                    - **tenant_id:**  Type: string 
                - **salt:**  Type: string 
                - **security:**  Type: string 
            - **region:**  Type: string 
+           - **sase_at:**  Type: string 
            - **telemetry_region:**  Type: string 
            - **tenant_id:**  Type: string 
+           - **tsg_id:**  Type: string 
+           - **tsg_instances:**           
+               - **app_id:**  Type: string 
+               - **region:**  Type: string 
+               - **tenant_id:**  Type: string 
 
         **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
         """
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
@@ -5936,14 +6031,46 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}".format(api_version,
                                                           tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "put", data=data)
 
+    def useridagents(self, useridagent_id, data, tenant_id=None, api_version="v2.0"):
+        """
+        PUT Useridagents API Function
+
+          **Parameters:**:
+
+          - **useridagent_id**: User Id Agent ID
+          - **data**: Dictionary containing data to PUT as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/useridagents/{}".format(api_version,
+                                                                          tenant_id,
+                                                                          useridagent_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "put", data=data)
+
     def users(self, user_id, data, tenant_id=None, api_version="v2.0"):
         """
         Put an user identity. (v2.0)
 
           **Parameters:**:
 
           - **user_id**: User ID
```

### Comparing `cloudgenix-6.1.2b1/cloudgenix/ws_api.py` & `cloudgenix-6.2.1b1/cloudgenix/ws_api.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.1.2b1/cloudgenix.egg-info/PKG-INFO` & `cloudgenix-6.2.1b1/cloudgenix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix
-Version: 6.1.2b1
+Version: 6.2.1b1
 Summary: Python2 and Python3 SDK for the CloudGenix AppFabric
 Home-page: https://github.com/CloudGenix/sdk-python
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.1.2b1
+# CloudGenix Python SDK v6.2.1b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
@@ -57,14 +57,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
 | **5.5.3** | **b1** | Support for June 2021 Controller release. |
```

### Comparing `cloudgenix-6.1.2b1/setup.py` & `cloudgenix-6.2.1b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='cloudgenix',
-      version='6.1.2b1',
+      version='6.2.1b1',
       description='Python2 and Python3 SDK for the CloudGenix AppFabric',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/CloudGenix/sdk-python',
       author='CloudGenix Developer Support',
       author_email='developers@cloudgenix.com',
       license='MIT',
```

