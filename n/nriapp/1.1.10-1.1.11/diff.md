# Comparing `tmp/nriapp-1.1.10.tar.gz` & `tmp/nriapp-1.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.10.tar", last modified: Wed Apr 19 14:05:54 2023, max compression
+gzip compressed data, was "nriapp-1.1.11.tar", last modified: Wed Apr 19 14:12:41 2023, max compression
```

## Comparing `nriapp-1.1.10.tar` & `nriapp-1.1.11.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.10/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.10/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-04-19 14:05:54.530306 nriapp-1.1.10/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.10/README
--rw-rw-rw-   0        0        0      287 2023-03-02 08:33:05.000000 nriapp-1.1.10/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 14:05:54.545906 nriapp-1.1.10/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-04-19 14:01:24.000000 nriapp-1.1.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.483506 nriapp-1.1.10/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.10/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    13766 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    25825 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.530306 nriapp-1.1.10/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.10/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/helper/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:05:54.514706 nriapp-1.1.10/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-04-19 14:05:54.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 14:05:53.000000 nriapp-1.1.10/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.10/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.133888 nriapp-1.1.11/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.11/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.11/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-04-19 14:12:41.133888 nriapp-1.1.11/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.11/README
+-rw-rw-rw-   0        0        0      336 2023-04-19 14:12:28.000000 nriapp-1.1.11/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 14:12:41.133888 nriapp-1.1.11/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-04-19 14:12:29.000000 nriapp-1.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.102688 nriapp-1.1.11/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.11/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    13766 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    25825 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.133888 nriapp-1.1.11/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/visualization.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.10/LICENSE` & `nriapp-1.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/setup.py` & `nriapp-1.1.11/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.10',
+   version='1.1.11',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.10/src/nriapp/changelog.txt` & `nriapp-1.1.11/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.11/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.11/src/nriapp/core/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.11/src/nriapp/core/msgraphapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.11/src/nriapp/core/mssentinelapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/multifactor.py` & `nriapp-1.1.11/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/core/vtquery.py` & `nriapp-1.1.11/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/helper/doc.py` & `nriapp-1.1.11/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/helper/login.py` & `nriapp-1.1.11/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/helper/pylog.py` & `nriapp-1.1.11/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/helper/requestheader.py` & `nriapp-1.1.11/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.11/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.10/src/nriapp/nriapp.py` & `nriapp-1.1.11/src/nriapp/nriapp.py`

 * *Files identical despite different names*

