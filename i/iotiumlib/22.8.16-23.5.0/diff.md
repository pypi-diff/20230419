# Comparing `tmp/iotiumlib-22.8.16.tar.gz` & `tmp/iotiumlib-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotiumlib-22.8.16.tar", last modified: Tue Aug 16 17:16:20 2022, max compression
+gzip compressed data, was "iotiumlib-23.5.0.tar", last modified: Wed Apr 19 16:17:41 2023, max compression
```

## Comparing `iotiumlib-22.8.16.tar` & `iotiumlib-23.5.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-08-16 17:16:20.896609 iotiumlib-22.8.16/
--rw-rw-rw-   0        0        0        0 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/LICENSE
--rw-rw-rw-   0        0        0    15790 2022-08-16 17:16:20.893108 iotiumlib-22.8.16/PKG-INFO
--rw-rw-rw-   0        0        0    15386 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/README.md
-drwxrwxrwx   0        0        0        0 2022-08-16 17:16:20.654605 iotiumlib-22.8.16/iotiumlib/
--rw-rw-rw-   0        0        0     1076 2022-08-16 17:10:43.000000 iotiumlib-22.8.16/iotiumlib/__init__.py
--rw-rw-rw-   0        0        0     7398 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/cluster.py
--rw-rw-rw-   0        0        0     6674 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/download.py
--rw-rw-rw-   0        0        0     7414 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/firewall.py
--rw-rw-rw-   0        0        0     5465 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/helper.py
--rw-rw-rw-   0        0        0     2948 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/image.py
-drwxrwxrwx   0        0        0        0 2022-08-16 17:16:20.784197 iotiumlib-22.8.16/iotiumlib/models/
--rw-rw-rw-   0        0        0        0 2022-04-27 22:46:00.000000 iotiumlib-22.8.16/iotiumlib/models/__init__.py
--rw-rw-rw-   0        0        0    10440 2022-04-26 05:52:48.000000 iotiumlib-22.8.16/iotiumlib/models/service_listener_creation_vo.py
--rw-rw-rw-   0        0        0     7208 2022-04-26 05:52:48.000000 iotiumlib-22.8.16/iotiumlib/models/service_listener_update_vo.py
--rw-rw-rw-   0        0        0     6417 2022-04-26 05:52:48.000000 iotiumlib-22.8.16/iotiumlib/models/service_ports_vo.py
--rw-rw-rw-   0        0        0     3576 2022-04-26 05:52:48.000000 iotiumlib-22.8.16/iotiumlib/models/service_selector_vo.py
--rw-rw-rw-   0        0        0    16868 2022-08-16 11:29:12.000000 iotiumlib-22.8.16/iotiumlib/network.py
--rw-rw-rw-   0        0        0    11025 2022-08-16 11:29:12.000000 iotiumlib-22.8.16/iotiumlib/node.py
--rw-rw-rw-   0        0        0     3457 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/nodecli.py
--rw-rw-rw-   0        0        0      538 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/orch.py
--rw-rw-rw-   0        0        0     2605 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/orchlogin.py
--rw-rw-rw-   0        0        0     5038 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/org.py
--rw-rw-rw-   0        0        0     2514 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/pki.py
--rw-rw-rw-   0        0        0     2407 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/profile.py
-drwxrwxrwx   0        0        0        0 2022-08-16 17:16:20.876824 iotiumlib-22.8.16/iotiumlib/requires/
--rw-rw-rw-   0        0        0     1425 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/requires/Exceptions.py
--rw-rw-rw-   0        0        0       58 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/requires/__init__.py
--rw-rw-rw-   0        0        0      687 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/requires/commonVariables.py
--rw-rw-rw-   0        0        0     4802 2022-08-16 17:10:43.000000 iotiumlib-22.8.16/iotiumlib/requires/commonWrapper.py
--rw-rw-rw-   0        0        0       38 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/requires/constants.py
--rw-rw-rw-   0        0        0    67164 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/requires/resourcePayload.py
--rw-rw-rw-   0        0        0    24444 2022-06-10 17:41:59.000000 iotiumlib-22.8.16/iotiumlib/requires/utils.py
--rw-rw-rw-   0        0        0     4109 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/secret.py
--rw-rw-rw-   0        0        0    11742 2022-04-27 22:34:36.000000 iotiumlib-22.8.16/iotiumlib/service.py
--rw-rw-rw-   0        0        0     2918 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/sshkey.py
--rw-rw-rw-   0        0        0    15172 2022-03-28 06:43:21.000000 iotiumlib-22.8.16/iotiumlib/user.py
-drwxrwxrwx   0        0        0        0 2022-08-16 17:16:20.702954 iotiumlib-22.8.16/iotiumlib.egg-info/
--rw-rw-rw-   0        0        0    15790 2022-08-16 17:16:20.000000 iotiumlib-22.8.16/iotiumlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2022-08-16 17:16:20.000000 iotiumlib-22.8.16/iotiumlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-16 17:16:20.000000 iotiumlib-22.8.16/iotiumlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-08-16 17:16:20.000000 iotiumlib-22.8.16/iotiumlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-16 17:16:20.000000 iotiumlib-22.8.16/iotiumlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-16 17:16:20.896609 iotiumlib-22.8.16/setup.cfg
--rw-rw-rw-   0        0        0      672 2022-08-16 17:10:43.000000 iotiumlib-22.8.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.278106 iotiumlib-23.5.0/
+-rw-rw-rw-   0        0        0        0 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/LICENSE
+-rw-rw-rw-   0        0        0    15806 2023-04-19 16:17:41.264581 iotiumlib-23.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15386 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.225728 iotiumlib-23.5.0/iotiumlib/
+-rw-rw-rw-   0        0        0     1084 2023-04-18 16:17:48.000000 iotiumlib-23.5.0/iotiumlib/__init__.py
+-rw-rw-rw-   0        0        0     8141 2023-04-18 15:55:13.000000 iotiumlib-23.5.0/iotiumlib/cluster.py
+-rw-rw-rw-   0        0        0     6674 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/download.py
+-rw-rw-rw-   0        0        0     7414 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/firewall.py
+-rw-rw-rw-   0        0        0     5465 2022-11-18 11:01:08.000000 iotiumlib-23.5.0/iotiumlib/helper.py
+-rw-rw-rw-   0        0        0     2948 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/image.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.263385 iotiumlib-23.5.0/iotiumlib/models/
+-rw-rw-rw-   0        0        0        0 2022-08-19 08:13:17.000000 iotiumlib-23.5.0/iotiumlib/models/__init__.py
+-rw-rw-rw-   0        0        0     7779 2022-10-27 06:17:54.000000 iotiumlib-23.5.0/iotiumlib/models/role_creation_vo.py
+-rw-rw-rw-   0        0        0     6541 2022-10-27 06:18:04.000000 iotiumlib-23.5.0/iotiumlib/models/role_updation_vo.py
+-rw-rw-rw-   0        0        0    10440 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_listener_creation_vo.py
+-rw-rw-rw-   0        0        0     7208 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_listener_update_vo.py
+-rw-rw-rw-   0        0        0     6417 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_ports_vo.py
+-rw-rw-rw-   0        0        0     3576 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_selector_vo.py
+-rw-rw-rw-   0        0        0    16868 2023-04-18 15:44:50.000000 iotiumlib-23.5.0/iotiumlib/network.py
+-rw-rw-rw-   0        0        0    11025 2022-08-16 11:29:12.000000 iotiumlib-23.5.0/iotiumlib/node.py
+-rw-rw-rw-   0        0        0     3457 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/nodecli.py
+-rw-rw-rw-   0        0        0      538 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/orch.py
+-rw-rw-rw-   0        0        0     2605 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/orchlogin.py
+-rw-rw-rw-   0        0        0     5038 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/org.py
+-rw-rw-rw-   0        0        0     2514 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/pki.py
+-rw-rw-rw-   0        0        0     2407 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/profile.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.264581 iotiumlib-23.5.0/iotiumlib/requires/
+-rw-rw-rw-   0        0        0     1425 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/Exceptions.py
+-rw-rw-rw-   0        0        0       58 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/__init__.py
+-rw-rw-rw-   0        0        0      687 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/commonVariables.py
+-rw-rw-rw-   0        0        0     4802 2023-04-18 16:04:11.000000 iotiumlib-23.5.0/iotiumlib/requires/commonWrapper.py
+-rw-rw-rw-   0        0        0       38 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/constants.py
+-rw-rw-rw-   0        0        0    68425 2023-04-18 16:03:29.000000 iotiumlib-23.5.0/iotiumlib/requires/resourcePayload.py
+-rw-rw-rw-   0        0        0    24444 2022-08-19 08:13:17.000000 iotiumlib-23.5.0/iotiumlib/requires/utils.py
+-rw-rw-rw-   0        0        0     4109 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/secret.py
+-rw-rw-rw-   0        0        0    11742 2022-04-27 22:34:36.000000 iotiumlib-23.5.0/iotiumlib/service.py
+-rw-rw-rw-   0        0        0     2918 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/sshkey.py
+-rw-rw-rw-   0        0        0    15172 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/user.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.247112 iotiumlib-23.5.0/iotiumlib.egg-info/
+-rw-rw-rw-   0        0        0    15806 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:17:41.278106 iotiumlib-23.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-04-18 16:19:09.000000 iotiumlib-23.5.0/setup.py
```

### Comparing `iotiumlib-22.8.16/PKG-INFO` & `iotiumlib-23.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: iotiumlib
-Version: 22.8.16
+Version: 23.5.0
 Summary: ioTium API library
