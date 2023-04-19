# Comparing `tmp/pvrhinodemo-2.2.0.tar.gz` & `tmp/pvrhinodemo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvrhinodemo-2.2.0.tar", last modified: Wed Apr 12 18:00:55 2023, max compression
+gzip compressed data, was "pvrhinodemo-2.2.1.tar", last modified: Wed Apr 19 17:44:58 2023, max compression
```

## Comparing `pvrhinodemo-2.2.0.tar` & `pvrhinodemo-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      102 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3359 2023-04-06 17:38:28.000000 pvrhinodemo-2.2.0/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/pvrhinodemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5697 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6001 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      303 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      118 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       33 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       12 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1979 2023-04-06 17:38:28.000000 pvrhinodemo-2.2.0/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      102 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3359 2023-04-19 17:34:19.000000 pvrhinodemo-2.2.1/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/pvrhinodemo/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5697 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_file.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6010 2023-04-19 17:44:57.000000 pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_mic.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      303 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      118 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/entry_points.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       33 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       12 2023-04-19 17:44:58.000000 pvrhinodemo-2.2.1/pvrhinodemo.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-19 17:44:58.731333 pvrhinodemo-2.2.1/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1979 2023-04-19 17:41:52.000000 pvrhinodemo-2.2.1/setup.py
```

### Comparing `pvrhinodemo-2.2.0/PKG-INFO` & `pvrhinodemo-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pvrhinodemo-2.2.0/README.md` & `pvrhinodemo-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_file.py` & `pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_mic.py` & `pvrhinodemo-2.2.1/pvrhinodemo/rhino_demo_mic.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     print('Context info: %s' % rhino.context_info)
 
     recorder = PvRecorder(
         device_index=args.audio_device_index,
         frame_length=rhino.frame_length)
     recorder.start()
 
-    print('Using device: %s' % recorder.device)
+    print('Using device: %s' % recorder.selected_device)
     print('Listening ... Press Ctrl+C to exit.\n')
 
     wav_file = None
     if args.output_path is not None:
         wav_file = wave.open(args.output_path, 'wb')
         wav_file.setnchannels(1)
         wav_file.setsampwidth(2)
```

### Comparing `pvrhinodemo-2.2.0/pvrhinodemo.egg-info/PKG-INFO` & `pvrhinodemo-2.2.1/pvrhinodemo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pvrhinodemo-2.2.0/setup.py` & `pvrhinodemo-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     f.write('include pvrhinodemo/rhino_demo_mic.py')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvrhinodemo",
-    version="2.2.0",
+    version="2.2.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Rhino Speech-to-Intent engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/rhino",
     packages=["pvrhinodemo"],
```

