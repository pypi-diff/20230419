# Comparing `tmp/mypy-boto3-comprehend-1.26.81.tar.gz` & `tmp/mypy-boto3-comprehend-1.26.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehend-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehend-1.26.99.tar", last modified: Fri Mar 24 19:32:25 2023, max compression
```

## Comparing `mypy-boto3-comprehend-1.26.81.tar` & `mypy-boto3-comprehend-1.26.99.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.534319 mypy-boto3-comprehend-1.26.81/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27488 2023-02-28 20:28:07.526319 mypy-boto3-comprehend-1.26.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25989 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.526319 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67076 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66975 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-02-28 20:26:59.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97399 2023-02-28 20:27:01.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-02-28 20:27:01.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.526319 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27488 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-28 20:28:07.000000 mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.534319 mypy-boto3-comprehend-1.26.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-28 20:26:58.000000 mypy-boto3-comprehend-1.26.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-03-24 19:32:05.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-03-24 19:32:04.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97427 2023-03-24 19:32:07.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97352 2023-03-24 19:32:05.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 19:32:25.000000 mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:25.581893 mypy-boto3-comprehend-1.26.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-24 19:32:03.000000 mypy-boto3-comprehend-1.26.99/setup.py
```

### Comparing `mypy-boto3-comprehend-1.26.81/LICENSE` & `mypy-boto3-comprehend-1.26.99/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-comprehend-1.26.81/PKG-INFO` & `mypy-boto3-comprehend-1.26.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.26.81
-Summary: Type annotations for boto3.Comprehend 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.99
+Summary: Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -680,42 +680,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehend-1.26.81/README.md` & `mypy-boto3-comprehend-1.26.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -648,42 +648,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__init__.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__init__.pyi` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/__main__.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Comprehend 1.26.81\nVersion:         1.26.81\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Comprehend 1.26.99\nVersion:         1.26.99\nBuilder version:"
+        " 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.81")
+    print("1.26.99")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/client.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         """
 
     def batch_detect_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns an inference of the prevailing
-        sentiment, `POSITIVE` , `NEUTRAL` , `MIXED` , or `NEGATIVE` , in each one.
+        sentiment, `POSITIVE`, `NEUTRAL`, `MIXED`, or `NEGATIVE`, in each one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_sentiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#batch_detect_sentiment)
         """
 
     def batch_detect_syntax(
         self, *, TextList: Sequence[str], LanguageCode: SyntaxLanguageCodeType
@@ -403,16 +403,16 @@
         TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
         DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
-        A flywheel is an AWS resource that orchestrates the ongoing training of a model
-        for custom classification or custom entity recognition.
+        A flywheel is an Amazon Web Services resource that orchestrates the ongoing
+        training of a model for custom classification or custom entity recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#create_flywheel)
         """
 
     def delete_document_classifier(self, *, DocumentClassifierArn: str) -> Dict[str, Any]:
         """
@@ -658,16 +658,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_pii_entities)
         """
 
     def detect_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectSentimentResponseTypeDef:
         """
-        Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`
-        , `NEUTRAL` , `MIXED` , or `NEGATIVE` ).
+        Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`,
+        `NEUTRAL`, `MIXED`, or `NEGATIVE`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_sentiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_sentiment)
         """
 
     def detect_syntax(
         self, *, Text: str, LanguageCode: SyntaxLanguageCodeType
@@ -727,15 +727,15 @@
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDatasetsResponseTypeDef:
         """
-        List the datasets that you have configured in this region.
+        List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#list_datasets)
         """
 
     def list_document_classification_jobs(
         self,
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/client.pyi` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#batch_detect_key_phrases)
         """
     def batch_detect_sentiment(
         self, *, TextList: Sequence[str], LanguageCode: LanguageCodeType
     ) -> BatchDetectSentimentResponseTypeDef:
         """
         Inspects a batch of documents and returns an inference of the prevailing
-        sentiment, `POSITIVE` , `NEUTRAL` , `MIXED` , or `NEGATIVE` , in each one.
+        sentiment, `POSITIVE`, `NEUTRAL`, `MIXED`, or `NEGATIVE`, in each one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_sentiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#batch_detect_sentiment)
         """
     def batch_detect_syntax(
         self, *, TextList: Sequence[str], LanguageCode: SyntaxLanguageCodeType
     ) -> BatchDetectSyntaxResponseTypeDef:
@@ -384,16 +384,16 @@
         TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
         DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
-        A flywheel is an AWS resource that orchestrates the ongoing training of a model
-        for custom classification or custom entity recognition.
+        A flywheel is an Amazon Web Services resource that orchestrates the ongoing
+        training of a model for custom classification or custom entity recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#create_flywheel)
         """
     def delete_document_classifier(self, *, DocumentClassifierArn: str) -> Dict[str, Any]:
         """
         Deletes a previously created document classifier Only those classifiers that are
@@ -613,16 +613,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_pii_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_pii_entities)
         """
     def detect_sentiment(
         self, *, Text: str, LanguageCode: LanguageCodeType
     ) -> DetectSentimentResponseTypeDef:
         """
-        Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`
-        , `NEUTRAL` , `MIXED` , or `NEGATIVE` ).
+        Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`,
+        `NEUTRAL`, `MIXED`, or `NEGATIVE`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_sentiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#detect_sentiment)
         """
     def detect_syntax(
         self, *, Text: str, LanguageCode: SyntaxLanguageCodeType
     ) -> DetectSyntaxResponseTypeDef:
