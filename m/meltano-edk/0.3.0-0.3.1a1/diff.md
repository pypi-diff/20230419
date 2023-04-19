# Comparing `tmp/meltano_edk-0.3.0.tar.gz` & `tmp/meltano_edk-0.3.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano_edk-0.3.0.tar", max compression
+gzip compressed data, was "meltano_edk-0.3.1a1.tar", max compression
```

## Comparing `meltano_edk-0.3.0.tar` & `meltano_edk-0.3.1a1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/LICENSE
--rw-r--r--   0        0        0     1617 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/README.md
--rw-r--r--   0        0        0       45 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/__init__.py
--rw-r--r--   0        0        0     4534 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/extension.py
--rw-r--r--   0        0        0     4780 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/logging.py
--rw-r--r--   0        0        0      904 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/models.py
--rw-r--r--   0        0        0     5357 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/process.py
--rw-r--r--   0        0        0      128 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/edk/types.py
--rw-r--r--   0        0        0        0 2023-02-09 22:25:12.028794 meltano_edk-0.3.0/meltano/py.typed
--rw-r--r--   0        0        0     2659 2023-02-09 22:25:32.461160 meltano_edk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2689 1970-01-01 00:00:00.000000 meltano_edk-0.3.0/setup.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 meltano_edk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/README.md
+-rw-r--r--   0        0        0       45 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/__init__.py
+-rw-r--r--   0        0        0     4534 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/extension.py
+-rw-r--r--   0        0        0     4780 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/logging.py
+-rw-r--r--   0        0        0      904 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/models.py
+-rw-r--r--   0        0        0     5357 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/process.py
+-rw-r--r--   0        0        0      128 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/edk/types.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:20:25.078576 meltano_edk-0.3.1a1/meltano/py.typed
+-rw-r--r--   0        0        0     2654 2023-04-19 17:20:46.210496 meltano_edk-0.3.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 meltano_edk-0.3.1a1/PKG-INFO
```

### Comparing `meltano_edk-0.3.0/LICENSE` & `meltano_edk-0.3.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/README.md` & `meltano_edk-0.3.1a1/README.md`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/meltano/edk/extension.py` & `meltano_edk-0.3.1a1/meltano/edk/extension.py`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/meltano/edk/logging.py` & `meltano_edk-0.3.1a1/meltano/edk/logging.py`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/meltano/edk/models.py` & `meltano_edk-0.3.1a1/meltano/edk/models.py`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/meltano/edk/process.py` & `meltano_edk-0.3.1a1/meltano/edk/process.py`

 * *Files identical despite different names*

### Comparing `meltano_edk-0.3.0/pyproject.toml` & `meltano_edk-0.3.1a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano.edk"
-version = "0.3.0"
+version = "0.3.1-a.1"
 description = "A framework for building Meltano extensions"
 authors = ["Meltano Team and Contributors"]
 maintainers = ["Meltano Team and Contributors"]
 readme = "README.md"
 homepage = "https://meltano.com"
 repository = "https://github.com/meltano/edk"
 keywords = [
@@ -39,49 +39,49 @@
 "Slack" = "https://meltano.com/slack"
 "Youtube" = "https://www.youtube.com/meltano"
 
 
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7"
-structlog = "^21"
+structlog = ">=21,<24"
 PyYAML = "^6.0.0"
 pydantic = ">=1.9.0,<2"
 devtools = ">=0.9.0,<1"
 
 # Sphinx dependencies installed as optional 'docs' extras
 # https://github.com/readthedocs/readthedocs.org/issues/4912#issuecomment-664002569
 sphinx = {version = ">=4.5,<6.0", optional = true}
-sphinx-rtd-theme = {version = ">=0.5.2,<1.3.0", optional = true}
+furo = {version = ">=2022.12.7,<2024.0.0", optional = true}
 sphinx-copybutton = {version = ">=0.3.1,<0.6.0", optional = true}
-myst-parser = {version = ">=0.17.2,<0.19.0", optional = true}
+myst-parser = {version = ">=0.17.2,<1.1.0", optional = true}
 sphinx-autobuild = {version = "^2021.3.14", optional = true}
 
 [tool.poetry.extras]
 docs = [
     "sphinx",
-    "sphinx-rtd-theme",
+    "furo",
     "sphinx-copybutton",
     "myst-parser",
     "sphinx-autobuild",
 ]
 
 [tool.poetry.dev-dependencies]
-mock = "^5.0.1"
-pytest = "^7.2.1"
+mock = "^5.0.2"
+pytest = "^7.3.1"
 # Cookiecutter tests
-mypy = "^1.0"
-black = "^23.1"
+mypy = "^1.2"
+black = "^23.3"
 darglint = "^1.8.0"
 flake8 = "^3.9.0"
 flake8-annotations = "^2.9.1"
 flake8-docstrings = "^1.7.0"
 
 [tool.poetry.group.dev.dependencies]
-copier = "^6.2.0"
+copier = ">=6.2,<8.0"
 types-pyyaml = "^6.0.12.4"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "meltano/edk"
 known_first_party = ["meltano"]
```

### Comparing `meltano_edk-0.3.0/PKG-INFO` & `meltano_edk-0.3.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano-edk
-Version: 0.3.0
+Version: 0.3.1a1
 Summary: A framework for building Meltano extensions
 Home-page: https://meltano.com
 License: Apache 2.0
 Keywords: Meltano,Meltano Extension,Meltano EDK
 Author: Meltano Team and Contributors
 Maintainer: Meltano Team and Contributors
 Requires-Python: >=3.7,<3.12
@@ -25,21 +25,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: devtools (>=0.9.0,<1)
-Requires-Dist: myst-parser (>=0.17.2,<0.19.0) ; extra == "docs"
+Requires-Dist: furo (>=2022.12.7,<2024.0.0) ; extra == "docs"
+Requires-Dist: myst-parser (>=0.17.2,<1.1.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.9.0,<2)
 Requires-Dist: sphinx (>=4.5,<6.0) ; extra == "docs"
 Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.3.1,<0.6.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<1.3.0) ; extra == "docs"
-Requires-Dist: structlog (>=21,<22)
+Requires-Dist: structlog (>=21,<24)
 Project-URL: Changelog, https://github.com/meltano/edk/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/meltano/edk/issues
 Project-URL: Repository, https://github.com/meltano/edk
 Project-URL: Slack, https://meltano.com/slack
 Project-URL: Twitter, https://twitter.com/meltanodata/
 Project-URL: Youtube, https://www.youtube.com/meltano
 Description-Content-Type: text/markdown
```

