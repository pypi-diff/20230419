# Comparing `tmp/ethraid-0.1.90.tar.gz` & `tmp/ethraid-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ethraid-0.1.90.tar", last modified: Tue Mar 21 23:49:07 2023, max compression
+gzip compressed data, was "dist/ethraid-1.0.0.tar", last modified: Wed Mar 22 17:11:05 2023, max compression
```

## Comparing `ethraid-0.1.90.tar` & `ethraid-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/
--rw-r--r--   0 judahvz    (501) staff       (20)      221 2023-03-17 18:23:27.000000 ethraid-0.1.90/MANIFEST.in
--rw-r--r--   0 judahvz    (501) staff       (20)      831 2023-03-21 23:49:07.000000 ethraid-0.1.90/PKG-INFO
--rw-r--r--   0 judahvz    (501) staff       (20)      656 2023-03-17 18:23:27.000000 ethraid-0.1.90/README.md
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/
--rw-r--r--   0 judahvz    (501) staff       (20)       83 2023-03-21 23:48:57.000000 ethraid-0.1.90/ethraid/__init__.py
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/c_kepler/
--rw-r--r--   0 judahvz    (501) staff       (20)        0 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/c_kepler/__init__.py
--rw-r--r--   0 judahvz    (501) staff       (20)   873411 2023-02-13 17:26:30.000000 ethraid-0.1.90/ethraid/c_kepler/_kepler.c
--rw-r--r--   0 judahvz    (501) staff       (20)     1562 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/c_kepler/_kepler.pyx
--rw-r--r--   0 judahvz    (501) staff       (20)     2315 2023-02-07 23:28:25.000000 ethraid-0.1.90/ethraid/c_kepler/kepler.c
--rw-r--r--   0 judahvz    (501) staff       (20)      211 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/c_kepler/radvel_requirements.txt
--rw-r--r--   0 judahvz    (501) staff       (20)     1546 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/c_kepler/radvel_setup.py
--rw-r--r--   0 judahvz    (501) staff       (20)     9706 2023-03-21 19:56:49.000000 ethraid-0.1.90/ethraid/cli.py
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/compiled/
--rwxr-xr-x   0 judahvz    (501) staff       (20)   181484 2023-03-10 18:17:42.000000 ethraid-0.1.90/ethraid/compiled/_kepler.cpython-37m-darwin.so
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/compiled/ethraid/
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/compiled/ethraid/c_kepler/
--rw-r--r--   0 judahvz    (501) staff       (20)   873796 2023-03-09 23:49:37.000000 ethraid-0.1.90/ethraid/compiled/ethraid/c_kepler/_kepler.c
--rw-r--r--   0 judahvz    (501) staff       (20)     2315 2023-02-07 23:28:25.000000 ethraid-0.1.90/ethraid/compiled/ethraid/c_kepler/kepler.c
--rw-r--r--   0 judahvz    (501) staff       (20)  1040969 2023-03-21 18:19:27.000000 ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_astro.c
--rw-r--r--   0 judahvz    (501) staff       (20)  1236710 2023-03-21 19:57:48.000000 ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_general.c
--rw-r--r--   0 judahvz    (501) staff       (20)   947428 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_rv.c
--rwxr-xr-x   0 judahvz    (501) staff       (20)   249080 2023-03-21 19:34:32.000000 ethraid-0.1.90/ethraid/compiled/helper_functions_astro.cpython-37m-darwin.so
--rwxr-xr-x   0 judahvz    (501) staff       (20)   385156 2023-03-21 19:57:53.000000 ethraid-0.1.90/ethraid/compiled/helper_functions_general.cpython-37m-darwin.so
--rwxr-xr-x   0 judahvz    (501) staff       (20)   214816 2023-03-21 23:39:48.000000 ethraid-0.1.90/ethraid/compiled/helper_functions_rv.cpython-37m-darwin.so
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid/data/
--rw-r--r--   0 judahvz    (501) staff       (20)     6148 2023-03-09 23:26:37.000000 ethraid-0.1.90/ethraid/data/.DS_Store
--rw-r--r--   0 judahvz    (501) staff       (20)      107 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/data/bands.csv
--rw-r--r--   0 judahvz    (501) staff       (20)     2078 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/data/baraffe_table_4.csv
--rw-r--r--   0 judahvz    (501) staff       (20)     6255 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/data/mamajek.csv
--rw-r--r--   0 judahvz    (501) staff       (20)     8895 2023-03-21 19:52:44.000000 ethraid-0.1.90/ethraid/driver.py
--rw-r--r--   0 judahvz    (501) staff       (20)    16663 2023-03-21 17:56:42.000000 ethraid-0.1.90/ethraid/helper_functions_astro.pyx
--rw-r--r--   0 judahvz    (501) staff       (20)    24041 2023-03-21 19:57:16.000000 ethraid-0.1.90/ethraid/helper_functions_general.pyx
--rw-r--r--   0 judahvz    (501) staff       (20)    11883 2023-03-16 23:32:11.000000 ethraid-0.1.90/ethraid/helper_functions_imaging.py
--rw-r--r--   0 judahvz    (501) staff       (20)     9603 2023-03-16 23:32:11.000000 ethraid-0.1.90/ethraid/helper_functions_plotting.py
--rw-r--r--   0 judahvz    (501) staff       (20)     8127 2023-03-21 23:45:57.000000 ethraid-0.1.90/ethraid/helper_functions_rv.pyx
--rw-r--r--   0 judahvz    (501) staff       (20)      308 2023-03-09 23:44:35.000000 ethraid-0.1.90/ethraid/kern_profiler_dummy.py
--rw-r--r--   0 judahvz    (501) staff       (20)    13647 2023-03-21 19:57:35.000000 ethraid-0.1.90/ethraid/load_save.py
--rw-r--r--   0 judahvz    (501) staff       (20)    12510 2023-03-21 17:56:42.000000 ethraid-0.1.90/ethraid/plotter.py
--rw-r--r--   0 judahvz    (501) staff       (20)      642 2023-03-17 18:23:27.000000 ethraid-0.1.90/ethraid/system_params.py
--rw-r--r--   0 judahvz    (501) staff       (20)     7739 2023-03-21 17:44:01.000000 ethraid-0.1.90/ethraid/system_params_local.py
-drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/
--rw-r--r--   0 judahvz    (501) staff       (20)      831 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/PKG-INFO
--rw-r--r--   0 judahvz    (501) staff       (20)     1349 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/SOURCES.txt
--rw-r--r--   0 judahvz    (501) staff       (20)        1 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/dependency_links.txt
--rw-r--r--   0 judahvz    (501) staff       (20)       45 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/entry_points.txt
--rw-r--r--   0 judahvz    (501) staff       (20)      164 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/requires.txt
--rw-r--r--   0 judahvz    (501) staff       (20)        8 2023-03-21 23:49:07.000000 ethraid-0.1.90/ethraid.egg-info/top_level.txt
--rw-r--r--   0 judahvz    (501) staff       (20)      164 2023-03-09 23:44:35.000000 ethraid-0.1.90/requirements.txt
--rw-r--r--   0 judahvz    (501) staff       (20)       38 2023-03-21 23:49:07.000000 ethraid-0.1.90/setup.cfg
--rw-r--r--   0 judahvz    (501) staff       (20)     3088 2023-03-15 17:29:43.000000 ethraid-0.1.90/setup.py
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/
+-rw-r--r--   0 judahvz    (501) staff       (20)      221 2023-03-17 18:23:27.000000 ethraid-1.0.0/MANIFEST.in
+-rw-r--r--   0 judahvz    (501) staff       (20)      922 2023-03-22 17:11:05.000000 ethraid-1.0.0/PKG-INFO
+-rw-r--r--   0 judahvz    (501) staff       (20)      748 2023-03-22 17:02:27.000000 ethraid-1.0.0/README.md
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/
+-rw-r--r--   0 judahvz    (501) staff       (20)       82 2023-03-22 17:06:00.000000 ethraid-1.0.0/ethraid/__init__.py
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/c_kepler/
+-rw-r--r--   0 judahvz    (501) staff       (20)        0 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/c_kepler/__init__.py
+-rw-r--r--   0 judahvz    (501) staff       (20)   873411 2023-02-13 17:26:30.000000 ethraid-1.0.0/ethraid/c_kepler/_kepler.c
+-rw-r--r--   0 judahvz    (501) staff       (20)     1562 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/c_kepler/_kepler.pyx
+-rw-r--r--   0 judahvz    (501) staff       (20)     2315 2023-02-07 23:28:25.000000 ethraid-1.0.0/ethraid/c_kepler/kepler.c
+-rw-r--r--   0 judahvz    (501) staff       (20)      211 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/c_kepler/radvel_requirements.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)     1546 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/c_kepler/radvel_setup.py
+-rw-r--r--   0 judahvz    (501) staff       (20)     9706 2023-03-22 00:09:56.000000 ethraid-1.0.0/ethraid/cli.py
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/compiled/
+-rwxr-xr-x   0 judahvz    (501) staff       (20)   181484 2023-03-10 18:17:42.000000 ethraid-1.0.0/ethraid/compiled/_kepler.cpython-37m-darwin.so
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/compiled/ethraid/
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/compiled/ethraid/c_kepler/
+-rw-r--r--   0 judahvz    (501) staff       (20)   873796 2023-03-09 23:49:37.000000 ethraid-1.0.0/ethraid/compiled/ethraid/c_kepler/_kepler.c
+-rw-r--r--   0 judahvz    (501) staff       (20)     2315 2023-02-07 23:28:25.000000 ethraid-1.0.0/ethraid/compiled/ethraid/c_kepler/kepler.c
+-rw-r--r--   0 judahvz    (501) staff       (20)  1040969 2023-03-21 18:19:27.000000 ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_astro.c
+-rw-r--r--   0 judahvz    (501) staff       (20)  1236710 2023-03-21 19:57:48.000000 ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_general.c
+-rw-r--r--   0 judahvz    (501) staff       (20)   947409 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_rv.c
+-rwxr-xr-x   0 judahvz    (501) staff       (20)   249080 2023-03-21 19:34:32.000000 ethraid-1.0.0/ethraid/compiled/helper_functions_astro.cpython-37m-darwin.so
+-rwxr-xr-x   0 judahvz    (501) staff       (20)   385156 2023-03-21 19:57:53.000000 ethraid-1.0.0/ethraid/compiled/helper_functions_general.cpython-37m-darwin.so
+-rwxr-xr-x   0 judahvz    (501) staff       (20)   214816 2023-03-22 00:09:03.000000 ethraid-1.0.0/ethraid/compiled/helper_functions_rv.cpython-37m-darwin.so
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid/data/
+-rw-r--r--   0 judahvz    (501) staff       (20)     6148 2023-03-09 23:26:37.000000 ethraid-1.0.0/ethraid/data/.DS_Store
+-rw-r--r--   0 judahvz    (501) staff       (20)      107 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/data/bands.csv
+-rw-r--r--   0 judahvz    (501) staff       (20)     2078 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/data/baraffe_table_4.csv
+-rw-r--r--   0 judahvz    (501) staff       (20)     6255 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/data/mamajek.csv
+-rw-r--r--   0 judahvz    (501) staff       (20)     8895 2023-03-22 00:09:56.000000 ethraid-1.0.0/ethraid/driver.py
+-rw-r--r--   0 judahvz    (501) staff       (20)    16663 2023-03-21 17:56:42.000000 ethraid-1.0.0/ethraid/helper_functions_astro.pyx
+-rw-r--r--   0 judahvz    (501) staff       (20)    24041 2023-03-21 19:57:16.000000 ethraid-1.0.0/ethraid/helper_functions_general.pyx
+-rw-r--r--   0 judahvz    (501) staff       (20)    11883 2023-03-16 23:32:11.000000 ethraid-1.0.0/ethraid/helper_functions_imaging.py
+-rw-r--r--   0 judahvz    (501) staff       (20)     9603 2023-03-16 23:32:11.000000 ethraid-1.0.0/ethraid/helper_functions_plotting.py
+-rw-r--r--   0 judahvz    (501) staff       (20)     8167 2023-03-22 00:09:56.000000 ethraid-1.0.0/ethraid/helper_functions_rv.pyx
+-rw-r--r--   0 judahvz    (501) staff       (20)      308 2023-03-09 23:44:35.000000 ethraid-1.0.0/ethraid/kern_profiler_dummy.py
+-rw-r--r--   0 judahvz    (501) staff       (20)    13647 2023-03-22 00:09:56.000000 ethraid-1.0.0/ethraid/load_save.py
+-rw-r--r--   0 judahvz    (501) staff       (20)    12510 2023-03-21 17:56:42.000000 ethraid-1.0.0/ethraid/plotter.py
+-rw-r--r--   0 judahvz    (501) staff       (20)      642 2023-03-17 18:23:27.000000 ethraid-1.0.0/ethraid/system_params.py
+-rw-r--r--   0 judahvz    (501) staff       (20)     7739 2023-03-21 17:44:01.000000 ethraid-1.0.0/ethraid/system_params_local.py
+drwxr-xr-x   0 judahvz    (501) staff       (20)        0 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid.egg-info/
+-rw-r--r--   0 judahvz    (501) staff       (20)      922 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid.egg-info/PKG-INFO
+-rw-r--r--   0 judahvz    (501) staff       (20)     1349 2023-03-22 17:11:05.000000 ethraid-1.0.0/ethraid.egg-info/SOURCES.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)        1 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid.egg-info/dependency_links.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)       45 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid.egg-info/entry_points.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)      164 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid.egg-info/requires.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)        8 2023-03-22 17:11:04.000000 ethraid-1.0.0/ethraid.egg-info/top_level.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)      164 2023-03-09 23:44:35.000000 ethraid-1.0.0/requirements.txt
+-rw-r--r--   0 judahvz    (501) staff       (20)       38 2023-03-22 17:11:05.000000 ethraid-1.0.0/setup.cfg
+-rw-r--r--   0 judahvz    (501) staff       (20)     3088 2023-03-15 17:29:43.000000 ethraid-1.0.0/setup.py
```

### Comparing `ethraid-0.1.90/PKG-INFO` & `ethraid-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethraid
-Version: 0.1.90
+Version: 1.0.0
 Summary: Command line application for trend code
 Home-page: 
 Author: Judah Van Zandt
 Author-email: judahvz@astro.ucla.edu
 
 
 # Trend Analysis
