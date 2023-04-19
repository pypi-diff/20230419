# Comparing `tmp/mypy-boto3-secretsmanager-1.26.49.tar.gz` & `tmp/mypy-boto3-secretsmanager-1.26.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-secretsmanager-1.26.49.tar", last modified: Thu Jan 12 20:34:32 2023, max compression
+gzip compressed data, was "mypy-boto3-secretsmanager-1.26.89.tar", last modified: Fri Mar 10 20:32:12 2023, max compression
```

## Comparing `mypy-boto3-secretsmanager-1.26.49.tar` & `mypy-boto3-secretsmanager-1.26.89.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.459099 mypy-boto3-secretsmanager-1.26.49/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-01-12 20:34:32.459099 mypy-boto3-secretsmanager-1.26.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.451099 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:22.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-01-12 20:34:23.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-01-12 20:34:23.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.459099 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-12 20:34:32.000000 mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 20:34:32.459099 mypy-boto3-secretsmanager-1.26.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-12 20:34:21.000000 mypy-boto3-secretsmanager-1.26.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.092089 mypy-boto3-secretsmanager-1.26.89/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-03-10 20:32:12.092089 mypy-boto3-secretsmanager-1.26.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.088089 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-10 20:32:03.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:32:12.092089 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-10 20:32:12.000000 mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:32:12.092089 mypy-boto3-secretsmanager-1.26.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-10 20:32:02.000000 mypy-boto3-secretsmanager-1.26.89/setup.py
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/LICENSE` & `mypy-boto3-secretsmanager-1.26.89/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/PKG-INFO` & `mypy-boto3-secretsmanager-1.26.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.26.49
-Summary: Type annotations for boto3.SecretsManager 1.26.49 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.89
+Summary: Type annotations for boto3.SecretsManager 1.26.89 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/README.md` & `mypy-boto3-secretsmanager-1.26.89/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__init__.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__init__.pyi` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/__main__.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecretsManager 1.26.49\nVersion:         1.26.49\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.SecretsManager 1.26.89\nVersion:         1.26.89\nBuilder"
+        " version: 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.49")
+    print("1.26.89")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/client.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/client.pyi` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/literals.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -182,14 +183,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -358,14 +360,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -399,14 +402,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/literals.pyi` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -180,14 +181,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -356,14 +358,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -397,14 +400,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/paginator.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/paginator.pyi` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/type_defs.py` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager/type_defs.pyi` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/PKG-INFO` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.26.49
-Summary: Type annotations for boto3.SecretsManager 1.26.49 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.89
+Summary: Type annotations for boto3.SecretsManager 1.26.89 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.26.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.26.49/mypy_boto3_secretsmanager.egg-info/SOURCES.txt` & `mypy-boto3-secretsmanager-1.26.89/mypy_boto3_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.26.49/setup.py` & `mypy-boto3-secretsmanager-1.26.89/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-secretsmanager",
-    version="1.26.49",
+    version="1.26.89",
     packages=["mypy_boto3_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecretsManager 1.26.49 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.SecretsManager 1.26.89 service generated with"
+        " mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

