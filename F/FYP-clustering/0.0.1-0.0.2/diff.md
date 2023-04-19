# Comparing `tmp/FYP_clustering-0.0.1.tar.gz` & `tmp/FYP_clustering-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FYP_clustering-0.0.1.tar", last modified: Wed Apr 19 14:36:53 2023, max compression
+gzip compressed data, was "dist\FYP_clustering-0.0.2.tar", last modified: Wed Apr 19 14:45:10 2023, max compression
```

## Comparing `FYP_clustering-0.0.1.tar` & `FYP_clustering-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering/
--rw-rw-rw-   0        0        0       34 2023-04-12 07:20:29.000000 FYP_clustering-0.0.1/FYP_clustering/__init__.py
--rw-rw-rw-   0        0        0     8022 2023-04-12 07:20:29.000000 FYP_clustering-0.0.1/FYP_clustering/mgp.py
--rw-rw-rw-   0        0        0     2027 2023-04-19 14:35:17.000000 FYP_clustering-0.0.1/FYP_clustering/test_gsdmm.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering.egg-info/
--rw-rw-rw-   0        0        0     1249 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/FYP_clustering.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1249 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-04-19 13:40:22.000000 FYP_clustering-0.0.1/README.md
--rw-rw-rw-   0        0        0      585 2023-04-19 04:12:37.000000 FYP_clustering-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:36:53.000000 FYP_clustering-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      506 2023-04-19 13:40:24.000000 FYP_clustering-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/FYP_clustering/
+-rw-rw-rw-   0        0        0    10051 2023-04-19 14:44:27.000000 FYP_clustering-0.0.2/FYP_clustering/FYP_clustering.py
+-rw-rw-rw-   0        0        0       34 2023-04-12 07:20:29.000000 FYP_clustering-0.0.2/FYP_clustering/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/FYP_clustering.egg-info/
+-rw-rw-rw-   0        0        0     1249 2023-04-19 14:45:09.000000 FYP_clustering-0.0.2/FYP_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/FYP_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:45:09.000000 FYP_clustering-0.0.2/FYP_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 14:45:09.000000 FYP_clustering-0.0.2/FYP_clustering.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1249 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-04-19 13:40:22.000000 FYP_clustering-0.0.2/README.md
+-rw-rw-rw-   0        0        0      585 2023-04-19 04:12:37.000000 FYP_clustering-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:45:10.000000 FYP_clustering-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-04-19 14:44:32.000000 FYP_clustering-0.0.2/setup.py
```

### Comparing `FYP_clustering-0.0.1/FYP_clustering.egg-info/PKG-INFO` & `FYP_clustering-0.0.2/FYP_clustering.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FYP-clustering
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://gitee.com/li-muquan/slgs1
 Author: slgs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: license.txt
```

### Comparing `FYP_clustering-0.0.1/PKG-INFO` & `FYP_clustering-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FYP_clustering
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://gitee.com/li-muquan/slgs1
 Author: slgs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: license.txt
```

### Comparing `FYP_clustering-0.0.1/README.md` & `FYP_clustering-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FYP_clustering-0.0.1/license.txt` & `FYP_clustering-0.0.2/license.txt`

 * *Files identical despite different names*

