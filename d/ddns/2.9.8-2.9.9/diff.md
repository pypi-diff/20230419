# Comparing `tmp/ddns-2.9.8.tar.gz` & `tmp/ddns-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddns-2.9.8.tar", last modified: Mon Feb 22 01:50:56 2021, max compression
+gzip compressed data, was "dist/ddns-2.9.9.tar", last modified: Tue Apr 13 04:00:16 2021, max compression
```

## Comparing `ddns-2.9.8.tar` & `ddns-2.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:56.000000 ddns-2.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2021-02-22 01:50:18.000000 ddns-2.9.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    16050 2021-02-22 01:50:56.000000 ddns-2.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    13108 2021-02-22 01:50:18.000000 ddns-2.9.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16050 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2021-02-22 01:50:56.000000 ddns-2.9.8/ddns.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:56.000000 ddns-2.9.8/dns/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5750 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/alidns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3183 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/callback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5333 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/cloudflare.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5304 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/dnscom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6062 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/dnspod.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/dnspod_com.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/he.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7996 2021-02-22 01:50:18.000000 ddns-2.9.8/dns/huaweidns.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7182 2021-02-22 01:50:23.000000 ddns-2.9.8/run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2021-02-22 01:50:56.000000 ddns-2.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     9397 2021-02-22 01:50:18.000000 ddns-2.9.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:56.000000 ddns-2.9.8/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-22 01:50:18.000000 ddns-2.9.8/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3337 2021-02-22 01:50:18.000000 ddns-2.9.8/util/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2021-02-22 01:50:18.000000 ddns-2.9.8/util/ip.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-13 04:00:16.000000 ddns-2.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2021-04-13 03:59:36.000000 ddns-2.9.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16086 2021-04-13 04:00:16.000000 ddns-2.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13144 2021-04-13 03:59:36.000000 ddns-2.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16086 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2021-04-13 04:00:16.000000 ddns-2.9.9/ddns.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-13 04:00:16.000000 ddns-2.9.9/dns/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5758 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/alidns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3183 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/callback.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5333 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/cloudflare.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5304 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/dnscom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6062 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/dnspod.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/dnspod_com.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/he.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7996 2021-04-13 03:59:36.000000 ddns-2.9.9/dns/huaweidns.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7182 2021-04-13 03:59:42.000000 ddns-2.9.9/run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2021-04-13 04:00:16.000000 ddns-2.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9397 2021-04-13 03:59:36.000000 ddns-2.9.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-13 04:00:16.000000 ddns-2.9.9/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-13 03:59:36.000000 ddns-2.9.9/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3337 2021-04-13 03:59:36.000000 ddns-2.9.9/util/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3845 2021-04-13 03:59:36.000000 ddns-2.9.9/util/ip.py
```

### Comparing `ddns-2.9.8/LICENSE` & `ddns-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/PKG-INFO` & `ddns-2.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddns
-Version: 2.9.8
+Version: 2.9.9
 Summary: automatically update DNS records to dynamic local IP [自动更新DNS记录指向本地IP]
 Home-page: https://ddns.newfuture.cc
 Author: NewFuture
 Author-email: python@newfuture.cc
 License: MIT
 Project-URL: Bug Reports, https://github.com/NewFuture/DDNS/issues
 Project-URL: Source, https://github.com/NewFuture/DDNS
