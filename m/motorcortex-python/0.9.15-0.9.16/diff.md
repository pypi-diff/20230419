# Comparing `tmp/motorcortex-python-0.9.15.tar.gz` & `tmp/motorcortex-python-0.9.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/motorcortex-python-0.9.15.tar", last modified: Tue Dec 11 14:46:13 2018, max compression
+gzip compressed data, was "dist/motorcortex-python-0.9.16.tar", last modified: Wed May 29 18:18:29 2019, max compression
```

## Comparing `motorcortex-python-0.9.15.tar` & `motorcortex-python-0.9.16.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/
-drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex/
--rw-r--r--   0 alexey    (1000) alexey    (1000)    88768 2018-12-06 13:00:21.000000 motorcortex-python-0.9.15/motorcortex/motorcortex_pb2.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)    15208 2018-12-06 16:33:20.000000 motorcortex-python-0.9.15/motorcortex/message_types.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     4290 2018-10-30 10:26:32.000000 motorcortex-python-0.9.15/motorcortex/subscribe.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     1932 2018-10-30 10:26:31.000000 motorcortex-python-0.9.15/motorcortex/parameter_tree.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     2239 2018-02-12 22:21:54.000000 motorcortex-python-0.9.15/motorcortex/reply.py
--rwxr-xr-x   0 alexey    (1000) alexey    (1000)     2212 2018-12-06 13:05:56.000000 motorcortex-python-0.9.15/motorcortex/__init__.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     7519 2018-10-30 10:24:40.000000 motorcortex-python-0.9.15/motorcortex/subscription.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)    12044 2018-12-06 13:11:02.000000 motorcortex-python-0.9.15/motorcortex/request.py
--rwxr-xr-x   0 alexey    (1000) alexey    (1000)     3572 2018-12-06 12:23:15.000000 motorcortex-python-0.9.15/motorcortex/motorcortex_hash.json
--rw-r--r--   0 alexey    (1000) alexey    (1000)      391 2018-02-12 22:21:54.000000 motorcortex-python-0.9.15/README.md
--rw-r--r--   0 alexey    (1000) alexey    (1000)      750 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/PKG-INFO
--rw-r--r--   0 alexey    (1000) alexey    (1000)       38 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/setup.cfg
--rw-r--r--   0 alexey    (1000) alexey    (1000)      900 2018-12-11 14:40:44.000000 motorcortex-python-0.9.15/setup.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)       62 2018-12-11 14:45:56.000000 motorcortex-python-0.9.15/MANIFEST.in
-drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/
--rw-r--r--   0 alexey    (1000) alexey    (1000)        1 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 alexey    (1000) alexey    (1000)       72 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/requires.txt
--rw-r--r--   0 alexey    (1000) alexey    (1000)      750 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/PKG-INFO
--rw-r--r--   0 alexey    (1000) alexey    (1000)       26 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/top_level.txt
--rw-r--r--   0 alexey    (1000) alexey    (1000)      610 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/motorcortex_python.egg-info/SOURCES.txt
-drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2018-12-11 14:46:13.000000 motorcortex-python-0.9.15/robot_control/
--rw-r--r--   0 alexey    (1000) alexey    (1000)     9043 2018-12-06 12:05:58.000000 motorcortex-python-0.9.15/robot_control/motion_program.py
--rwxr-xr-x   0 alexey    (1000) alexey    (1000)      409 2018-02-18 11:33:16.000000 motorcortex-python-0.9.15/robot_control/__init__.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     2365 2018-02-11 12:20:44.000000 motorcortex-python-0.9.15/robot_control/system_defs.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)    13868 2018-02-11 12:54:01.000000 motorcortex-python-0.9.15/robot_control/robot_command.py
--rw-r--r--   0 alexey    (1000) alexey    (1000)     1147 2018-12-11 14:30:25.000000 motorcortex-python-0.9.15/LICENSE
+drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/
+drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex/
+-rw-r--r--   0 alexey    (1000) alexey    (1000)    88768 2018-12-06 13:00:21.000000 motorcortex-python-0.9.16/motorcortex/motorcortex_pb2.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)    15208 2019-05-29 18:04:05.000000 motorcortex-python-0.9.16/motorcortex/message_types.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     4290 2018-10-30 10:26:32.000000 motorcortex-python-0.9.16/motorcortex/subscribe.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     1932 2018-10-30 10:26:31.000000 motorcortex-python-0.9.16/motorcortex/parameter_tree.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     2239 2018-02-12 22:21:54.000000 motorcortex-python-0.9.16/motorcortex/reply.py
+-rwxr-xr-x   0 alexey    (1000) alexey    (1000)     2212 2018-12-06 13:05:56.000000 motorcortex-python-0.9.16/motorcortex/__init__.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     7519 2018-10-30 10:24:40.000000 motorcortex-python-0.9.16/motorcortex/subscription.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)    12044 2018-12-06 13:11:02.000000 motorcortex-python-0.9.16/motorcortex/request.py
+-rwxr-xr-x   0 alexey    (1000) alexey    (1000)     3572 2018-12-06 12:23:15.000000 motorcortex-python-0.9.16/motorcortex/motorcortex_hash.json
+-rw-r--r--   0 alexey    (1000) alexey    (1000)      391 2018-02-12 22:21:54.000000 motorcortex-python-0.9.16/README.md
+-rw-r--r--   0 alexey    (1000) alexey    (1000)      750 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/PKG-INFO
+-rw-r--r--   0 alexey    (1000) alexey    (1000)       38 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/setup.cfg
+-rw-r--r--   0 alexey    (1000) alexey    (1000)      900 2019-05-29 18:18:09.000000 motorcortex-python-0.9.16/setup.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)       62 2018-12-11 14:45:56.000000 motorcortex-python-0.9.16/MANIFEST.in
+drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/
+-rw-r--r--   0 alexey    (1000) alexey    (1000)        1 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey    (1000) alexey    (1000)       72 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/requires.txt
+-rw-r--r--   0 alexey    (1000) alexey    (1000)      750 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/PKG-INFO
+-rw-r--r--   0 alexey    (1000) alexey    (1000)       26 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/top_level.txt
+-rw-r--r--   0 alexey    (1000) alexey    (1000)      610 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/motorcortex_python.egg-info/SOURCES.txt
+drwxr-xr-x   0 alexey    (1000) alexey    (1000)        0 2019-05-29 18:18:29.000000 motorcortex-python-0.9.16/robot_control/
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     9043 2018-12-06 12:05:58.000000 motorcortex-python-0.9.16/robot_control/motion_program.py
+-rwxr-xr-x   0 alexey    (1000) alexey    (1000)      409 2018-02-18 11:33:16.000000 motorcortex-python-0.9.16/robot_control/__init__.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     2365 2018-02-11 12:20:44.000000 motorcortex-python-0.9.16/robot_control/system_defs.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)    13868 2018-02-11 12:54:01.000000 motorcortex-python-0.9.16/robot_control/robot_command.py
+-rw-r--r--   0 alexey    (1000) alexey    (1000)     1147 2018-12-11 14:30:25.000000 motorcortex-python-0.9.16/LICENSE
```

### Comparing `motorcortex-python-0.9.15/motorcortex/motorcortex_pb2.py` & `motorcortex-python-0.9.16/motorcortex/motorcortex_pb2.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/message_types.py` & `motorcortex-python-0.9.16/motorcortex/message_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
             self.__encoder = lambda len, val: struct.pack('%db' % len, *val)
             self.__prepare = lambda val: [bool(x) for x in val.split(",")]
         elif (type_name == "DOUBLE"):
             self.__decoder = lambda len, val: struct.unpack('%dd' % len, val)
             self.__encoder = lambda len, val: struct.pack('%dd' % len, *val)
             self.__prepare = lambda val: [float(x) for x in val.split(",")]
         elif (type_name == "FLOAT"):
