# Comparing `tmp/xiaogpt-1.41.tar.gz` & `tmp/xiaogpt-1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.41.tar", last modified: Wed Apr 19 13:22:54 2023, max compression
+gzip compressed data, was "xiaogpt-1.42.tar", last modified: Wed Apr 19 13:30:55 2023, max compression
```

## Comparing `xiaogpt-1.41.tar` & `xiaogpt-1.42.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-19 13:22:43.233904 xiaogpt-1.41/LICENSE
--rw-r--r--   0        0        0    11110 2023-04-19 13:22:43.233904 xiaogpt-1.41/README.md
--rw-r--r--   0        0        0      911 2023-04-19 13:22:54.113975 xiaogpt-1.41/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/__main__.py
--rw-r--r--   0        0        0      189 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      218 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     2895 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1386 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1732 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/cli.py
--rw-r--r--   0        0        0     5263 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/config.py
--rw-r--r--   0        0        0     1991 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/utils.py
--rw-r--r--   0        0        0    19359 2023-04-19 13:22:43.237905 xiaogpt-1.41/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11688 1970-01-01 00:00:00.000000 xiaogpt-1.41/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-19 13:30:41.945454 xiaogpt-1.42/LICENSE
+-rw-r--r--   0        0        0    11110 2023-04-19 13:30:41.945454 xiaogpt-1.42/README.md
+-rw-r--r--   0        0        0      919 2023-04-19 13:30:55.297498 xiaogpt-1.42/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      189 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     2895 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1386 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1732 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5263 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/config.py
+-rw-r--r--   0        0        0     1991 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/utils.py
+-rw-r--r--   0        0        0    19359 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.42/PKG-INFO
```

### Comparing `xiaogpt-1.41/LICENSE` & `xiaogpt-1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/README.md` & `xiaogpt-1.42/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/pyproject.toml` & `xiaogpt-1.42/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 requires-python = ">=3.7.1"
 dependencies = [
     "miservice_fork",
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
-    "EdgeGPT",
+    "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.41"
+version = "1.42"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.41/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.42/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.42/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.42/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/cli.py` & `xiaogpt-1.42/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/config.py` & `xiaogpt-1.42/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/utils.py` & `xiaogpt-1.42/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/xiaogpt/xiaogpt.py` & `xiaogpt-1.42/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.41/PKG-INFO` & `xiaogpt-1.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.41
+Version: 1.42
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
 Requires-Python: >=3.7.1
 Requires-Dist: miservice_fork
 Requires-Dist: openai
 Requires-Dist: aiohttp
 Requires-Dist: rich
 Requires-Dist: edge-tts>=6.1.3
-Requires-Dist: EdgeGPT
+Requires-Dist: EdgeGPT==0.1.26
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
```

