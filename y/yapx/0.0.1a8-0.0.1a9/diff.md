# Comparing `tmp/yapx-0.0.1a8.tar.gz` & `tmp/yapx-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.0.1a8.tar", last modified: Mon Jan  2 22:49:14 2023, max compression
+gzip compressed data, was "yapx-0.0.1a9.tar", last modified: Wed Jan 18 19:05:20 2023, max compression
```

## Comparing `yapx-0.0.1a8.tar` & `yapx-0.0.1a9.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 22:49:14.683781 yapx-0.0.1a8/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-01-02 22:46:13.000000 yapx-0.0.1a8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-02 22:46:13.000000 yapx-0.0.1a8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2125 2023-01-02 22:49:14.683781 yapx-0.0.1a8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-01-02 22:46:13.000000 yapx-0.0.1a8/README.md
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 22:46:13.000000 yapx-0.0.1a8/VERSION
--rw-r--r--   0 root         (0) root         (0)     2674 2023-01-02 22:49:14.683781 yapx-0.0.1a8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-02 22:46:13.000000 yapx-0.0.1a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 22:49:14.679781 yapx-0.0.1a8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 22:49:14.683781 yapx-0.0.1a8/src/yapx/
--rw-r--r--   0 root         (0) root         (0)      392 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-01-02 22:49:08.000000 yapx-0.0.1a8/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4493 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     6881 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/argparse_action.py
--rw-r--r--   0 root         (0) root         (0)    27354 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)      598 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-01-02 22:46:13.000000 yapx-0.0.1a8/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 22:49:14.683781 yapx-0.0.1a8/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2125 2023-01-02 22:49:14.000000 yapx-0.0.1a8/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      429 2023-01-02 22:49:14.000000 yapx-0.0.1a8/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 22:49:14.000000 yapx-0.0.1a8/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      549 2023-01-02 22:49:14.000000 yapx-0.0.1a8/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-02 22:49:14.000000 yapx-0.0.1a8/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-01-18 19:01:42.000000 yapx-0.0.1a9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-01-18 19:01:42.000000 yapx-0.0.1a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-01-18 19:05:20.040428 yapx-0.0.1a9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-01-18 19:01:42.000000 yapx-0.0.1a9/README.md
+-rw-r--r--   0 root         (0) root         (0)        8 2023-01-18 19:01:42.000000 yapx-0.0.1a9/VERSION
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-01-18 19:05:20.040428 yapx-0.0.1a9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 19:01:42.000000 yapx-0.0.1a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.036428 yapx-0.0.1a9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      468 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      150 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5514 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/argparse_action.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    17589 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      126 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-01-18 19:02:49.000000 yapx-0.0.1a9/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       24 2023-01-18 19:05:13.000000 yapx-0.0.1a9/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4493 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     6969 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/argparse_action.py
+-rw-r--r--   0 root         (0) root         (0)    27459 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)      598 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-01-18 19:01:42.000000 yapx-0.0.1a9/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 19:05:20.040428 yapx-0.0.1a9/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      559 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-01-18 19:05:20.000000 yapx-0.0.1a9/src/yapx.egg-info/top_level.txt
```

### Comparing `yapx-0.0.1a8/LICENSE` & `yapx-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/PKG-INFO` & `yapx-0.0.1a9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.0.1a8
+Version: 0.0.1a9
+Summary: WIP
 Home-page: https://codeberg.org/Fresh2dev/yapx
 Author: donald
 Author-email: hello@Fresh2.dev
 Project-URL: Repository, https://codeberg.org/Fresh2dev/yapx
 Project-URL: License, https://www.Fresh2.dev/code/r/yapx/i/license
 Project-URL: Documentation, https://www.Fresh2.dev/code/r/yapx/i
 Project-URL: Issues, https://codeberg.org/Fresh2dev/yapx/issues
```

### Comparing `yapx-0.0.1a8/README.md` & `yapx-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/setup.cfg` & `yapx-0.0.1a9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [metadata]
 name = yapx
 version = file: VERSION
+description = WIP
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = donald
 author_email = hello@Fresh2.dev
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
@@ -22,23 +23,23 @@
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	typing-extensions; python_version<'3.10'
 
 [options.package_data]
-* = *
+* = **
 
 [options.extras_require]
 build = 
+	setuptools>=62.3.0
 	build
-	setuptools
 	twine
 	wheel
-	myke[io]==0.0.1a9
+	myke[io]==0.0.1a11
 docs = 
 	mkdocs==1.*
 	mkdocstrings[python]==0.19.0
 	mkdocs-autorefs
 dev = 
 	black
 	flake8
@@ -52,15 +53,15 @@
 	isort
 	mypy[reports]
 	pydantic==1.*,>=1.10.2
 	pylint
 	pylint-pytest
 	rope
 	tox
-	myke[io]==0.0.1a9
+	myke[io]==0.0.1a11
 tests = 
 	pytest==7.*
 	pytest-cov
 	pytest-html
 	pytest-sugar
 	hypothesis==6.*
 	packaging
