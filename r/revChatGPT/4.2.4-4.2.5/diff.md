# Comparing `tmp/revChatGPT-4.2.4.tar.gz` & `tmp/revChatGPT-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.4.tar", last modified: Tue Apr 18 02:36:58 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.5.tar", last modified: Wed Apr 19 00:35:23 2023, max compression
```

## Comparing `revChatGPT-4.2.4.tar` & `revChatGPT-4.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.282492 revChatGPT-4.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47267 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-18 02:36:29.000000 revChatGPT-4.2.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:36:58.286491 revChatGPT-4.2.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 02:36:58.000000 revChatGPT-4.2.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-19 00:35:22.000000 revChatGPT-4.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47161 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-19 00:34:54.000000 revChatGPT-4.2.5/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:35:23.014792 revChatGPT-4.2.5/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 00:35:23.000000 revChatGPT-4.2.5/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.2.4/LICENSE` & `revChatGPT-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.4/PKG-INFO` & `revChatGPT-4.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.4
+Version: 4.2.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

### Comparing `revChatGPT-4.2.4/README.md` & `revChatGPT-4.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

### Comparing `revChatGPT-4.2.4/setup.py` & `revChatGPT-4.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.4",
+    version="4.2.5",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.2.4/src/revChatGPT/V1.py` & `revChatGPT-4.2.5/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,22 +496,16 @@
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
-                    log.debug(
-                        f"Conversation ID {conversation_id} not found in conversation mapping, mapping conversations",
-                    )
                     self.__map_conversations()
             if conversation_id in self.conversation_mapping:
-                log.debug(
-                    f"Conversation ID {conversation_id} found in conversation mapping, setting parent_id to {self.conversation_mapping[conversation_id]}",
-                )
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
@@ -636,17 +630,14 @@
                         ]
                 else:
                     log.debug(
                         f"Conversation ID {conversation_id} not found in conversation mapping, mapping conversations",
                     )
                     self.__map_conversations()
             if conversation_id in self.conversation_mapping:
-                log.debug(
-                    f"Conversation ID {conversation_id} found in conversation mapping, setting parent_id to {self.conversation_mapping[conversation_id]}",
-                )
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "continue",
@@ -942,15 +933,19 @@
 
         parent_id = parent_id or self.parent_id or ""
         if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 await self.__map_conversations()
-            parent_id = self.conversation_mapping[conversation_id]
+            if conversation_id in self.conversation_mapping:
+                parent_id = self.conversation_mapping[conversation_id]
+            else:  # invalid conversation_id provided, treat as a new conversation
+                conversation_id = None
+                parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
@@ -1061,15 +1056,19 @@
 
         parent_id = parent_id or self.parent_id or ""
         if not conversation_id and not parent_id:
             parent_id = str(uuid.uuid4())
         if conversation_id and not parent_id:
             if conversation_id not in self.conversation_mapping:
                 await self.__map_conversations()
-            parent_id = self.conversation_mapping[conversation_id]
+            if conversation_id in self.conversation_mapping:
+                parent_id = self.conversation_mapping[conversation_id]
+            else:  # invalid conversation_id provided, treat as a new conversation
+                conversation_id = None
+                parent_id = str(uuid.uuid4())
 
         data = {
             "action": "continue",
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
             or self.config.get("model")
```

### Comparing `revChatGPT-4.2.4/src/revChatGPT/V3.py` & `revChatGPT-4.2.5/src/revChatGPT/V3.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             "gpt-3.5-turbo",
             "gpt-3.5-turbo-0301",
             "gpt-4",
             "gpt-4-0314",
             "gpt-4-32k",
             "gpt-4-32k-0314",
         ]:
-            raise NotImplementedError("Unsupported engine {self.engine}")
+            raise NotImplementedError(f"Unsupported engine {self.engine}")
 
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
```

### Comparing `revChatGPT-4.2.4/src/revChatGPT/__init__.py` & `revChatGPT-4.2.5/src/revChatGPT/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The __init__ file does not a main file
 
 You can import the following module to use:
 revChatGPT.V0
 revChatGPT.V1
 revChatGPT.V3
 """
-__version__ = "4.2.2"
+__version__ = "4.2.4"
 __all__ = ()
 
 # Available Python Version Verify
 from . import typings as t
 from platform import python_version_tuple
 from platform import python_version
 from warnings import warn
```

### Comparing `revChatGPT-4.2.4/src/revChatGPT/__main__.py` & `revChatGPT-4.2.5/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.5/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.4/src/revChatGPT/typings.py` & `revChatGPT-4.2.5/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.4/src/revChatGPT/utils.py` & `revChatGPT-4.2.5/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.5/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.4
+Version: 4.2.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

