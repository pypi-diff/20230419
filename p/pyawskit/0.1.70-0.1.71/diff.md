# Comparing `tmp/pyawskit-0.1.70.tar.gz` & `tmp/pyawskit-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.70.tar", last modified: Wed Apr 19 20:07:08 2023, max compression
+gzip compressed data, was "pyawskit-0.1.71.tar", last modified: Wed Apr 19 20:13:06 2023, max compression
```

## Comparing `pyawskit-0.1.70.tar` & `pyawskit-0.1.71.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-19 20:06:54.000000 pyawskit-0.1.70/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:07:08.952781 pyawskit-0.1.70/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-19 20:06:54.000000 pyawskit-0.1.70/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.70/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.70/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.70/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.70/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1823 2023-04-19 20:06:31.000000 pyawskit-0.1.70/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.70/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.70/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14844 2023-04-19 20:03:40.000000 pyawskit-0.1.70/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.70/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-19 20:06:54.000000 pyawskit-0.1.70/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.70/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-19 20:07:08.953781 pyawskit-0.1.70/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1787 2023-04-19 20:06:54.000000 pyawskit-0.1.70/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.763088 pyawskit-0.1.71/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-19 20:12:50.000000 pyawskit-0.1.71/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:13:06.763088 pyawskit-0.1.71/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-19 20:12:50.000000 pyawskit-0.1.71/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.762088 pyawskit-0.1.71/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.71/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.71/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.71/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.71/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1826 2023-04-19 20:12:23.000000 pyawskit-0.1.71/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.71/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.71/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14844 2023-04-19 20:03:40.000000 pyawskit-0.1.71/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.71/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-19 20:12:50.000000 pyawskit-0.1.71/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.71/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:13:06.763088 pyawskit-0.1.71/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-19 20:13:06.000000 pyawskit-0.1.71/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-19 20:13:06.763088 pyawskit-0.1.71/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1787 2023-04-19 20:12:50.000000 pyawskit-0.1.71/setup.py
```

### Comparing `pyawskit-0.1.70/LICENSE` & `pyawskit-0.1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/PKG-INFO` & `pyawskit-0.1.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.70
+Version: 0.1.71
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.70
+version: 0.1.71
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.70/pyawskit/aws.py` & `pyawskit-0.1.71/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.71/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.71/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/aws_ecr_login_code.py` & `pyawskit-0.1.71/pyawskit/aws_ecr_login_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             sys.exit()
 
     with open("/dev/tty", "wt", encoding="utf-8") as f:
         print("Creating new tepm key for ecr", file=f)
 
     client = boto3.client("ecr")
     res = client.get_authorization_token()
-    authorizationData = res["authorizationData"]
+    authorizationData = res["authorizationData"][0]
     d_authorizationToken = authorizationData["authorizationToken"]
     d_expiresAt = authorizationData["expiresAt"]
     d_proxyEndpoint = authorizationData["proxyEndpoint"]
 
     # decode the password
     base64decode = base64.b64decode(d_authorizationToken).decode("ASCII")
     (d_user, d_password) = base64decode.split(":")
```

### Comparing `pyawskit-0.1.70/pyawskit/common.py` & `pyawskit-0.1.71/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/configs.py` & `pyawskit-0.1.71/pyawskit/configs.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/main.py` & `pyawskit-0.1.71/pyawskit/main.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/os_utils.py` & `pyawskit-0.1.71/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit/utils.py` & `pyawskit-0.1.71/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.70/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.71/pyawskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.70
+Version: 0.1.71
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.70
+version: 0.1.71
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.70/setup.py` & `pyawskit-0.1.71/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.70",
+    version="0.1.71",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="pyawskit is a collection of utilities to help interact with aws",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

