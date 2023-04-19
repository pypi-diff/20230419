# Comparing `tmp/odoogap-mtd-0.1.1.tar.gz` & `tmp/odoogap-mtd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoogap-mtd-0.1.1.tar", last modified: Mon Jan 18 18:05:41 2021, max compression
+gzip compressed data, was "dist/odoogap-mtd-0.1.2.tar", last modified: Wed Apr 19 11:01:44 2023, max compression
```

## Comparing `odoogap-mtd-0.1.1.tar` & `odoogap-mtd-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2021-01-18 18:05:41.000000 odoogap-mtd-0.1.1/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2021-01-18 18:05:41.000000 odoogap-mtd-0.1.1/odoogap_mtd.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2021-01-18 18:05:40.000000 odoogap-mtd-0.1.1/odoogap_mtd.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      209 2021-01-18 18:05:40.000000 odoogap-mtd-0.1.1/odoogap_mtd.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      454 2021-01-18 18:05:40.000000 odoogap-mtd-0.1.1/odoogap_mtd.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       12 2021-01-18 18:05:40.000000 odoogap-mtd-0.1.1/odoogap_mtd.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       50 2021-01-18 17:10:50.000000 odoogap-mtd-0.1.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       38 2021-01-18 18:05:41.000000 odoogap-mtd-0.1.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2021-01-18 18:05:41.000000 odoogap-mtd-0.1.1/odoogap_mtd/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2484 2021-01-18 16:50:12.000000 odoogap-mtd-0.1.1/odoogap_mtd/mtd_headers.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       26 2021-01-18 18:03:51.000000 odoogap-mtd-0.1.1/odoogap_mtd/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      454 2021-01-18 18:05:41.000000 odoogap-mtd-0.1.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      630 2021-01-18 18:05:34.000000 odoogap-mtd-0.1.1/setup.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      209 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      454 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       12 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       50 2021-01-18 17:10:50.000000 odoogap-mtd-0.1.2/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       38 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/odoogap_mtd/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2512 2023-04-19 10:58:01.000000 odoogap-mtd-0.1.2/odoogap_mtd/mtd_headers.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       26 2021-01-18 18:03:51.000000 odoogap-mtd-0.1.2/odoogap_mtd/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      454 2023-04-19 11:01:44.000000 odoogap-mtd-0.1.2/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      630 2023-04-19 11:01:33.000000 odoogap-mtd-0.1.2/setup.py
```

### Comparing `odoogap-mtd-0.1.1/odoogap_mtd/mtd_headers.py` & `odoogap-mtd-0.1.2/odoogap_mtd/mtd_headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import time
 
 def get_local_ip():
     hostname = socket.gethostname()
     return socket.gethostbyname(hostname)
     
 
-def create_headers_dic(public_port, device_id, user_id, screens, window_size, browser_plugin, js_user_agent, login_date_format, unique_reference, module_version, licence_ids):
+def create_headers_dic(public_port, device_id, user_id, screens, window_size, browser_plugin, js_user_agent,
+                       login_date_format, unique_reference, module_version, licence_ids):
     
     public_ip_timestamp = datetime.utcnow().isoformat(sep='T', timespec='milliseconds') + 'Z'
     public_ip = get('https://api.ipify.org').text
 
-    public_vendor_ip = socket.gethostbyname('odoomtd.co.uk')
+    public_vendor_ip = socket.gethostbyname('api.odoomtd.co.uk')
 
     timestamp = login_date_format.replace("/", "-").replace(",", "").replace(" ", "T").replace(":", "%3A") + "Z"
     
     date_string = str(datetime.now(timezone.utc).astimezone().isoformat())
     
     if '+' in date_string:
         data = date_string.rsplit('+', 1)
@@ -43,8 +44,8 @@
         'Gov-Client-Browser-Do-Not-Track': "false",
         'Gov-Client-Multi-Factor': "type=OTHER&timestamp=" + timestamp + "&unique-reference=" + str(hash(unique_reference)),
         'Gov-Vendor-Version': "hmrc_mtd_client" + "=" + str(module_version) + "&hmrc_mtd_server" + "=" + "0.1",
         'Gov-Vendor-License-IDs': "hmrc_mtd_server" + "=" + str(hash(licence_ids)),
         'Gov-Vendor-Public-IP': public_vendor_ip,
         'Gov-Vendor-Forwarded': "by=" + public_vendor_ip + "&for=" + public_ip,
         'Gov-Vendor-Product-Name': 'OdooGAP'
-    }
+    }
```

### Comparing `odoogap-mtd-0.1.1/setup.py` & `odoogap-mtd-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="odoogap-mtd",
-    version="0.1.1",
+    version="0.1.2",
     author="OdooGap",
     author_email="",
     description="MTD Library For OdooGAP",
     long_description="OdooGAP MTD external libray",
     long_description_content_type="text/markdown",
     url="https://github.com/odoogap/mtd_library",
     packages=setuptools.find_packages(),
```

