# Comparing `tmp/mypy-boto3-s3-1.26.97.post3.tar.gz` & `tmp/mypy-boto3-s3-1.26.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.26.97.post3.tar", last modified: Mon Mar 27 17:39:29 2023, max compression
+gzip compressed data, was "mypy-boto3-s3-1.26.99.tar", last modified: Mon Mar 27 17:41:27 2023, max compression
```

## Comparing `mypy-boto3-s3-1.26.97.post3.tar` & `mypy-boto3-s3-1.26.99.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:39:29.404349 mypy-boto3-s3-1.26.97.post3/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33971 2023-03-27 17:39:29.404349 mypy-boto3-s3-1.26.97.post3/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    32498 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:39:29.404349 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2283 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2281 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      899 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    83389 2023-03-27 17:39:08.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    83270 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16183 2023-03-27 17:39:11.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16181 2023-03-27 17:39:11.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6978 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6970 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   117341 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   117125 2023-03-27 17:39:09.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   183478 2023-03-27 17:39:18.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   183166 2023-03-27 17:39:15.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5328 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5323 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:39:29.404349 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33971 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      703 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       14 2023-03-27 17:39:29.000000 mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-03-27 17:39:29.404349 mypy-boto3-s3-1.26.97.post3/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1956 2023-03-27 17:39:05.000000 mypy-boto3-s3-1.26.97.post3/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:41:27.812687 mypy-boto3-s3-1.26.99/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.99/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33965 2023-03-27 17:41:27.812687 mypy-boto3-s3-1.26.99/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32498 2023-03-27 17:41:06.000000 mypy-boto3-s3-1.26.99/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:41:27.812687 mypy-boto3-s3-1.26.99/mypy_boto3_s3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2283 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2281 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-03-27 17:41:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83389 2023-03-27 17:39:08.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83270 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16203 2023-03-27 17:41:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16201 2023-03-27 17:41:09.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6978 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6970 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:39:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   117341 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   117125 2023-03-27 17:39:09.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   183478 2023-03-27 17:39:18.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   183166 2023-03-27 17:39:15.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-03-27 17:41:06.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5328 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5323 2023-03-27 17:39:10.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-27 17:41:27.812687 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33965 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      703 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       14 2023-03-27 17:41:27.000000 mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-03-27 17:41:27.812687 mypy-boto3-s3-1.26.99/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1950 2023-03-27 17:41:05.000000 mypy-boto3-s3-1.26.99/setup.py
```

### Comparing `mypy-boto3-s3-1.26.97.post3/LICENSE` & `mypy-boto3-s3-1.26.99/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/PKG-INFO` & `mypy-boto3-s3-1.26.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.26.97.post3
-Summary: Type annotations for boto3.S3 1.26.97 service generated with mypy-boto3-builder 7.14.4
+Version: 1.26.99
+Summary: Type annotations for boto3.S3 1.26.99 service generated with mypy-boto3-builder 7.14.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3-1.26.97.post3/README.md` & `mypy-boto3-s3-1.26.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__init__.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__init__.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/__main__.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.26.97\nVersion:         1.26.97.post3\nBuilder version:"
+        "Type annotations for boto3.S3 1.26.99\nVersion:         1.26.99\nBuilder version:"
         " 7.14.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97.post3")
+    print("1.26.99")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/client.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/client.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/literals.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/literals.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/paginator.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/paginator.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/service_resource.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/service_resource.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/type_defs.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/type_defs.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/waiter.py` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3/waiter.pyi` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.26.97.post3
-Summary: Type annotations for boto3.S3 1.26.97 service generated with mypy-boto3-builder 7.14.4
+Version: 1.26.99
+Summary: Type annotations for boto3.S3 1.26.99 service generated with mypy-boto3-builder 7.14.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3-1.26.97.post3/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy-boto3-s3-1.26.99/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.26.97.post3/setup.py` & `mypy-boto3-s3-1.26.99/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.26.97.post3",
+    version="1.26.99",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3 1.26.97 service generated with mypy-boto3-builder 7.14.4"
+        "Type annotations for boto3.S3 1.26.99 service generated with mypy-boto3-builder 7.14.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

