# Comparing `tmp/chat-spiral-0.0.4.tar.gz` & `tmp/chat-spiral-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-spiral-0.0.4.tar", last modified: Sat Apr 15 02:18:49 2023, max compression
+gzip compressed data, was "chat-spiral-0.0.5.tar", last modified: Wed Apr 19 00:12:37 2023, max compression
```

## Comparing `chat-spiral-0.0.4.tar` & `chat-spiral-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.264073 chat-spiral-0.0.4/
--rw-rw-rw-   0        0        0     1092 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    12666 2023-04-15 02:18:49.263098 chat-spiral-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    12143 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.200752 chat-spiral-0.0.4/chat_spiral.egg-info/
--rw-rw-rw-   0        0        0    12666 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-04-15 02:18:49.000000 chat-spiral-0.0.4/chat_spiral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 02:18:49.264073 chat-spiral-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-04-15 02:17:11.000000 chat-spiral-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.261117 chat-spiral-0.0.4/spiral/
--rw-rw-rw-   0        0        0       21 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/chat_llm.py
--rw-rw-rw-   0        0        0    51040 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/flow.py
--rw-rw-rw-   0        0        0     7551 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/memory.py
--rw-rw-rw-   0        0        0    14377 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/message.py
--rw-rw-rw-   0        0        0     2266 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:12:37.054072 chat-spiral-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 chat-spiral-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    12666 2023-04-19 00:12:37.050081 chat-spiral-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12143 2023-04-14 15:30:44.000000 chat-spiral-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 00:12:37.030637 chat-spiral-0.0.5/chat_spiral.egg-info/
+-rw-rw-rw-   0        0        0    12666 2023-04-19 00:12:36.000000 chat-spiral-0.0.5/chat_spiral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-04-19 00:12:36.000000 chat-spiral-0.0.5/chat_spiral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 00:12:36.000000 chat-spiral-0.0.5/chat_spiral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-19 00:12:36.000000 chat-spiral-0.0.5/chat_spiral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 00:12:36.000000 chat-spiral-0.0.5/chat_spiral.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 00:12:37.054072 chat-spiral-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-04-19 00:12:05.000000 chat-spiral-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:12:37.047563 chat-spiral-0.0.5/spiral/
+-rw-rw-rw-   0        0        0       21 2023-04-19 00:12:13.000000 chat-spiral-0.0.5/spiral/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 chat-spiral-0.0.5/spiral/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 chat-spiral-0.0.5/spiral/chat_llm.py
+-rw-rw-rw-   0        0        0    51040 2023-04-14 15:31:34.000000 chat-spiral-0.0.5/spiral/flow.py
+-rw-rw-rw-   0        0        0     7551 2023-04-14 21:28:49.000000 chat-spiral-0.0.5/spiral/memory.py
+-rw-rw-rw-   0        0        0    14377 2023-04-14 20:40:16.000000 chat-spiral-0.0.5/spiral/message.py
+-rw-rw-rw-   0        0        0     2266 2023-04-14 15:31:34.000000 chat-spiral-0.0.5/spiral/tools.py
```

### Comparing `chat-spiral-0.0.4/LICENSE` & `chat-spiral-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/PKG-INFO` & `chat-spiral-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chat-spiral-0.0.4/README.md` & `chat-spiral-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/chat_spiral.egg-info/PKG-INFO` & `chat-spiral-0.0.5/chat_spiral.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chat-spiral-0.0.4/setup.py` & `chat-spiral-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chat-spiral",
-    version="0.0.4",
+    version="0.0.5",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/spiral",
     packages=setuptools.find_packages(),
     install_requires=[
         "regex",
         "openai",
         "pandas",
         "tiktoken",
-        "faiss"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
```

### Comparing `chat-spiral-0.0.4/spiral/chat_history.py` & `chat-spiral-0.0.5/spiral/chat_history.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/spiral/chat_llm.py` & `chat-spiral-0.0.5/spiral/chat_llm.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/spiral/flow.py` & `chat-spiral-0.0.5/spiral/flow.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/spiral/memory.py` & `chat-spiral-0.0.5/spiral/memory.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/spiral/message.py` & `chat-spiral-0.0.5/spiral/message.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.4/spiral/tools.py` & `chat-spiral-0.0.5/spiral/tools.py`

 * *Files identical despite different names*