@@ -13,14 +13,15 @@
 ## Environment
 - Create new environment with python 3.7
 - *\$ conda create --name trends_env python=3.7*
 - *\$ conda activate trends_env*
 
 ## Download from Test PyPI (regular pip download coming soon)
 - *\$ python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple ethraid*
+- You may have to upgrade pip using *\$ curl https://bootstrap.pypa.io/get-pip.py | python*
 
 ## If downloading repo
 - Install dependencies using requirements.txt 
 - *\$ pip install -r requirements.txt*
 
 - Build code from top level of repo
 - *\$ cd trends/*
```

### Comparing `ethraid-0.1.90/README.md` & `ethraid-1.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## Environment
 - Create new environment with python 3.7
 - *\$ conda create --name trends_env python=3.7*
 - *\$ conda activate trends_env*
 
 ## Download from Test PyPI (regular pip download coming soon)
 - *\$ python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple ethraid*
+- You may have to upgrade pip using *\$ curl https://bootstrap.pypa.io/get-pip.py | python*
 
 ## If downloading repo
 - Install dependencies using requirements.txt 
 - *\$ pip install -r requirements.txt*
 
 - Build code from top level of repo
 - *\$ cd trends/*
```

### Comparing `ethraid-0.1.90/ethraid/c_kepler/_kepler.c` & `ethraid-1.0.0/ethraid/c_kepler/_kepler.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/c_kepler/_kepler.pyx` & `ethraid-1.0.0/ethraid/c_kepler/_kepler.pyx`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/c_kepler/kepler.c` & `ethraid-1.0.0/ethraid/c_kepler/kepler.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/c_kepler/radvel_setup.py` & `ethraid-1.0.0/ethraid/c_kepler/radvel_setup.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/cli.py` & `ethraid-1.0.0/ethraid/cli.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/_kepler.cpython-37m-darwin.so` & `ethraid-1.0.0/ethraid/compiled/_kepler.cpython-37m-darwin.so`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/ethraid/c_kepler/_kepler.c` & `ethraid-1.0.0/ethraid/compiled/ethraid/c_kepler/_kepler.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/ethraid/c_kepler/kepler.c` & `ethraid-1.0.0/ethraid/compiled/ethraid/c_kepler/kepler.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_astro.c` & `ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_astro.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_general.c` & `ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_general.c`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/ethraid/helper_functions_rv.c` & `ethraid-1.0.0/ethraid/compiled/ethraid/helper_functions_rv.c`

 * *Files 0% similar despite different names*

```diff
@@ -3997,122 +3997,122 @@
   __pyx_v_cos_E = cos(__pyx_v_E);
 
   /* "ethraid/helper_functions_rv.pyx":162
  * 
  *     cos_E = cos(E)
  *     sin_E = sin(E)             # <<<<<<<<<<<<<<
  * 
- *     ## Two-argument arctan function to avoid div by 0 when E=pi
+ *     #####################################
  */
   __pyx_v_sin_E = sin(__pyx_v_E);
 
