# Comparing `tmp/chatblade-0.2.2.tar.gz` & `tmp/chatblade-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatblade-0.2.2.tar", last modified: Tue Apr 11 09:31:41 2023, max compression
+gzip compressed data, was "chatblade-0.2.3.tar", last modified: Wed Apr 19 05:28:09 2023, max compression
```

## Comparing `chatblade-0.2.2.tar` & `chatblade-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489752 chatblade-0.2.2/
--rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.2.2/LICENSE
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-11 09:31:41.489806 chatblade-0.2.2/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)    10405 2023-04-11 09:29:23.000000 chatblade-0.2.2/README.md
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489031 chatblade-0.2.2/chatblade/
--rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.2.2/chatblade/__init__.py
--rw-r--r--   0 npiv       (501) staff       (20)       86 2023-03-18 14:05:20.000000 chatblade-0.2.2/chatblade/__main__.py
--rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/chat.py
--rw-r--r--   0 npiv       (501) staff       (20)     4584 2023-04-09 08:15:38.000000 chatblade-0.2.2/chatblade/cli.py
--rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.2.2/chatblade/errors.py
--rw-r--r--   0 npiv       (501) staff       (20)     5590 2023-04-09 08:15:38.000000 chatblade-0.2.2/chatblade/parser.py
--rw-r--r--   0 npiv       (501) staff       (20)     4543 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/printer.py
--rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/session.py
--rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.2.2/chatblade/storage.py
--rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/utils.py
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489658 chatblade-0.2.2/chatblade.egg-info/
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)      452 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/SOURCES.txt
--rw-r--r--   0 npiv       (501) staff       (20)        1 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/dependency_links.txt
--rw-r--r--   0 npiv       (501) staff       (20)       54 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/entry_points.txt
--rw-r--r--   0 npiv       (501) staff       (20)       49 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/requires.txt
--rw-r--r--   0 npiv       (501) staff       (20)       10 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/top_level.txt
--rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.2.2/pyproject.toml
--rw-r--r--   0 npiv       (501) staff       (20)      567 2023-04-11 09:31:41.490054 chatblade-0.2.2/setup.cfg
--rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.2.2/setup.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.353952 chatblade-0.2.3/
+-rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.2.3/LICENSE
+-rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-19 05:28:09.354025 chatblade-0.2.3/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)    10405 2023-04-11 09:29:23.000000 chatblade-0.2.3/README.md
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.346266 chatblade-0.2.3/chatblade/
+-rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.2.3/chatblade/__init__.py
+-rw-r--r--   0 npiv       (501) staff       (20)       86 2023-03-18 14:05:20.000000 chatblade-0.2.3/chatblade/__main__.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/chat.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4613 2023-04-19 05:17:37.000000 chatblade-0.2.3/chatblade/cli.py
+-rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.2.3/chatblade/errors.py
+-rw-r--r--   0 npiv       (501) staff       (20)     5590 2023-04-09 08:15:38.000000 chatblade-0.2.3/chatblade/parser.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4543 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/printer.py
+-rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/session.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.2.3/chatblade/storage.py
+-rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.2.3/chatblade/utils.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-19 05:28:09.353856 chatblade-0.2.3/chatblade.egg-info/
+-rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)      452 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/SOURCES.txt
+-rw-r--r--   0 npiv       (501) staff       (20)        1 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/dependency_links.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       54 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/entry_points.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       49 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/requires.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       10 2023-04-19 05:28:09.000000 chatblade-0.2.3/chatblade.egg-info/top_level.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.2.3/pyproject.toml
+-rw-r--r--   0 npiv       (501) staff       (20)      567 2023-04-19 05:28:09.354397 chatblade-0.2.3/setup.cfg
+-rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.2.3/setup.py
```

### Comparing `chatblade-0.2.2/LICENSE` & `chatblade-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/PKG-INFO` & `chatblade-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chatblade-0.2.2/README.md` & `chatblade-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/chat.py` & `chatblade-0.2.3/chatblade/chat.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/cli.py` & `chatblade-0.2.3/chatblade/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def fetch_and_cache(messages, params):
     result = chat.query_chat_gpt(messages, params)
     if isinstance(result, types.GeneratorType):
         text = Text("")
         message = None
-        with Live(text, refresh_per_second=4) as live:
+        with Live(text, refresh_per_second=4, vertical_overflow="visible") as live:
             for message in result:
                 live.update(message.content)
             live.update("")
         response_msg = message
     else:
         response_msg = chat.query_chat_gpt(messages, params)
     messages.append(response_msg)
```

### Comparing `chatblade-0.2.2/chatblade/parser.py` & `chatblade-0.2.3/chatblade/parser.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/printer.py` & `chatblade-0.2.3/chatblade/printer.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/session.py` & `chatblade-0.2.3/chatblade/session.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/storage.py` & `chatblade-0.2.3/chatblade/storage.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade/utils.py` & `chatblade-0.2.3/chatblade/utils.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.2/chatblade.egg-info/PKG-INFO` & `chatblade-0.2.3/chatblade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chatblade-0.2.2/setup.cfg` & `chatblade-0.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chatblade
-version = 0.2.2
+version = 0.2.3
 description = CLI Swiss Army Knife for ChatGPT
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/npiv/chatblade
 keywords = chatblade chatgpt cli python
 project_urls =
```

