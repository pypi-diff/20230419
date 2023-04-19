# Comparing `tmp/compress_gpt-0.1.0.tar.gz` & `tmp/compress_gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compress_gpt-0.1.0.tar", max compression
+gzip compressed data, was "compress_gpt-0.1.1.tar", max compression
```

## Comparing `compress_gpt-0.1.0.tar` & `compress_gpt-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1044 2023-04-19 09:03:30.128324 compress_gpt-0.1.0/README.md
--rw-r--r--   0        0        0     1041 2023-04-18 05:20:31.785485 compress_gpt-0.1.0/compress_gpt/__init__.py
--rw-r--r--   0        0        0     9622 2023-04-19 02:25:37.251335 compress_gpt-0.1.0/compress_gpt/compress.py
--rw-r--r--   0        0        0      120 2023-04-19 02:10:33.981609 compress_gpt-0.1.0/compress_gpt/langchain/__init__.py
--rw-r--r--   0        0        0      942 2023-04-19 02:20:25.197490 compress_gpt-0.1.0/compress_gpt/langchain/prompt.py
--rw-r--r--   0        0        0     1380 2023-04-17 08:04:52.833264 compress_gpt-0.1.0/compress_gpt/prompts/__init__.py
--rw-r--r--   0        0        0     2003 2023-04-18 06:31:12.894939 compress_gpt-0.1.0/compress_gpt/prompts/compare_prompts.py
--rw-r--r--   0        0        0     2818 2023-04-17 09:01:59.044283 compress_gpt-0.1.0/compress_gpt/prompts/compress_chunks.py
--rw-r--r--   0        0        0     1260 2023-04-17 08:39:07.016128 compress_gpt-0.1.0/compress_gpt/prompts/decompress.py
--rw-r--r--   0        0        0     1482 2023-04-18 05:35:19.245911 compress_gpt-0.1.0/compress_gpt/prompts/diff_prompts.py
--rw-r--r--   0        0        0     1692 2023-04-18 06:38:00.014984 compress_gpt-0.1.0/compress_gpt/prompts/fix.py
--rw-r--r--   0        0        0     1019 2023-04-14 04:45:56.656456 compress_gpt-0.1.0/compress_gpt/prompts/fix_json.py
--rw-r--r--   0        0        0     2984 2023-04-18 05:39:07.544685 compress_gpt-0.1.0/compress_gpt/prompts/identify_format.py
--rw-r--r--   0        0        0     2958 2023-04-17 08:06:02.837919 compress_gpt-0.1.0/compress_gpt/prompts/identify_static.py
--rw-r--r--   0        0        0     2197 2023-04-18 06:54:20.875709 compress_gpt-0.1.0/compress_gpt/prompts/output_parser.py
--rw-r--r--   0        0        0        0 2023-04-07 00:13:56.095488 compress_gpt-0.1.0/compress_gpt/tests/__init__.py
--rw-r--r--   0        0        0    15483 2023-04-19 02:18:58.271768 compress_gpt-0.1.0/compress_gpt/tests/test_compress.py
--rw-r--r--   0        0        0     2049 2023-04-19 02:28:53.345393 compress_gpt-0.1.0/compress_gpt/utils.py
--rw-r--r--   0        0        0      699 2023-04-19 09:16:03.634756 compress_gpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 compress_gpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-04-19 18:06:12.449465 compress_gpt-0.1.1/README.md
+-rw-r--r--   0        0        0     1110 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/__init__.py
+-rw-r--r--   0        0        0     9622 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/compress.py
+-rw-r--r--   0        0        0      120 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/langchain/__init__.py
+-rw-r--r--   0        0        0      942 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/langchain/prompt.py
+-rw-r--r--   0        0        0     1380 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/compare_prompts.py
+-rw-r--r--   0        0        0     2818 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/compress_chunks.py
+-rw-r--r--   0        0        0     1260 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/decompress.py
+-rw-r--r--   0        0        0     1482 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/diff_prompts.py
+-rw-r--r--   0        0        0     1692 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/fix.py
+-rw-r--r--   0        0        0     1019 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/fix_json.py
+-rw-r--r--   0        0        0     2984 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/identify_format.py
+-rw-r--r--   0        0        0     2958 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/identify_static.py
+-rw-r--r--   0        0        0     2197 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/prompts/output_parser.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/tests/__init__.py
+-rw-r--r--   0        0        0    15483 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/tests/test_compress.py
+-rw-r--r--   0        0        0     2049 2023-04-19 18:06:12.477465 compress_gpt-0.1.1/compress_gpt/utils.py
+-rw-r--r--   0        0        0      699 2023-04-19 18:06:12.481465 compress_gpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 compress_gpt-0.1.1/PKG-INFO
```

### Comparing `compress_gpt-0.1.0/compress_gpt/__init__.py` & `compress_gpt-0.1.1/compress_gpt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 from datetime import timedelta
 from functools import partial
 from pathlib import Path
 
 import langchain
 import nest_asyncio
