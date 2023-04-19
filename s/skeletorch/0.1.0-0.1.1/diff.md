# Comparing `tmp/skeletorch-0.1.0.tar.gz` & `tmp/skeletorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletorch-0.1.0.tar", last modified: Wed Apr 19 10:21:34 2023, max compression
+gzip compressed data, was "skeletorch-0.1.1.tar", last modified: Wed Apr 19 17:23:44 2023, max compression
```

## Comparing `skeletorch-0.1.0.tar` & `skeletorch-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:21:34.117985 skeletorch-0.1.0/
--rw-rw-rw-   0        0        0     1089 2023-04-18 01:31:12.000000 skeletorch-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-04-19 10:03:27.000000 skeletorch-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      914 2023-04-19 10:21:34.116360 skeletorch-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-04-19 10:01:48.000000 skeletorch-0.1.0/README.md
--rw-rw-rw-   0        0        0      208 2023-04-19 10:21:25.000000 skeletorch-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 10:21:34.117985 skeletorch-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-04-19 10:01:31.000000 skeletorch-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:21:34.037652 skeletorch-0.1.0/skeletorch/
--rw-rw-rw-   0        0        0      255 2023-04-19 09:58:26.000000 skeletorch-0.1.0/skeletorch/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-04-19 09:27:05.000000 skeletorch-0.1.0/skeletorch/skeletorch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:21:34.114767 skeletorch-0.1.0/skeletorch.egg-info/
--rw-rw-rw-   0        0        0      914 2023-04-19 10:21:33.000000 skeletorch-0.1.0/skeletorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-19 10:21:33.000000 skeletorch-0.1.0/skeletorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:21:33.000000 skeletorch-0.1.0/skeletorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2023-04-19 10:21:33.000000 skeletorch-0.1.0/skeletorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 10:21:33.000000 skeletorch-0.1.0/skeletorch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 17:23:44.438110 skeletorch-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-18 01:31:12.000000 skeletorch-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-04-19 10:03:27.000000 skeletorch-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2499 2023-04-19 17:23:44.435534 skeletorch-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1599 2023-04-19 17:20:30.000000 skeletorch-0.1.1/README.md
+-rw-rw-rw-   0        0        0      208 2023-04-19 10:21:25.000000 skeletorch-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:23:44.438110 skeletorch-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1344 2023-04-19 17:17:28.000000 skeletorch-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:23:44.416561 skeletorch-0.1.1/skeletorch/
+-rw-rw-rw-   0        0        0      255 2023-04-19 09:58:26.000000 skeletorch-0.1.1/skeletorch/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-04-19 09:27:05.000000 skeletorch-0.1.1/skeletorch/skeletorch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:23:44.433534 skeletorch-0.1.1/skeletorch.egg-info/
+-rw-rw-rw-   0        0        0     2499 2023-04-19 17:23:44.000000 skeletorch-0.1.1/skeletorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-19 17:23:44.000000 skeletorch-0.1.1/skeletorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:23:44.000000 skeletorch-0.1.1/skeletorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-04-19 17:23:44.000000 skeletorch-0.1.1/skeletorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 17:23:44.000000 skeletorch-0.1.1/skeletorch.egg-info/top_level.txt
```

### Comparing `skeletorch-0.1.0/LICENSE` & `skeletorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletorch-0.1.0/setup.py` & `skeletorch-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     return [name.rstrip() for name in open(path.join(root_dir, 'requirements.txt'), encoding="utf-8-sig").readlines()]
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=package_name,
-    description='Punycode Converter Library for Python',
-    version='0.1.0',
+    description='Pytorch implementation of skeleton transformer module',
+    version='0.1.1',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Yutsuro/skeleton-transformer-Pytorch',
     author='Yutsuro',
     author_email='Yuki@utsu.ro',
     license='MIT',
     keywords='Skeleton-Transformer Python Pytorch Action-Recognition Skeleton Pose-Estimation',
```

### Comparing `skeletorch-0.1.0/skeletorch/skeletorch.py` & `skeletorch-0.1.1/skeletorch/skeletorch.py`

 * *Files identical despite different names*

