# Comparing `tmp/pyawskit-0.1.68.tar.gz` & `tmp/pyawskit-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.68.tar", last modified: Mon Apr 17 09:06:49 2023, max compression
+gzip compressed data, was "pyawskit-0.1.70.tar", last modified: Wed Apr 19 20:07:08 2023, max compression
```

## Comparing `pyawskit-0.1.68.tar` & `pyawskit-0.1.70.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-17 09:06:49.266778 pyawskit-0.1.68/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-17 09:06:23.000000 pyawskit-0.1.68/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-17 09:06:49.266778 pyawskit-0.1.68/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-17 09:06:23.000000 pyawskit-0.1.68/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-17 09:06:49.266778 pyawskit-0.1.68/pyawskit/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:09.000000 pyawskit-0.1.68/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2022-06-13 04:33:09.000000 pyawskit-0.1.68/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-17 07:19:49.000000 pyawskit-0.1.68/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-17 07:19:49.000000 pyawskit-0.1.68/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)      722 2023-04-17 07:19:49.000000 pyawskit-0.1.68/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-12 10:00:43.000000 pyawskit-0.1.68/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2286 2023-04-17 07:19:49.000000 pyawskit-0.1.68/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14917 2023-04-17 07:19:49.000000 pyawskit-0.1.68/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-09-11 10:30:52.000000 pyawskit-0.1.68/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-17 09:06:23.000000 pyawskit-0.1.68/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-09-11 10:30:52.000000 pyawskit-0.1.68/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-17 09:06:49.266778 pyawskit-0.1.68/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       94 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-17 09:06:49.000000 pyawskit-0.1.68/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-17 09:06:49.267778 pyawskit-0.1.68/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1766 2023-04-17 09:06:23.000000 pyawskit-0.1.68/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-19 20:06:54.000000 pyawskit-0.1.70/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:07:08.952781 pyawskit-0.1.70/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-04-19 20:06:54.000000 pyawskit-0.1.70/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.70/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.70/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.70/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.70/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1823 2023-04-19 20:06:31.000000 pyawskit-0.1.70/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.70/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.70/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14844 2023-04-19 20:03:40.000000 pyawskit-0.1.70/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.70/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-19 20:06:54.000000 pyawskit-0.1.70/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.70/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-19 20:07:08.952781 pyawskit-0.1.70/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-19 20:07:08.000000 pyawskit-0.1.70/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-19 20:07:08.953781 pyawskit-0.1.70/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1787 2023-04-19 20:06:54.000000 pyawskit-0.1.70/setup.py
```

### Comparing `pyawskit-0.1.68/LICENSE` & `pyawskit-0.1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/PKG-INFO` & `pyawskit-0.1.70/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.68
+Version: 0.1.70
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
 
-version: 0.1.68
+version: 0.1.70
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.68/pyawskit/aws.py` & `pyawskit-0.1.70/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.70/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.70/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit/common.py` & `pyawskit-0.1.70/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit/configs.py` & `pyawskit-0.1.70/pyawskit/configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,12 +43,7 @@
     env_npm_repository = ParamCreator.create_str(help_string="env npm repository")
 
 
 class ConfigAwsCodeartifactPip(Config):
     env_pip_domain = ParamCreator.create_str(help_string="env pip domain")
     env_pip_domain_owner = ParamCreator.create_str(help_string="env pip domain owner")
     env_pip_repository = ParamCreator.create_str(help_string="env pip repository")
-
-
-class ConfigAwsEcrLogin(Config):
-    env_ecr_region = ParamCreator.create_str(help_string="env ecr region")
-    env_ecr_account_id = ParamCreator.create_str(help_string="env ecr account id")
```

### Comparing `pyawskit-0.1.68/pyawskit/main.py` & `pyawskit-0.1.70/pyawskit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from pytconf import register_main, config_arg_parse_and_launch, register_endpoint
 
 import pyawskit.common
 from pyawskit.aws import ProcessData, request_spot_instances, tag_resources, poll_instances_till_done, wait_for_ssh, \
     attach_disks
 from pyawskit.common import update_etc_hosts, update_ssh_config, update_file, do_hush_login, wait_net_service, \
     get_disks, erase_partition_table, reread_partition_table, format_device, mount_disk
-from pyawskit.configs import ConfigFilter, ConfigName, ConfigWork, ConfigAwsCodeartifactNpm, ConfigAwsCodeartifactPip, \
-    ConfigAwsEcrLogin
+from pyawskit.configs import ConfigFilter, ConfigName, ConfigWork, ConfigAwsCodeartifactNpm, ConfigAwsCodeartifactPip
 
 from pyawskit.static import APP_NAME, VERSION_STR
 from pyawskit.utils import object_exists, compress_one_file, print_exception
 
 import pyawskit.aws_codeartifact_npm_env_config_code
 import pyawskit.aws_codeartifact_pip_env_config_code
 import pyawskit.aws_ecr_login_code
@@ -48,17 +47,14 @@
 )
 def aws_codeartifact_pip_env_config() -> None:
     pyawskit.aws_codeartifact_pip_env_config_code.run()
 
 
 @register_endpoint(
     description="docker login to aws acr",
-    configs=[
-        ConfigAwsEcrLogin,
-    ],
 )
 def aws_ecr_login() -> None:
     pyawskit.aws_ecr_login_code.run()
 
 
 @register_endpoint(
     description="Compress an S3 folder",
```

### Comparing `pyawskit-0.1.68/pyawskit/os_utils.py` & `pyawskit-0.1.70/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit/utils.py` & `pyawskit-0.1.70/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.68/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.70/pyawskit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.68
+Version: 0.1.70
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
 
-version: 0.1.68
+version: 0.1.70
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.68/setup.py` & `pyawskit-0.1.70/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.68",
+    version="0.1.70",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="pyawskit is a collection of utilities to help interact with aws",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
@@ -44,14 +44,15 @@
         "boto3",
         "pymount",
         "ujson",
         "sultan",
         "pytconf",
         "pyapikey",
         "furl",
+        "docker-py",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