@@ -33,12 +34,16 @@
         cached,
         cache=Cache.MEMORY,
         serializer=PickleSerializer(),
         noself=True,
     )
 
 
-async def clear_cache():
+async def aclear_cache():
     await Cache(cache.keywords["cache"]).clear()
 
 
+def clear_cache():
+    asyncio.run(aclear_cache())
+
+
 from .compress import Compressor as Compressor
```

### Comparing `compress_gpt-0.1.0/compress_gpt/compress.py` & `compress_gpt-0.1.1/compress_gpt/compress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/langchain/prompt.py` & `compress_gpt-0.1.1/compress_gpt/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/__init__.py` & `compress_gpt-0.1.1/compress_gpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/compare_prompts.py` & `compress_gpt-0.1.1/compress_gpt/prompts/compare_prompts.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/compress_chunks.py` & `compress_gpt-0.1.1/compress_gpt/prompts/compress_chunks.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/decompress.py` & `compress_gpt-0.1.1/compress_gpt/prompts/decompress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/diff_prompts.py` & `compress_gpt-0.1.1/compress_gpt/prompts/diff_prompts.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/fix.py` & `compress_gpt-0.1.1/compress_gpt/prompts/fix.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/fix_json.py` & `compress_gpt-0.1.1/compress_gpt/prompts/fix_json.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/identify_format.py` & `compress_gpt-0.1.1/compress_gpt/prompts/identify_format.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/identify_static.py` & `compress_gpt-0.1.1/compress_gpt/prompts/identify_static.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/prompts/output_parser.py` & `compress_gpt-0.1.1/compress_gpt/prompts/output_parser.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/tests/test_compress.py` & `compress_gpt-0.1.1/compress_gpt/tests/test_compress.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/compress_gpt/utils.py` & `compress_gpt-0.1.1/compress_gpt/utils.py`

 * *Files identical despite different names*

### Comparing `compress_gpt-0.1.0/pyproject.toml` & `compress_gpt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compress-gpt"
-version = "0.1.0"
+version = "0.1.1"
 description = "Self-extracting GPT prompts for ~70% token savings."
 authors = ["Yasyf Mohamedali <yasyfm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "compress_gpt" }]
 
 [tool.poetry.dependencies]
```

### Comparing `compress_gpt-0.1.0/PKG-INFO` & `compress_gpt-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compress-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Self-extracting GPT prompts for ~70% token savings.
 License: MIT
 Author: Yasyf Mohamedali
 Author-email: yasyfm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -44,14 +44,22 @@
 +from compress_gpt.langchain import CompressPrompt as PromptTemplate
 ```
 
 For very simple prompts, use `CompressSimplePrompt` and `CompressSimpleTemplate` instead.
 
 If compression ever fails or results in extra tokens, the original prompt will be used. Each compression result is aggressively cached, but the first run can take a hot sec.
 
+#### Clearing the cache
+
+```python
+import compress_gpt
+
+compress_gpt.clear_cache()
+```
+
 ### Demo
 
 [![asciicast](https://asciinema.org/a/578285.svg)](https://asciinema.org/a/578285)
 
 
 ### How CompressGPT Works
```