-            self.__decoder = lambda len, val: struct.unpack('%fd' % len, val)
-            self.__encoder = lambda len, val: struct.pack('%fd' % len, *val)
+            self.__decoder = lambda len, val: struct.unpack('%df' % len, val)
+            self.__encoder = lambda len, val: struct.pack('%df' % len, *val)
             self.__prepare = lambda val: [float(x) for x in val.split(",")]
         elif (type_name == "INT8"):
             self.__decoder = lambda len, val: struct.unpack('%db' % len, val)
             self.__encoder = lambda len, val: struct.pack('%db' % len, *val)
             self.__prepare = lambda val: [int(float(x)) & 0x7f for x in val.split(",")]
         elif (type_name == "UINT8"):
             self.__decoder = lambda len, val: struct.unpack('%dB' % len, val)
```

### Comparing `motorcortex-python-0.9.15/motorcortex/subscribe.py` & `motorcortex-python-0.9.16/motorcortex/subscribe.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/parameter_tree.py` & `motorcortex-python-0.9.16/motorcortex/parameter_tree.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/reply.py` & `motorcortex-python-0.9.16/motorcortex/reply.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/__init__.py` & `motorcortex-python-0.9.16/motorcortex/__init__.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/subscription.py` & `motorcortex-python-0.9.16/motorcortex/subscription.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/request.py` & `motorcortex-python-0.9.16/motorcortex/request.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/motorcortex/motorcortex_hash.json` & `motorcortex-python-0.9.16/motorcortex/motorcortex_hash.json`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/PKG-INFO` & `motorcortex-python-0.9.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motorcortex-python
-Version: 0.9.15
+Version: 0.9.16
 Summary: Python bindings for Motorcortex Engine
 Home-page: https://www.motorcortex.io
 Author: Alexey Zakharov
 Author-email: alexey.zakharov@vectioneer.com
 License: MIT
 Description: Motorcortex Python is a communication library to develop Python client 
         applications for the Motorcortex Core. Motorcortex Python provides an
```

### Comparing `motorcortex-python-0.9.15/setup.py` & `motorcortex-python-0.9.16/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='motorcortex-python',
-      version='0.9.15',
+      version='0.9.16',
       description='Python bindings for Motorcortex Engine',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Alexey Zakharov',
       author_email='alexey.zakharov@vectioneer.com',
       url='https://www.motorcortex.io',
       license='MIT',
```

### Comparing `motorcortex-python-0.9.15/motorcortex_python.egg-info/PKG-INFO` & `motorcortex-python-0.9.16/motorcortex_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motorcortex-python
-Version: 0.9.15
+Version: 0.9.16
 Summary: Python bindings for Motorcortex Engine
 Home-page: https://www.motorcortex.io
 Author: Alexey Zakharov
 Author-email: alexey.zakharov@vectioneer.com
 License: MIT
 Description: Motorcortex Python is a communication library to develop Python client 
         applications for the Motorcortex Core. Motorcortex Python provides an
```

### Comparing `motorcortex-python-0.9.15/motorcortex_python.egg-info/SOURCES.txt` & `motorcortex-python-0.9.16/motorcortex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/robot_control/motion_program.py` & `motorcortex-python-0.9.16/robot_control/motion_program.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/robot_control/system_defs.py` & `motorcortex-python-0.9.16/robot_control/system_defs.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/robot_control/robot_command.py` & `motorcortex-python-0.9.16/robot_control/robot_command.py`

 * *Files identical despite different names*

### Comparing `motorcortex-python-0.9.15/LICENSE` & `motorcortex-python-0.9.16/LICENSE`

 * *Files identical despite different names*