```

### Comparing `yapx-0.0.1a8/src/yapx/actions.py` & `yapx-0.0.1a9/src/yapx/actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/src/yapx/arg.py` & `yapx-0.0.1a9/src/yapx/arg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from argparse import Action
 from contextlib import suppress
 from dataclasses import MISSING, Field, dataclass, field, make_dataclass
 from inspect import _empty, signature
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
 
+from typing_extensions import Literal  # noqa: keep this so eval of `Literal` works...
+
 from .types import Dataclass
 
 __all__ = ["arg"]
 
 
 try:
     from typing import get_type_hints
```

### Comparing `yapx-0.0.1a8/src/yapx/argparse_action.py` & `yapx-0.0.1a9/src/yapx/argparse_action.py`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/src/yapx/argument_parser.py` & `yapx-0.0.1a9/src/yapx/argument_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,15 +589,15 @@
             )
             if subparsers:
                 for choice, subparser in subparsers.choices.items():
                     print(separator)
                     print(f">>> {choice}")
                     print(subparser.format_help())
 
-    def print_help_all(self) -> None:
+    def print_help_full(self) -> None:
         self._print_help(parser=self, include_all=True)
 
     @staticmethod
     def _docstring_to_description(
         parser: argparse.ArgumentParser,
         args_model: Union[Callable[..., Any], Type[Dataclass]],
     ) -> None:
@@ -680,21 +680,21 @@
         parser._register_funcs(
             *cmd_funcs,
             subparser_kwargs=parser_shared_kwargs,
             use_docstr_description=_use_docstr_description,
             **kwargs,
         )
 
-        if _print_help:
-            parser.print_help_all()
-            parser.exit()
-
         if not _args:
             _args = sys.argv[1:]
 
+        if _print_help or "--help-full" in _args:
+            parser.print_help_full()
+            parser.exit()
+
         parsed_args: Dict[str, Any] = vars(parser.parse_args(_args))
 
         # parsed_args.get(cls.COMMAND_ATTRIBUTE_NAME)
 
         func: Optional[Callable[..., Any]] = parsed_args.get(cls.FUNC_ATTRIBUTE_NAME)
         args_model: Optional[Type[Any]] = parsed_args.get(cls.ARGS_ATTRIBUTE_NAME)
         func_result: Any = None
@@ -709,27 +709,28 @@
 
         if is_instance(setup_result, GeneratorType):
             with suppress(StopIteration):
                 func_result = next(setup_result)
         else:
             func_result = setup_result
 
-        if func:
-            func_result = cls._run_func(
-                parser=parser,
-                func=func,
-                args_model=args_model,
-                args=_args,
-                use_pydantic=_use_pydantic,
-            )
-
-        if is_instance(setup_result, GeneratorType):
-            for gen_result in setup_result:
-                if not func:
-                    func_result = gen_result
+        try:
+            if func:
+                func_result = cls._run_func(
+                    parser=parser,
+                    func=func,
+                    args_model=args_model,
+                    args=_args,
+                    use_pydantic=_use_pydantic,
+                )
+        finally:
+            if is_instance(setup_result, GeneratorType):
+                for gen_result in setup_result:
+                    if not func:
+                        func_result = gen_result
 
         return func_result
 
 
 def run(
     *args: Optional[Callable[..., Any]],
     _args: Optional[List[str]] = None,
```

### Comparing `yapx-0.0.1a8/src/yapx/types.py` & `yapx-0.0.1a9/src/yapx/types.py`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/src/yapx/utils.py` & `yapx-0.0.1a9/src/yapx/utils.py`

 * *Files identical despite different names*

### Comparing `yapx-0.0.1a8/src/yapx.egg-info/PKG-INFO` & `yapx-0.0.1a9/src/yapx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.0.1a8
+Version: 0.0.1a9
+Summary: WIP
 Home-page: https://codeberg.org/Fresh2dev/yapx
 Author: donald
 Author-email: hello@Fresh2.dev
 Project-URL: Repository, https://codeberg.org/Fresh2dev/yapx
 Project-URL: License, https://www.Fresh2.dev/code/r/yapx/i/license
 Project-URL: Documentation, https://www.Fresh2.dev/code/r/yapx/i
 Project-URL: Issues, https://codeberg.org/Fresh2dev/yapx/issues
```

### Comparing `yapx-0.0.1a8/src/yapx.egg-info/requires.txt` & `yapx-0.0.1a9/src/yapx.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 [:python_version < "3.10"]
 typing-extensions
 
 [build]
+setuptools>=62.3.0
 build
-setuptools
 twine
 wheel
-myke[io]==0.0.1a9
+myke[io]==0.0.1a11
 
 [dev]
 black
 flake8
 flake8-bugbear
 flake8-comprehensions
 flake8-pytest-style
@@ -22,15 +22,15 @@
 isort
 mypy[reports]
 pydantic==1.*,>=1.10.2
 pylint
 pylint-pytest
 rope
 tox
-myke[io]==0.0.1a9
+myke[io]==0.0.1a11
 
 [docs]
 mkdocs==1.*
 mkdocstrings[python]==0.19.0
 mkdocs-autorefs
 
 [pydantic]
```

