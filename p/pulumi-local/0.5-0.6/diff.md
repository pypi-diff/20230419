# Comparing `tmp/pulumi-local-0.5.tar.gz` & `tmp/pulumi-local-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-local-0.5.tar", last modified: Fri Dec 30 22:54:21 2022, max compression
+gzip compressed data, was "pulumi-local-0.6.tar", last modified: Wed Apr 19 10:17:00 2023, max compression
```

## Comparing `pulumi-local-0.5.tar` & `pulumi-local-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2022-12-30 22:54:21.296694 pulumi-local-0.5/
--rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-14 22:27:33.000000 pulumi-local-0.5/LICENSE
--rw-r--r--   0 whummer    (501) staff       (20)      839 2022-12-30 22:54:21.296586 pulumi-local-0.5/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     1903 2022-12-30 22:51:23.000000 pulumi-local-0.5/README.md
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2022-12-30 22:54:21.295836 pulumi-local-0.5/bin/
--rwxr-xr-x   0 whummer    (501) staff       (20)     8401 2022-12-30 22:52:33.000000 pulumi-local-0.5/bin/pulumilocal
--rwxr-xr-x   0 whummer    (501) staff       (20)       41 2022-10-25 16:58:31.000000 pulumi-local-0.5/bin/pulumilocal.bat
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2022-12-30 22:54:21.296446 pulumi-local-0.5/pulumi_local.egg-info/
--rw-r--r--   0 whummer    (501) staff       (20)      839 2022-12-30 22:54:21.000000 pulumi-local-0.5/pulumi_local.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)      241 2022-12-30 22:54:21.000000 pulumi-local-0.5/pulumi_local.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2022-12-30 22:54:21.000000 pulumi-local-0.5/pulumi_local.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (501) staff       (20)        7 2022-12-30 22:54:21.000000 pulumi-local-0.5/pulumi_local.egg-info/requires.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2022-12-30 22:54:21.000000 pulumi-local-0.5/pulumi_local.egg-info/top_level.txt
--rw-r--r--   0 whummer    (501) staff       (20)       38 2022-12-30 22:54:21.296727 pulumi-local-0.5/setup.cfg
--rwxr-xr-x   0 whummer    (501) staff       (20)     1191 2022-12-30 22:54:15.000000 pulumi-local-0.5/setup.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-19 10:17:00.343766 pulumi-local-0.6/
+-rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-14 22:27:33.000000 pulumi-local-0.6/LICENSE
+-rw-r--r--   0 whummer    (501) staff       (20)      839 2023-04-19 10:17:00.343642 pulumi-local-0.6/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     1989 2023-04-19 10:15:12.000000 pulumi-local-0.6/README.md
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-19 10:17:00.342680 pulumi-local-0.6/bin/
+-rwxr-xr-x   0 whummer    (501) staff       (20)     8399 2023-04-19 10:15:12.000000 pulumi-local-0.6/bin/pulumilocal
+-rwxr-xr-x   0 whummer    (501) staff       (20)       41 2022-10-25 16:58:31.000000 pulumi-local-0.6/bin/pulumilocal.bat
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-19 10:17:00.343485 pulumi-local-0.6/pulumi_local.egg-info/
+-rw-r--r--   0 whummer    (501) staff       (20)      839 2023-04-19 10:17:00.000000 pulumi-local-0.6/pulumi_local.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)      241 2023-04-19 10:17:00.000000 pulumi-local-0.6/pulumi_local.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2023-04-19 10:17:00.000000 pulumi-local-0.6/pulumi_local.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        7 2023-04-19 10:17:00.000000 pulumi-local-0.6/pulumi_local.egg-info/requires.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2023-04-19 10:17:00.000000 pulumi-local-0.6/pulumi_local.egg-info/top_level.txt
+-rw-r--r--   0 whummer    (501) staff       (20)       38 2023-04-19 10:17:00.343804 pulumi-local-0.6/setup.cfg
+-rwxr-xr-x   0 whummer    (501) staff       (20)     1191 2023-04-19 10:15:12.000000 pulumi-local-0.6/setup.py
```

### Comparing `pulumi-local-0.5/LICENSE` & `pulumi-local-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pulumi-local-0.5/PKG-INFO` & `pulumi-local-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-local
-Version: 0.5
+Version: 0.6
 Summary: Thin wrapper script to use Pulumi with LocalStack
 Home-page: https://github.com/localstack/pulumi-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `pulumi-local-0.5/README.md` & `pulumi-local-0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 * `LOCALSTACK_HOSTNAME`: Target host to use for connecting to LocalStack (default: `localhost`)
 * `EDGE_PORT`: Target port to use for connecting to LocalStack (default: `4566`)
 * `PULUMI_CMD`: Name of the executable Pulumi command on the system PATH (default: `pulumi`)
 * `PULUMI_STACK_NAME`: Name of the Pulumi stack used to configure local endpoints (default: `localstack`)
 
 ## Change Log
 
+* v0.6: Replace deprecated `s3ForcePathStyle` with `s3UsePathStyle` in default config
 * v0.5: Remove deprecated `mobileanalytics` service config to fix invalid key error
 * v0.4: Point pulumilocal.bat to the correct script
 * v0.3: Add apigatewayv2 service endpoint
 * v0.2: Add init command and add aws:region key by default
 * v0.1: Initial release
 
 ## License
```

### Comparing `pulumi-local-0.5/bin/pulumilocal` & `pulumi-local-0.6/bin/pulumilocal`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 DEFAULT_CONFIG = {
     'config': {
         'aws:accessKey': 'test',
         'aws:secretKey': 'test',
         'aws:endpoints': [],
         'aws:region': 'us-east-1',
-        'aws:s3ForcePathStyle': 'true',
+        'aws:s3UsePathStyle': 'true',
         'aws:skipCredentialsValidation': 'true',
         'aws:skipRequestingAccountId': 'true',
     }
 }
 
 # Unfortunately, we need to hardcode the service names here, as importing from
 # localstack-client doesn't work (some keys differ / are unavailable in Pulumi)
```

### Comparing `pulumi-local-0.5/pulumi_local.egg-info/PKG-INFO` & `pulumi-local-0.6/pulumi_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-local
-Version: 0.5
+Version: 0.6
 Summary: Thin wrapper script to use Pulumi with LocalStack
 Home-page: https://github.com/localstack/pulumi-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `pulumi-local-0.5/setup.py` & `pulumi-local-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 if __name__ == '__main__':
 
     setup(
         name='pulumi-local',
-        version='0.5',
+        version='0.6',
         description='Thin wrapper script to use Pulumi with LocalStack',
         author='LocalStack Team',
         author_email='info@localstack.cloud',
         url='https://github.com/localstack/pulumi-local',
         packages=[],
         scripts=['bin/pulumilocal', 'bin/pulumilocal.bat'],
         package_data={},
```