-  /* "ethraid/helper_functions_rv.pyx":166
+  /* "ethraid/helper_functions_rv.pyx":167
  *     ## Two-argument arctan function to avoid div by 0 when E=pi
  *     ## Also replacing sin(E/2)/cos(E/2) with equivalent sinE/(1+cosE) to save calculation
  *     nu = 2*atan2(sqrt_eterm*sin_E, (1+cos_E))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_nu = (2.0 * atan2((__pyx_v_sqrt_eterm * __pyx_v_sin_E), (1.0 + __pyx_v_cos_E)));
 
-  /* "ethraid/helper_functions_rv.pyx":170
+  /* "ethraid/helper_functions_rv.pyx":171
  * 
  *     # nu derivatives use days (not seconds) to give gdot/gddot correct units
  *     nu_dot = two_pi*sqrt_e_sq_term/(per*(1-e*cos_E)**2) # Units of day^-1             # <<<<<<<<<<<<<<
- *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term ## Units of day^-2
+ *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term # # Units of day^-2
  * 
  */
   __pyx_t_2 = (__pyx_v_7ethraid_8compiled_19helper_functions_rv_two_pi * __pyx_v_sqrt_e_sq_term);
   __pyx_t_1 = (__pyx_v_per * pow((1.0 - (__pyx_v_e * __pyx_v_cos_E)), 2.0));
   if (unlikely(__pyx_t_1 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 170, __pyx_L1_error)
+    __PYX_ERR(0, 171, __pyx_L1_error)
   }
   __pyx_v_nu_dot = (__pyx_t_2 / __pyx_t_1);
 
