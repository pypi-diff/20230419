# Comparing `tmp/ts2python-0.6.6.tar.gz` & `tmp/ts2python-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts2python-0.6.6.tar", max compression
+gzip compressed data, was "ts2python-0.6.8.tar", max compression
```

## Comparing `ts2python-0.6.6.tar` & `ts2python-0.6.8.tar`

### file list

```diff
@@ -1,46 +1,54 @@
--rw-r--r--   0        0        0    11357 2021-09-18 19:34:24.274869 ts2python-0.6.6/LICENSE
--rw-r--r--   0        0        0     7823 2022-10-03 17:32:01.622331 ts2python-0.6.6/README.md
--rw-r--r--   0        0        0     1288 2021-11-29 20:19:15.625394 ts2python-0.6.6/demo/README_example.py
--rwxr-xr-x   0        0        0      356 2022-10-03 17:32:01.622331 ts2python-0.6.6/demo/demo.bat
--rwxr-xr-x   0        0        0      447 2022-10-03 17:32:01.622331 ts2python-0.6.6/demo/demo.sh
--rwxr-xr-x   0        0        0     1788 2022-10-03 17:32:01.622331 ts2python-0.6.6/demo/extract_ts_from_lsp_specs.py
--rw-r--r--   0        0        0    50592 2023-01-30 21:12:53.180397 ts2python-0.6.6/demo/specification-3-16.py
--rw-r--r--   0        0        0   130174 2023-01-30 21:12:52.760391 ts2python-0.6.6/demo/specification-3-16.ts
--rw-r--r--   0        0        0    48948 2022-02-08 15:58:20.072649 ts2python-0.6.6/demo/specification-current.py
--rw-r--r--   0        0        0   130175 2022-02-08 15:58:19.782648 ts2python-0.6.6/demo/specification-current.ts
--rwxr-xr-x   0        0        0      237 2022-10-03 17:32:01.622331 ts2python-0.6.6/demo/test.sh
--rw-r--r--   0        0        0     2919 2021-12-03 00:17:17.386684 ts2python-0.6.6/docs/BasicUsage.rst
--rw-r--r--   0        0        0      634 2021-10-08 06:32:17.377642 ts2python-0.6.6/docs/Makefile
--rw-r--r--   0        0        0    11469 2022-02-09 18:24:03.026270 ts2python-0.6.6/docs/Mapping.rst
--rw-r--r--   0        0        0     5069 2022-02-08 21:17:18.798784 ts2python-0.6.6/docs/Validation.rst
--rw-r--r--   0        0        0     1928 2021-10-08 06:32:17.370975 ts2python-0.6.6/docs/conf.py
--rw-r--r--   0        0        0     3713 2022-02-19 06:40:31.782335 ts2python-0.6.6/docs/index.rst
--rw-r--r--   0        0        0      800 2021-10-08 06:32:17.377642 ts2python-0.6.6/docs/make.bat
--rw-r--r--   0        0        0     1733 2023-01-30 21:14:56.872300 ts2python-0.6.6/pyproject.toml
--rwxr-xr-x   0        0        0      501 2022-02-08 15:57:19.925635 ts2python-0.6.6/tests/run.sh
--rwxr-xr-x   0        0        0     7369 2022-02-08 15:53:14.564099 ts2python-0.6.6/tests/runner.py
--rwxr-xr-x   0        0        0     1713 2023-01-30 21:14:56.872300 ts2python-0.6.6/tests/test_singledispatch_shim.py
--rwxr-xr-x   0        0        0    12020 2022-10-03 17:32:01.625665 ts2python-0.6.6/tests/test_ts2python.py
--rwxr-xr-x   0        0        0   108600 2022-10-03 17:32:01.625665 ts2python-0.6.6/tests/typing_extensions.py
--rw-r--r--   0        0        0      161 2021-11-30 22:02:27.196833 ts2python-0.6.6/tests_grammar/01_test_Entities.ini
--rw-r--r--   0        0        0      122 2021-11-30 22:02:27.196833 ts2python-0.6.6/tests_grammar/02_test_Keywords.ini
--rw-r--r--   0        0        0      711 2021-11-30 22:02:27.196833 ts2python-0.6.6/tests_grammar/03_test_literals.ini
--rw-r--r--   0        0        0      608 2022-02-19 06:40:31.782335 ts2python-0.6.6/tests_grammar/04_test_Consts.ini
--rw-r--r--   0        0        0      704 2022-02-09 18:24:03.029594 ts2python-0.6.6/tests_grammar/05_test_Enums.ini
--rw-r--r--   0        0        0     2992 2022-03-30 16:21:12.016755 ts2python-0.6.6/tests_grammar/06_test_Namespaces.ini
--rw-r--r--   0        0        0     1667 2022-02-19 06:40:31.782335 ts2python-0.6.6/tests_grammar/07_test_Types.ini
--rw-r--r--   0        0        0     8266 2022-05-23 06:57:15.853747 ts2python-0.6.6/tests_grammar/08_test_Interfaces.ini
--rw-r--r--   0        0        0     4000 2022-02-19 06:40:31.782335 ts2python-0.6.6/tests_grammar/09_test_Typescript_Document.ini
--rw-r--r--   0        0        0        0 2022-10-03 17:32:01.625665 ts2python-0.6.6/tests_grammar/10_test_overloaded_methods.ini
--rw-r--r--   0        0        0     2634 2022-03-03 10:39:50.422999 ts2python-0.6.6/tests_grammar/99_test_Playground.ini
--rw-r--r--   0        0        0        0 2021-11-29 21:52:57.935510 ts2python-0.6.6/tests_grammar/package.py
--rw-r--r--   0        0        0     1175 2021-09-18 19:34:24.274869 ts2python-0.6.6/ts2python/__init__.py
--rw-r--r--   0        0        0    14803 2023-01-30 21:14:56.872300 ts2python-0.6.6/ts2python/json_validation.py
--rw-r--r--   0        0        0     8230 2023-01-30 21:14:56.872300 ts2python-0.6.6/ts2python/singledispatch_shim.py
--rw-r--r--   0        0        0      378 2021-11-30 22:02:27.196833 ts2python-0.6.6/ts2python/ts2pythonParser.ini
--rw-r--r--   0        0        0    11327 2023-01-30 21:14:56.872300 ts2python-0.6.6/ts2python/typeddict_shim.py
--rw-r--r--   0        0        0    12069 2022-10-08 21:13:56.400857 ts2python-0.6.6/ts2python/typeddict_shim2.py
--rw-r--r--   0        0        0   108600 2021-11-30 22:02:27.196833 ts2python-0.6.6/ts2python/typing_extensions.py
--rwxr-xr-x   0        0        0    60959 2023-01-30 21:17:24.324599 ts2python-0.6.6/ts2pythonParser.py
--rw-r--r--   0        0        0     8956 1970-01-01 00:00:00.000000 ts2python-0.6.6/setup.py
--rw-r--r--   0        0        0     9441 1970-01-01 00:00:00.000000 ts2python-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-09-18 19:34:24.274869 ts2python-0.6.8/LICENSE
+-rw-r--r--   0        0        0     8018 2023-04-19 20:06:43.510779 ts2python-0.6.8/README.md
+-rwxr-xr-x   0        0        0     1288 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/README_example.py
+-rw-r--r--   0        0        0      351 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/demo-3-16.bat
+-rwxr-xr-x   0        0        0      447 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/demo-3-16.sh
+-rwxr-xr-x   0        0        0      350 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/demo.bat
+-rwxr-xr-x   0        0        0      431 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/demo.sh
+-rwxr-xr-x   0        0        0     2716 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/extract_ts_from_lsp_specs.py
+-rw-r--r--   0        0        0    50592 2023-01-30 21:12:53.180397 ts2python-0.6.8/demo/specification-3-16.py
+-rw-r--r--   0        0        0   130174 2023-01-30 21:12:52.760391 ts2python-0.6.8/demo/specification-3-16.ts
+-rw-r--r--   0        0        0    65964 2023-03-24 12:03:19.986072 ts2python-0.6.8/demo/specification-3.17.py
+-rw-r--r--   0        0        0   178050 2023-03-24 11:40:19.639613 ts2python-0.6.8/demo/specification-3.17.ts
+-rw-r--r--   0        0        0    48948 2022-02-08 15:58:20.072649 ts2python-0.6.8/demo/specification-current.py
+-rw-r--r--   0        0        0   130175 2022-02-08 15:58:19.782648 ts2python-0.6.8/demo/specification-current.ts
+-rw-r--r--   0        0        0    27339 2023-03-24 12:18:08.693378 ts2python-0.6.8/demo/specification.js
+-rw-r--r--   0        0        0    65964 2023-03-24 12:17:28.126236 ts2python-0.6.8/demo/specification.py
+-rw-r--r--   0        0        0   178133 2023-03-24 12:19:38.577762 ts2python-0.6.8/demo/specification.ts
+-rwxr-xr-x   0        0        0      237 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/test-3-16.sh
+-rwxr-xr-x   0        0        0      202 2023-04-19 20:06:43.510779 ts2python-0.6.8/demo/test.sh
+-rw-r--r--   0        0        0     2919 2021-12-03 00:17:17.386684 ts2python-0.6.8/docs/BasicUsage.rst
+-rw-r--r--   0        0        0      634 2021-10-08 06:32:17.377642 ts2python-0.6.8/docs/Makefile
+-rw-r--r--   0        0        0    11469 2022-02-09 18:24:03.026270 ts2python-0.6.8/docs/Mapping.rst
+-rw-r--r--   0        0        0     5069 2022-02-08 21:17:18.798784 ts2python-0.6.8/docs/Validation.rst
+-rw-r--r--   0        0        0     1928 2021-10-08 06:32:17.370975 ts2python-0.6.8/docs/conf.py
+-rw-r--r--   0        0        0     3713 2022-02-19 06:40:31.782335 ts2python-0.6.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2021-10-08 06:32:17.377642 ts2python-0.6.8/docs/make.bat
+-rw-r--r--   0        0        0     1733 2023-04-19 20:06:43.510779 ts2python-0.6.8/pyproject.toml
+-rwxr-xr-x   0        0        0      501 2022-02-08 15:57:19.925635 ts2python-0.6.8/tests/run.sh
+-rwxr-xr-x   0        0        0     7369 2022-02-08 15:53:14.564099 ts2python-0.6.8/tests/runner.py
+-rwxr-xr-x   0        0        0     1713 2023-01-30 21:14:56.872300 ts2python-0.6.8/tests/test_singledispatch_shim.py
+-rwxr-xr-x   0        0        0    12017 2023-04-19 20:06:43.510779 ts2python-0.6.8/tests/test_ts2python.py
+-rwxr-xr-x   0        0        0   108600 2022-10-03 17:32:01.625665 ts2python-0.6.8/tests/typing_extensions.py
+-rw-r--r--   0        0        0      161 2021-11-30 22:02:27.196833 ts2python-0.6.8/tests_grammar/01_test_Entities.ini
+-rw-r--r--   0        0        0      122 2021-11-30 22:02:27.196833 ts2python-0.6.8/tests_grammar/02_test_Keywords.ini
+-rw-r--r--   0        0        0      711 2021-11-30 22:02:27.196833 ts2python-0.6.8/tests_grammar/03_test_literals.ini
+-rw-r--r--   0        0        0      608 2022-02-19 06:40:31.782335 ts2python-0.6.8/tests_grammar/04_test_Consts.ini
+-rw-r--r--   0        0        0      704 2022-02-09 18:24:03.029594 ts2python-0.6.8/tests_grammar/05_test_Enums.ini
+-rw-r--r--   0        0        0     2992 2022-03-30 16:21:12.016755 ts2python-0.6.8/tests_grammar/06_test_Namespaces.ini
+-rw-r--r--   0        0        0     1667 2022-02-19 06:40:31.782335 ts2python-0.6.8/tests_grammar/07_test_Types.ini
+-rw-r--r--   0        0        0     8680 2023-04-19 20:06:43.510779 ts2python-0.6.8/tests_grammar/08_test_Interfaces.ini
+-rw-r--r--   0        0        0     4000 2022-02-19 06:40:31.782335 ts2python-0.6.8/tests_grammar/09_test_Typescript_Document.ini
+-rw-r--r--   0        0        0        0 2022-10-03 17:32:01.625665 ts2python-0.6.8/tests_grammar/10_test_overloaded_methods.ini
+-rw-r--r--   0        0        0     2634 2022-03-03 10:39:50.422999 ts2python-0.6.8/tests_grammar/99_test_Playground.ini
+-rw-r--r--   0        0        0        0 2021-11-29 21:52:57.935510 ts2python-0.6.8/tests_grammar/package.py
+-rw-r--r--   0        0        0     1175 2021-09-18 19:34:24.274869 ts2python-0.6.8/ts2python/__init__.py
+-rw-r--r--   0        0        0    14849 2023-04-19 20:06:43.510779 ts2python-0.6.8/ts2python/json_validation.py
+-rw-r--r--   0        0        0     8230 2023-01-30 21:14:56.872300 ts2python-0.6.8/ts2python/singledispatch_shim.py
+-rw-r--r--   0        0        0      378 2021-11-30 22:02:27.196833 ts2python-0.6.8/ts2python/ts2pythonParser.ini
+-rw-r--r--   0        0        0    11647 2023-04-19 20:06:43.510779 ts2python-0.6.8/ts2python/typeddict_shim.py
+-rw-r--r--   0        0        0    12069 2022-10-08 21:13:56.400857 ts2python-0.6.8/ts2python/typeddict_shim2.py
+-rw-r--r--   0        0        0    88509 2023-04-19 20:06:43.510779 ts2python-0.6.8/ts2python/typing_extensions.py
+-rw-r--r--   0        0        0   108600 2023-04-19 20:06:43.510779 ts2python-0.6.8/ts2python/typing_extensions.py_ALT
+-rwxr-xr-x   0        0        0    60727 2023-04-19 20:06:43.510779 ts2python-0.6.8/ts2pythonParser.py
+-rw-r--r--   0        0        0     9636 1970-01-01 00:00:00.000000 ts2python-0.6.8/PKG-INFO
```

### Comparing `ts2python-0.6.6/LICENSE` & `ts2python-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/README.md` & `ts2python-0.6.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 TypedDicts, plus support for run-time type-checking 
 of JSON-data.
 
 ## License and Source Code
 
 ts2python is open source software under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)
 
