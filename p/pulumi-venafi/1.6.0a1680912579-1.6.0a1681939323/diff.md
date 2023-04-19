# Comparing `tmp/pulumi_venafi-1.6.0a1680912579.tar.gz` & `tmp/pulumi_venafi-1.6.0a1681939323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.6.0a1680912579.tar", last modified: Sat Apr  8 00:16:14 2023, max compression
+gzip compressed data, was "pulumi_venafi-1.6.0a1681939323.tar", last modified: Wed Apr 19 21:30:34 2023, max compression
```

## Comparing `pulumi_venafi-1.6.0a1680912579.tar` & `pulumi_venafi-1.6.0a1681939323.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:16:14.709709 pulumi_venafi-1.6.0a1680912579/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-08 00:16:14.000000 pulumi_venafi-1.6.0a1680912579/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:30:34.796271 pulumi_venafi-1.6.0a1681939323/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-19 21:30:34.796271 pulumi_venafi-1.6.0a1681939323/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:30:34.792271 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:30:34.796271 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:30:34.792271 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:30:34.796271 pulumi_venafi-1.6.0a1681939323/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-19 21:30:34.000000 pulumi_venafi-1.6.0a1681939323/setup.py
```

### Comparing `pulumi_venafi-1.6.0a1680912579/PKG-INFO` & `pulumi_venafi-1.6.0a1681939323/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.6.0a1680912579
+Version: 1.6.0a1681939323
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.6.0a1680912579/README.md` & `pulumi_venafi-1.6.0a1681939323/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/__init__.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/certificate.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/policy.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/provider.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-venafi
-Version: 1.6.0a1680912579
+Version: 1.6.0a1681939323
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.6.0a1680912579/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.6.0a1681939323/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1680912579/setup.py` & `pulumi_venafi-1.6.0a1681939323/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.6.0a1680912579"
-PLUGIN_VERSION = "1.6.0-alpha.1680912579+5cadca93"
+VERSION = "1.6.0a1681939323"
+PLUGIN_VERSION = "1.6.0-alpha.1681939323+71663102"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'venafi', PLUGIN_VERSION])
         except OSError as error:
```

