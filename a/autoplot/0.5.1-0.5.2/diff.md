# Comparing `tmp/autoplot-0.5.1.tar.gz` & `tmp/autoplot-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplot-0.5.1.tar", last modified: Wed Apr 19 17:01:01 2023, max compression
+gzip compressed data, was "autoplot-0.5.2.tar", last modified: Wed Apr 19 17:08:01 2023, max compression
```

## Comparing `autoplot-0.5.1.tar` & `autoplot-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.5.1/LICENSE.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:01:01.231355 autoplot-0.5.1/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.5.1/README.rst
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      271 2023-04-19 17:00:38.000000 autoplot-0.5.1/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    22041 2023-04-19 17:00:38.000000 autoplot-0.5.1/autoplot/autoplot.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:01:01.231355 autoplot-0.5.1/autoplot.egg-info/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/requires.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-19 17:01:01.000000 autoplot-0.5.1/autoplot.egg-info/top_level.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-19 17:01:01.231355 autoplot-0.5.1/setup.cfg
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-19 17:00:38.000000 autoplot-0.5.1/setup.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.5.2/LICENSE.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:08:01.994746 autoplot-0.5.2/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.5.2/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      271 2023-04-19 17:00:38.000000 autoplot-0.5.2/autoplot/__init__.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    22041 2023-04-19 17:06:47.000000 autoplot-0.5.2/autoplot/autoplot.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-19 17:08:01.994746 autoplot-0.5.2/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-19 17:07:08.000000 autoplot-0.5.2/setup.py
```

### Comparing `autoplot-0.5.1/LICENSE.txt` & `autoplot-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoplot-0.5.1/PKG-INFO` & `autoplot-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: autoplot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
 Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
         Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
```

### Comparing `autoplot-0.5.1/README.rst` & `autoplot-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `autoplot-0.5.1/autoplot/autoplot.py` & `autoplot-0.5.2/autoplot/autoplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import print_function
 
 
 def version():
-    return '0.4.1'
+    return '0.5.2'
 
 
 def printNoNewline(s):
     print(s, end=' ')
 
 
 def javaaddpath(url='', jdwpPort=-1):
```

### Comparing `autoplot-0.5.1/autoplot.egg-info/PKG-INFO` & `autoplot-0.5.2/autoplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: autoplot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
 Description: Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
         Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
```

### Comparing `autoplot-0.5.1/setup.py` & `autoplot-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.5.1',
+    version='0.5.2',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
     url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
```