-Home-page: https://iotium.io
-Author: Jawahar A
-Author-email: jawahar.a@iotium.io
-License: Iotium | All rights reserved.
-Platform: UNKNOWN
+Home-page: https://view.com
+Author: Rashtrapathy C
+Author-email: rashtrapathy.chandrasekar@view.com
+License: Copyright 2023 View, Inc. | All Rights Reserved.
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
 
@@ -328,8 +327,7 @@
 iotiumlib.user.notifications(node_id=NODE_ID, filters={"start_date":"", "end_date":""}, type="node").Response.output
 iotiumlib.user.notifications(org_id=ORG_ID, filters={"start_date":"", "end_date":""}, type="node").Response.output
 
 ###### Using Webhooks #######
 iotiumlib.user.webhook.add(name="Webhook Name", "url"="https://abc.com/api/iotiumalerts", "secret"="test")
 
 ```  
-
```

### Comparing `iotiumlib-22.8.16/README.md` & `iotiumlib-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/__init__.py` & `iotiumlib-23.5.0/iotiumlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Rashtrapathy"
-__copyright__ = "Copyright (c) 2018-2021 by Iotium, Inc."
+__copyright__ = "Copyright 2023 View, Inc. | All Rights Reserved"
 __license__ = "All rights reserved."
-__version__ = "22.8.16"
+__version__ = "23.5.00"
 __credits__ = ["Rashtrapathy", "Thyagarajan", "Jawahar", "Venkatesan", "Raja"]
 __maintainer__ = "Rashtrapathy C"
 __email__ = "rashtrapathy.chandrasekar@view.com"
 __status__ = "Development"
 __name__ = "iotiumlib"
 
 from .node import *
