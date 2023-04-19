# Comparing `tmp/picovoicedemo-2.2.0.tar.gz` & `tmp/picovoicedemo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoicedemo-2.2.0.tar", last modified: Wed Apr 12 18:12:50 2023, max compression
+gzip compressed data, was "picovoicedemo-2.2.1.tar", last modified: Wed Apr 19 17:57:19 2023, max compression
```

## Comparing `picovoicedemo-2.2.0.tar` & `picovoicedemo-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      119 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4236 2023-04-10 19:55:03.000000 picovoicedemo-2.2.0/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.022604 picovoicedemo-2.2.0/picovoicedemo/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6576 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_file.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6876 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_mic.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/picovoicedemo.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      349 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      138 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/entry_points.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       35 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       14 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2537 2023-04-12 18:08:55.000000 picovoicedemo-2.2.0/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      119 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4236 2023-04-18 21:24:31.000000 picovoicedemo-2.2.1/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/picovoicedemo/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/LICENSE
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6568 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_file.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6876 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_mic.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/picovoicedemo.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      349 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      138 2023-04-19 17:57:18.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       35 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       14 2023-04-19 17:57:19.000000 picovoicedemo-2.2.1/picovoicedemo.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-19 17:57:19.188887 picovoicedemo-2.2.1/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2537 2023-04-19 17:54:51.000000 picovoicedemo-2.2.1/setup.py
```

### Comparing `picovoicedemo-2.2.0/PKG-INFO` & `picovoicedemo-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `picovoicedemo-2.2.0/README.md` & `picovoicedemo-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.0/picovoicedemo/LICENSE` & `picovoicedemo-2.2.1/picovoicedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_file.py` & `picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     except PicovoiceActivationThrottledError as e:
         print("AccessKey '%s has been throttled" % args.access_key)
         raise e
     except PicovoiceError as e:
         print("Failed to initialize Picovoice")
         raise e
 
-    audio = read_file(args.input_audio_path, pv.sample_rate)
+    audio = read_file(args.wav_path, pv.sample_rate)
 
     for i in range(len(audio) // pv.frame_length):
         frame = audio[i * pv.frame_length:(i + 1) * pv.frame_length]
         pv.process(frame)
 
     pv.delete()
```

### Comparing `picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_mic.py` & `picovoicedemo-2.2.1/picovoicedemo/picovoice_demo_mic.py`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.2.0/picovoicedemo.egg-info/PKG-INFO` & `picovoicedemo-2.2.1/picovoicedemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `picovoicedemo-2.2.0/setup.py` & `picovoicedemo-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     f.write('include picovoicedemo/picovoice_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoicedemo",
-    version="2.2.0",
+    version="2.2.1",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoicedemo"],
```