@@ -677,15 +677,15 @@
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDatasetsResponseTypeDef:
         """
-        List the datasets that you have configured in this region.
+        List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/client/#list_datasets)
         """
     def list_document_classification_jobs(
         self,
         *,
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/literals.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,22 @@
 ListEntitiesDetectionJobsPaginatorName = Literal["list_entities_detection_jobs"]
 ListEntityRecognizersPaginatorName = Literal["list_entity_recognizers"]
 ListKeyPhrasesDetectionJobsPaginatorName = Literal["list_key_phrases_detection_jobs"]
 ListPiiEntitiesDetectionJobsPaginatorName = Literal["list_pii_entities_detection_jobs"]
 ListSentimentDetectionJobsPaginatorName = Literal["list_sentiment_detection_jobs"]
 ListTopicsDetectionJobsPaginatorName = Literal["list_topics_detection_jobs"]
 ModelStatusType = Literal[
-    "DELETING", "IN_ERROR", "STOPPED", "STOP_REQUESTED", "SUBMITTED", "TRAINED", "TRAINING"
+    "DELETING",
+    "IN_ERROR",
+    "STOPPED",
+    "STOP_REQUESTED",
+    "SUBMITTED",
+    "TRAINED",
+    "TRAINED_WITH_WARNING",
+    "TRAINING",
 ]
 ModelTypeType = Literal["DOCUMENT_CLASSIFIER", "ENTITY_RECOGNIZER"]
 PageBasedErrorCodeType = Literal[
     "INTERNAL_SERVER_ERROR",
     "PAGE_CHARACTERS_EXCEEDED",
     "PAGE_SIZE_EXCEEDED",
     "TEXTRACT_BAD_PAGE",
@@ -383,14 +390,15 @@
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

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/literals.pyi` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,22 @@
 ListEntitiesDetectionJobsPaginatorName = Literal["list_entities_detection_jobs"]
 ListEntityRecognizersPaginatorName = Literal["list_entity_recognizers"]
 ListKeyPhrasesDetectionJobsPaginatorName = Literal["list_key_phrases_detection_jobs"]
 ListPiiEntitiesDetectionJobsPaginatorName = Literal["list_pii_entities_detection_jobs"]
 ListSentimentDetectionJobsPaginatorName = Literal["list_sentiment_detection_jobs"]
 ListTopicsDetectionJobsPaginatorName = Literal["list_topics_detection_jobs"]
 ModelStatusType = Literal[
-    "DELETING", "IN_ERROR", "STOPPED", "STOP_REQUESTED", "SUBMITTED", "TRAINED", "TRAINING"
+    "DELETING",
+    "IN_ERROR",
+    "STOPPED",
+    "STOP_REQUESTED",
+    "SUBMITTED",
+    "TRAINED",
+    "TRAINED_WITH_WARNING",
+    "TRAINING",
 ]
 ModelTypeType = Literal["DOCUMENT_CLASSIFIER", "ENTITY_RECOGNIZER"]
 PageBasedErrorCodeType = Literal[
     "INTERNAL_SERVER_ERROR",
     "PAGE_CHARACTERS_EXCEEDED",
     "PAGE_SIZE_EXCEEDED",
     "TEXTRACT_BAD_PAGE",
@@ -381,14 +388,15 @@
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

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/paginator.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/paginator.pyi` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/type_defs.py` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2621,14 +2621,15 @@
         "EntityRecognizerArn": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
 EventsDetectionJobPropertiesTypeDef = TypedDict(
     "EventsDetectionJobPropertiesTypeDef",
     {
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend/type_defs.pyi` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2574,14 +2574,15 @@
         "EntityRecognizerArn": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
 EventsDetectionJobPropertiesTypeDef = TypedDict(
     "EventsDetectionJobPropertiesTypeDef",
     {
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/PKG-INFO` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.26.81
-Summary: Type annotations for boto3.Comprehend 1.26.81 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.99
+Summary: Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -680,42 +680,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehend-1.26.81/mypy_boto3_comprehend.egg-info/SOURCES.txt` & `mypy-boto3-comprehend-1.26.99/mypy_boto3_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.26.81/setup.py` & `mypy-boto3-comprehend-1.26.99/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-comprehend.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehend",
-    version="1.26.81",
+    version="1.26.99",
     packages=["mypy_boto3_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Comprehend 1.26.81 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.Comprehend 1.26.99 service generated with mypy-boto3-builder"
+        " 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