```

### Comparing `iotiumlib-22.8.16/iotiumlib/cluster.py` & `iotiumlib-23.5.0/iotiumlib/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,29 +92,42 @@
         else:
             return self.Response
         self.Response.output = respOp.json()
         self.Response.code = respOp.status_code
         return self.Response
 
     @staticmethod
-    def add(name, labels=None, nodes=None, container_timezone=None, instance_id=100):
+    def add(name, labels=None, nodes=None, container_timezone=None, instance_id=100, election_network_type='WAN'):
         return cluster(action='add', payload=locals())
 
     @staticmethod
-    def edit(cluster_id, name=None, labels=None, nodes=None, container_timezone=None, instance_id=None):
+    def edit(cluster_id, name=None, labels=None, nodes=None, container_timezone=None, instance_id=None,
+             election_network_type=None, election_network_id=None):
         resp = cluster.get(cluster_id=cluster_id)
 
         name = resp.Response.output['name'] if name is None else name
 
         if instance_id is None:
             if 'config' in resp.Response.output and 'instance_id' in resp.Response.output['config']:
                 instance_id = resp.Response.output['config']['instance_id']
         else:
             instance_id =  instance_id
 
+        if election_network_type is None:
+            if 'config' in resp.Response.output and 'election_network_type' in resp.Response.output['config']:
+                election_network_type = resp.Response.output['config']['election_network_type']
+        else:
+            election_network_type =  election_network_type
+
+        if election_network_id is None:
+            if 'config' in resp.Response.output and 'election_network_id' in resp.Response.output['config']:
+                election_network_id = resp.Response.output['config']['election_network_id']
+        else:
+            election_network_id =  election_network_id
+
         if nodes is None:
             nodes = []
             if 'nodes' in resp.Response.output:
                 for n in resp.Response.output['nodes']:
                     node_id = str()
                     priority = int()
                     is_candidate = bool()
