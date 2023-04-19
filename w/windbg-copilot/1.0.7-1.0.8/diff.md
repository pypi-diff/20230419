# Comparing `tmp/windbg_copilot-1.0.7.tar.gz` & `tmp/windbg_copilot-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.7.tar", last modified: Wed Apr 19 06:19:33 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.8.tar", last modified: Wed Apr 19 06:31:10 2023, max compression
```

## Comparing `windbg_copilot-1.0.7.tar` & `windbg_copilot-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-04-18 06:19:04.000000 windbg_copilot-1.0.7/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.633989 windbg_copilot-1.0.7/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.7/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-19 06:19:11.000000 windbg_copilot-1.0.7/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7043 2023-04-19 06:18:42.000000 windbg_copilot-1.0.7/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:19:33.662331 windbg_copilot-1.0.7/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-19 06:19:32.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 06:19:32.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 06:19:33.000000 windbg_copilot-1.0.7/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2979 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-04-19 06:30:34.000000 windbg_copilot-1.0.8/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.868481 windbg_copilot-1.0.8/windbg_copilot/
+-rw-rw-rw-   0        0        0       82 2023-04-19 06:29:21.000000 windbg_copilot-1.0.8/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-19 06:30:47.000000 windbg_copilot-1.0.8/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7034 2023-04-19 06:29:08.000000 windbg_copilot-1.0.8/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2979 2023-04-19 06:31:09.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:31:09.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.7/LICENSE.txt` & `windbg_copilot-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.7/PKG-INFO` & `windbg_copilot-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.7
+Version: 1.0.8
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -44,14 +44,15 @@
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
         import windbg_copilot
+        windbg_copilot.start()
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

### Comparing `windbg_copilot-1.0.7/README.md` & `windbg_copilot-1.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
         import windbg_copilot
+        windbg_copilot.start()
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

### Comparing `windbg_copilot-1.0.7/setup.cfg` & `windbg_copilot-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.7/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.8/windbg_copilot/windbg_copilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             else:
                 temp = self.output
         with self.buffer_lock:
             temp = self.output
             self.output = ""
         return temp
 
-def windbg_copilot():
+def start():
     print("Hello, I am Windows debugger copilot, I'm here to assist you.")
     speak("Hello, I am Windows debugger copilot, I'm here to assist you.")
 
     print("\nThis software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
     speak("This software is used for Windows debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
 
     print("\nFirst, please enter the memory dump file path.")
```

### Comparing `windbg_copilot-1.0.7/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.8/windbg_copilot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.7
+Version: 1.0.8
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -44,14 +44,15 @@
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
         import windbg_copilot
+        windbg_copilot.start()
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

