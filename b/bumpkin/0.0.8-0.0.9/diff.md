# Comparing `tmp/bumpkin-0.0.8.tar.gz` & `tmp/bumpkin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpkin-0.0.8.tar", last modified: Mon Mar  6 18:47:33 2023, max compression
+gzip compressed data, was "bumpkin-0.0.9.tar", last modified: Tue Mar  7 14:37:54 2023, max compression
```

## Comparing `bumpkin-0.0.8.tar` & `bumpkin-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.124004 bumpkin-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-06 18:47:20.000000 bumpkin-0.0.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-06 18:47:20.000000 bumpkin-0.0.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-06 18:47:20.000000 bumpkin-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-06 18:47:20.000000 bumpkin-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-06 18:47:33.124004 bumpkin-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-06 18:47:20.000000 bumpkin-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.120004 bumpkin-0.0.8/bumpkin/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.120004 bumpkin-0.0.8/bumpkin/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.120004 bumpkin-0.0.8/bumpkin/sources/basicgithub/
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basicgithub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basicgithub/default.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.120004 bumpkin-0.0.8/bumpkin/sources/basichttp/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basichttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basichttp/default.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.124004 bumpkin-0.0.8/bumpkin/sources/basichttpjsonvendor/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basichttpjsonvendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/basichttpjsonvendor/default.nix
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-06 18:47:20.000000 bumpkin-0.0.8/bumpkin/sources/default.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.120004 bumpkin-0.0.8/bumpkin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-06 18:47:33.000000 bumpkin-0.0.8/bumpkin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 18:47:33.124004 bumpkin-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-06 18:47:20.000000 bumpkin-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:33.124004 bumpkin-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 18:47:20.000000 bumpkin-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-06 18:47:20.000000 bumpkin-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-06 18:47:20.000000 bumpkin-0.0.8/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.136017 bumpkin-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-07 14:37:45.000000 bumpkin-0.0.9/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-07 14:37:45.000000 bumpkin-0.0.9/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-07 14:37:45.000000 bumpkin-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-07 14:37:45.000000 bumpkin-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-07 14:37:54.136017 bumpkin-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-07 14:37:45.000000 bumpkin-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.132017 bumpkin-0.0.9/bumpkin/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.132017 bumpkin-0.0.9/bumpkin/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.132017 bumpkin-0.0.9/bumpkin/sources/basicgithub/
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basicgithub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basicgithub/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.136017 bumpkin-0.0.9/bumpkin/sources/basichttp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basichttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basichttp/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.136017 bumpkin-0.0.9/bumpkin/sources/basichttpjsonvendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basichttpjsonvendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/basichttpjsonvendor/default.nix
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-07 14:37:45.000000 bumpkin-0.0.9/bumpkin/sources/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.132017 bumpkin-0.0.9/bumpkin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-07 14:37:54.000000 bumpkin-0.0.9/bumpkin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 14:37:54.136017 bumpkin-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-07 14:37:45.000000 bumpkin-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:54.136017 bumpkin-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:45.000000 bumpkin-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-07 14:37:45.000000 bumpkin-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-07 14:37:45.000000 bumpkin-0.0.9/tests/test_base.py
```

### Comparing `bumpkin-0.0.8/HISTORY.md` & `bumpkin-0.0.9/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Eval_nodes: ignore missing keys. [lucasew]
+- Option to not generate minified json. [lucasew]
+- Lintwork. [lucasew]
+- Selective bump, bump older items first. [lucasew]
+- Command to list nodes in a json. [lucasew]
+
+
+0.0.8 (2023-03-06)
+------------------
+- Release: version 0.0.8 🚀 [lucasew]
 - Save old state if assertion error when evaluating node. [lucasew]
 
 
 0.0.7 (2023-03-06)
 ------------------
 - Release: version 0.0.7 🚀 [lucasew]
 - Resilience work. [lucasew]
```

### Comparing `bumpkin-0.0.8/LICENSE` & `bumpkin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/PKG-INFO` & `bumpkin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpkin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to do source bumps
 Home-page: https://github.com/lucasew/bumpkin/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `bumpkin-0.0.8/README.md` & `bumpkin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/bumpkin/cli.py` & `bumpkin-0.0.9/bumpkin/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,27 +30,77 @@
     subparser.add_argument("-v,--verbose", dest="verbose", action="store_true")
     subparser.add_argument(
         "-i,--input", dest="input_file", type=Path, required=True
     )
     subparser.add_argument(
         "-o,--output", dest="output_file", type=Path, required=True
     )
