# Comparing `tmp/scikit-surgerynditracker-0.2.3.tar.gz` & `tmp/scikit-surgerynditracker-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-surgerynditracker-0.2.3.tar", last modified: Wed Jan 18 10:07:39 2023, max compression
+gzip compressed data, was "dist/scikit-surgerynditracker-0.2.4.tar", last modified: Wed Apr 19 15:33:28 2023, max compression
```

## Comparing `scikit-surgerynditracker-0.2.3.tar` & `scikit-surgerynditracker-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/
--rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/nditracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:07:39.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/serial_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/serial_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/sksurgerynditracker/serial_utils/com_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-18 10:07:30.000000 scikit-surgerynditracker-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/nditracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:33:28.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/serial_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/serial_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/sksurgerynditracker/serial_utils/com_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-19 15:33:20.000000 scikit-surgerynditracker-0.2.4/versioneer.py
```

### Comparing `scikit-surgerynditracker-0.2.3/PKG-INFO` & `scikit-surgerynditracker-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-surgerynditracker
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interface for Northern Digital (NDI) Trackers with data to NumPy arrays
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerynditracker
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgerynditracker
         ===============================
```

### Comparing `scikit-surgerynditracker-0.2.3/README.rst` & `scikit-surgerynditracker-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-surgerynditracker-0.2.3/scikit_surgerynditracker.egg-info/PKG-INFO` & `scikit-surgerynditracker-0.2.4/scikit_surgerynditracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-surgerynditracker
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interface for Northern Digital (NDI) Trackers with data to NumPy arrays
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerynditracker
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgerynditracker
         ===============================
```

### Comparing `scikit-surgerynditracker-0.2.3/setup.py` & `scikit-surgerynditracker-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerynditracker-0.2.3/sksurgerynditracker/demo.py` & `scikit-surgerynditracker-0.2.4/sksurgerynditracker/demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerynditracker-0.2.3/sksurgerynditracker/nditracker.py` & `scikit-surgerynditracker-0.2.4/sksurgerynditracker/nditracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,16 @@
         """
         self._get_frame = getattr(ndicapy, 'ndiGetBXFrame')
         self._get_transform = getattr(ndicapy, 'ndiGetBXTransform')
         self._capture_string = 'BX:0801'
 
         firmware = self._get_firmware_version()
         if firmware in (' AURORA Rev 007', ' AURORA Rev 008',
-                        ' Polaris Vega 008', ' Polaris Spectra Rev 006'):
+                        ' Polaris Vega 008',
+                        ' Polaris Spectra Rev 006', ' Polaris Spectra Rev 007'):
             self._get_frame = getattr(ndicapy, 'ndiGetTXFrame')
             self._get_transform = getattr(ndicapy, 'ndiGetTXTransform')
             self._capture_string = 'TX:0801'
 
     def _get_firmware_version(self):
         """
         Gets the device's firmware version, and sets
```

### Comparing `scikit-surgerynditracker-0.2.3/versioneer.py` & `scikit-surgerynditracker-0.2.4/versioneer.py`

 * *Files identical despite different names*