@@ -20,18 +20,18 @@
         
         <details>
         
         <summary markdown="span">Build Details
         </summary>
         
         - Linux Python (2 和 3): [![Travis build](https://img.shields.io/travis/com/NewFuture/DDNS/master.svg?label=python2%2Cpython3&logo=ubuntu&logoColor=white)](https://travis-ci.com/NewFuture/DDNS)
-        - Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
         
         </details>
         
         ---
         
         ## Features
```

### Comparing `ddns-2.9.8/README.md` & `ddns-2.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 <details>
 
 <summary markdown="span">Build Details
 </summary>
 
 - Linux Python (2 和 3): [![Travis build](https://img.shields.io/travis/com/NewFuture/DDNS/master.svg?label=python2%2Cpython3&logo=ubuntu&logoColor=white)](https://travis-ci.com/NewFuture/DDNS)
-- Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-- Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-- Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-- Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+- Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+- Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+- Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+- Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
 
 </details>
 
 ---
 
 ## Features
```

### Comparing `ddns-2.9.8/ddns.egg-info/PKG-INFO` & `ddns-2.9.9/ddns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddns
-Version: 2.9.8
+Version: 2.9.9
 Summary: automatically update DNS records to dynamic local IP [自动更新DNS记录指向本地IP]
 Home-page: https://ddns.newfuture.cc
 Author: NewFuture
 Author-email: python@newfuture.cc
 License: MIT
 Project-URL: Bug Reports, https://github.com/NewFuture/DDNS/issues
 Project-URL: Source, https://github.com/NewFuture/DDNS
@@ -20,18 +20,18 @@
         
         <details>
         
         <summary markdown="span">Build Details
         </summary>
         
         - Linux Python (2 和 3): [![Travis build](https://img.shields.io/travis/com/NewFuture/DDNS/master.svg?label=python2%2Cpython3&logo=ubuntu&logoColor=white)](https://travis-ci.com/NewFuture/DDNS)
-        - Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
-        - Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Windows Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Windows Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=Windows&configuration=Windows%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Mac OSX Python3.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python37)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
+        - Mac OSX Python2.7: [![Build Status](https://dev.azure.com/NewFuture-CI/ddns-ci/_apis/build/status/NewFuture.DDNS?branchName=master&jobName=MacOS&configuration=MacOS%20Python27)](https://dev.azure.com/NewFuture-CI/ddns-ci/_build/latest?definitionId=2&branchName=master)
         
         </details>
         
         ---
         
         ## Features
```

### Comparing `ddns-2.9.8/dns/alidns.py` & `ddns-2.9.9/dns/alidns.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,17 @@
         'Version': '2015-01-09',
         'AccessKeyId': Config.ID,
         'Timestamp': datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ'),
         'SignatureMethod': 'HMAC-SHA1',
         'SignatureNonce': uuid4(),
         'SignatureVersion': "1.0",
     })
-    query = urlencode(sorted(params.items()))
+    query = urlencode(sorted(params.items()), quote_via=quote)
     debug(query)
-    sign = API.METHOD + "&" + quote_plus("/") + "&" + quote(query, safe='')
+    sign = API.METHOD + "&" + quote_plus("/") + "&" + quote(query)
     debug("signString: %s", sign)
 
     sign = hmac((Config.TOKEN + "&").encode('utf-8'),
                 sign.encode('utf-8'), sha1).digest()
     sign = b64encode(sign).strip()
     params["Signature"] = sign
     return params
```

### Comparing `ddns-2.9.8/dns/callback.py` & `ddns-2.9.9/dns/callback.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/dns/cloudflare.py` & `ddns-2.9.9/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/dns/dnscom.py` & `ddns-2.9.9/dns/dnscom.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/dns/dnspod.py` & `ddns-2.9.9/dns/dnspod.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/dns/he.py` & `ddns-2.9.9/dns/he.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/dns/huaweidns.py` & `ddns-2.9.9/dns/huaweidns.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/run.py` & `ddns-2.9.9/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 from subprocess import check_output
 
 import sys
 
 from util import ip
 from util.cache import Cache
 
-__version__ = "v2.9.8@2021-02-22T01:50:23+00:00"  # CI 时会被Tag替换
+__version__ = "v2.9.9@2021-04-13T03:59:42+00:00"  # CI 时会被Tag替换
 __description__ = "automatically update DNS records to dynamic local IP [自动更新DNS记录指向本地IP]"
 __doc__ = """
 ddns[%s]
 (i) homepage or docs [文档主页]: https://ddns.newfuture.cc/
 (?) issues or bugs [问题和帮助]: https://github.com/NewFuture/DDNS/issues
 Copyright (c) New Future (MIT License)
 """ % (__version__)
 
-environ["DDNS_VERSION"] = "v2.9.8"
+environ["DDNS_VERSION"] = "v2.9.9"
 
 if getattr(sys, 'frozen', False):
     # https://github.com/pyinstaller/pyinstaller/wiki/Recipe-OpenSSL-Certificate
     environ['SSL_CERT_FILE'] = path.join(
         getattr(sys, '_MEIPASS'), 'lib', 'cert.pem')
 
 CACHE_FILE = path.join(gettempdir(), 'ddns.cache')
@@ -48,15 +48,15 @@
                 get_config.config = loadjson(configfile)
                 get_config.time = stat(path).st_mtime
         except IOError:
             error(' Config file `%s` does not exist!' % path)
             with open(path, 'w') as configfile:
                 configure = {
                     "$schema": "https://ddns.newfuture.cc/schema/v2.8.json",
-                    "id": "YOUR ID or EAMIL for DNS Provider",
+                    "id": "YOUR ID or EMAIL for DNS Provider",
                     "token": "YOUR TOKEN or KEY for DNS Provider",
                     "dns": "dnspod",
                     "ipv4": [
                         "newfuture.cc",
                         "ddns.newfuture.cc"
                     ],
                     "ipv6": [
```

### Comparing `ddns-2.9.8/setup.py` & `ddns-2.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/util/cache.py` & `ddns-2.9.9/util/cache.py`

 * *Files identical despite different names*

### Comparing `ddns-2.9.8/util/ip.py` & `ddns-2.9.9/util/ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     return _ip_regex_match(regex_str, reg)
 
 
 def regex_v6(reg):  # ipv6 正则提取
     if os_name == 'nt':  # Windows: IPv4 xxx: ::1
         regex_str = r'IPv6 .*: ([\:\dabcdef]*)?\W'
     else:
-        regex_str = r'inet6 (?:addr\:)?([\:\dabcdef]*)?[\s/%]'
+        regex_str = r'inet6 (?:addr\:\s*)?([\:\dabcdef]*)?[\s/%]'
     return _ip_regex_match(regex_str, reg)
```

