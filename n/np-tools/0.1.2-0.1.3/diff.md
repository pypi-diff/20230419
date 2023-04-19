# Comparing `tmp/np_tools-0.1.2.tar.gz` & `tmp/np_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.2.tar", last modified: Tue Apr 18 21:31:18 2023, max compression
+gzip compressed data, was "np_tools-0.1.3.tar", last modified: Wed Apr 19 21:45:17 2023, max compression
```

## Comparing `np_tools-0.1.2.tar` & `np_tools-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.2/README.md
--rw-r--r--   0        0        0     2344 2023-04-18 21:31:18.505373 np_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      238 2023-04-18 21:29:53.450239 np_tools-0.1.2/src/np_tools/__init__.py
--rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.2/src/np_tools/config.py
--rw-r--r--   0        0        0     4195 2023-04-18 21:29:53.558658 np_tools-0.1.2/src/np_tools/remote.py
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 np_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.3/README.md
+-rw-r--r--   0        0        0     2417 2023-04-19 21:45:17.183930 np_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.3/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.3/src/np_tools/config.py
+-rw-r--r--   0        0        0     8654 2023-04-19 21:43:54.151453 np_tools-0.1.3/src/np_tools/openephys.py
+-rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.3/src/np_tools/remote.py
+-rw-r--r--   0        0        0     2811 2023-04-19 20:43:03.942122 np_tools-0.1.3/src/np_tools/tools.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 np_tools-0.1.3/PKG-INFO
```

### Comparing `np_tools-0.1.2/pyproject.toml` & `np_tools-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.pdm.scripts]
-ruff = "ruff --fix src"
+ruff = "ruff check src --fix-only"
 blue = "blue src"
 pytest = "pytest --cov"
 bump = "bump -p pyproject.toml"
 
 [tool.pdm.scripts.prebuild]
 composite = [
     "blue",
@@ -35,14 +35,15 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [tool.ruff]
 ignore-init-module-imports = true
+line-length = 79
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--doctest-modules",
 ]
 doctest_optionflags = [
@@ -59,31 +60,35 @@
 source = [
     "src",
 ]
 
 [tool.coverage.run]
 branch = true
 source = [
-    "np_tools",
+    "src",
+]
+omit = [
+    "*__init__*",
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.2"
+version = "0.1.3"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "fabric>=3.0.0",
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
+    "black>=22.1.0",
 ]
 requires-python = ">=3.7,<4"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `np_tools-0.1.2/src/np_tools/remote.py` & `np_tools-0.1.3/src/np_tools/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tools for running commands via ssh on remote hosts.
 """
 from __future__ import annotations
 
+
 import doctest
 import subprocess
 import sys
 from typing import Any
 
 import fabric
 import np_config
```

### Comparing `np_tools-0.1.2/PKG-INFO` & `np_tools-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Repository, https://github.com/AllenInstitute/np_tools
 Project-URL: Bug tracker, https://github.com/AllenInstitute/np_tools/issues
 Requires-Python: <4,>=3.7
 Requires-Dist: fabric>=3.0.0
 Requires-Dist: np-config>=0.4.17
 Requires-Dist: np-logging>=0.5.1
+Requires-Dist: black>=22.1.0
 Requires-Dist: blue>=0.9.1; extra == "dev"
 Requires-Dist: pytest>=7.2.2; extra == "dev"
 Requires-Dist: mypy>=1.1.1; extra == "dev"
 Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: bump>=1.3.2; extra == "dev"
```

