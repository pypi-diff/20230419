# Comparing `tmp/linqex-1.3.tar.gz` & `tmp/linqex-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linqex-1.3.tar", last modified: Sun Mar 26 22:40:11 2023, max compression
+gzip compressed data, was "linqex-1.4.tar", last modified: Wed Apr 19 00:13:24 2023, max compression
```

## Comparing `linqex-1.3.tar` & `linqex-1.4.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 22:40:11.060973 linqex-1.3/
--rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.3/LICENSE
--rw-rw-rw-   0        0        0     4334 2023-03-26 22:40:11.059996 linqex-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3800 2023-03-26 21:48:17.000000 linqex-1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-26 22:40:11.017970 linqex-1.3/linqex/
--rw-rw-rw-   0        0        0       56 2023-03-26 15:26:10.000000 linqex-1.3/linqex/__init__.py
--rw-rw-rw-   0        0        0    12879 2023-03-26 21:37:18.000000 linqex-1.3/linqex/builds.py
--rw-rw-rw-   0        0        0    14212 2023-03-26 21:38:06.000000 linqex-1.3/linqex/linq.py
-drwxrwxrwx   0        0        0        0 2023-03-26 22:40:11.056970 linqex-1.3/linqex.egg-info/
--rw-rw-rw-   0        0        0     4334 2023-03-26 22:40:10.000000 linqex-1.3/linqex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-03-26 22:40:10.000000 linqex-1.3/linqex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 22:40:10.000000 linqex-1.3/linqex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-03-26 22:40:10.000000 linqex-1.3/linqex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 22:40:11.060973 linqex-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-03-26 22:30:12.000000 linqex-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 22:40:11.057968 linqex-1.3/tests/
--rw-rw-rw-   0        0        0      883 2023-03-24 16:37:26.000000 linqex-1.3/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.034762 linqex-1.4/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.4/LICENSE
+-rw-rw-rw-   0        0        0     4334 2023-04-19 00:13:24.033728 linqex-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3800 2023-03-26 21:48:17.000000 linqex-1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 00:13:23.982292 linqex-1.4/linqex/
+-rw-rw-rw-   0        0        0       55 2023-04-10 13:14:49.000000 linqex-1.4/linqex/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-04-18 21:14:02.000000 linqex-1.4/linqex/_typing.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.023729 linqex-1.4/linqex/build/
+-rw-rw-rw-   0        0        0      373 2023-04-10 13:52:19.000000 linqex-1.4/linqex/build/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-04-10 21:41:43.000000 linqex-1.4/linqex/build/iterablebase.py
+-rw-rw-rw-   0        0        0    15180 2023-04-18 23:38:32.000000 linqex-1.4/linqex/build/iterdictbase.py
+-rw-rw-rw-   0        0        0    13262 2023-04-18 23:25:08.000000 linqex-1.4/linqex/build/iterlistbase.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.031726 linqex-1.4/linqex/linq/
+-rw-rw-rw-   0        0        0      334 2023-04-10 13:52:07.000000 linqex-1.4/linqex/linq/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-04-10 21:41:47.000000 linqex-1.4/linqex/linq/iterable.py
+-rw-rw-rw-   0        0        0    15402 2023-04-18 23:19:40.000000 linqex-1.4/linqex/linq/iterdict.py
+-rw-rw-rw-   0        0        0    15046 2023-04-18 23:11:20.000000 linqex-1.4/linqex/linq/iterlist.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.015725 linqex-1.4/linqex.egg-info/
+-rw-rw-rw-   0        0        0     4334 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 00:13:24.035731 linqex-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2023-04-10 13:11:55.000000 linqex-1.4/setup.py
```

### Comparing `linqex-1.3/LICENSE` & `linqex-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linqex-1.3/PKG-INFO` & `linqex-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linqex
-Version: 1.3
+Version: 1.4
 Summary: The linq module in C# has been adapted for python with some modifications.
 Home-page: https://github.com/TahsinCr/python-linqex
 Author: TahsinCr
 Author-email: TahsinCr@outlook.com
 License: MIT
 Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: linqex Version: 1.3 Summary: The linq module in C#
+Metadata-Version: 2.1 Name: linqex Version: 1.4 Summary: The linq module in C#
 has been adapted for python with some modifications. Home-page: https://
 github.com/TahsinCr/python-linqex Author: TahsinCr Author-email:
 TahsinCr@outlook.com License: MIT Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE  [![Contributors][contributors-shield]][contributors-url] [![Forks]
```

### Comparing `linqex-1.3/README.rst` & `linqex-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `linqex-1.3/linqex.egg-info/PKG-INFO` & `linqex-1.4/linqex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linqex
-Version: 1.3
+Version: 1.4
 Summary: The linq module in C# has been adapted for python with some modifications.
 Home-page: https://github.com/TahsinCr/python-linqex
 Author: TahsinCr
 Author-email: TahsinCr@outlook.com
 License: MIT
 Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: linqex Version: 1.3 Summary: The linq module in C#
+Metadata-Version: 2.1 Name: linqex Version: 1.4 Summary: The linq module in C#
 has been adapted for python with some modifications. Home-page: https://
 github.com/TahsinCr/python-linqex Author: TahsinCr Author-email:
 TahsinCr@outlook.com License: MIT Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE  [![Contributors][contributors-shield]][contributors-url] [![Forks]
```

### Comparing `linqex-1.3/setup.py` & `linqex-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r', encoding='utf-8') as file:
     LONG_DESCRIPTION = file.read() 
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
 
 NAME = 'linqex'
-VERSION = '1.3'
+VERSION = '1.4'
 DESCRIPTION = 'The linq module in C# has been adapted for python with some modifications.'
 URL = 'https://github.com/TahsinCr/python-linqex'
 AUTHOR = 'TahsinCr'
 AUTHOR_EMAIL = 'TahsinCr@outlook.com'
 LICENSE = 'MIT'
 KEYWORDS = ['linq', 'linqex', 'ex', 'enumerable']
 SRC = 'linqex'
```

