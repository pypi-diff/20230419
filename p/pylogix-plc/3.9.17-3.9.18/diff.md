# Comparing `tmp/pylogix-plc-3.9.17.tar.gz` & `tmp/pylogix-plc-3.9.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogix-plc-3.9.17.tar", last modified: Wed Apr 19 18:08:10 2023, max compression
+gzip compressed data, was "pylogix-plc-3.9.18.tar", last modified: Wed Apr 19 18:09:37 2023, max compression
```

## Comparing `pylogix-plc-3.9.17.tar` & `pylogix-plc-3.9.18.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:08:10.972611 pylogix-plc-3.9.17/
--rw-rw-rw-   0        0        0    11357 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/LICENSE.txt
--rw-rw-rw-   0        0        0     5436 2023-04-19 18:08:10.970606 pylogix-plc-3.9.17/PKG-INFO
--rw-rw-rw-   0        0        0     4573 2023-04-19 17:44:52.000000 pylogix-plc-3.9.17/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:08:10.928610 pylogix-plc-3.9.17/pylogix/
--rw-rw-rw-   0        0        0      108 2023-04-19 18:08:00.000000 pylogix-plc-3.9.17/pylogix/__init__.py
--rw-rw-rw-   0        0        0    60430 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/pylogix/eip.py
--rw-rw-rw-   0        0        0    26181 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/pylogix/lgx_comm.py
--rw-rw-rw-   0        0        0    66691 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/pylogix/lgx_device.py
--rw-rw-rw-   0        0        0     4153 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/pylogix/lgx_response.py
--rw-rw-rw-   0        0        0     4026 2023-04-10 15:05:32.000000 pylogix-plc-3.9.17/pylogix/lgx_tag.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:08:10.966607 pylogix-plc-3.9.17/pylogix_plc.egg-info/
--rw-rw-rw-   0        0        0     5436 2023-04-19 18:08:10.000000 pylogix-plc-3.9.17/pylogix_plc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-19 18:08:10.000000 pylogix-plc-3.9.17/pylogix_plc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:08:10.000000 pylogix-plc-3.9.17/pylogix_plc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 18:08:10.000000 pylogix-plc-3.9.17/pylogix_plc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:08:10.973606 pylogix-plc-3.9.17/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-04-19 18:06:49.000000 pylogix-plc-3.9.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.145827 pylogix-plc-3.9.18/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/LICENSE.txt
+-rw-rw-rw-   0        0        0     5436 2023-04-19 18:09:37.143829 pylogix-plc-3.9.18/PKG-INFO
+-rw-rw-rw-   0        0        0     4573 2023-04-19 17:44:52.000000 pylogix-plc-3.9.18/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.090829 pylogix-plc-3.9.18/pylogix/
+-rw-rw-rw-   0        0        0      108 2023-04-19 18:09:29.000000 pylogix-plc-3.9.18/pylogix/__init__.py
+-rw-rw-rw-   0        0        0    60430 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/eip.py
+-rw-rw-rw-   0        0        0    26181 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_comm.py
+-rw-rw-rw-   0        0        0    66691 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_device.py
+-rw-rw-rw-   0        0        0     4153 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_response.py
+-rw-rw-rw-   0        0        0     4026 2023-04-10 15:05:32.000000 pylogix-plc-3.9.18/pylogix/lgx_tag.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:09:37.137826 pylogix-plc-3.9.18/pylogix_plc.egg-info/
+-rw-rw-rw-   0        0        0     5436 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 18:09:36.000000 pylogix-plc-3.9.18/pylogix_plc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 18:09:37.146828 pylogix-plc-3.9.18/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-04-19 18:09:20.000000 pylogix-plc-3.9.18/setup.py
```

### Comparing `pylogix-plc-3.9.17/LICENSE.txt` & `pylogix-plc-3.9.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/PKG-INFO` & `pylogix-plc-3.9.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pylogix-plc
-Version: 3.9.17
-Summary: Pylogix plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.
+Version: 3.9.18
+Summary: Pylogix-plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.
 Home-page: https://github.com/PYLOGiX-DEV/pylogix_
 Author: https://pylogix.com/
 Author-email: dev@pylogix.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylogix-plc Version: 3.9.17 Summary: Pylogix plc is
+Metadata-Version: 2.1 Name: pylogix-plc Version: 3.9.18 Summary: Pylogix-plc is
 a Python package developed by PYLOGiX - https://pylogix.com/, which is a
 software company that allows you to easily read/write values from tags in
 Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over
 Ethernet I/P. Home-page: https://github.com/PYLOGiX-DEV/pylogix_ Author: https:
 //pylogix.com/ Author-email: dev@pylogix.com License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
 Language :: Python :: 3.6 Classifier: License :: OSI Approved :: Apache
```

### Comparing `pylogix-plc-3.9.17/README.md` & `pylogix-plc-3.9.18/README.md`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix/eip.py` & `pylogix-plc-3.9.18/pylogix/eip.py`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix/lgx_comm.py` & `pylogix-plc-3.9.18/pylogix/lgx_comm.py`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix/lgx_device.py` & `pylogix-plc-3.9.18/pylogix/lgx_device.py`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix/lgx_response.py` & `pylogix-plc-3.9.18/pylogix/lgx_response.py`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix/lgx_tag.py` & `pylogix-plc-3.9.18/pylogix/lgx_tag.py`

 * *Files identical despite different names*

### Comparing `pylogix-plc-3.9.17/pylogix_plc.egg-info/PKG-INFO` & `pylogix-plc-3.9.18/pylogix_plc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pylogix-plc
-Version: 3.9.17
-Summary: Pylogix plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.
+Version: 3.9.18
+Summary: Pylogix-plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.
 Home-page: https://github.com/PYLOGiX-DEV/pylogix_
 Author: https://pylogix.com/
 Author-email: dev@pylogix.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylogix-plc Version: 3.9.17 Summary: Pylogix plc is
+Metadata-Version: 2.1 Name: pylogix-plc Version: 3.9.18 Summary: Pylogix-plc is
 a Python package developed by PYLOGiX - https://pylogix.com/, which is a
 software company that allows you to easily read/write values from tags in
 Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over
 Ethernet I/P. Home-page: https://github.com/PYLOGiX-DEV/pylogix_ Author: https:
 //pylogix.com/ Author-email: dev@pylogix.com License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
 Language :: Python :: 3.6 Classifier: License :: OSI Approved :: Apache
```

### Comparing `pylogix-plc-3.9.17/setup.py` & `pylogix-plc-3.9.18/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="pylogix-plc",
     version=pylogix.__version__,
     author="https://pylogix.com/",
     author_email="dev@pylogix.com",
-    description="""Pylogix plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.""",
+    description="""Pylogix-plc is a Python package developed by PYLOGiX - https://pylogix.com/, which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/PYLOGiX-DEV/pylogix_",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 2.7",
```

