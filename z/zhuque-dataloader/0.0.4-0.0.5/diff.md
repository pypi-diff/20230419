# Comparing `tmp/zhuque-dataloader-0.0.4.tar.gz` & `tmp/zhuque-dataloader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.0.4.tar", last modified: Wed Apr 19 09:33:05 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.0.5.tar", last modified: Wed Apr 19 09:42:41 2023, max compression
```

## Comparing `zhuque-dataloader-0.0.4.tar` & `zhuque-dataloader-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:33:05.526514 zhuque-dataloader-0.0.4/
--rw-rw-rw-   0        0        0      192 2023-04-19 09:33:05.525515 zhuque-dataloader-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13435 2023-04-19 07:33:46.000000 zhuque-dataloader-0.0.4/loader.py
--rw-rw-rw-   0        0        0       42 2023-04-19 09:33:05.526514 zhuque-dataloader-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-04-19 09:32:35.000000 zhuque-dataloader-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:33:05.523515 zhuque-dataloader-0.0.4/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-19 09:33:05.000000 zhuque-dataloader-0.0.4/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-19 09:33:05.000000 zhuque-dataloader-0.0.4/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:33:05.000000 zhuque-dataloader-0.0.4/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 09:33:05.000000 zhuque-dataloader-0.0.4/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 09:42:41.992579 zhuque-dataloader-0.0.5/
+-rw-rw-rw-   0        0        0      192 2023-04-19 09:42:41.991579 zhuque-dataloader-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13435 2023-04-19 07:33:46.000000 zhuque-dataloader-0.0.5/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:42:41.992579 zhuque-dataloader-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-19 09:42:21.000000 zhuque-dataloader-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:42:41.989579 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/top_level.txt
```

### Comparing `zhuque-dataloader-0.0.4/loader.py` & `zhuque-dataloader-0.0.5/loader.py`

 * *Files identical despite different names*

### Comparing `zhuque-dataloader-0.0.4/setup.py` & `zhuque-dataloader-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhuque-dataloader',
-    version='0.0.4',
+    version='0.0.5',
     description='zhuque graph platform dataloader component',
     author='yanrisheng',
     author_email='yanrs@zhejianglab.com',
     packages=find_packages(),
     py_modules=['loader'],
     requires=[],  # 定义依赖
     license='GPL 3.0'
```