+    subparser.add_argument(
+        "-p,--pretty",
+        dest="indent",
+        help="Enable JSON identations instead of minified",
+        action="store_true",
+    )
+    subparser.add_argument(
+        dest="keys",
+        nargs="*",
+        type=str,
+        help="Bump only these keys. If ommited, bump all.",
+    )
 
-    def handle(input_file, output_file, **kwargs):
+    def handle(input_file, output_file, keys, indent, **kwargs):
         from json import dumps, loads
 
         from .sources import eval_nodes
 
         assert input_file.exists(), f"'{input_file.resolve()}' does not exist"
         input_file_data = loads(input_file.read_text())
         output_file_data = None
         if output_file.exists():
             output_file_data = loads(output_file.read_text())
-        processed = eval_nodes(input_file_data, output_file_data)
-        output_file.write_text(dumps(processed))
+        processed = eval_nodes(input_file_data, output_file_data, keys)
+        output_file.write_text(dumps(processed, indent=4 if indent else None))
+
+    subparser.set_defaults(fn=handle)
+    # todo implement
+
+
+def list_subcommand(subparser):
+    from pathlib import Path
+
+    subparser.description = "List bumpable nodes in JSON"
+    subparser.add_argument("-v,--verbose", dest="verbose", action="store_true")
+    subparser.add_argument(
+        "-i,--input", dest="input_file", type=Path, required=True
+    )
+    subparser.add_argument(
+        "-o,--output", dest="output_file", type=Path, required=True
+    )
+    subparser.add_argument(
+        "-s,--show-state", dest="show_state", action="store_true"
+    )
+
+    def handle(input_file, output_file, show_state=False, **kwargs):
+        from json import loads
+
+        from .sources import list_nodes
+
+        assert input_file.exists(), f"'{input_file.resolve()}' does not exist"
+        input_file_data = loads(input_file.read_text())
+        output_file_data = None
+        if output_file.exists():
+            output_file_data = loads(output_file.read_text())
+        nodes = list_nodes(input_file_data, output_file_data)
+        node_keys = list(nodes.keys())
+        node_keys.sort()
+        for node in node_keys:
+            if show_state:
+                print(node, nodes[node])
+            else:
+                print(node)
 
     subparser.set_defaults(fn=handle)
     # todo implement
 
 
 def main():  # pragma: no cover
     """
@@ -71,18 +121,21 @@
     from argparse import ArgumentParser
     from sys import argv
 
     parser = ArgumentParser()
     subparsers = parser.add_subparsers()
     demo_subcommand(subparsers.add_parser("demo"))
     eval_subcommand(subparsers.add_parser("eval"))
+    list_subcommand(subparsers.add_parser("list"))
     args = vars(parser.parse_args())
 
     if args.get("verbose"):
         logger.root.setLevel(logging.DEBUG)
     else:
         logger.root.setLevel(logging.INFO)
 
+    logger.debug(f"args: {args}")
+
     if args.get("fn"):
         args["fn"](**args.copy())
     else:
         parser.parse_args([*argv[1:], "--help"])
```

### Comparing `bumpkin-0.0.8/bumpkin/sources/basicgithub/__init__.py` & `bumpkin-0.0.9/bumpkin/sources/basicgithub/__init__.py`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/bumpkin/sources/basichttp/__init__.py` & `bumpkin-0.0.9/bumpkin/sources/basichttp/__init__.py`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/bumpkin/sources/basichttpjsonvendor/__init__.py` & `bumpkin-0.0.9/bumpkin/sources/basichttpjsonvendor/__init__.py`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/bumpkin/sources/default.nix` & `bumpkin-0.0.9/bumpkin/sources/default.nix`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/bumpkin.egg-info/PKG-INFO` & `bumpkin-0.0.9/bumpkin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpkin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to do source bumps
 Home-page: https://github.com/lucasew/bumpkin/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `bumpkin-0.0.8/bumpkin.egg-info/SOURCES.txt` & `bumpkin-0.0.9/bumpkin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bumpkin-0.0.8/setup.py` & `bumpkin-0.0.9/setup.py`

 * *Files identical despite different names*

