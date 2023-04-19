# Comparing `tmp/ipymock-0.0.1.tar.gz` & `tmp/ipymock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.0.1.tar", last modified: Tue Apr 18 09:17:57 2023, max compression
+gzip compressed data, was "ipymock-0.0.2.tar", last modified: Wed Apr 19 01:57:12 2023, max compression
```

## Comparing `ipymock-0.0.1.tar` & `ipymock-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-18 09:17:57.086678 ipymock-0.0.1/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.1/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.1/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-18 09:17:57.086108 ipymock-0.0.1/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-13 14:43:22.000000 ipymock-0.0.1/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-18 09:17:57.082391 ipymock-0.0.1/ipymock.egg-info/
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-18 09:17:56.000000 ipymock-0.0.1/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.1/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.1/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.1/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-18 09:17:56.000000 ipymock-0.0.1/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.1/ipymock.egg-info/top_level.txt
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-18 09:17:57.083912 ipymock-0.0.1/ipytest/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-18 08:51:53.000000 ipymock-0.0.1/ipytest/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1163 2023-04-18 08:51:53.000000 ipymock-0.0.1/ipytest/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     8340 2023-04-18 08:51:53.000000 ipymock-0.0.1/ipytest/mock.py
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-18 09:17:42.000000 ipymock-0.0.1/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-18 09:17:57.091263 ipymock-0.0.1/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.1/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.695889 ipymock-0.0.2/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.2/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.2/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 01:57:12.695591 ipymock-0.0.2/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-19 01:54:26.000000 ipymock-0.0.2/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.693112 ipymock-0.0.2/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1163 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     8411 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.694659 ipymock-0.0.2/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.695203 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.2/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 01:56:51.000000 ipymock-0.0.2/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 01:57:12.696004 ipymock-0.0.2/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.2/setup.py
```

### Comparing `ipymock-0.0.1/LICENSE` & `ipymock-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.1/PKG-INFO` & `ipymock-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -200,15 +200,15 @@
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
 ```python
-from ipytest import do
+from ipymock import do
 ```
 
 ```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
```

### Comparing `ipymock-0.0.1/README.md` & `ipymock-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
 ```python
-from ipytest import do
+from ipymock import do
 ```
 
 ```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
```

### Comparing `ipymock-0.0.1/ipymock.egg-info/PKG-INFO` & `ipymock-0.0.2/ipymock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -200,15 +200,15 @@
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
 ```python
-from ipytest import do
+from ipymock import do
 ```
 
 ```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
```

### Comparing `ipymock-0.0.1/ipytest/__init__.py` & `ipymock-0.0.2/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.1/ipytest/_nbdev.py` & `ipymock-0.0.2/ipymock/_nbdev.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,12 +23,12 @@
          "delta": "mock.ipynb",
          "mock_create": "mock.ipynb",
          "mock_openai": "mock.ipynb"}
 
 modules = ["__init__.py",
            "mock.py"]
 
-doc_url = "https://seii-saintway.github.io/ipytest/"
+doc_url = "https://seii-saintway.github.io/ipymock/"
 
-git_url = "https://github.com/seii-saintway/ipytest/tree/main/"
+git_url = "https://github.com/seii-saintway/ipymock/tree/main/"
 
 def custom_doc_links(name): return None
```

### Comparing `ipymock-0.0.1/ipytest/mock.py` & `ipymock-0.0.2/ipymock/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             common.message_channel.append(message)
 
 temp_conversation_id = ''
 
 def start_conversation(content):
     parent_message_id = common.parent_message_id
     if parent_message_id == '' or common.conversation_id == '':
+        common.conversation_id = ''
         parent_message_id = str(uuid.uuid4())
     response = requests.post(
         f'{chat_gpt_base_url}/conversation',
         headers = {
             'Authorization': access_token,
             'Content-Type': 'application/json',
             'Accept': 'text/event-stream'
@@ -184,19 +185,20 @@
 # Internal Cell
 # open the JSON file and read the conversation_id
 with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
     conversation_id = json.load(f).get('conversation_id', None)
 
 # Internal Cell
 try:
-    get_conversation(conversation_id)
     common.conversation_id = conversation_id
+    get_conversation(conversation_id)
 except requests.exceptions.ConnectionError as errc:
     print('Error Connecting:', errc)
-    common.conversation_id = ''
+except RecursionError as errr:
+    print('Error Recursion:', errr)
 
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
 def attributize(obj):
```

### Comparing `ipymock-0.0.1/settings.ini` & `ipymock-0.0.2/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.0.1
+version = 0.0.2
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.0.1/setup.py` & `ipymock-0.0.2/setup.py`

 * *Files identical despite different names*

