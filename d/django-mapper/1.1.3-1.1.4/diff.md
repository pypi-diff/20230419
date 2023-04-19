# Comparing `tmp/django-mapper-1.1.3.tar.gz` & `tmp/django-mapper-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.3.tar", last modified: Tue Apr 18 05:46:00 2023, max compression
+gzip compressed data, was "django-mapper-1.1.4.tar", last modified: Wed Apr 19 08:00:25 2023, max compression
```

## Comparing `django-mapper-1.1.3.tar` & `django-mapper-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:46:00.863100 django-mapper-1.1.3/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.3/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.3/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2805 2023-04-18 05:10:47.000000 django-mapper-1.1.3/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-18 05:46:00.863100 django-mapper-1.1.3/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-18 05:46:00.000000 django-mapper-1.1.3/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-18 05:46:00.863100 django-mapper-1.1.3/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-18 05:44:16.000000 django-mapper-1.1.3/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.461548 django-mapper-1.1.4/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-19 08:00:25.461548 django-mapper-1.1.4/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.4/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.457548 django-mapper-1.1.4/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.4/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     4532 2023-04-19 07:59:30.000000 django-mapper-1.1.4/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-19 08:00:25.461548 django-mapper-1.1.4/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-19 08:00:25.000000 django-mapper-1.1.4/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-19 08:00:25.461548 django-mapper-1.1.4/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-19 07:59:46.000000 django-mapper-1.1.4/setup.py
```

### Comparing `django-mapper-1.1.3/PKG-INFO` & `django-mapper-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.3
+Version: 1.1.4
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.3/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.4/django_mapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.3
+Version: 1.1.4
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.3/setup.py` & `django-mapper-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.3',
+    version='1.1.4',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

