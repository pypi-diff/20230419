# Comparing `tmp/wyoming_piper-0.0.1.tar.gz` & `tmp/wyoming_piper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_piper-0.0.1.tar", last modified: Wed Apr 19 19:09:45 2023, max compression
+gzip compressed data, was "wyoming_piper-0.0.2.tar", last modified: Wed Apr 19 20:16:08 2023, max compression
```

## Comparing `wyoming_piper-0.0.1.tar` & `wyoming_piper-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 19:09:45.281654 wyoming_piper-0.0.1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-19 16:16:21.000000 wyoming_piper-0.0.1/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 19:09:45.281654 wyoming_piper-0.0.1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 18:47:39.000000 wyoming_piper-0.0.1/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-19 19:09:45.281654 wyoming_piper-0.0.1/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1205 2023-04-19 18:48:00.000000 wyoming_piper-0.0.1/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 19:09:45.281654 wyoming_piper-0.0.1/wyoming_piper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-19 19:04:59.000000 wyoming_piper-0.0.1/wyoming_piper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4539 2023-04-19 19:06:21.000000 wyoming_piper-0.0.1/wyoming_piper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-19 15:13:49.000000 wyoming_piper-0.0.1/wyoming_piper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     1106 2023-04-19 19:08:21.000000 wyoming_piper-0.0.1/wyoming_piper/download.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3634 2023-04-19 19:09:15.000000 wyoming_piper-0.0.1/wyoming_piper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 19:09:45.281654 wyoming_piper-0.0.1/wyoming_piper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 19:09:45.000000 wyoming_piper-0.0.1/wyoming_piper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      347 2023-04-19 19:09:45.000000 wyoming_piper-0.0.1/wyoming_piper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-19 19:09:45.000000 wyoming_piper-0.0.1/wyoming_piper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 19:09:45.000000 wyoming_piper-0.0.1/wyoming_piper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-04-19 19:09:45.000000 wyoming_piper-0.0.1/wyoming_piper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-19 16:16:21.000000 wyoming_piper-0.0.2/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 18:47:39.000000 wyoming_piper-0.0.2/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1205 2023-04-19 20:14:32.000000 wyoming_piper-0.0.2/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/wyoming_piper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-19 19:04:59.000000 wyoming_piper-0.0.2/wyoming_piper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4503 2023-04-19 20:03:45.000000 wyoming_piper-0.0.2/wyoming_piper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-19 15:13:49.000000 wyoming_piper-0.0.2/wyoming_piper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     1106 2023-04-19 19:08:21.000000 wyoming_piper-0.0.2/wyoming_piper/download.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3634 2023-04-19 19:09:15.000000 wyoming_piper-0.0.2/wyoming_piper/handler.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/wyoming_piper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      347 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/top_level.txt
```

### Comparing `wyoming_piper-0.0.1/PKG-INFO` & `wyoming_piper-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming_piper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming piper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_piper-0.0.1/setup.py` & `wyoming_piper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_piper",
-    version="0.0.1",
+    version="0.0.2",
     description="Wyoming Server for Piper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_piper-0.0.1/wyoming_piper/__main__.py` & `wyoming_piper-0.0.2/wyoming_piper/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,21 +107,21 @@
             "--output_dir",
             str(temp_dir),
         ]
 
         if (args.speaker is not None) and (num_speakers > 1):
             piper_args.extend(["--speaker", str(args.speaker)])
 
-        if args.noise_scale is not None:
+        if args.noise_scale:
             piper_args.extend(["--noise-scale", str(args.noise_scale)])
 
-        if args.length_scale is not None:
+        if args.length_scale:
             piper_args.extend(["--length-scale", str(args.length_scale)])
 
-        if args.noise_w is not None:
+        if args.noise_w:
             piper_args.extend(["--noise-w", str(args.noise_w)])
 
         proc = await asyncio.create_subprocess_exec(
             args.piper,
             *piper_args,
             stdin=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE,
```

### Comparing `wyoming_piper-0.0.1/wyoming_piper/const.py` & `wyoming_piper-0.0.2/wyoming_piper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.1/wyoming_piper/download.py` & `wyoming_piper-0.0.2/wyoming_piper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.1/wyoming_piper/handler.py` & `wyoming_piper-0.0.2/wyoming_piper/handler.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.1/wyoming_piper.egg-info/PKG-INFO` & `wyoming_piper-0.0.2/wyoming_piper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming-piper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming piper
 Classifier: Development Status :: 3 - Alpha
```