```

### Comparing `iotiumlib-22.8.16/iotiumlib/download.py` & `iotiumlib-23.5.0/iotiumlib/download.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/firewall.py` & `iotiumlib-23.5.0/iotiumlib/firewall.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/helper.py` & `iotiumlib-23.5.0/iotiumlib/helper.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/image.py` & `iotiumlib-23.5.0/iotiumlib/image.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/models/service_listener_creation_vo.py` & `iotiumlib-23.5.0/iotiumlib/models/service_listener_creation_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/models/service_listener_update_vo.py` & `iotiumlib-23.5.0/iotiumlib/models/service_listener_update_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/models/service_ports_vo.py` & `iotiumlib-23.5.0/iotiumlib/models/service_ports_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/models/service_selector_vo.py` & `iotiumlib-23.5.0/iotiumlib/models/service_selector_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/network.py` & `iotiumlib-23.5.0/iotiumlib/network.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/node.py` & `iotiumlib-23.5.0/iotiumlib/node.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/nodecli.py` & `iotiumlib-23.5.0/iotiumlib/nodecli.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/orch.py` & `iotiumlib-23.5.0/iotiumlib/orch.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/orchlogin.py` & `iotiumlib-23.5.0/iotiumlib/orchlogin.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/org.py` & `iotiumlib-23.5.0/iotiumlib/org.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/pki.py` & `iotiumlib-23.5.0/iotiumlib/pki.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/profile.py` & `iotiumlib-23.5.0/iotiumlib/profile.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/requires/Exceptions.py` & `iotiumlib-23.5.0/iotiumlib/requires/Exceptions.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/requires/commonVariables.py` & `iotiumlib-23.5.0/iotiumlib/requires/commonVariables.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/requires/commonWrapper.py` & `iotiumlib-23.5.0/iotiumlib/requires/commonWrapper.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/requires/resourcePayload.py` & `iotiumlib-23.5.0/iotiumlib/requires/resourcePayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,19 +464,21 @@
 
             if 'firewall_selector' in payload and payload['firewall_selector'] is not None and payload['firewall_selector']:
                 setattr(firewallObj, 'firewall_selector', payload['firewall_selector'])
                 self.firewall_selector = getattr(firewallObj, 'firewall_selector')
             else:
                 self.firewall_selector = None
 
-
             if 'firewall_policy' in payload and payload['firewall_policy'] is not None and payload['firewall_policy']:
                 setattr(policyObj, 'firewall_policy', payload['firewall_policy'])
             self.policy = getattr(policyObj, 'firewall_policy', {"firewall": {"debug": False}})
 
+            if 'enable_vrrp_tan' in payload and payload['enable_vrrp_tan'] is not None:
+                self.enable_vrrp_tan = payload['enable_vrrp_tan']
+
         class InterfaceIp(object):
             def __init__(self):
                 self._ip = str()
 
             @property
             def interface_ip(self):
                 return self._ip
@@ -1627,29 +1629,39 @@
             self.metadata = getattr(labelObj, 'metadata', {"labels": {}})
 
             nodesObj = resourcePaylod.Cluster.Nodes()
             if 'nodes' in payload and payload['nodes'] is not None and payload['nodes']:
                 setattr(nodesObj, "nodes", payload["nodes"])
             self.nodes = getattr(nodesObj, 'nodes', [])
 
-            InstanceIdObj = resourcePaylod.Cluster.InstanceId()
-            if 'instance_id' in payload and payload['instance_id'] is not None and payload['instance_id']:
-                setattr(InstanceIdObj, "instance_id", payload["instance_id"])
-                self.config = getattr(InstanceIdObj, 'instance_id')
-
             containerTimeZoneObj = resourcePaylod.Cluster.ContainerTimeZone()
             if 'container_timezone' in payload and payload['container_timezone'] is not None:
                 setattr(containerTimeZoneObj, 'container_timezone', payload['container_timezone'])
                 self.container_timezone = getattr(containerTimeZoneObj, 'container_timezone')
 
             upgradePolicyObj = resourcePaylod.UpgradePolicy.Channel()
             if 'policy' in payload and payload['policy'] is not None:
                 setattr(upgradePolicyObj, 'policy', payload['policy'])
                 self.channel = getattr(upgradePolicyObj, 'policy')
 
+            config_Obj = resourcePaylod.Cluster.ClusterConfig()
+            self.config = dict()
+            if 'election_network_type' in payload and payload['election_network_type'] is not None:
+                setattr(config_Obj, 'election_network_type', payload['election_network_type'])
+                self.config.update(getattr(config_Obj, 'election_network_type'))
+
+            if 'election_network_id' in payload and payload['election_network_id'] is not None:
+                setattr(config_Obj, 'election_network_id', payload['election_network_id'])
+                self.config.update(getattr(config_Obj, 'election_network_id'))
+
+            if 'instance_id' in payload and payload['instance_id'] is not None and payload['instance_id']:
+                setattr(config_Obj, "instance_id", payload["instance_id"])
+                self.config.update(getattr(config_Obj, 'instance_id'))
+
+
         class ClusterName(object):
             def __init__(self):
                 self._value = str()
 
             @property
             def name(self):
                 return self._value
