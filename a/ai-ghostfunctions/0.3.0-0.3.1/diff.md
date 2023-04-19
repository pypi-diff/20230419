# Comparing `tmp/ai_ghostfunctions-0.3.0.tar.gz` & `tmp/ai_ghostfunctions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_ghostfunctions-0.3.0.tar", max compression
+gzip compressed data, was "ai_ghostfunctions-0.3.1.tar", max compression
```

## Comparing `ai_ghostfunctions-0.3.0.tar` & `ai_ghostfunctions-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/LICENSE
--rw-r--r--   0        0        0     4451 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/README.md
--rw-r--r--   0        0        0     1828 2023-04-05 02:12:57.432142 ai_ghostfunctions-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/__init__.py
--rw-r--r--   0        0        0     6078 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/ghostfunctions.py
--rw-r--r--   0        0        0      231 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/keywords.py
--rw-r--r--   0        0        0        0 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/py.typed
--rw-r--r--   0        0        0      343 2023-04-05 02:12:44.679898 ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/types.py
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-19 20:58:17.657236 ai_ghostfunctions-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4451 2023-04-19 20:58:17.657236 ai_ghostfunctions-0.3.1/README.md
+-rw-r--r--   0        0        0     1828 2023-04-19 20:58:31.241477 ai_ghostfunctions-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/__init__.py
+-rw-r--r--   0        0        0     6266 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/ghostfunctions.py
+-rw-r--r--   0        0        0      231 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/keywords.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/py.typed
+-rw-r--r--   0        0        0      343 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/types.py
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.3.1/PKG-INFO
```

### Comparing `ai_ghostfunctions-0.3.0/LICENSE` & `ai_ghostfunctions-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.3.0/README.md` & `ai_ghostfunctions-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.3.0/pyproject.toml` & `ai_ghostfunctions-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-ghostfunctions"
-version = "0.3.0"
+version = "0.3.1"
 description = "AI Ghostfunctions"
 authors = ["Brian M. Ritz <brianmritz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bmritz/ai-ghostfunctions"
 repository = "https://github.com/bmritz/ai-ghostfunctions"
 documentation = "https://ai-ghostfunctions.readthedocs.io"
```

### Comparing `ai_ghostfunctions-0.3.0/src/ai_ghostfunctions/ghostfunctions.py` & `ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/ghostfunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,26 @@
 from .types import Message
 
 
 def _make_chatgpt_message_from_function(
     f: Callable[..., Any], **kwargs: Any
 ) -> Message:
     sig = inspect.signature(f)
+    if not f.__doc__:
+        raise ValueError("The function must have a docstring.")
     prompt = (
-        f"from mymodule import {f.__name__}\n"
-        f"""
+        (
+            f"from mymodule import {f.__name__}\n"
+            f"""
 # The return type annotation for the function {f.__name__} is {get_type_hints(f)['return']}
 # The docstring for the function {f.__name__} is the following:
-# {f.__doc__}
+"""
+        )
+        + "\n".join([f"# {line}" for line in f.__doc__.split("\n")])
+        + f"""
 result = {f.__name__}({",".join(f"{k}={kwargs[k].__repr__()}" for k in sig.parameters)})
 print(result)
 """
     )
     return Message(role=USER, content=prompt)
```

### Comparing `ai_ghostfunctions-0.3.0/PKG-INFO` & `ai_ghostfunctions-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-ghostfunctions
-Version: 0.3.0
+Version: 0.3.1
 Summary: AI Ghostfunctions
 Home-page: https://github.com/bmritz/ai-ghostfunctions
 License: MIT
 Author: Brian M. Ritz
 Author-email: brianmritz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

