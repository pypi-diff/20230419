# Comparing `tmp/ipymock-0.0.3.tar.gz` & `tmp/ipymock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.0.3.tar", last modified: Wed Apr 19 04:19:06 2023, max compression
+gzip compressed data, was "ipymock-0.0.4.tar", last modified: Wed Apr 19 06:43:48 2023, max compression
```

## Comparing `ipymock-0.0.3.tar` & `ipymock-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.103449 ipymock-0.0.3/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.3/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.3/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 04:19:06.103081 ipymock-0.0.3/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-19 04:17:33.000000 ipymock-0.0.3/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.098782 ipymock-0.0.3/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1163 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     8430 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.101274 ipymock-0.0.3/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.102260 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 04:19:06.000000 ipymock-0.0.3/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.3/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 04:18:49.000000 ipymock-0.0.3/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 04:19:06.103591 ipymock-0.0.3/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.3/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 06:43:48.668012 ipymock-0.0.4/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.4/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.4/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 06:43:48.667692 ipymock-0.0.4/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-19 06:43:37.000000 ipymock-0.0.4/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 06:43:48.663887 ipymock-0.0.4/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 06:43:27.000000 ipymock-0.0.4/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1116 2023-04-19 06:43:27.000000 ipymock-0.0.4/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     8418 2023-04-19 06:43:27.000000 ipymock-0.0.4/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 06:43:48.665809 ipymock-0.0.4/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 06:43:48.666834 ipymock-0.0.4/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.4/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.4/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 06:43:48.000000 ipymock-0.0.4/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 06:43:48.000000 ipymock-0.0.4/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 06:43:48.000000 ipymock-0.0.4/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.4/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 06:43:48.000000 ipymock-0.0.4/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 06:43:48.000000 ipymock-0.0.4/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 06:42:39.000000 ipymock-0.0.4/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 06:43:48.668161 ipymock-0.0.4/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.4/setup.py
```

### Comparing `ipymock-0.0.3/LICENSE` & `ipymock-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.3/PKG-INFO` & `ipymock-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.3/README.md` & `ipymock-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.3/ipymock/__init__.py` & `ipymock-0.0.4/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.3/ipymock/_nbdev.py` & `ipymock-0.0.4/ipymock/_nbdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
          "generate_title": "mock.ipynb",
          "rename_title": "mock.ipynb",
          "delete_conversation": "mock.ipynb",
          "recover_conversation": "mock.ipynb",
          "clear_conversations": "mock.ipynb",
          "chat_gpt_base_url": "mock.ipynb",
          "common": "mock.ipynb",
-         "temp_conversation_id": "mock.ipynb",
          "attrdict": "mock.ipynb",
          "attributize": "mock.ipynb",
          "delta": "mock.ipynb",
          "mock_create": "mock.ipynb",
          "mock_openai": "mock.ipynb"}
 
 modules = ["__init__.py",
```

### Comparing `ipymock-0.0.3/ipymock/mock.py` & `ipymock-0.0.4/ipymock/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/mock.ipynb (unless otherwise specified).
 
 __all__ = ['get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
-           'chat_gpt_base_url', 'common', 'temp_conversation_id', 'attrdict', 'attributize', 'delta', 'mock_create',
-           'mock_openai']
+           'chat_gpt_base_url', 'common', 'attrdict', 'attributize', 'delta', 'mock_create', 'mock_openai']
 
 # Internal Cell
 class Common:
     chat_gpt_model = 'gpt-3.5-turbo'
     role_user = 'user'
     role_assistant = 'assistant'
 
@@ -56,16 +55,14 @@
         return
     message = conversation_detail['message']
     parts = message['content']['parts']
     if len(parts) > 0 and parts[0] != '':
         if message['author']['role'] == common.role_user:
             common.message_channel.append(message)
 
-temp_conversation_id = ''
-
 def start_conversation(content):
     parent_message_id = common.parent_message_id
     if parent_message_id == '' or common.conversation_id == '':
         common.conversation_id = ''
         parent_message_id = str(uuid.uuid4())
     response = requests.post(
         f'{chat_gpt_base_url}/conversation',
@@ -93,40 +90,41 @@
             'continue_text': 'continue'
         }),
         stream=True
     )
 
     # get it again from response
     common.parent_message_id = ''
+    temp_conversation_id = ''
 
     for line in response.iter_lines():
         if not line.startswith(b'data: '):
             continue
 
         if line.endswith(b'[DONE]'):
             common.conversation_done_channel.append(True)
             break
 
         make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
         if common.parent_message_id == '':
             common.parent_message_id = make_conversation_response['message']['id']
-        global temp_conversation_id
-        if common.conversation_id == '' and temp_conversation_id == '':
+        if common.conversation_id == '':
             temp_conversation_id = make_conversation_response['conversation_id']
         if make_conversation_response is not None:
             parts = make_conversation_response['message']['content']['parts']
             if len(parts) > 0:
                 common.response_text_channel.append(parts[0])
                 yield parts[0]
             if make_conversation_response['message']['end_turn'] == True:
                 common.conversation_done_channel.append(True)
                 break
 
-    if common.conversation_id == '':
-        generate_title(temp_conversation_id)
+    if common.conversation_id == '' and temp_conversation_id != '':
+        common.conversation_id = temp_conversation_id
+        generate_title(common.conversation_id)
     else:
         common.reload_conversations_channel.append(True)
 
 def generate_title(conversation_id):
     requests.post(
         f'{chat_gpt_base_url}/conversation/gen_title/{conversation_id}',
         headers = {
```

### Comparing `ipymock-0.0.3/ipymock.egg-info/PKG-INFO` & `ipymock-0.0.4/ipymock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.3/settings.ini` & `ipymock-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.0.3
+version = 0.0.4
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.0.3/setup.py` & `ipymock-0.0.4/setup.py`

 * *Files identical despite different names*

