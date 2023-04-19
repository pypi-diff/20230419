# Comparing `tmp/python-outbreak-info-1.0.tar.gz` & `tmp/python_outbreak_info-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-outbreak-info-1.0.tar", last modified: Sun Apr 16 12:45:40 2023, max compression
+gzip compressed data, was "python_outbreak_info-1.0.1.tar", last modified: Wed Apr 19 14:18:08 2023, max compression
```

## Comparing `python-outbreak-info-1.0.tar` & `python_outbreak_info-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-16 12:45:40.895733 python-outbreak-info-1.0/
--rw-r--r--   0 josh       (501) staff       (20)     1079 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/LICENSE.md
--rw-r--r--   0 josh       (501) staff       (20)      942 2023-04-16 12:45:40.895810 python-outbreak-info-1.0/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      609 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/README.md
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-16 12:45:40.893635 python-outbreak-info-1.0/outbreak_tools/
--rw-r--r--   0 josh       (501) staff       (20)        0 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/outbreak_tools/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     5511 2023-04-16 12:42:15.000000 python-outbreak-info-1.0/outbreak_tools/outbreak_tools.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-16 12:45:40.894540 python-outbreak-info-1.0/python_outbreak_info.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      942 2023-04-16 12:45:40.000000 python-outbreak-info-1.0/python_outbreak_info.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      420 2023-04-16 12:45:40.000000 python-outbreak-info-1.0/python_outbreak_info.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-04-16 12:45:40.000000 python-outbreak-info-1.0/python_outbreak_info.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)       22 2023-04-16 12:45:40.000000 python-outbreak-info-1.0/python_outbreak_info.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       21 2023-04-16 12:45:40.000000 python-outbreak-info-1.0/python_outbreak_info.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)      106 2023-04-16 12:45:40.896143 python-outbreak-info-1.0/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      966 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-16 12:45:40.895542 python-outbreak-info-1.0/tests/
--rw-r--r--   0 josh       (501) staff       (20)       26 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4588 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/tests/replace_test_data.py
--rw-r--r--   0 josh       (501) staff       (20)    12952 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/tests/test_outbreak_data.py
--rw-r--r--   0 josh       (501) staff       (20)      307 2023-04-05 02:41:54.000000 python-outbreak-info-1.0/tests/test_outbreak_tools.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 14:18:08.208838 python_outbreak_info-1.0.1/
+-rw-r--r--   0 josh       (501) staff       (20)     1079 2023-04-05 02:41:54.000000 python_outbreak_info-1.0.1/LICENSE.md
+-rw-r--r--   0 josh       (501) staff       (20)      944 2023-04-19 14:18:08.208915 python_outbreak_info-1.0.1/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      609 2023-04-05 02:41:54.000000 python_outbreak_info-1.0.1/README.md
+-rw-r--r--   0 josh       (501) staff       (20)      106 2023-04-19 14:18:08.209240 python_outbreak_info-1.0.1/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)     1008 2023-04-19 14:17:40.000000 python_outbreak_info-1.0.1/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 14:18:08.205803 python_outbreak_info-1.0.1/src/
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 14:18:08.207148 python_outbreak_info-1.0.1/src/outbreak_data/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2023-04-18 09:46:21.000000 python_outbreak_info-1.0.1/src/outbreak_data/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     5476 2023-04-05 02:41:54.000000 python_outbreak_info-1.0.1/src/outbreak_data/authenticate_user.py
+-rw-r--r--   0 josh       (501) staff       (20)    25020 2023-04-18 19:32:38.000000 python_outbreak_info-1.0.1/src/outbreak_data/outbreak_data.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 14:18:08.207787 python_outbreak_info-1.0.1/src/outbreak_tools/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2023-04-05 02:41:54.000000 python_outbreak_info-1.0.1/src/outbreak_tools/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     5511 2023-04-16 12:42:15.000000 python_outbreak_info-1.0.1/src/outbreak_tools/outbreak_tools.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 14:18:08.208714 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      944 2023-04-19 14:18:08.000000 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      450 2023-04-19 14:18:08.000000 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-04-19 14:18:08.000000 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       22 2023-04-19 14:18:08.000000 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       29 2023-04-19 14:18:08.000000 python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/top_level.txt
```

### Comparing `python-outbreak-info-1.0/LICENSE.md` & `python_outbreak_info-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-outbreak-info-1.0/PKG-INFO` & `python_outbreak_info-1.0.1/src/python_outbreak_info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-outbreak-info
-Version: 1.0
+Version: 1.0.1
 Summary: Python interface to Outbreak.info, powered by GISAID
 Home-page: https://github.com/outbreak-info/python-outbreak-info
 Author: Outbreak.info dev team
 Author-email: lhughes@scripps.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `python-outbreak-info-1.0/README.md` & `python_outbreak_info-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-outbreak-info-1.0/outbreak_tools/outbreak_tools.py` & `python_outbreak_info-1.0.1/src/outbreak_tools/outbreak_tools.py`

 * *Files identical despite different names*

### Comparing `python-outbreak-info-1.0/python_outbreak_info.egg-info/PKG-INFO` & `python_outbreak_info-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-outbreak-info
-Version: 1.0
+Name: python_outbreak_info
+Version: 1.0.1
 Summary: Python interface to Outbreak.info, powered by GISAID
 Home-page: https://github.com/outbreak-info/python-outbreak-info
 Author: Outbreak.info dev team
 Author-email: lhughes@scripps.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `python-outbreak-info-1.0/setup.py` & `python_outbreak_info-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 
 description = ("Python interface to Outbreak.info,"
                " powered by GISAID")
 
 
 setup(
-    name="python-outbreak-info",
-    version="1.0",
-    packages=find_packages(),
+    name="python_outbreak_info",
+    version="1.0.1",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
     author="Outbreak.info dev team",
     license='MIT',
     author_email="lhughes@scripps.edu",
     url="https://github.com/outbreak-info/python-outbreak-info",
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
```

