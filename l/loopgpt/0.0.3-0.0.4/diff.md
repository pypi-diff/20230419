# Comparing `tmp/loopgpt-0.0.3.tar.gz` & `tmp/loopgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.3.tar", last modified: Wed Apr 19 00:28:04 2023, max compression
+gzip compressed data, was "loopgpt-0.0.4.tar", last modified: Wed Apr 19 00:32:10 2023, max compression
```

## Comparing `loopgpt-0.0.3.tar` & `loopgpt-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.303547 loopgpt-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-19 00:28:04.303547 loopgpt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8005 2023-04-19 00:00:57.000000 loopgpt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.279332 loopgpt-0.0.3/loopgpt/
--rw-rw-rw-   0        0        0      486 2023-04-19 00:27:55.000000 loopgpt-0.0.3/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16188 2023-04-18 22:30:05.000000 loopgpt-0.0.3/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.3/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.287435 loopgpt-0.0.3/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.3/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.287435 loopgpt-0.0.3/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.3/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0      964 2023-04-18 01:42:45.000000 loopgpt-0.0.3/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     6710 2023-04-18 23:45:53.000000 loopgpt-0.0.3/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.3/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.295503 loopgpt-0.0.3/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.295503 loopgpt-0.0.3/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.3/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.3/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.3/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.303547 loopgpt-0.0.3/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.3/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.3/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.3/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.3/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.3/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.3/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.3/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.3/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.3/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:28:04.279332 loopgpt-0.0.3/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      911 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 00:28:04.000000 loopgpt-0.0.3/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 00:28:04.303547 loopgpt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-19 00:27:51.000000 loopgpt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.299148 loopgpt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8005 2023-04-19 00:00:57.000000 loopgpt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.266986 loopgpt-0.0.4/loopgpt/
+-rw-rw-rw-   0        0        0      486 2023-04-19 00:31:06.000000 loopgpt-0.0.4/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    16188 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/agent.py
+-rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.275039 loopgpt-0.0.4/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/embeddings/provider.py
+-rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.4/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.4/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-04-18 01:42:45.000000 loopgpt-0.0.4/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     6710 2023-04-18 23:45:53.000000 loopgpt-0.0.4/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.4/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.283056 loopgpt-0.0.4/loopgpt/models/
+-rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.4/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.4/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.4/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.4/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.4/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.4/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.4/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.4/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.4/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.4/loopgpt/tools/simple_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.299148 loopgpt-0.0.4/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.4/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.4/loopgpt/utils/spinner.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:32:10.275039 loopgpt-0.0.4/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 00:32:10.000000 loopgpt-0.0.4/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 00:32:10.299148 loopgpt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-04-19 00:31:02.000000 loopgpt-0.0.4/setup.py
```

### Comparing `loopgpt-0.0.3/LICENSE` & `loopgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/README.md` & `loopgpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/agent.py` & `loopgpt-0.0.4/loopgpt/agent.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/constants.py` & `loopgpt-0.0.4/loopgpt/constants.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/embeddings/__init__.py` & `loopgpt-0.0.4/loopgpt/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/embeddings/openai_.py` & `loopgpt-0.0.4/loopgpt/embeddings/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/loops/cli.py` & `loopgpt-0.0.4/loopgpt/loops/cli.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/loops/repl.py` & `loopgpt-0.0.4/loopgpt/loops/repl.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/loops/ui.py` & `loopgpt-0.0.4/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/memory/__init__.py` & `loopgpt-0.0.4/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/memory/local_memory.py` & `loopgpt-0.0.4/loopgpt/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/models/openai_.py` & `loopgpt-0.0.4/loopgpt/models/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/summarizer.py` & `loopgpt-0.0.4/loopgpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/__init__.py` & `loopgpt-0.0.4/loopgpt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/agent_manager.py` & `loopgpt-0.0.4/loopgpt/tools/agent_manager.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/base_tool.py` & `loopgpt-0.0.4/loopgpt/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/browser.py` & `loopgpt-0.0.4/loopgpt/tools/browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/code.py` & `loopgpt-0.0.4/loopgpt/tools/code.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/filesystem.py` & `loopgpt-0.0.4/loopgpt/tools/filesystem.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/google_search.py` & `loopgpt-0.0.4/loopgpt/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/shell.py` & `loopgpt-0.0.4/loopgpt/tools/shell.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt/tools/simple_browser.py` & `loopgpt-0.0.4/loopgpt/tools/simple_browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.3/loopgpt.egg-info/SOURCES.txt` & `loopgpt-0.0.4/loopgpt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -29,8 +29,10 @@
 loopgpt/tools/base_tool.py
 loopgpt/tools/browser.py
 loopgpt/tools/code.py
 loopgpt/tools/filesystem.py
 loopgpt/tools/google_search.py
 loopgpt/tools/memory_manager.py
 loopgpt/tools/shell.py
-loopgpt/tools/simple_browser.py
+loopgpt/tools/simple_browser.py
+loopgpt/utils/__init__.py
+loopgpt/utils/spinner.py
```