-Copyright 2021 Eckhart Arnold <arnold@badw.de>, Bavarian Academy of Sciences and Humanities
+Copyright 2021-2023 Eckhart Arnold <arnold@badw.de>, Bavarian Academy of Sciences and Humanities
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
@@ -193,13 +193,17 @@
     $ python runner.py
 
 It is also possible to run the tests with [pytest](https://docs.pytest.org/) 
 or [nose](https://nose.readthedocs.io), in case you have
 either of theses testing-frameworks installed.
 
 For a demonstration how the TypeScript-Interfaces are transpiled
-to Python-code, run the `demo.sh`-script (or `demo.bat` on Windows)
+to Python-code, run the `demo-3-16.sh`-script (or `demo-3-16.bat` on Windows)
 in the "demo"-sub-directory or the ts2python-repository. 
 
+(Presently, this does not work with the LSP 3.17 specs, because the
+specs contain typescript bugs at a few places and thus would need to 
+be corrected by hand after downloading.)
+
 Or, run the `tst_ts2python_grammar.py` in the ts2python-directory
 and look up the grammar-test-reports in the "REPORT"-sub-directory 
 of the "test_grammar"-subdirectory.
```

### Comparing `ts2python-0.6.6/demo/README_example.py` & `ts2python-0.6.8/demo/README_example.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/demo/extract_ts_from_lsp_specs.py` & `ts2python-0.6.8/demo/extract_ts_from_lsp_specs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,89 @@
 #!/usr/bin/env python3
 
 """extract_ts_from_lsp.py - extracts the typescript parts from the
 specification of the language server protocol:
 https://github.com/microsoft/language-server-protocol/tree/gh-pages/_specifications
 """
 
+import re
+
+
 LSP_SPEC_SOURCE = \
     "https://raw.githubusercontent.com/microsoft/language-server-protocol/" \
-    "gh-pages/_specifications/specification-3-16.md"
+    "gh-pages/_specifications/lsp/3.18/specification.md"
+
+
+def top_level_literal(l):
+    if l[0:1] in ("{", "["):
+        return True
+    return False
 
 
 def extract(specs, dest):
     lines = specs.split('\n')
     ts = []
     copy_flag = False
     for l in lines:
         if l.strip() == '```typescript':
             copy_flag = True
         elif l.strip() == '```':
             copy_flag = False
             ts.append('')
         else:
             if copy_flag:
-                ts.append(l)
+                if top_level_literal(l):
+                    copy_flag = False  # exclude top-level-literals
+                elif l[0:2] != "//":
+                    ts.append(l)
     with open(dest, 'w', encoding='utf-8') as f:
         f.write('\n'.join(ts))
 
 
-def download_specs(url: str) -> str:
+def download_specfile(url: str) -> str:
     import urllib.request
     max_indirections = 2
     while max_indirections > 0:
         if url.startswith('http:') or url.startswith('https:'):
             print('fetching: ' + url)
             with urllib.request.urlopen(url) as f:
                 specs = f.read()
         else:
             with open(url, 'rb') as f:
                 specs = f.read()
-        if len(specs) < 255:
+        if len(specs) < 255 and specs.find(b'\n') < 0:
             url = url[: url.rfind('/') + 1] + specs.decode('utf-8').strip()
             max_indirections -= 1
         else:
             max_indirections = 0
     return specs.decode('utf-8')
 
 
+RX_INCLUDE = re.compile(r'{%\s*include_relative\s*([A-Za-z/.]+?\.md)\s*%}')
+
+
+def download_specs(url: str) -> str:
+    specfile = download_specfile(url)
+    url_path = url[:url.rfind('/') + 1]
+    parts = []
+    e = 0
+    for m in RX_INCLUDE.finditer(specfile):
+        s = m.start()
+        parts.append(specfile[e:s])
+        relpath = m.group(1)
+        parts.append(f'\n```typescript\n\n/* source file: "{relpath}" */\n```\n')
+        incl_url = url_path + relpath
+        include = download_specs(incl_url)
+        parts.append(include)
+        e = m.end()
+    parts.append(specfile[e:])
+    specs = ''.join(parts)
+    return specs
+
+
 if __name__ == "__main__":
     import sys
     if len(sys.argv) > 1:
         url = sys.argv[1]
         if url.startswith('www.'):  url = 'https://' + url
     else:
         url = LSP_SPEC_SOURCE
```

### Comparing `ts2python-0.6.6/demo/specification-3-16.py` & `ts2python-0.6.8/demo/specification-3-16.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/demo/specification-3-16.ts` & `ts2python-0.6.8/demo/specification-3-16.ts`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/demo/specification-current.py` & `ts2python-0.6.8/demo/specification-current.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/demo/specification-current.ts` & `ts2python-0.6.8/demo/specification-current.ts`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/BasicUsage.rst` & `ts2python-0.6.8/docs/BasicUsage.rst`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/Makefile` & `ts2python-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/Mapping.rst` & `ts2python-0.6.8/docs/Mapping.rst`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/Validation.rst` & `ts2python-0.6.8/docs/Validation.rst`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/conf.py` & `ts2python-0.6.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/index.rst` & `ts2python-0.6.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/docs/make.bat` & `ts2python-0.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/pyproject.toml` & `ts2python-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ts2python"
-version = "0.6.6"
+version = "0.6.8"
 description = "Python-Interoperability for Typescript-Interfaces"
 
 license = "Apache-2.0"
 
 authors = ["Eckhart Arnold <eckhart.arnold@posteo.de>"]
 
 readme = "README.md"
@@ -43,15 +43,15 @@
     { include = "tests", format = "sdist" },
     { include = "docs", format = "sdist" }
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-DHParser = { version = "~1.2", optional = false }
+DHParser = { version = "~1.4", optional = false }
 typing_extensions = { version = "^4.0", optional = true }
 
 [tool.poetry.scripts]
 ts2python = 'ts2pythonParser:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools", "wheel"]
```

### Comparing `ts2python-0.6.6/tests/runner.py` & `ts2python-0.6.8/tests/runner.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests/test_singledispatch_shim.py` & `ts2python-0.6.8/tests/test_singledispatch_shim.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests/test_ts2python.py` & `ts2python-0.6.8/tests/test_ts2python.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,13 +369,10 @@
             script = PATH_FIX + f.read()
         with open('testdata.py', 'w', encoding='utf-8') as f:
             f.write(script)
         result = subprocess.run(['python', 'testdata.py'])
         assert result.returncode == 0
 
 
-
-
-
 if __name__ == "__main__":
     from runner import runner
     runner("", globals())
```

### Comparing `ts2python-0.6.6/tests/typing_extensions.py` & `ts2python-0.6.8/tests/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/03_test_literals.ini` & `ts2python-0.6.8/tests_grammar/03_test_literals.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/04_test_Consts.ini` & `ts2python-0.6.8/tests_grammar/04_test_Consts.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/05_test_Enums.ini` & `ts2python-0.6.8/tests_grammar/05_test_Enums.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/06_test_Namespaces.ini` & `ts2python-0.6.8/tests_grammar/06_test_Namespaces.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/07_test_Types.ini` & `ts2python-0.6.8/tests_grammar/07_test_Types.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/08_test_Interfaces.ini` & `ts2python-0.6.8/tests_grammar/08_test_Interfaces.ini`

 * *Files 10% similar despite different names*

```diff
@@ -125,37 +125,52 @@
 M15: """export interface CustomEditorProvider<T extends CustomDocument = CustomDocument> extends CustomReadonlyEditorProvider<T> {
 		readonly onDidChangeCustomDocument: Event<CustomDocumentEditEvent<T>> | Event<CustomDocumentContentChangeEvent<T>>;
 		saveCustomDocument(document: T, cancellation: CancellationToken): Thenable<void>;
 		saveCustomDocumentAs(document: T, destination: Uri, cancellation: CancellationToken): Thenable<void>;
 		revertCustomDocument(document: T, cancellation: CancellationToken): Thenable<void>;
 		backupCustomDocument(document: T, context: CustomDocumentBackupContext, cancellation: CancellationToken): Thenable<CustomDocumentBackup>;
 	}"""
+M16: """export interface WorkspaceUnchangedDocumentDiagnosticReport extends
+        UnchangedDocumentDiagnosticReport {
+
+        /**
+         * The URI for which diagnostic information is reported.
+         */
+        uri: DocumentUri;
+
+        /**
+         * The version number for which the diagnostics are reported.
+         * If the document is not marked as open `null` can be provided.
+         */
+        version: integer | null;
+    };"""
+
 
 
 [py:interface]
 M7: """
 	class SemanticTokensRegistrationOptions(TextDocumentRegistrationOptions, SemanticTokensOptions, StaticRegistrationOptions):
 	    pass
     """
 M9: """
-	class SemanticTokensClientCapabilities(TypedDict, total=False):
-	    class Requests_0(TypedDict, total=False):
-	        class Range_1(TypedDict, total=True):
+	class SemanticTokensClientCapabilities(TypedDict):
+	    class Requests_0(TypedDict):
+	        class Range_1(TypedDict):
 	            pass
-	        class Full_1(TypedDict, total=False):
-	            delta: Optional[bool]
-	        range: Union[bool, Range_1, None]
-	        full: Union[bool, Full_1, None]
-	    dynamicRegistration: Optional[bool]
+	        class Full_1(TypedDict):
+	            delta: NotRequired[bool]
+	        range: NotRequired[Union[bool, Range_1]]
+	        full: NotRequired[Union[bool, Full_1]]
+	    dynamicRegistration: NotRequired[bool]
 	    requests: Requests_0
 	    tokenTypes: List[str]
 	    tokenModifiers: List[str]
 	    formats: List['TokenFormat']
-	    overlappingTokenSupport: Optional[bool]
-	    multilineTokenSupport: Optional[bool]
+	    overlappingTokenSupport: NotRequired[bool]
+	    multilineTokenSupport: NotRequired[bool]
     """
 
 [fail:interface]
 
 
 [match:type_alias]
 M1: """export type integer = number;"""
@@ -220,18 +235,18 @@
 
 [ast:declaration]
 
 [fail:declaration]
 
 [py:declaration]
 M2: """
-	class Documentation_0(TypedDict, total=True):
+	class Documentation_0(TypedDict):
     	kind: 'CodeActionKind'
         command: 'Command'
-    documentation: Optional[List[Documentation_0]]"""
+    documentation: NotRequired[List[Documentation_0]]"""
 
 
 [match:function]
 M1: """lineAt(line: number): TextLine"""
 M2: """save(): Thenable<boolean>"""
 M3: """edit(callback: (editBuilder: TextEditorEdit) => void, options?: { readonly undoStopBefore: boolean; readonly undoStopAfter: boolean }): Thenable<boolean>"""
 M4: """function registerTextEditorCommand(command: string, callback: (textEditor: TextEditor, edit: TextEditorEdit, ...args: any[]) => void, thisArg?: any): Disposable"""
```

### Comparing `ts2python-0.6.6/tests_grammar/09_test_Typescript_Document.ini` & `ts2python-0.6.8/tests_grammar/09_test_Typescript_Document.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/tests_grammar/99_test_Playground.ini` & `ts2python-0.6.8/tests_grammar/99_test_Playground.ini`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/ts2python/__init__.py` & `ts2python-0.6.8/ts2python/__init__.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/ts2python/json_validation.py` & `ts2python-0.6.8/ts2python/json_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,25 @@
     Generic, TypeVar, Iterable, Callable, get_type_hints
 try:
     from typing_extensions import GenericMeta, \
         ClassVar, Final, Protocol, NoReturn
 except (ImportError, ModuleNotFoundError):
     from .typing_extensions import GenericMeta, \
         ClassVar, Final, Protocol, NoReturn
-# try:
-#     from typing import ForwardRef, _GenericAlias, _SpecialForm
-# except ImportError:
-#     from typing import _ForwardRef  # Python 3.6 compatibility
-#     ForwardRef = _ForwardRef
-#     _GenericAlias = GenericMeta
-#     _SpecialForm = Any
-# try:
-#     from typing_extensions import get_origin
-# except ImportError:
-#     def get_origin(typ):
-#         try:
-#             return typ.__origin__
-#         except AttributeError:
-#             return Generic
-try:
-    from typeddict_shim import TypedDict, GenericTypedDict, _TypedDictMeta, get_origin, ForwardRef
-except (ImportError, ModuleNotFoundError):
-    from .typeddict_shim import TypedDict, GenericTypedDict, _TypedDictMeta, get_origin, ForwardRef
+
+if sys.version_info >= (3, 11):
+    from typing import TypedDict, _TypedDictMeta, get_origin, ForwardRef
+else:
+    try:
+        from ts2python.typeddict_shim import TypedDict, _TypedDictMeta, get_origin, ForwardRef
+    except (ImportError, ModuleNotFoundError):
+        try:
+            from typeddict_shim import TypedDict, _TypedDictMeta, get_origin, ForwardRef
+        except (ImportError, ModuleNotFoundError):
+            from .typeddict_shim import TypedDict, _TypedDictMeta, get_origin, ForwardRef
 
 
 
 __all__ = ['validate_type', 'type_check', 'validate_uniform_sequence']
 
 
 def strdata(data: Any) -> str:
@@ -81,14 +73,22 @@
     #     raise ValueError(f"{val} is not contained in enum {typ}")
     if not hasattr(typ, '__value_set__'):
         typ.__value_set__ = {member.value for member in typ.__members__.values()}
     if val not in typ.__value_set__:
         raise ValueError(f"{val} is not contained in enum {typ}")
 
 
+def is_TypedDictClass(typ) -> bool:
+    """True, if typ is an instance of _TypedDictMeta."""
+    return isinstance(typ, _TypedDictMeta)
+    # try:
+    #   return isinstance(typ, _TypedDictMeta) or str(typ.__class__)[-16:-2] == "_TypedDictMeta"
+    # except AttributeError:
+    #     return False
+
 def validate_type(val: Any, typ):
     """Raises a TypeError if value `val` is not of type `typ`.
     In particualr, `validate_type()` can be used to validate
     dictionaries against TypedDict-types and, more general,
     to validate JSON-data.
     Examples::
     >>> validate_type(1, int)
@@ -103,15 +103,15 @@
     >>> try:
     ...     validate_type(bad_json_data, Position)
     ... except TypeError as e:
     ...     print(e)
     Type error(s) in dictionary of type <class 'json_validation.Position'>:
     Field character: 'A' is not a <class 'int'>, but a <class 'str'>
     """
-    if isinstance(typ, _TypedDictMeta):
+    if is_TypedDictClass(typ):
         if not isinstance(val, Dict):
             raise TypeError(f"{val} is not even a dictionary")
         validate_TypedDict(val, typ)
     elif hasattr(typ, '__args__'):
         validate_compound_type(val, typ)
     else:
         if not isinstance(val, typ):
@@ -133,15 +133,15 @@
     3 is not of type <class 'str'>
 
     :param sequence: An iterable to be validated
     :param item_type: The expected type of all items the iterable `sequence` yields.
 
     """
     # assert not isinstance(item_type, str), f'Unresolved type name or forward reference for {item_type}!'
-    if isinstance(item_type, _TypedDictMeta):
+    if is_TypedDictClass(item_type):
         for val in sequence:
             if not isinstance(val, Dict):
                 raise TypeError(f"{val} is not of type {item_type}")
             validate_TypedDict(val, item_type)
     elif hasattr(item_type, '__args__'):
         for val in sequence:
             validate_compound_type(val, item_type)
@@ -217,42 +217,42 @@
 
     :param D: the dictionary to be validated
     :param T: the assumed TypedDict type of that dictionary
     :return: None
     :raise: TypeError in case a type error has been detected.
     """
     assert isinstance(D, Dict), str(D)
-    assert isinstance(T, _TypedDictMeta), str(T)
+    assert is_TypedDictClass(T), str(T)
     type_errors = []
     missing = T.__required_keys__ - D.keys()
     if missing:
         type_errors.append(f"Missing required keys: {missing}")
     unexpected = D.keys() - (T.__required_keys__ | T.__optional_keys__)
     if unexpected:
         type_errors.append(f"Unexpected keys: {unexpected}")
     for field, field_type in get_type_hints(T).items():
         if field not in D:
             continue
         resolved_field_type = resolve_forward_refs(field_type, T)
         if resolved_field_type != field_type:
             field_type = resolved_field_type
             T.__annotations__[field] = field_type
-        if isinstance(field_type, _TypedDictMeta):
+        if is_TypedDictClass(field_type):
             value = D[field]
             if isinstance(value, Dict):
                 validate_TypedDict(value, field_type)
             else:
                 type_errors.append(f"Field {field}: '{strdata(D[field])}' is not of {field_type}, "
                                    f"but of type {type(D[field])}")
         elif get_origin(field_type) is Union:
             value = D[field]
             for union_typ in field_type.__args__:
                 # if isinstance(union_typ, ForwardRef):
                 #     union_typ = union_typ._evaluate(globals(), sys.modules[T.__module__].__dict__)
-                if isinstance(union_typ, _TypedDictMeta):
+                if is_TypedDictClass(union_typ):
                     if isinstance(value, Dict):
                         try:
                             validate_TypedDict(value, union_typ)
                             break
                         except TypeError:
                             pass
                 elif hasattr(union_typ, '__args__'):
```

### Comparing `ts2python-0.6.6/ts2python/singledispatch_shim.py` & `ts2python-0.6.8/ts2python/singledispatch_shim.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/ts2python/typeddict_shim.py` & `ts2python-0.6.8/ts2python/typeddict_shim.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 try:
     from typing import ForwardRef, _GenericAlias, _SpecialForm
 except (ImportError, ModuleNotFoundError):
     from typing import _ForwardRef  # Python 3.6 compatibility
     ForwardRef = _ForwardRef
     _GenericAlias = GenericMeta
-    _SpecialForm = Any
+    _SpecialForm = object
 
 try:
     from typing_extensions import get_origin
 except (ImportError, ModuleNotFoundError):
     try:
         from .typing_extensions import get_origin
     except (ImportError, ModuleNotFoundError):
@@ -150,20 +150,23 @@
         required_keys.update(base.__dict__.get('__required_keys__', ()))
         optional_keys.update(base.__dict__.get('__optional_keys__', ()))
 
     annotations.update(own_annotations)
 
     total = True
     for field, field_type in own_annotations.items():
-        if ((isinstance(field_type, ForwardRef)
-             and (field_type.__forward_arg__.startswith('Optional[')
-                  or (field_type.__forward_arg__.startswith('Union[')
-                      and field_type.__forward_arg__.endswith(', None]'))))
-            or (get_origin(field_type) is Union
-                and type(None) in field_type.__args__)):
+        field_type_origin = get_origin(field_type)
+        if (field_type_origin is NotRequired
+            or (field_type_origin is Union
+                and type(None) in field_type.__args__)
+            or (isinstance(field_type, ForwardRef)
+                and (field_type.__forward_arg__.startswith('Optional[')
+                     or field_type.__forward_arg__.startswith('NotRequired')
+                     or (field_type.__forward_arg__.startswith('Union[')
+                         and field_type.__forward_arg__.endswith(', None]'))))):
             optional_keys.add(field)
             total = False
         else:
             required_keys.add(field)
 
     tp_dict.__annotations__ = annotations
     tp_dict.__required_keys__ = frozenset(required_keys)
@@ -192,15 +195,15 @@
         raise TypeError('TypedDict does not support instance and class checks')
 
     __instancecheck__ = __subclasscheck__
 
 
 _is_pypy = hasattr(sys, 'pypy_version_info')
     
-if sys.version_info >= (3,11) and not _is_pypy:
+if sys.version_info >= (3, 11) and not _is_pypy:
     from typing import TypedDict
     GenericTypedDict = TypedDict
 
 elif sys.version_info >= (3, 7) and not _is_pypy:
     def TypedDict(typename, fields=None, *, total=True, **kwargs):
         """An alternative implementation of typing.TypedDict that, instead of
         relying on the `total`-parameter, allows to treat individual fields
@@ -257,26 +260,29 @@
             # Setting correct module is necessary to make typed dict classes pickleable.
             ns['__module__'] = module
 
         return _TypedDictMeta(typename, (), ns)
 
     GenericTypedDict = TypedDict
 
+    _TypedDict = type.__new__(_TypedDictMeta, 'TypedDict', (), {})
+    TypedDict.__mro_entries__ = lambda bases: (_TypedDict,)
+
 else:  # Python Version 3.6
     TypedDict = _TypedDictMeta('TypedDict', (dict,), {})
     TypedDict.__module__ = __name__
     class _GenericTypedDictMeta(GenericMeta):
         def __new__(cls, name, bases, ns, total=True):
             return _new_typed_dict(_GenericTypedDictMeta, name, bases, ns)
         __call__ = dict
         def __subclasscheck__(cls, other):
             return False  # hack to support Python 3.6
         __instancecheck__ = __subclasscheck__
 
     GenericTypedDict = _GenericTypedDictMeta('TypedDict', (dict,), {})
     GenericTypedDict.__module__ = __name__
 
-_TypedDict = type.__new__(_TypedDictMeta, 'TypedDict', (), {})
-TypedDict.__mro_entries__ = lambda bases: (_TypedDict,)
+    _TypedDict = type.__new__(_TypedDictMeta, 'TypedDict', (), {})
+    TypedDict.__mro_entries__ = lambda bases: (_TypedDict,)
 
 # up to this point all functions have been copied and adapted from
 # the typing.py module of the Python-STL
```

### Comparing `ts2python-0.6.6/ts2python/typeddict_shim2.py` & `ts2python-0.6.8/ts2python/typeddict_shim2.py`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/ts2python/typing_extensions.py` & `ts2python-0.6.8/ts2python/typing_extensions.py_ALT`

 * *Files identical despite different names*

### Comparing `ts2python-0.6.6/ts2pythonParser.py` & `ts2python-0.6.8/ts2pythonParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     trace_history, has_descendant, neg, has_ancestor, optional_last_value, insert, \
     positions_of, replace_child_names, add_attributes, delimit_children, merge_connected, \
     has_attr, has_parent, ThreadLocalSingletonFactory, Error, canonical_error_strings, \
     has_errors, WARNING, ERROR, FATAL, set_preset_value, get_preset_value, NEVER_MATCH_PATTERN, \
     gen_find_include_func, preprocess_includes, make_preprocessor, chain_preprocessors, \
     pick_from_path, json_dumps, RootNode, get_config_values, md5, StringView, as_list
 
+from DHParser.dsl import PseudoJunction, create_parser_transition
+
 
 #######################################################################
 #
 # PREPROCESSOR SECTION - Can be edited. Changes will be preserved.
 #
 #######################################################################
 
@@ -112,16 +114,16 @@
     declarations_block = Forward()
     document = Forward()
     function = Forward()
     generic_type = Forward()
     literal = Forward()
     type = Forward()
     types = Forward()
-    source_hash__ = "78f0bf127eb18af0d7d13aa2aae2cf3f"
-    disposable__ = re.compile('INT$|NEG$|FRAC$|DOT$|EXP$|EOF$|_array_ellipsis$|_top_level_assignment$|_top_level_literal$|_quoted_identifier$|_root$|_namespace$|_part$')
+    source_hash__ = "56adb196bd5a140ba91a3f2f70f056df"
+    disposable__ = re.compile('(?:INT$|NEG$|FRAC$|DOT$|EXP$|EOF$|_array_ellipsis$|_top_level_assignment$|_top_level_literal$|_quoted_identifier$|_root$|_namespace$|_part$)|(?:INT$|NEG$|FRAC$|DOT$|EXP$|EOF$|_array_ellipsis$|_top_level_assignment$|_top_level_literal$|_quoted_identifier$|_root$|_namespace$|_part$)')
     static_analysis_pending__ = []  # type: List[bool]
     parser_initialization__ = ["upon instantiation"]
     COMMENT__ = r'(?:\/\/.*)|(?:\/\*(?:.|\n)*?\*\/)'
     comment_rx__ = re.compile(COMMENT__)
     WHITESPACE__ = r'\s*'
     WSP_RE__ = mixin_comment(whitespace=WHITESPACE__, comment=COMMENT__)
     wsp__ = Whitespace(WSP_RE__)
@@ -134,15 +136,15 @@
     INT = Series(Option(NEG), Alternative(RegExp('[1-9][0-9]+'), RegExp('[0-9]')))
     _part = RegExp('(?!\\d)\\w+')
     identifier = Series(NegativeLookahead(Alternative(Text("true"), Text("false"))), _part, ZeroOrMore(Series(Text("."), _part)), dwsp__)
     _quoted_identifier = Alternative(identifier, Series(Series(Drop(Text('"')), dwsp__), identifier, Series(Drop(Text('"')), dwsp__), mandatory=2), Series(Series(Drop(Text("\'")), dwsp__), identifier, Series(Drop(Text("\'")), dwsp__), mandatory=2))
     variable = Series(identifier, ZeroOrMore(Series(Text("."), identifier)))
     basic_type = Series(Alternative(Text("object"), Text("array"), Text("string"), Text("number"), Text("boolean"), Text("null"), Text("integer"), Text("uinteger"), Text("decimal"), Text("unknown"), Text("any"), Text("void")), dwsp__)
     name = Alternative(identifier, Series(Series(Drop(Text('"')), dwsp__), identifier, Series(Drop(Text('"')), dwsp__)))
-    association = Series(name, Series(Drop(Text(":")), dwsp__), literal)
+    association = Series(name, Series(Drop(Text(":")), dwsp__), literal, mandatory=1)
     object = Series(Series(Drop(Text("{")), dwsp__), Option(Series(association, ZeroOrMore(Series(Series(Drop(Text(",")), dwsp__), association)))), Option(Series(Drop(Text(",")), dwsp__)), Series(Drop(Text("}")), dwsp__))
     array = Series(Series(Drop(Text("[")), dwsp__), Option(Series(literal, ZeroOrMore(Series(Series(Drop(Text(",")), dwsp__), literal)))), Series(Drop(Text("]")), dwsp__))
     string = Alternative(Series(RegExp('"[^"\\n]*"'), dwsp__), Series(RegExp("'[^'\\n]*'"), dwsp__))
     boolean = Series(Alternative(Text("true"), Text("false")), dwsp__)
     number = Series(INT, FRAC, EXP, dwsp__)
     integer = Series(INT, NegativeLookahead(RegExp('[.Ee]')), dwsp__)
     type_tuple = Series(Series(Drop(Text("[")), dwsp__), types, ZeroOrMore(Series(Series(Drop(Text(",")), dwsp__), types)), Series(Drop(Text("]")), dwsp__))
@@ -164,15 +166,15 @@
     extends = Series(Series(Drop(Text("extends")), dwsp__), Alternative(generic_type, type_name), ZeroOrMore(Series(Series(Drop(Text(",")), dwsp__), Alternative(generic_type, type_name))))
     array_types = Synonym(array_type)
     array_of = Series(Option(Series(Drop(Text("readonly")), dwsp__)), array_types, Series(Drop(Text("[]")), dwsp__))
     arg_tail = Series(Series(Drop(Text("...")), dwsp__), identifier, Option(Series(Series(Drop(Text(":")), dwsp__), array_of)))
     parameter_type = Alternative(array_of, basic_type, generic_type, Series(type_name, Option(extends_type), Option(equals_type)), declarations_block, type_tuple)
     parameter_types = Series(parameter_type, ZeroOrMore(Series(Series(Drop(Text("|")), dwsp__), parameter_type)))
     type_parameters = Series(Series(Drop(Text("<")), dwsp__), parameter_types, ZeroOrMore(Series(Series(Drop(Text(",")), dwsp__), parameter_types)), Series(Drop(Text(">")), dwsp__), mandatory=1)
-    interface = Series(Option(Series(Drop(Text("export")), dwsp__)), Alternative(Series(Drop(Text("interface")), dwsp__), Series(Drop(Text("class")), dwsp__)), identifier, Option(type_parameters), Option(extends), declarations_block, mandatory=2)
+    interface = Series(Option(Series(Drop(Text("export")), dwsp__)), Alternative(Series(Drop(Text("interface")), dwsp__), Series(Drop(Text("class")), dwsp__)), identifier, Option(type_parameters), Option(extends), declarations_block, Option(Series(Drop(Text(";")), dwsp__)), mandatory=2)
     type_alias = Series(Option(Series(Drop(Text("export")), dwsp__)), Series(Drop(Text("type")), dwsp__), identifier, Option(type_parameters), Series(Drop(Text("=")), dwsp__), types, Series(Drop(Text(";")), dwsp__), mandatory=2)
     module = Series(Series(Drop(Text("declare")), dwsp__), Series(Drop(Text("module")), dwsp__), _quoted_identifier, Series(Drop(Text("{")), dwsp__), document, Series(Drop(Text("}")), dwsp__))
     namespace = Series(Option(Series(Drop(Text("export")), dwsp__)), Series(Drop(Text("namespace")), dwsp__), identifier, Series(Drop(Text("{")), dwsp__), ZeroOrMore(Alternative(interface, type_alias, enum, const, Series(Option(Series(Drop(Text("export")), dwsp__)), declaration, Series(Drop(Text(";")), dwsp__)), Series(Option(Series(Drop(Text("export")), dwsp__)), function, Series(Drop(Text(";")), dwsp__)))), Series(Drop(Text("}")), dwsp__), mandatory=2)
     intersection = Series(type, OneOrMore(Series(Series(Drop(Text("&")), dwsp__), type, mandatory=1)))
     virtual_enum = Series(Option(Series(Drop(Text("export")), dwsp__)), Series(Drop(Text("namespace")), dwsp__), identifier, Series(Drop(Text("{")), dwsp__), ZeroOrMore(Alternative(interface, type_alias, enum, const, Series(declaration, Series(Drop(Text(";")), dwsp__)))), Series(Drop(Text("}")), dwsp__))
     _namespace = Alternative(virtual_enum, namespace)
     optional = Series(Text("?"), dwsp__)
@@ -196,32 +198,18 @@
                       'const': [re.compile(r'(?=export|$)')],
                       'declaration': [re.compile(r'(?=export|$)')],
                       '_top_level_assignment': [re.compile(r'(?=export|$)')],
                       '_top_level_literal': [re.compile(r'(?=export|$)')],
                       'module': [re.compile(r'(?=export|$)')]}
     root__ = TreeReduction(_root, CombinedParser.MERGE_TREETOPS)
     
-
-_raw_grammar = ThreadLocalSingletonFactory(ts2pythonGrammar)
-
-def get_grammar() -> ts2pythonGrammar:
-    grammar = _raw_grammar()
-    if get_config_value('resume_notices'):
-        resume_notices_on(grammar)
-    elif get_config_value('history_tracking'):
-        set_tracer(grammar, trace_history)
-    try:
-        if not grammar.__class__.python_src__:
-            grammar.__class__.python_src__ = get_grammar.python_src__
-    except AttributeError:
-        pass
-    return grammar
     
-def parse_ts2python(document, start_parser = "root_parser__", *, complete_match=True):
-    return get_grammar()(document, start_parser, complete_match=complete_match)
+parsing: PseudoJunction = create_parser_transition(
+    ts2pythonGrammar)
+get_grammar = parsing.factory # for backwards compatibility, only    
 
 
 #######################################################################
 #
 # AST SECTION - Can be edited. Changes will be preserved.
 #
 #######################################################################
@@ -277,14 +265,16 @@
     # do not use list, tuple, dict, because contained types won't be forward ref'd
     from collections.abc import Coroutine
 else:
     from typing import Union, List, Tuple, Optional, Dict, Any, Generic, TypeVar, Callable, Coroutine
 """
 
 TYPEDDICT_IMPORTS = """
+
+
 try:
     from ts2python.typeddict_shim import TypedDict, GenericTypedDict, NotRequired, Literal
     # Overwrite typing.TypedDict for Runtime-Validation
 except ImportError:
     print("Module ts2python.typeddict_shim not found. Only coarse-grained " 
           "runtime type-validation of TypedDicts possible")
     try:
@@ -322,16 +312,16 @@
         from functools import singledispatch, singledispatchmethod
     except ImportError:
         print(f"functools.singledispatchmethod does not exist in Python Version "
               f"{sys.version}. This module may therefore fail to run if "
               f"singledispatchmethod is needed, anywhere!")     
 """
 
-PEP655_IMPORTS = """
-"""
+# PEP655_IMPORTS = """
+# """
 
 
 def to_typename(varname: str) -> str:
     # assert varname[-1:] != '_' or keyword.iskeyword(varname[:-1]), varname  # and varname[0].islower()
     return varname[0].upper() + varname[1:] + '_'
 
 
@@ -384,15 +374,15 @@
         if self.class_decorator:
             if self.class_decorator[0] != '@':
                 self.class_decorator = '@' + self.class_decorator
             self.class_decorator += '\n'
         self.use_enums = get_config_value('ts2python.UseEnum', True)
         self.use_type_union = get_config_value('ts2python.UseTypeUnion', False)
         self.use_literal_type = get_config_value('ts2python.UseLiteralType', True)
-        self.use_not_required = get_config_value('ts2python.UseNotRequired', False)
+        self.use_not_required = get_config_value('ts2python.UseNotRequired', True)
 
         self.overloaded_type_names: Set[str] = set()
         self.known_types: List[Set[str]] = [
             {'Union', 'List', 'Tuple', 'Optional', 'Dict', 'Any',
              'Generic', 'Coroutine', 'list'}]
         self.local_classes: List[List[str]] = [[]]
         self.base_classes: Dict[str, List[str]] = {}
@@ -439,16 +429,16 @@
         chksum = f'source_hash__ = "{source_hash(self.tree.source)}"'
         if self.tree.name == 'document':
             code_blocks = [
                 f'# Generated by ts2python on {datetime.datetime.now()}\n',
                 GENERAL_IMPORTS, TYPEDDICT_IMPORTS, FUNCTOOLS_IMPORTS,
                 self.additional_imports, chksum, '\n##### BEGIN OF LSP SPECS\n'
             ]
-            if self.base_class_name == 'TypedDict':
-                code_blocks.append(PEP655_IMPORTS)
+            # if self.base_class_name == 'TypedDict':
+            #     code_blocks.append(PEP655_IMPORTS)
         else:
             code_blocks = []
         code_blocks.append(python_code)
         if self.tree.name == 'document':
             code_blocks.append('\n##### END OF LSP SPECS\n')
         cooked = '\n\n'.join(code_blocks)
         cooked = re.sub(' +(?=\n)', '', cooked)
```

### Comparing `ts2python-0.6.6/setup.py` & `ts2python-0.6.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,246 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ts2python
+Version: 0.6.8
+Summary: Python-Interoperability for Typescript-Interfaces
+Home-page: https://github.com/jecki/ts2python
+License: Apache-2.0
+Keywords: Typescript to Python converter,Typescript Interface,Python TypedDict
+Author: Eckhart Arnold
+Author-email: eckhart.arnold@posteo.de
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Text Processing :: Markup
+Requires-Dist: DHParser (>=1.4,<1.5)
+Requires-Dist: typing_extensions (>=4.0,<5.0)
+Project-URL: Repository, https://github.com/jecki/ts2python
+Description-Content-Type: text/markdown
+
+# ts2python
+
+![](https://img.shields.io/pypi/v/ts2python) 
+![](https://img.shields.io/pypi/status/ts2python) 
+![](https://img.shields.io/pypi/pyversions/ts2python) 
+![](https://img.shields.io/pypi/l/ts2python)
+
+Python-interoperability for Typescript-Interfaces.
+Transpiles TypeScript-Interface-definitions to Python 
+TypedDicts, plus support for run-time type-checking 
+of JSON-data.
+
+## License and Source Code
+
+ts2python is open source software under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)
+
+Copyright 2021-2023 Eckhart Arnold <arnold@badw.de>, Bavarian Academy of Sciences and Humanities
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    https://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+The complete source-code of ts2python can be downloaded from the [its git-repository](https://github.com/jecki/ts2python).
+
+## Purpose
+
+When processing JSON data, as for example form a 
+[JSON-RPC](https://www.jsonrpc.org/) call, with Python, it would
+be helpful to have Python-definitions of the JSON-structures at
+hand, in order to solicit IDE-Support, static type checking and,
+potentially to enable structural validation at runtime. 
+
+There exist different technologies for defining the structure of
+JSON-data. Next to [JSON-schema](http://json-schema.org/), a 
+de facto very popular technology for defining JSON-obejcts are
+[Typescript-Interfaces](https://www.typescriptlang.org/docs/handbook/2/objects.html). 
+For example, the 
+[language server protocol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/) 
+defines the structure of the JSON-data exchanged between client 
+and server with Typescript-Interfaces.
+
+In order to enable structural validation on the Python-side, 
+ts2python transpiles the typescript-interface definitions
+to Python-data structure definitions, primarily, 
+[TypedDicts](https://www.python.org/dev/peps/pep-0589/),
+but with some postprocessing it can also be adjusted to
+other popular models for records or data structures in
+Python, e.g.
+[pydantic](https://pydantic-docs.helpmanual.io/)-Classes
+and the like.
+
+ts2python aims to support translation of TypeScript-Interfaces on two
+different tiers:
+
+1. *Tier 1: Transpilation of passive data-structures*, that is, 
+   Typescript-definition-files that contain only data definitions 
+   and no function definitions and, in particular,
+   only "passive" Typescript-Interface that define data-structures 
+   but do not contain any methods.
+
+2. *Tier 2: Tanspilation of active data-structures, function- 
+   and method-definitions*, i.e. Translation of (almost) any
+   Typescript-definition-file.
+
+## Status
+
+Presently, Tier 1 support, i.e. transpilation of passive data 
+structures works quite well. So, for example, all Interfaces
+from the
+[language server protocol V3.16](https://microsoft.github.io/language-server-protocol/specifications/specification-3-16/) 
+can be transpiled to Python Typed-Dicts. 
+
+Tier 2 support is still very much work in progress. I am 
+using "vscode.d.ts"-definition file as test case. Some things work,
+but there are still some unsupported constructs and the Python
+code emitted for features that go beyond Tier 1 may not even
+be valid Python all the time! Please, keep that in mind.
+
+The documentation presently only covers Tier 1 support. 
+
+
+## Installation
+
+ts2python can be installed from the command line with the command:
+
+    $ pip install ts2python
+
+ts2python requires the parsing-expression-grammar-framwork 
+[DHParser](https://gitlab.lrz.de/badw-it/DHParser)
+which will automatically be installed as a dependency by 
+the `pip`-command. ts2python requires at least Python Version 3.8
+to run. (If there is any interest, I might backport it to Python 3.6.)
+However, the Python-code it produces is backwards compatible 
+down to Python 3.6, if the 
+[typing extensions](https://pypi.org/project/typing-extensions/) 
+have been installed.
+
+## Usage
+
+In order to generate TypedDict-classes from Typescript-Interfaces,
+run `ts2python` on the Typescript-Interface definitions:
+
+    $ ts2python interfaces.ts
+
+This generates a .py-file in same directory as the source
+file that contains the TypedDict-classes and can simpy be 
+imported in Python-Code:
+
+    from interfaces import *
+
+Json-data which adheres to a specific structure (no matter
+whether defined on the typescript side via interfaces or
+on the Python-side via TypedDicts) can easily be interchanged
+and deserialized:
+
+    import json
+    request_msg: RequestMessage = json.loads(input_data)
+
+The root-type (``RootMessage`` in the above example) can
+be arbitrarily complex and deeply nested.
+
+
+## Validation
+
+ts2python ships support for runtime-type validation. While type
+errors can be detected by static type checkers, runtime type 
+validation can be useful when processing data from an outside
+source which cannot statically be checked, like, for example,
+json-data stemming from an RPC-call. ts2python runtime-type
+validation can be invoked via dedicated functions or via
+decorator as in this example:
+
+    from ts2python.json_validation import TypedDict, type_check
+
+    class Position(TypedDict, total=True):
+        line: int
+        character: int 
+
+    class Range(TypedDict, total=True):
+        start: Position
+        end: Position
+
+    @type_check
+    def middle_line(rng: Range) -> Position:
+        line = (rng['start']['line'] + rng['end']['line']) // 2
+        character = 0
+        return Position(line=line, character=character)
+
+    data = {'start': {'line': 1, 'character': 1},
+           'end': {'line': 8, 'character': 17}}
+    assert middle_line(data) == {'line': 4, 'character': 0}
+
+    malformed_data = {'start': 1, 'end': 8}
+    middle_line(malformed_data)  # <- TypeError raised by @type_check 
+
+With the type decorator the last call fails with a TypeError:
+
+    TypeError: Parameter "rng" of function "middle_line" failed the type-check, because:
+    Type error(s) in dictionary of type <class '__main__.Range'>:
+    Field start: '1' is not of <class '__main__.Position'>, but of type <class 'int'>
+    Field end: '8' is not of <class '__main__.Position'>, but of type <class 'int'>
+
+Both the call and the return types can be validated.
+
+
+## Full Documentation
+
+See [ts2python.readthedocs.io](https://ts2python.readthedocs.io) for the comprehensive
+documentation of ts2python
+
+
+## Tests and Demonstration
+
+The [git-repository of ts2python](https://github.com/jecki/ts2python) contains unit-tests 
+as well as [doctests](https://docs.python.org/3/library/doctest.html).
+After cloning ts2python from the git-repository with:
+
+    $ git clone https://github.com/jecki/ts2python
+
+the unit tests can be found in the `tests` subdirectory. 
+Both the unit and the doctests can be run by changing to the 
+`tests`-sub-directory and calling the `runner.py`-skript therein. 
+
+    $ cd tests
+    $ python runner.py
+
+It is also possible to run the tests with [pytest](https://docs.pytest.org/) 
+or [nose](https://nose.readthedocs.io), in case you have
+either of theses testing-frameworks installed.
+
+For a demonstration how the TypeScript-Interfaces are transpiled
+to Python-code, run the `demo-3-16.sh`-script (or `demo-3-16.bat` on Windows)
+in the "demo"-sub-directory or the ts2python-repository. 
+
+(Presently, this does not work with the LSP 3.17 specs, because the
+specs contain typescript bugs at a few places and thus would need to 
+be corrected by hand after downloading.)
+
+Or, run the `tst_ts2python_grammar.py` in the ts2python-directory
+and look up the grammar-test-reports in the "REPORT"-sub-directory 
+of the "test_grammar"-subdirectory.
 
-packages = \
-['demo', 'docs', 'tests', 'tests_grammar', 'ts2python']
-
-package_data = \
-{'': ['*']}
-
-modules = \
-['ts2pythonParser']
-install_requires = \
-['DHParser>=1.2,<1.3']
-
-entry_points = \
-{'console_scripts': ['ts2python = ts2pythonParser:main']}
-
-setup_kwargs = {
-    'name': 'ts2python',
-    'version': '0.6.6',
-    'description': 'Python-Interoperability for Typescript-Interfaces',
-    'long_description': '# ts2python\n\n![](https://img.shields.io/pypi/v/ts2python) \n![](https://img.shields.io/pypi/status/ts2python) \n![](https://img.shields.io/pypi/pyversions/ts2python) \n![](https://img.shields.io/pypi/l/ts2python)\n\nPython-interoperability for Typescript-Interfaces.\nTranspiles TypeScript-Interface-definitions to Python \nTypedDicts, plus support for run-time type-checking \nof JSON-data.\n\n## License and Source Code\n\nts2python is open source software under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)\n\nCopyright 2021 Eckhart Arnold <arnold@badw.de>, Bavarian Academy of Sciences and Humanities\n\nLicensed under the Apache License, Version 2.0 (the "License");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\n\n    https://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and\nlimitations under the License.\n\nThe complete source-code of ts2python can be downloaded from the [its git-repository](https://github.com/jecki/ts2python).\n\n## Purpose\n\nWhen processing JSON data, as for example form a \n[JSON-RPC](https://www.jsonrpc.org/) call, with Python, it would\nbe helpful to have Python-definitions of the JSON-structures at\nhand, in order to solicit IDE-Support, static type checking and,\npotentially to enable structural validation at runtime. \n\nThere exist different technologies for defining the structure of\nJSON-data. Next to [JSON-schema](http://json-schema.org/), a \nde facto very popular technology for defining JSON-obejcts are\n[Typescript-Interfaces](https://www.typescriptlang.org/docs/handbook/2/objects.html). \nFor example, the \n[language server protocol](https://microsoft.github.io/language-server-protocol/specifications/specification-current/) \ndefines the structure of the JSON-data exchanged between client \nand server with Typescript-Interfaces.\n\nIn order to enable structural validation on the Python-side, \nts2python transpiles the typescript-interface definitions\nto Python-data structure definitions, primarily, \n[TypedDicts](https://www.python.org/dev/peps/pep-0589/),\nbut with some postprocessing it can also be adjusted to\nother popular models for records or data structures in\nPython, e.g.\n[pydantic](https://pydantic-docs.helpmanual.io/)-Classes\nand the like.\n\nts2python aims to support translation of TypeScript-Interfaces on two\ndifferent tiers:\n\n1. *Tier 1: Transpilation of passive data-structures*, that is, \n   Typescript-definition-files that contain only data definitions \n   and no function definitions and, in particular,\n   only "passive" Typescript-Interface that define data-structures \n   but do not contain any methods.\n\n2. *Tier 2: Tanspilation of active data-structures, function- \n   and method-definitions*, i.e. Translation of (almost) any\n   Typescript-definition-file.\n\n## Status\n\nPresently, Tier 1 support, i.e. transpilation of passive data \nstructures works quite well. So, for example, all Interfaces\nfrom the\n[language server protocol V3.16](https://microsoft.github.io/language-server-protocol/specifications/specification-3-16/) \ncan be transpiled to Python Typed-Dicts. \n\nTier 2 support is still very much work in progress. I am \nusing "vscode.d.ts"-definition file as test case. Some things work,\nbut there are still some unsupported constructs and the Python\ncode emitted for features that go beyond Tier 1 may not even\nbe valid Python all the time! Please, keep that in mind.\n\nThe documentation presently only covers Tier 1 support. \n\n\n## Installation\n\nts2python can be installed from the command line with the command:\n\n    $ pip install ts2python\n\nts2python requires the parsing-expression-grammar-framwork \n[DHParser](https://gitlab.lrz.de/badw-it/DHParser)\nwhich will automatically be installed as a dependency by \nthe `pip`-command. ts2python requires at least Python Version 3.8\nto run. (If there is any interest, I might backport it to Python 3.6.)\nHowever, the Python-code it produces is backwards compatible \ndown to Python 3.6, if the \n[typing extensions](https://pypi.org/project/typing-extensions/) \nhave been installed.\n\n## Usage\n\nIn order to generate TypedDict-classes from Typescript-Interfaces,\nrun `ts2python` on the Typescript-Interface definitions:\n\n    $ ts2python interfaces.ts\n\nThis generates a .py-file in same directory as the source\nfile that contains the TypedDict-classes and can simpy be \nimported in Python-Code:\n\n    from interfaces import *\n\nJson-data which adheres to a specific structure (no matter\nwhether defined on the typescript side via interfaces or\non the Python-side via TypedDicts) can easily be interchanged\nand deserialized:\n\n    import json\n    request_msg: RequestMessage = json.loads(input_data)\n\nThe root-type (``RootMessage`` in the above example) can\nbe arbitrarily complex and deeply nested.\n\n\n## Validation\n\nts2python ships support for runtime-type validation. While type\nerrors can be detected by static type checkers, runtime type \nvalidation can be useful when processing data from an outside\nsource which cannot statically be checked, like, for example,\njson-data stemming from an RPC-call. ts2python runtime-type\nvalidation can be invoked via dedicated functions or via\ndecorator as in this example:\n\n    from ts2python.json_validation import TypedDict, type_check\n\n    class Position(TypedDict, total=True):\n        line: int\n        character: int \n\n    class Range(TypedDict, total=True):\n        start: Position\n        end: Position\n\n    @type_check\n    def middle_line(rng: Range) -> Position:\n        line = (rng[\'start\'][\'line\'] + rng[\'end\'][\'line\']) // 2\n        character = 0\n        return Position(line=line, character=character)\n\n    data = {\'start\': {\'line\': 1, \'character\': 1},\n           \'end\': {\'line\': 8, \'character\': 17}}\n    assert middle_line(data) == {\'line\': 4, \'character\': 0}\n\n    malformed_data = {\'start\': 1, \'end\': 8}\n    middle_line(malformed_data)  # <- TypeError raised by @type_check \n\nWith the type decorator the last call fails with a TypeError:\n\n    TypeError: Parameter "rng" of function "middle_line" failed the type-check, because:\n    Type error(s) in dictionary of type <class \'__main__.Range\'>:\n    Field start: \'1\' is not of <class \'__main__.Position\'>, but of type <class \'int\'>\n    Field end: \'8\' is not of <class \'__main__.Position\'>, but of type <class \'int\'>\n\nBoth the call and the return types can be validated.\n\n\n## Full Documentation\n\nSee [ts2python.readthedocs.io](https://ts2python.readthedocs.io) for the comprehensive\ndocumentation of ts2python\n\n\n## Tests and Demonstration\n\nThe [git-repository of ts2python](https://github.com/jecki/ts2python) contains unit-tests \nas well as [doctests](https://docs.python.org/3/library/doctest.html).\nAfter cloning ts2python from the git-repository with:\n\n    $ git clone https://github.com/jecki/ts2python\n\nthe unit tests can be found in the `tests` subdirectory. \nBoth the unit and the doctests can be run by changing to the \n`tests`-sub-directory and calling the `runner.py`-skript therein. \n\n    $ cd tests\n    $ python runner.py\n\nIt is also possible to run the tests with [pytest](https://docs.pytest.org/) \nor [nose](https://nose.readthedocs.io), in case you have\neither of theses testing-frameworks installed.\n\nFor a demonstration how the TypeScript-Interfaces are transpiled\nto Python-code, run the `demo.sh`-script (or `demo.bat` on Windows)\nin the "demo"-sub-directory or the ts2python-repository. \n\nOr, run the `tst_ts2python_grammar.py` in the ts2python-directory\nand look up the grammar-test-reports in the "REPORT"-sub-directory \nof the "test_grammar"-subdirectory.\n',
-    'author': 'Eckhart Arnold',
-    'author_email': 'eckhart.arnold@posteo.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jecki/ts2python',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