-  /* "ethraid/helper_functions_rv.pyx":171
+  /* "ethraid/helper_functions_rv.pyx":172
  *     # nu derivatives use days (not seconds) to give gdot/gddot correct units
  *     nu_dot = two_pi*sqrt_e_sq_term/(per*(1-e*cos_E)**2) # Units of day^-1
- *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term ## Units of day^-2             # <<<<<<<<<<<<<<
+ *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term # # Units of day^-2             # <<<<<<<<<<<<<<
  * 
  *     cos_nu_om = cos(nu+om)
  */
   __pyx_t_1 = ((((-pow(__pyx_v_nu_dot, 2.0)) * 2.0) * __pyx_v_e) * __pyx_v_sin_E);
   if (unlikely(__pyx_v_sqrt_e_sq_term == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 171, __pyx_L1_error)
+    __PYX_ERR(0, 172, __pyx_L1_error)
   }
   __pyx_v_nu_ddot = (__pyx_t_1 / __pyx_v_sqrt_e_sq_term);
 
-  /* "ethraid/helper_functions_rv.pyx":173
- *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term ## Units of day^-2
+  /* "ethraid/helper_functions_rv.pyx":174
+ *     nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term # # Units of day^-2
  * 
  *     cos_nu_om = cos(nu+om)             # <<<<<<<<<<<<<<
  *     sin_nu_om = sin(nu+om)
  *     sin_i = sin(i)
  */
   __pyx_v_cos_nu_om = cos((__pyx_v_nu + __pyx_v_om));
 
