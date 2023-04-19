# Comparing `tmp/chatterstack-0.1.2.tar.gz` & `tmp/chatterstack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatterstack-0.1.2.tar", last modified: Wed Apr 19 08:27:38 2023, max compression
+gzip compressed data, was "chatterstack-0.1.3.tar", last modified: Wed Apr 19 09:02:42 2023, max compression
```

## Comparing `chatterstack-0.1.2.tar` & `chatterstack-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 08:27:38.705594 chatterstack-0.1.2/
--rw-r--r--   0 davidschiller   (501) staff       (20)     9993 2023-04-19 08:27:38.705465 chatterstack-0.1.2/PKG-INFO
--rw-r--r--   0 davidschiller   (501) staff       (20)     9262 2023-04-19 07:51:23.000000 chatterstack-0.1.2/README.md
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 08:27:38.704501 chatterstack-0.1.2/chatterstack/
--rw-r--r--   0 davidschiller   (501) staff       (20)       39 2023-04-17 05:16:34.000000 chatterstack-0.1.2/chatterstack/__init__.py
--rw-r--r--   0 davidschiller   (501) staff       (20)    10339 2023-04-19 07:38:38.000000 chatterstack-0.1.2/chatterstack/chatterstack.py
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 08:27:38.705242 chatterstack-0.1.2/chatterstack.egg-info/
--rw-r--r--   0 davidschiller   (501) staff       (20)     9993 2023-04-19 08:27:38.000000 chatterstack-0.1.2/chatterstack.egg-info/PKG-INFO
--rw-r--r--   0 davidschiller   (501) staff       (20)      251 2023-04-19 08:27:38.000000 chatterstack-0.1.2/chatterstack.egg-info/SOURCES.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)        1 2023-04-19 08:27:38.000000 chatterstack-0.1.2/chatterstack.egg-info/dependency_links.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)        7 2023-04-19 08:27:38.000000 chatterstack-0.1.2/chatterstack.egg-info/requires.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)       13 2023-04-19 08:27:38.000000 chatterstack-0.1.2/chatterstack.egg-info/top_level.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)       38 2023-04-19 08:27:38.705638 chatterstack-0.1.2/setup.cfg
--rw-r--r--   0 davidschiller   (501) staff       (20)      949 2023-04-19 08:26:47.000000 chatterstack-0.1.2/setup.py
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 09:02:42.425899 chatterstack-0.1.3/
+-rw-r--r--   0 davidschiller   (501) staff       (20)    10000 2023-04-19 09:02:42.425778 chatterstack-0.1.3/PKG-INFO
+-rw-r--r--   0 davidschiller   (501) staff       (20)     9269 2023-04-19 08:46:45.000000 chatterstack-0.1.3/README.md
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 09:02:42.424766 chatterstack-0.1.3/chatterstack/
+-rw-r--r--   0 davidschiller   (501) staff       (20)       39 2023-04-17 05:16:34.000000 chatterstack-0.1.3/chatterstack/__init__.py
+-rw-r--r--   0 davidschiller   (501) staff       (20)    10220 2023-04-19 08:54:59.000000 chatterstack-0.1.3/chatterstack/chatterstack.py
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-04-19 09:02:42.425539 chatterstack-0.1.3/chatterstack.egg-info/
+-rw-r--r--   0 davidschiller   (501) staff       (20)    10000 2023-04-19 09:02:42.000000 chatterstack-0.1.3/chatterstack.egg-info/PKG-INFO
+-rw-r--r--   0 davidschiller   (501) staff       (20)      251 2023-04-19 09:02:42.000000 chatterstack-0.1.3/chatterstack.egg-info/SOURCES.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)        1 2023-04-19 09:02:42.000000 chatterstack-0.1.3/chatterstack.egg-info/dependency_links.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)        7 2023-04-19 09:02:42.000000 chatterstack-0.1.3/chatterstack.egg-info/requires.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)       13 2023-04-19 09:02:42.000000 chatterstack-0.1.3/chatterstack.egg-info/top_level.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)       38 2023-04-19 09:02:42.425941 chatterstack-0.1.3/setup.cfg
+-rw-r--r--   0 davidschiller   (501) staff       (20)      949 2023-04-19 08:55:49.000000 chatterstack-0.1.3/setup.py
```

### Comparing `chatterstack-0.1.2/PKG-INFO` & `chatterstack-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatterstack
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.
 Home-page: https://github.com/dschil138/chatterstack
 Author: David Schiller
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -89,22 +89,24 @@
 while True:
     # Change the terminal prefix
     convo.user_input(user_prefix="ME: ")
 
     # any of the API arguments
     convo.send_to_bot(model="gpt-4", temperature=1, max_tokens=40)
 
-    # remove the empty spacer lines
-    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=0)
+    # change the prefix and line spacing
+    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=2)
 ```
 Now the conversation looks like this:
 
 ```txt
 ME: hey, can you help me with something?
 GPT: Of course! I'm here to help. Please let me know what you need assistance with, and I'll do my best to help you.
+
+
 ME: I need to know if France has a President or a Prime Minister
 GPT: France has both a President and a Prime Minister. The President of France is [...bot goes on]
 ```
 There is more info about the current defaults and various methods to change them below in the section about sending messages to the API
 
 ---
```

