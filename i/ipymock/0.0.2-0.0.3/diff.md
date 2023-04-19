# Comparing `tmp/ipymock-0.0.2.tar.gz` & `tmp/ipymock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.0.2.tar", last modified: Wed Apr 19 01:57:12 2023, max compression
+gzip compressed data, was "ipymock-0.0.3.tar", last modified: Wed Apr 19 04:19:06 2023, max compression
```

## Comparing `ipymock-0.0.2.tar` & `ipymock-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.695889 ipymock-0.0.2/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.2/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.2/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 01:57:12.695591 ipymock-0.0.2/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-19 01:54:26.000000 ipymock-0.0.2/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.693112 ipymock-0.0.2/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1163 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     8411 2023-04-19 01:54:20.000000 ipymock-0.0.2/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.694659 ipymock-0.0.2/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 01:57:12.695203 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.2/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 01:57:12.000000 ipymock-0.0.2/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 01:56:51.000000 ipymock-0.0.2/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 01:57:12.696004 ipymock-0.0.2/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.2/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.103449 ipymock-0.0.3/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.0.3/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.0.3/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 04:19:06.103081 ipymock-0.0.3/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-19 04:17:33.000000 ipymock-0.0.3/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.098782 ipymock-0.0.3/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1163 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     8430 2023-04-19 04:17:24.000000 ipymock-0.0.3/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.101274 ipymock-0.0.3/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-19 04:19:06.102260 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.0.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-19 04:19:06.000000 ipymock-0.0.3/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.0.3/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-19 04:19:05.000000 ipymock-0.0.3/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-19 04:18:49.000000 ipymock-0.0.3/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-19 04:19:06.103591 ipymock-0.0.3/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.0.3/setup.py
```

### Comparing `ipymock-0.0.2/LICENSE` & `ipymock-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.2/PKG-INFO` & `ipymock-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.2/README.md` & `ipymock-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.2/ipymock/__init__.py` & `ipymock-0.0.3/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.2/ipymock/_nbdev.py` & `ipymock-0.0.3/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.0.2/ipymock/mock.py` & `ipymock-0.0.3/ipymock/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         stream=True
     )
 
     # get it again from response
     common.parent_message_id = ''
 
     for line in response.iter_lines():
-        if line == b'':
+        if not line.startswith(b'data: '):
             continue
 
         if line.endswith(b'[DONE]'):
             common.conversation_done_channel.append(True)
             break
 
         make_conversation_response = json.loads(line.decode('utf-8')[len('data: '):])
```

### Comparing `ipymock-0.0.2/ipymock.egg-info/PKG-INFO` & `ipymock-0.0.3/ipymock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.0.2/settings.ini` & `ipymock-0.0.3/settings.ini`

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
-version = 0.0.2
+version = 0.0.3
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.0.2/setup.py` & `ipymock-0.0.3/setup.py`

 * *Files identical despite different names*