@@ -1679,38 +1691,54 @@
                             _temp['config'].setdefault("priority", 100)
                         if 'is_candidate' in nodes:
                             _temp['config'].setdefault("is_candidate", nodes['is_candidate'])
                         else:
                             _temp['config'].setdefault("is_candidate", False)
                         self._value.append(_temp)
 
-        class InstanceId(object):
-            def __init__(self):
-                self._value = {"instance_id" : 100}
-
-            @property
-            def instance_id(self):
-                return self._value
-
-            @instance_id.setter
-            def instance_id(self, value):
-                self._value['instance_id'] = value
-
         class ContainerTimeZone(object):
             def __init__(self):
                 self._value = str()
 
             @property
             def container_timezone(self):
                 return self._value
 
             @container_timezone.setter
             def container_timezone(self, value):
                 self._value = value
 
+        class ClusterConfig(object):
+            def __init__(self):
+                self._value = dict()
+
+            @property
+            def election_network_type(self):
+                return self._value
+
+            @election_network_type.setter
+            def election_network_type(self, value):
+                self._value = {"election_network_type":value}
+
+            @property
+            def election_network_id(self):
+                return self._value
+
+            @election_network_id.setter
+            def election_network_id(self, value):
+                self._value = {"election_network_id":value}
+
+            @property
+            def instance_id(self):
+                return self._value
+
+            @instance_id.setter
+            def instance_id(self, value):
+                self._value = {"instance_id":value}
+
     class DownloadEvent(object):
         def __init__(self, payload):
             if payload == {}:
                 return
 
             orgId_Obj = resourcePaylod.Organisation.orgId()
             if 'org_id' in payload and payload['org_id'] is not None:
```

### Comparing `iotiumlib-22.8.16/iotiumlib/requires/utils.py` & `iotiumlib-23.5.0/iotiumlib/requires/utils.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/secret.py` & `iotiumlib-23.5.0/iotiumlib/secret.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/service.py` & `iotiumlib-23.5.0/iotiumlib/service.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/sshkey.py` & `iotiumlib-23.5.0/iotiumlib/sshkey.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib/user.py` & `iotiumlib-23.5.0/iotiumlib/user.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-22.8.16/iotiumlib.egg-info/PKG-INFO` & `iotiumlib-23.5.0/iotiumlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: iotiumlib
-Version: 22.8.16
+Version: 23.5.0
 Summary: ioTium API library
-Home-page: https://iotium.io
-Author: Jawahar A
-Author-email: jawahar.a@iotium.io
-License: Iotium | All rights reserved.
-Platform: UNKNOWN
+Home-page: https://view.com
+Author: Rashtrapathy C
+Author-email: rashtrapathy.chandrasekar@view.com
+License: Copyright 2023 View, Inc. | All Rights Reserved.
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
 
@@ -328,8 +327,7 @@
 iotiumlib.user.notifications(node_id=NODE_ID, filters={"start_date":"", "end_date":""}, type="node").Response.output
 iotiumlib.user.notifications(org_id=ORG_ID, filters={"start_date":"", "end_date":""}, type="node").Response.output
 
 ###### Using Webhooks #######
 iotiumlib.user.webhook.add(name="Webhook Name", "url"="https://abc.com/api/iotiumalerts", "secret"="test")
 
 ```  
-
```

### Comparing `iotiumlib-22.8.16/iotiumlib.egg-info/SOURCES.txt` & `iotiumlib-23.5.0/iotiumlib.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 iotiumlib/user.py
 iotiumlib.egg-info/PKG-INFO
 iotiumlib.egg-info/SOURCES.txt
 iotiumlib.egg-info/dependency_links.txt
 iotiumlib.egg-info/requires.txt
 iotiumlib.egg-info/top_level.txt
 iotiumlib/models/__init__.py
+iotiumlib/models/role_creation_vo.py
+iotiumlib/models/role_updation_vo.py
 iotiumlib/models/service_listener_creation_vo.py
 iotiumlib/models/service_listener_update_vo.py
 iotiumlib/models/service_ports_vo.py
 iotiumlib/models/service_selector_vo.py
 iotiumlib/requires/Exceptions.py
 iotiumlib/requires/__init__.py
 iotiumlib/requires/commonVariables.py
```