### Comparing `chatterstack-0.1.2/README.md` & `chatterstack-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,24 @@
 while True:
     # Change the terminal prefix
     convo.user_input(user_prefix="ME: ")
 
     # any of the API arguments
     convo.send_to_bot(model="gpt-4", temperature=1, max_tokens=40)
 
-    # remove the empty spacer lines
-    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=0)
+    # change the prefix and line spacing
+    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=2)
 ```
 Now the conversation looks like this:
 
 ```txt
 ME: hey, can you help me with something?
 GPT: Of course! I'm here to help. Please let me know what you need assistance with, and I'll do my best to help you.
+
+
 ME: I need to know if France has a President or a Prime Minister
 GPT: France has both a President and a Prime Minister. The President of France is [...bot goes on]
 ```
 There is more info about the current defaults and various methods to change them below in the section about sending messages to the API
 
 ---
```

### Comparing `chatterstack-0.1.2/chatterstack/chatterstack.py` & `chatterstack-0.1.3/chatterstack/chatterstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 class Chatterstack:
     
     def __init__(self, user_defaults=None, existing_list=None):
         """Initialize the Chatist class with optional user default values & existing list, if any."""
         self.config = {
             key: value
             for key, value in (user_defaults or {}).items()
-            if key in {"MODEL", "TEMPERATURE", "TOP_P", "FREQUENCY_PENALTY", "PRESENCE_PENALTY", "MAX_TOKENS", "STOP", "LOG_PROBS", "STREAM", "LOGIT_BIAS"}
+            if key in {"MODEL", "TEMPERATURE", "TOP_P", "FREQUENCY_PENALTY", "PRESENCE_PENALTY", "MAX_TOKENS", "STOP", "STREAM", "LOGIT_BIAS"}
         }
 
         if existing_list is None:
             self.list = []
         else:
             self.list = existing_list
 
         self.reminders = []
         self.timestamps = True
 
         self.last_response_prompt_tokens=0
         self.last_response_assistant_tokens=0
         self.last_response_tokens=0
-
         self.total_prompt_tokens=0
         self.total_assistant_tokens=0
         self.total_tokens=0
     
     def __str__(self):
         """Return a string representation of the conversation."""
         return str(self.list)
@@ -117,29 +116,27 @@
         """Send the conversation to the OpenAI API and append the response to the end of the conversation. Uses 3.5-turbo by default."""
         model = kwargs.get("model", self.config.get("model", "gpt-3.5-turbo"))
         temperature = kwargs.get("temperature", self.config.get("temperature", 0.8))
         top_p = kwargs.get("top_p", self.config.get("top_p", 1))
         frequency_penalty = kwargs.get("frequency_penalty", self.config.get("frequency_penalty", 0))
         presence_penalty = kwargs.get("presence_penalty", self.config.get("presence_penalty", 0))
         max_tokens = kwargs.get("max_tokens", self.config.get("max_tokens", 200))
-        stop = kwargs.get("stop", self.config.get("stop", 200))
-        logprobs = kwargs.get("logprobs", self.config.get("logprobs", 200))
-        stream = kwargs.get("stream", self.config.get("stream", 200))
-        logit_bias = kwargs.get("logit_bias", self.config.get("logit_bias", 200))
+        stop = kwargs.get("stop", self.config.get("stop", None))
+        stream = kwargs.get("stream", self.config.get("stream", False))
+        logit_bias = kwargs.get("logit_bias", self.config.get("logit_bias", {}))
 
         response = openai.ChatCompletion.create(
             model=model,
             messages=self.list,
             temperature=temperature,
             top_p=top_p,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             max_tokens=max_tokens,
             stop=stop,
-            logprobs=logprobs,
             stream=stream,
             logit_bias=logit_bias,
         )
         print(response.choices[0].message.content.strip())
         api_usage = response['usage']
         new_prompt_tokens = int((api_usage['prompt_tokens']))
         new_assistant_tokens = int((api_usage['completion_tokens']))
```

### Comparing `chatterstack-0.1.2/chatterstack.egg-info/PKG-INFO` & `chatterstack-0.1.3/chatterstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatterstack
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.
 Home-page: https://github.com/dschil138/chatterstack
 Author: David Schiller
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -89,22 +89,24 @@
 while True:
     # Change the terminal prefix
     convo.user_input(user_prefix="ME: ")
 
     # any of the API arguments
     convo.send_to_bot(model="gpt-4", temperature=1, max_tokens=40)
 
-    # remove the empty spacer lines
-    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=0)
+    # change the prefix and line spacing
+    convo.print_last_message(assistant_prefix="GPT: ", lines_before=0, lines_after=2)
 ```
 Now the conversation looks like this:
 
 ```txt
 ME: hey, can you help me with something?
 GPT: Of course! I'm here to help. Please let me know what you need assistance with, and I'll do my best to help you.
+
+
 ME: I need to know if France has a President or a Prime Minister
 GPT: France has both a President and a Prime Minister. The President of France is [...bot goes on]
 ```
 There is more info about the current defaults and various methods to change them below in the section about sending messages to the API
 
 ---
```

### Comparing `chatterstack-0.1.2/setup.py` & `chatterstack-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatterstack",
-    version="0.1.2",
+    version="0.1.3",
     description="A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="David Schiller",
     url="https://github.com/dschil138/chatterstack",
     packages=find_packages(),
     classifiers=[
```

