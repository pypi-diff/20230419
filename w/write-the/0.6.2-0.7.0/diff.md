# Comparing `tmp/write_the-0.6.2.tar.gz` & `tmp/write_the-0.7.0.tar.gz`

## Comparing `write_the-0.6.2.tar` & `write_the-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.6.2/mkdocs.yml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.6.2/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.6.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/README.md
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.6.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/CNAME
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/docs/reference/utils.md
--rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.6.2/images/docs-help.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.6.2/images/mkdocs-help.png
--rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.6.2/images/multiply.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.6.2/images/tests-help.png
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.6.2/images/write-the-icon.svg
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cli_main.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/test_cst_utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.6.2/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/__main__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cli/main.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/chain.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/mkdocs/write.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/__init__.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/chain.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 write_the-0.6.2/write_the/tests/write.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.6.2/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 write_the-0.6.2/README.md
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 write_the-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 write_the-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.7.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.7.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/CNAME
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/tests.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.0/docs/reference/utils.md
+-rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.7.0/images/docs-help.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.0/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.0/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.0/images/tests-help.png
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.0/images/write-the-icon.svg
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cli_main.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/test_cst_utils.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/data/expected.dat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.0/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/mkdocs/write.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/tests/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/tests/chain.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 write_the-0.7.0/write_the/tests/write.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 write_the-0.7.0/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 write_the-0.7.0/PKG-INFO
```

### Comparing `write_the-0.6.2/mkdocs.yml` & `write_the-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/.github/workflows/tests.yml` & `write_the-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/.pytest_cache/v/cache/lastfailed` & `write_the-0.7.0/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/.pytest_cache/v/cache/nodeids` & `write_the-0.7.0/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/docs/index.md` & `write_the-0.7.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
 
 -----
 
 **Table of Contents**
 
 - [Features](#Features)
 - [Requirements](#Requirements)
```

### Comparing `write_the-0.6.2/images/docs-help.png` & `write_the-0.7.0/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/images/mkdocs-help.png` & `write_the-0.7.0/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/images/tests-help.png` & `write_the-0.7.0/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/images/write-the-icon.svg` & `write_the-0.7.0/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cli_main.py` & `write_the-0.7.0/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_docstring_adder.py` & `write_the-0.7.0/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_docstring_remover.py` & `write_the-0.7.0/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_function_and_class_collector.py` & `write_the-0.7.0/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_node_extractor.py` & `write_the-0.7.0/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_node_remover.py` & `write_the-0.7.0/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/tests/test_cst_utils.py` & `write_the-0.7.0/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/utils.py` & `write_the-0.7.0/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cli/main.py` & `write_the-0.7.0/write_the/cli/main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/docstring_adder.py` & `write_the-0.7.0/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/docstring_remover.py` & `write_the-0.7.0/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/function_and_class_collector.py` & `write_the-0.7.0/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/node_extractor.py` & `write_the-0.7.0/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/node_remover.py` & `write_the-0.7.0/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/cst/utils.py` & `write_the-0.7.0/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/docs/write.py` & `write_the-0.7.0/write_the/docs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/mkdocs/write.py` & `write_the-0.7.0/write_the/mkdocs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/write_the/tests/chain.py` & `write_the-0.7.0/write_the/tests/chain.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenAI
 
 
 tests_template = """
-Please generate unit tests for the following code using the pytest framework. 
-Include fixtures and parametrize function where appropriate, and only return test code. 
-The tests should cover all possible scenarios, including edge cases. 
-Include imports where required. Do not provide explanations or additional information. 
-Remember to import the code from `{path}` and fix any relative imports. 
-Please generate pytest test functions for the following code:
+Generate pytest unit tests for the code below, covering all possible scenarios and edge cases. 
+Use fixtures and parametrize when appropriate. 
+Import the code from {path} and adjust any relative imports. 
+Return only the test code.
+
+Code:
 ```python
 {code}
 ```
 """
 docs_prompt = PromptTemplate(input_variables=["code", "path"], template=tests_template)
 
-def run(code, path, temperature=0, max_tokens=2000, gpt_4=False) -> str:
+def run(code, path, temperature=0, max_tokens=-1, gpt_4=False) -> str:
     """
     Generates unit tests for a given code snippet using the pytest framework.
     Args:
       code (str): The code snippet to generate tests for.
       path (str): The path to the code snippet.
       temperature (float, optional): The temperature parameter for the OpenAI model. Defaults to 0.
       max_tokens (int, optional): The maximum number of tokens to generate. Defaults to 2000.
```

### Comparing `write_the-0.6.2/write_the/tests/write.py` & `write_the-0.7.0/write_the/tests/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,9 +18,9 @@
       >>> write_the_tests(Path("test.py"), gpt_4=True)
       "Formatted and tested code"
     """
     with open(filename, "r") as file:
         source_code = file.read()
     source_code = format_str(source_code, mode=FileMode())
     result = run(code=source_code, path=filename, gpt_4=gpt_4)
-    code = result.strip().lstrip("```python").lstrip("```").rstrip("```")
+    code = result.strip().lstrip("Test Code:\n```python").lstrip("```python").lstrip("```").rstrip("```")
     return format_str(code, mode=FileMode())
```

### Comparing `write_the-0.6.2/LICENSE.txt` & `write_the-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.6.2/README.md` & `write_the-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
 
 -----
 
 **Table of Contents**
 
 - [Features](#Features)
 - [Requirements](#Requirements)
```

### Comparing `write_the-0.6.2/pyproject.toml` & `write_the-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typer[all]",
   "langchain",
+  "openai",
+  "tiktoken",
   "black",
   "libcst",
   "mkdocstrings[python]",
   "mkdocs-material"
 ]
 dynamic = ["version"]
```

### Comparing `write_the-0.6.2/PKG-INFO` & `write_the-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.6.2
+Version: 0.7.0
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: black
 Requires-Dist: langchain
 Requires-Dist: libcst
 Requires-Dist: mkdocs-material
 Requires-Dist: mkdocstrings[python]
+Requires-Dist: openai
+Requires-Dist: tiktoken
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # 🤖 write-the
 
 AI-powered Documentation and Test Generation Tool
 
@@ -33,15 +35,15 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
 
 -----
 
 **Table of Contents**
 
 - [Features](#Features)
 - [Requirements](#Requirements)
```