-  /* "ethraid/helper_functions_rv.pyx":174
+  /* "ethraid/helper_functions_rv.pyx":175
  * 
  *     cos_nu_om = cos(nu+om)
  *     sin_nu_om = sin(nu+om)             # <<<<<<<<<<<<<<
  *     sin_i = sin(i)
  * 
  */
   __pyx_v_sin_nu_om = sin((__pyx_v_nu + __pyx_v_om));
 
-  /* "ethraid/helper_functions_rv.pyx":175
+  /* "ethraid/helper_functions_rv.pyx":176
  *     cos_nu_om = cos(nu+om)
  *     sin_nu_om = sin(nu+om)
  *     sin_i = sin(i)             # <<<<<<<<<<<<<<
  * 
  *     # Lovis+Fischer 2010 (analytic)
  */
   __pyx_v_sin_i = sin(__pyx_v_i);
 
-  /* "ethraid/helper_functions_rv.pyx":178
+  /* "ethraid/helper_functions_rv.pyx":179
  * 
  *     # Lovis+Fischer 2010 (analytic)
  *     pre_fac = sqrt(G)/sqrt_e_sq_term * m*sin_i/sqrt((m+m_star)*(a)) * auday2ms # AU/day ==> m/s             # <<<<<<<<<<<<<<
  * 
  *     gamma_dot = -pre_fac*nu_dot*sin_nu_om # m/s/day
  */
   __pyx_t_1 = sqrt(__pyx_v_7ethraid_8compiled_19helper_functions_rv_G);
   if (unlikely(__pyx_v_sqrt_e_sq_term == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 178, __pyx_L1_error)
+    __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_t_2 = (((__pyx_t_1 / __pyx_v_sqrt_e_sq_term) * __pyx_v_m) * __pyx_v_sin_i);
   __pyx_t_1 = sqrt(((__pyx_v_m + __pyx_v_m_star) * __pyx_v_a));
   if (unlikely(__pyx_t_1 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 178, __pyx_L1_error)
+    __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_v_pre_fac = ((__pyx_t_2 / __pyx_t_1) * __pyx_v_7ethraid_8compiled_19helper_functions_rv_auday2ms);
 
-  /* "ethraid/helper_functions_rv.pyx":180
+  /* "ethraid/helper_functions_rv.pyx":181
  *     pre_fac = sqrt(G)/sqrt_e_sq_term * m*sin_i/sqrt((m+m_star)*(a)) * auday2ms # AU/day ==> m/s
  * 
  *     gamma_dot = -pre_fac*nu_dot*sin_nu_om # m/s/day             # <<<<<<<<<<<<<<
  *     gamma_ddot = -pre_fac*(nu_dot**2*cos_nu_om + nu_ddot*sin_nu_om) # m/s/day/day
  * 
  */
   __pyx_v_gamma_dot = (((-__pyx_v_pre_fac) * __pyx_v_nu_dot) * __pyx_v_sin_nu_om);
 
-  /* "ethraid/helper_functions_rv.pyx":181
+  /* "ethraid/helper_functions_rv.pyx":182
  * 
  *     gamma_dot = -pre_fac*nu_dot*sin_nu_om # m/s/day
  *     gamma_ddot = -pre_fac*(nu_dot**2*cos_nu_om + nu_ddot*sin_nu_om) # m/s/day/day             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_gamma_ddot = ((-__pyx_v_pre_fac) * ((pow(__pyx_v_nu_dot, 2.0) * __pyx_v_cos_nu_om) + (__pyx_v_nu_ddot * __pyx_v_sin_nu_om)));
 
-  /* "ethraid/helper_functions_rv.pyx":184
+  /* "ethraid/helper_functions_rv.pyx":185
  * 
  * 
  *     return gamma_dot, gamma_ddot             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_3.f0 = __pyx_v_gamma_dot;
@@ -4290,15 +4290,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ethraid/helper_functions_rv.pyx":187
+/* "ethraid/helper_functions_rv.pyx":188
  * 
  * 
  * cpdef M_2_evolvedE(double M0, double per, double e, double rv_epoch):             # <<<<<<<<<<<<<<
  *     """
  *     Use Radvel Kepler solver to take a mean anomaly at the beginning
  */
 
@@ -4317,44 +4317,44 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("M_2_evolvedE", 0);
 
-  /* "ethraid/helper_functions_rv.pyx":211
+  /* "ethraid/helper_functions_rv.pyx":212
  *     # Fewer python references with no declarations. Not sure why.
  * 
  *     M_evolved = ((two_pi/per)*(rv_epoch - hip_beginning) + M0)%two_pi             # <<<<<<<<<<<<<<
  * 
  *     E = kepler_single(M_evolved, e)
  */
   if (unlikely(__pyx_v_per == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 212, __pyx_L1_error)
   }
   __pyx_t_1 = (((__pyx_v_7ethraid_8compiled_19helper_functions_rv_two_pi / __pyx_v_per) * (__pyx_v_rv_epoch - __pyx_v_7ethraid_8compiled_19helper_functions_rv_hip_beginning)) + __pyx_v_M0);
   if (unlikely(__pyx_v_7ethraid_8compiled_19helper_functions_rv_two_pi == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float divmod()");
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 212, __pyx_L1_error)
   }
   __pyx_v_M_evolved = __Pyx_mod_double(__pyx_t_1, __pyx_v_7ethraid_8compiled_19helper_functions_rv_two_pi);
 
-  /* "ethraid/helper_functions_rv.pyx":213
+  /* "ethraid/helper_functions_rv.pyx":214
  *     M_evolved = ((two_pi/per)*(rv_epoch - hip_beginning) + M0)%two_pi
  * 
  *     E = kepler_single(M_evolved, e)             # <<<<<<<<<<<<<<
  * 
  *     return E
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kepler_single); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kepler_single); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_M_evolved); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_M_evolved); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_e); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_e); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4363,63 +4363,63 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_E = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "ethraid/helper_functions_rv.pyx":215
+  /* "ethraid/helper_functions_rv.pyx":216
  *     E = kepler_single(M_evolved, e)
  * 
  *     return E             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_E);
   __pyx_r = __pyx_v_E;
   goto __pyx_L0;
 
-  /* "ethraid/helper_functions_rv.pyx":187
+  /* "ethraid/helper_functions_rv.pyx":188
  * 
  * 
  * cpdef M_2_evolvedE(double M0, double per, double e, double rv_epoch):             # <<<<<<<<<<<<<<
  *     """
  *     Use Radvel Kepler solver to take a mean anomaly at the beginning
  */
 
@@ -4477,48 +4477,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M0)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_per)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 1); __PYX_ERR(0, 187, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 1); __PYX_ERR(0, 188, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_e)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 2); __PYX_ERR(0, 187, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 2); __PYX_ERR(0, 188, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rv_epoch)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 3); __PYX_ERR(0, 187, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, 3); __PYX_ERR(0, 188, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "M_2_evolvedE") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "M_2_evolvedE") < 0)) __PYX_ERR(0, 188, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_M0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_M0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
-    __pyx_v_per = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_per == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
-    __pyx_v_e = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_e == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
-    __pyx_v_rv_epoch = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_rv_epoch == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_M0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_M0 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+    __pyx_v_per = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_per == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+    __pyx_v_e = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_e == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+    __pyx_v_rv_epoch = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_rv_epoch == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("M_2_evolvedE", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 188, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ethraid.compiled.helper_functions_rv.M_2_evolvedE", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7ethraid_8compiled_19helper_functions_rv_6M_2_evolvedE(__pyx_self, __pyx_v_M0, __pyx_v_per, __pyx_v_e, __pyx_v_rv_epoch);
 
@@ -4532,15 +4532,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("M_2_evolvedE", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7ethraid_8compiled_19helper_functions_rv_M_2_evolvedE(__pyx_v_M0, __pyx_v_per, __pyx_v_e, __pyx_v_rv_epoch, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7ethraid_8compiled_19helper_functions_rv_M_2_evolvedE(__pyx_v_M0, __pyx_v_per, __pyx_v_e, __pyx_v_rv_epoch, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
```

### Comparing `ethraid-0.1.90/ethraid/compiled/helper_functions_astro.cpython-37m-darwin.so` & `ethraid-1.0.0/ethraid/compiled/helper_functions_astro.cpython-37m-darwin.so`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/helper_functions_general.cpython-37m-darwin.so` & `ethraid-1.0.0/ethraid/compiled/helper_functions_general.cpython-37m-darwin.so`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/compiled/helper_functions_rv.cpython-37m-darwin.so` & `ethraid-1.0.0/ethraid/compiled/helper_functions_rv.cpython-37m-darwin.so`

 * *Files 1% similar despite different names*

#### llvm-readobj --symbols {}

```diff
@@ -4695,15 +4695,15 @@
   Symbol {
     Name: /Users/judahvz/research/code/GitHub/ethraid/build/temp.macosx-10.9-x86_64-cpython-37/ethraid/compiled/ethraid/helper_functions_rv.o (17680)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x641A4044
+    Value: 0x641A471F
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

#### x86_64

##### llvm-objdump --arch=x86_64 --section=__TEXT,__text --macho --demangle --no-leading-addr --no-show-raw-insn {}

```diff
@@ -762,15 +762,15 @@
 	leaq	118604(%rip), %r9 ## literal pool for: "s"
 	movl	$4, %r8d
 	xorl	%eax, %eax
 	callq	0x1e08e ## symbol stub for: _PyErr_Format
 	movl	$4517, %esi
 	leaq	118784(%rip), %rdi ## literal pool for: "ethraid.compiled.helper_functions_rv.M_2_evolvedE"
 	leaq	116000(%rip), %rcx
-	movl	$187, %edx
+	movl	$188, %edx
 	callq	___Pyx_AddTraceback
 	xorl	%eax, %eax
 	movq	126333(%rip), %rcx ## literal pool symbol address: ___stack_chk_guard
 	movq	(%rcx), %rcx
 	cmpq	-48(%rbp), %rcx
 	jne	0x23bb
 	addq	$88, %rsp
@@ -1793,22 +1793,22 @@
 	jne	0x3520
 	jmp	0x3516
 	movq	122314(%rip), %rax ## literal pool symbol address: _PyExc_ZeroDivisionError
 	movq	(%rax), %rdi
 	leaq	114842(%rip), %rsi ## literal pool for: "float division"
 	callq	0x1e0c4 ## symbol stub for: _PyErr_SetString
 	movl	$4333, %r14d
-	movl	$211, %ebx
+	movl	$212, %ebx
 	jmp	0x3579
 	movq	122276(%rip), %rax ## literal pool symbol address: _PyExc_ZeroDivisionError
 	movq	(%rax), %rdi
 	leaq	114869(%rip), %rsi ## literal pool for: "float divmod()"
 	callq	0x1e0c4 ## symbol stub for: _PyErr_SetString
 	movl	$4338, %r14d
-	movl	$211, %ebx
+	movl	$212, %ebx
 	jmp	0x3579
 	movsd	%xmm0, -104(%rbp)
 	movq	___pyx_n_s_kepler_single(%rip), %rsi
 	movq	24(%rsi), %rdx
 	movq	%rsi, -96(%rbp)
 	callq	0x1e2a4 ## symbol stub for: __PyDict_GetItem_KnownHash
 	movq	%rax, %r15
@@ -1843,15 +1843,15 @@
 	movq	122005(%rip), %rax ## literal pool symbol address: _PyExc_NameError
 	movq	(%rax), %rdi
 	leaq	114685(%rip), %rsi ## literal pool for: "name '%U' is not defined"
 	movq	-96(%rbp), %rdx
 	xorl	%eax, %eax
 	callq	0x1e08e ## symbol stub for: _PyErr_Format
 	movl	$4349, %r14d
-	movl	$213, %ebx
+	movl	$214, %ebx
 	jmp	0x3579
 	movl	$4353, %r14d
 	xorl	%ebx, %ebx
 	xorl	%r12d, %r12d
 	xorl	%r13d, %r13d
 	decq	(%r15)
 	jne	0x3520
@@ -1950,15 +1950,15 @@
 	testq	%r12, %r12
 	je	0x355f
 	decq	(%r12)
 	jne	0x355f
 	movq	8(%r12), %rax
 	movq	%r12, %rdi
 	callq	*48(%rax)
-	movl	$213, %ebx
+	movl	$214, %ebx
 	testq	%r13, %r13
 	je	0x3579
 	decq	(%r13)
 	jne	0x3579
 	movq	8(%r13), %rax
 	movq	%r13, %rdi
 	callq	*48(%rax)
```

### Comparing `ethraid-0.1.90/ethraid/data/.DS_Store` & `ethraid-1.0.0/ethraid/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/data/baraffe_table_4.csv` & `ethraid-1.0.0/ethraid/data/baraffe_table_4.csv`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/data/mamajek.csv` & `ethraid-1.0.0/ethraid/data/mamajek.csv`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/driver.py` & `ethraid-1.0.0/ethraid/driver.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/helper_functions_astro.pyx` & `ethraid-1.0.0/ethraid/helper_functions_astro.pyx`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/helper_functions_general.pyx` & `ethraid-1.0.0/ethraid/helper_functions_general.pyx`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/helper_functions_imaging.py` & `ethraid-1.0.0/ethraid/helper_functions_imaging.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/helper_functions_plotting.py` & `ethraid-1.0.0/ethraid/helper_functions_plotting.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/helper_functions_rv.pyx` & `ethraid-1.0.0/ethraid/helper_functions_rv.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -146,33 +146,34 @@
     Returns:
         gdot (float, m/s/day): Model linear trend term
         gddot (float, m/s/day/day): Model quadratic curvature term
     """
 
     cdef double     e_term, sqrt_eterm,\
                     sqrt_e_sq_term, cos_E, sin_E,\
-                    tan_Eovr2, nu, nu_dot, nu_ddot,\
+                    nu, nu_dot, nu_ddot,\
                     cos_nu_om, sin_nu_om, sin_i,\
                     pre_fac, gamma_dot, gamma_ddot
                  
     e_term = (1+e)/(1-e)
     sqrt_eterm = sqrt(e_term)
     sqrt_e_sq_term = sqrt(1-e*e)
 
     cos_E = cos(E)
     sin_E = sin(E)
-
+    
+    #####################################
     ## Two-argument arctan function to avoid div by 0 when E=pi
     ## Also replacing sin(E/2)/cos(E/2) with equivalent sinE/(1+cosE) to save calculation
     nu = 2*atan2(sqrt_eterm*sin_E, (1+cos_E))
-    
+        
 
     # nu derivatives use days (not seconds) to give gdot/gddot correct units 
     nu_dot = two_pi*sqrt_e_sq_term/(per*(1-e*cos_E)**2) # Units of day^-1
-    nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term ## Units of day^-2
+    nu_ddot = -nu_dot**2 * 2*e*sin_E/sqrt_e_sq_term # # Units of day^-2
 
     cos_nu_om = cos(nu+om)
     sin_nu_om = sin(nu+om)
     sin_i = sin(i)
 
     # Lovis+Fischer 2010 (analytic)
     pre_fac = sqrt(G)/sqrt_e_sq_term * m*sin_i/sqrt((m+m_star)*(a)) * auday2ms # AU/day ==> m/s
```

### Comparing `ethraid-0.1.90/ethraid/load_save.py` & `ethraid-1.0.0/ethraid/load_save.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/plotter.py` & `ethraid-1.0.0/ethraid/plotter.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/system_params.py` & `ethraid-1.0.0/ethraid/system_params.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid/system_params_local.py` & `ethraid-1.0.0/ethraid/system_params_local.py`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/ethraid.egg-info/PKG-INFO` & `ethraid-1.0.0/ethraid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethraid
-Version: 0.1.90
+Version: 1.0.0
 Summary: Command line application for trend code
 Home-page: 
 Author: Judah Van Zandt
 Author-email: judahvz@astro.ucla.edu
 
 
 # Trend Analysis
@@ -13,14 +13,15 @@
 ## Environment
 - Create new environment with python 3.7
 - *\$ conda create --name trends_env python=3.7*
 - *\$ conda activate trends_env*
 
 ## Download from Test PyPI (regular pip download coming soon)
 - *\$ python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple ethraid*
+- You may have to upgrade pip using *\$ curl https://bootstrap.pypa.io/get-pip.py | python*
 
 ## If downloading repo
 - Install dependencies using requirements.txt 
 - *\$ pip install -r requirements.txt*
 
 - Build code from top level of repo
 - *\$ cd trends/*
```

### Comparing `ethraid-0.1.90/ethraid.egg-info/SOURCES.txt` & `ethraid-1.0.0/ethraid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethraid-0.1.90/setup.py` & `ethraid-1.0.0/setup.py`

 * *Files identical despite different names*

