# Comparing `tmp/abuscom-libs-0.1.4.tar.gz` & `tmp/abuscom-libs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.4.tar", last modified: Thu Apr 13 12:25:29 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.5.tar", last modified: Wed Apr 19 09:18:34 2023, max compression
```

## Comparing `abuscom-libs-0.1.4.tar` & `abuscom-libs-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.272921 abuscom-libs-0.1.4/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-13 12:25:29.272547 abuscom-libs-0.1.4/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.4/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.262384 abuscom-libs-0.1.4/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.269010 abuscom-libs-0.1.4/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.4/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     1359 2023-02-21 13:45:27.000000 abuscom-libs-0.1.4/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.4/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5983 2023-04-07 09:46:30.000000 abuscom-libs-0.1.4/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.4/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.4/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-13 12:25:29.271978 abuscom-libs-0.1.4/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-13 12:25:28.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-13 12:25:28.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-13 12:25:29.000000 abuscom-libs-0.1.4/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-13 12:25:29.273030 abuscom-libs-0.1.4/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-13 12:24:19.000000 abuscom-libs-0.1.4/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.939946 abuscom-libs-0.1.5/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-19 09:18:34.939512 abuscom-libs-0.1.5/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.5/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.928371 abuscom-libs-0.1.5/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.935422 abuscom-libs-0.1.5/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.5/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.5/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.5/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5983 2023-04-07 09:46:30.000000 abuscom-libs-0.1.5/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.5/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.5/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.938708 abuscom-libs-0.1.5/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-19 09:18:34.940172 abuscom-libs-0.1.5/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-19 09:17:30.000000 abuscom-libs-0.1.5/setup.py
```

### Comparing `abuscom-libs-0.1.4/README.md` & `abuscom-libs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.4/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.5/abuscom/connectors/hubspot.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.4/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.5/abuscom/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.4/abuscom/connectors/planio.py` & `abuscom-libs-0.1.5/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.4/abuscom/connectors/postgres.py` & `abuscom-libs-0.1.5/abuscom/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.4/setup.py` & `abuscom-libs-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.4',
+    version='0.1.5',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

