# Comparing `tmp/otelib-0.2.0.tar.gz` & `tmp/otelib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otelib-0.2.0.tar", last modified: Wed Nov  9 14:34:51 2022, max compression
+gzip compressed data, was "otelib-0.3.0.tar", last modified: Wed Apr 19 07:44:55 2023, max compression
```

## Comparing `otelib-0.2.0.tar` & `otelib-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.242200 otelib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-09 14:31:08.000000 otelib-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-09 14:31:08.000000 otelib-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8739 2022-11-09 14:34:51.242200 otelib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-11-09 14:31:08.000000 otelib-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.238200 otelib-0.2.0/otelib/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-09 14:34:32.000000 otelib-0.2.0/otelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.242200 otelib-0.2.0/otelib/backends/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.242200 otelib-0.2.0/otelib/backends/python/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/dataresource.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/function.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/python/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.242200 otelib-0.2.0/otelib/backends/services/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/dataresource.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/function.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/services/transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/backends/strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-11-09 14:31:08.000000 otelib-0.2.0/otelib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 14:34:51.242200 otelib-0.2.0/otelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8739 2022-11-09 14:34:51.000000 otelib-0.2.0/otelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-11-09 14:34:51.000000 otelib-0.2.0/otelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 14:34:51.000000 otelib-0.2.0/otelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-09 14:34:51.000000 otelib-0.2.0/otelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-09 14:34:51.000000 otelib-0.2.0/otelib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-09 14:31:08.000000 otelib-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-09 14:31:08.000000 otelib-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-09 14:31:08.000000 otelib-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 14:34:51.242200 otelib-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-11-09 14:31:08.000000 otelib-0.2.0/setup.py
+-rw-r--r--   0        0        0      184 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/pull_request_template.md
+-rwxr-xr-x   0        0        0     3658 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/utils/wait_for_it.sh
+-rw-r--r--   0        0        0      675 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      437 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_automerge_dependabot.yml
+-rw-r--r--   0        0        0      479 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_cd_updated_master.yml
+-rw-r--r--   0        0        0      544 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0      920 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_dependabot.yml
+-rw-r--r--   0        0        0     3537 2023-04-19 07:44:10.777655 otelib-0.3.0/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0     3152 2023-04-19 07:44:10.777655 otelib-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1731 2023-04-19 07:44:10.777655 otelib-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8745 2023-04-19 07:44:52.569902 otelib-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1050 2023-04-19 07:44:10.777655 otelib-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8173 2023-04-19 07:44:10.777655 otelib-0.3.0/README.md
+-rw-r--r--   0        0        0     2438 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/demo-notebooks/execute.ipynb
+-rw-r--r--   0        0        0    11095 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/img/classes.svg
+-rw-r--r--   0        0        0     5473 2023-04-19 07:44:10.777655 otelib-0.3.0/docs/img/filters.drawio
+-rw-r--r--   0        0        0     6814 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/generic-pipeline.svg
+-rw-r--r--   0        0        0    43501 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/otelib-overview.png
+-rw-r--r--   0        0        0    22053 2023-04-19 07:44:10.781656 otelib-0.3.0/docs/img/pipeline.jpg
+-rw-r--r--   0        0        0      226 2023-04-19 07:44:53.029904 otelib-0.3.0/otelib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/__init__.py
+-rw-r--r--   0        0        0     2189 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/client.py
+-rw-r--r--   0        0        0     1960 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/factories.py
+-rw-r--r--   0        0        0      354 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/__init__.py
+-rw-r--r--   0        0        0     4911 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/base.py
+-rw-r--r--   0        0        0     1856 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/client.py
+-rw-r--r--   0        0        0     2678 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/dataresource.py
+-rw-r--r--   0        0        0      438 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/filter.py
+-rw-r--r--   0        0        0      461 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/function.py
+-rw-r--r--   0        0        0      445 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/mapping.py
+-rw-r--r--   0        0        0      487 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/python/transformation.py
+-rw-r--r--   0        0        0      354 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/__init__.py
+-rw-r--r--   0        0        0     4038 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/base.py
+-rw-r--r--   0        0        0      899 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/client.py
+-rw-r--r--   0        0        0      388 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/dataresource.py
+-rw-r--r--   0        0        0      288 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/filter.py
+-rw-r--r--   0        0        0      300 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/function.py
+-rw-r--r--   0        0        0      294 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/mapping.py
+-rw-r--r--   0        0        0      328 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/services/transformation.py
+-rw-r--r--   0        0        0     3827 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/strategies.py
+-rw-r--r--   0        0        0      582 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/backends/utils.py
+-rw-r--r--   0        0        0     2932 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/client.py
+-rw-r--r--   0        0        0     1260 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/exceptions.py
+-rw-r--r--   0        0        0      562 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/pipe.py
+-rw-r--r--   0        0        0      484 2023-04-19 07:44:10.781656 otelib-0.3.0/otelib/settings.py
+-rw-r--r--   0        0        0     1865 2023-04-19 07:44:10.781656 otelib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11856 2023-04-19 07:44:10.781656 otelib-0.3.0/test_pythonbackend.ipynb
+-rw-r--r--   0        0        0     8762 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/conftest.py
+-rw-r--r--   0        0        0     7010 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/test_abc.py
+-rw-r--r--   0        0        0     9783 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/strategies/test_all_strategies.py
+-rw-r--r--   0        0        0     5021 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/test_oteclient.py
+-rw-r--r--   0        0        0    10937 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/test_pipe.py
+-rw-r--r--   0        0        0     3904 2023-04-19 07:44:10.781656 otelib-0.3.0/tests/utils.py
+-rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 otelib-0.3.0/PKG-INFO
```

### Comparing `otelib-0.2.0/LICENSE` & `otelib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otelib-0.2.0/PKG-INFO` & `otelib-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: otelib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Open Translation Environment (OTE) REST API client library.
-Home-page: https://github.com/EMMC-ASBL/otelib
-Author: SINTEF
-Author-email: Team4.0@SINTEF.no
+Keywords: OTE,OTE-API
+Author-email: SINTEF <TEAM4.0@SINTEF.no>
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Requires-Dist: oteapi-core >=0.4.1,<1
+Requires-Dist: pre-commit ~=3.2 ; extra == "dev"
+Requires-Dist: pylint ~=2.17 ; extra == "dev"
+Requires-Dist: pytest ~=7.3 ; extra == "dev"
+Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
+Requires-Dist: requests-mock ~=1.10 ; extra == "dev"
+Project-URL: Changelog, https://github.com/EMMC-ASBL/otelib/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://EMMC-ASBL.github.io/otelib
+Project-URL: Home, https://github.com/EMMC-ASBL/otelib
+Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/otelib/issues
+Project-URL: Package, https://pypi.org/project/otelib
+Project-URL: Source, https://github.com/EMMC-ASBL/otelib
 Provides-Extra: dev
-License-File: LICENSE
 
 # OTELib
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![PyPI](https://img.shields.io/pypi/v/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![Codecov master](https://img.shields.io/codecov/c/github/EMMC-ASBL/otelib/master?logo=codecov)](https://app.codecov.io/gh/EMMC-ASBL/otelib)
 [![CI - Tests](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml/badge.svg?branch=master)](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml?query=branch%3Amaster)
@@ -164,7 +176,8 @@
 OTEAPI Core has been supported by the following projects:
 
 * **OntoTrans** (2020-2024) that receives funding from the European Union’s Horizon 2020 Research and Innovation Programme, under Grant Agreement no. 862136.
 
 * **VIPCOAT** (2021-2025) receives funding from the European Union’s Horizon 2020 Research and Innovation Programme - DT-NMBP-11-2020 Open Innovation Platform for Materials Modelling, under Grant Agreement no: 952903.
 
 * **OpenModel** (2021-2025) receives funding from the European Union’s Horizon 2020 Research and Innovation Programme - DT-NMBP-11-2020 Open Innovation Platform for Materials Modelling, under Grant Agreement no: 953167.
+
```

### Comparing `otelib-0.2.0/README.md` & `otelib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `otelib-0.2.0/otelib/backends/python/base.py` & `otelib-0.3.0/otelib/backends/python/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,144 +1,137 @@
 """Base class for strategies in the Python backend."""
 import json
-import os
+import warnings
+from copy import deepcopy
 from typing import TYPE_CHECKING
 from uuid import uuid4
 
-from oteapi.models import AttrDict
-from oteapi.models.genericconfig import GenericConfig
 from oteapi.plugins import create_strategy
 
 from otelib.backends.strategies import AbstractBaseStrategy
+from otelib.exceptions import ItemNotFoundInCache, PythonBackendException
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pathlib import Path
-    from typing import Optional
+    from typing import Any, Dict, Literal, Optional
 
-    from otelib.pipe import Pipe
-
-
-class Singleton:
-    """
-    Initializes a singleton object
-    """
-
-    def __new__(cls):
-        if not hasattr(cls, "instance"):
-            cls.instance = super(Singleton, cls).__new__(cls)
-        return cls.instance
-
-
-class Cache(Singleton, dict):
-    """
-    Singleton dictionary class. Can be cleared with the .clear() method
-    """
+    from oteapi.models import SessionUpdate
 
 
 class BasePythonStrategy(AbstractBaseStrategy):
     """Base class for strategies for the python backend.
 
     Parameters:
-        interpreter (str): Must be set to `"python"` or a `ValueError` is raised.
+        source (str): The Python interpreter to use in the local environment.
+            Currently only `python` is allowed.
 
     Attributes:
-        interpreter (str): This is always `"python"` for the Python backend.
+        interpreter (str): This is always `python` for the Python backend.
         input_pipe (Optional[Pipe]): An input pipeline.
 
     """
 
-    strategy_name: str
-    strategy_config: GenericConfig
-
-    cache = Cache()
+    def __init__(self, source: str, cache: "Optional[Dict[str, Any]]" = None) -> None:
+        super().__init__(source)
 
-    def __init__(
-        self,
-        interpreter: "Optional[str]" = None,
-    ) -> None:
-        """Initiates a strategy."""
-        if not interpreter:
-            raise ValueError("Interpreter (python) must be specified.")
-
-        self.interpreter: "Optional[str]" = interpreter
-
-        if interpreter != "python":
-            raise NotImplementedError(
-                "Only python interpreter supported for python backend"
+        self.interpreter: "Optional[str]" = source
+        if cache is None:
+            warnings.warn(f"No global cache used for Python backend strategy {self}")
+        self.cache = cache if cache is not None else {}
+
+        if self.interpreter != "python":
+            raise ValueError(
+                "Only the 'python' interpreter source is currently supported."
             )
 
-        self.input_pipe: "Optional[Pipe]" = None
-        self.id: "Optional[str]" = None  # pylint: disable=invalid-name
+    def create(self, **config) -> None:
+        session_id = config.pop("session_id", None)
+        data = self.strategy_config(**config)
 
-        # For debugging/testing
-        self.debug: bool = bool(os.getenv("OTELIB_DEBUG", ""))
-        self._session_id: "Optional[str]" = None
-
-    def create(self, **kwargs) -> None:
-        session_id = kwargs.pop("session_id", None)
-        data = self.strategy_config(**kwargs)
-
-        self.id = f"{self.strategy_name}-{str(uuid4())}"
-        self.id = self.id
-        self.cache[self.id] = data.json()
+        self.strategy_id = f"{self.strategy_name}-{uuid4()}"
+        self.cache[self.strategy_id] = data.json()
 
         if session_id:
-            session = self.cache[session_id]
+            if session_id not in self.cache:
+                raise ItemNotFoundInCache(
+                    "Session not found in cache, but given to create()", session_id
+                )
+
+            # Add strategy ID information to the session object.
             list_key = f"{self.strategy_name}_info"
-            if list_key in session:
-                session[list_key].extend([self.id])
+            if list_key in self.cache[session_id]:
+                if not isinstance(self.cache[session_id][list_key], list):
+                    raise TypeError(
+                        f"Expected type for {list_key!r} field in session to be a "
+                        f"list, found {type(self.cache[session_id][list_key])!r}."
+                    )
+                self.cache[session_id][list_key].append(self.strategy_id)
             else:
-                session[list_key] = [self.id]
+                self.cache[session_id][list_key] = [self.strategy_id]
 
     def fetch(self, session_id: str) -> bytes:
-        config = self.strategy_config(**json.loads(self.cache[self.id]))
-        session_data = None if not session_id else self.cache[session_id]
-        session_update = create_strategy(self.strategy_name, config)
-        session_update = session_update.get(session=session_data)
+        return self._run_strategy_method("get", session_id)
 
-        if session_update and session_id:
-            self.cache[session_id].update(session_update)
+    def initialize(self, session_id: str) -> bytes:
+        return self._run_strategy_method("initialize", session_id)
 
-        return bytes(AttrDict(**session_update).json(), encoding="utf-8")
+    def _create_session(self) -> str:
+        session_id = f"session-{uuid4()}"
+        self.cache[session_id] = {}
+        return session_id
+
+    def _run_strategy_method(
+        self, method_name: "Literal['get', 'initialize']", session_id: str
+    ) -> bytes:
+        """Generic implementation of the `fetch()` and `initialize()` methods.
 
-    def initialize(self, session_id: str) -> bytes:
-        config = self.strategy_config(**json.loads(self.cache[self.id]))
-        if session_id:
-            session_data = self.cache[session_id]
-        else:
-            session_data = None
+        This will run the `method_name` method on the strategy and return the
+        serialized session update object.
+
+        Parameters:
+            method_name: The name of the strategy's method to execute.
+            session_id: The ID of the session shared by the pipeline.
+
+        Returns:
+            The bytes-serialized output from the given strategy method.
+
+        """
+        if method_name not in ["get", "initialize"]:
+            raise PythonBackendException(
+                "method_name should be either 'get' or 'initialize'."
+            )
+
+        self._sanity_checks(session_id)
 
+        config = self.strategy_config(**json.loads(self.cache[self.strategy_id]))
         strategy = create_strategy(self.strategy_name, config)
-        session_update = strategy.initialize(session=session_data)
-        if session_update and session_id:
-            self.cache[session_id].update(session_update)
 
-        return bytes(AttrDict(**session_update).json(), encoding="utf-8")
+        if not hasattr(strategy, method_name):
+            raise PythonBackendException(
+                f"{method_name!r} is not a valid method for {strategy}"
+            )
+
+        session_update: "SessionUpdate" = getattr(strategy, method_name)(
+            session=deepcopy(self.cache[session_id])
+        )
 
-    def get(self, session_id: "Optional[str]" = None) -> bytes:
-        """Executes a pipeline.
+        self.cache[session_id].update(session_update)
 
-        This will call `initialize()` and then the `get()` method on the
-        input pipe, which in turn will call the `get()` method on the
-        strategy connected to its input and so forth until the beginning
-        of the pipeline.
+        return session_update.json().encode(encoding="utf-8")
 
-        Finally, `fetch()` is called and its output is returned.
+    def _sanity_checks(self, session_id: str) -> None:
+        """Perform sanity checks before running a strategy method.
 
         Parameters:
             session_id: The ID of the session shared by the pipeline.
 
-        Returns:
-            The output from `fetch()`.
-
         """
-        if session_id is None:
-            session_id = f"session-{str(uuid4())}"
-            self.cache[session_id] = {}
-
-        if self.debug:
-            self._session_id = session_id
-
-        self.initialize(session_id)
-        if self.input_pipe:
-            self.input_pipe.get(session_id)
-        return self.fetch(session_id)
+        if not self.strategy_id or self.strategy_id not in self.cache:
+            raise ItemNotFoundInCache(
+                "Run create() prior to initialize()", self.strategy_id
+            )
+
+        if session_id not in self.cache or not isinstance(
+            self.cache.get(session_id, {}), dict
+        ):
+            raise ItemNotFoundInCache(
+                "Did you run this method through get()?", session_id
+            )
```

### Comparing `otelib-0.2.0/otelib/backends/python/dataresource.py` & `otelib-0.3.0/otelib/backends/python/dataresource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 """Common strategy for Download, Parse and Resource strategies."""
 import json
+from copy import deepcopy
 from typing import TYPE_CHECKING
 
-from oteapi.models import AttrDict, ResourceConfig
+from oteapi.models import ResourceConfig
 from oteapi.plugins import create_strategy
 
 from otelib.backends.python.base import BasePythonStrategy
 
 if TYPE_CHECKING:  # pragma: no cover
-    from typing import Optional
+    from typing import Type
 
 
 class DataResource(BasePythonStrategy):
     """Context class for the data resource strategy interfaces for managing i/o
     operations."""
 
     strategy_name = "dataresource"
-    strategy_config = ResourceConfig
+    strategy_config: "Type[ResourceConfig]" = ResourceConfig
 
     def fetch(self, session_id: str) -> bytes:
-        resource_id = self.id
+        self._sanity_checks(session_id)
 
-        config = self.strategy_config(**json.loads(self.cache[resource_id]))
-        session_data = None if not session_id else self.cache[session_id]
+        config = self.strategy_config(**json.loads(self.cache[self.strategy_id]))
 
         if config.downloadUrl and config.mediaType:
             # Download strategy
             session_update = create_strategy("download", config).get(
-                session=session_data
+                session=deepcopy(self.cache[session_id])
             )
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            self.cache[session_id].update(session_update)
 
             # Parse strategy
-            session_update = create_strategy("parse", config).get(session=session_data)
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            session_update = create_strategy("parse", config).get(
+                session=deepcopy(self.cache[session_id])
+            )
+            self.cache[session_id].update(session_update)
 
         elif config.accessUrl and config.accessService:
             # Resource strategy
             session_update = create_strategy("resource", config).get(
-                session=session_data
+                session=deepcopy(self.cache[session_id])
             )
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            self.cache[session_id].update(session_update)
 
-        return bytes(AttrDict(**session_update).json(), encoding="utf-8")
+        return session_update.json().encode(encoding="utf-8")
 
     def initialize(self, session_id: str) -> bytes:
-        resource_id = self.id
+        self._sanity_checks(session_id)
 
-        config = self.strategy_config(**json.loads(self.cache[resource_id]))
-        if session_id:
-            session_data = self.cache[session_id]
-        else:
-            session_data = None
+        config = self.strategy_config(**json.loads(self.cache[self.strategy_id]))
 
         if config.downloadUrl and config.mediaType:
             # Download strategy
             session_update = create_strategy("download", config).initialize(
-                session=session_data
+                session=deepcopy(self.cache[session_id])
             )
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            self.cache[session_id].update(session_update)
 
             # Parse strategy
             session_update = create_strategy("parse", config).initialize(
-                session=session_data
+                session=deepcopy(self.cache[session_id])
             )
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            self.cache[session_id].update(session_update)
 
         elif config.accessUrl and config.accessService:
             # Resource strategy
             session_update = create_strategy("resource", config).initialize(
-                session=session_data
+                session=deepcopy(self.cache[session_id])
             )
-            if session_update and session_id:
-                self.cache[session_id].update(session_update)
+            self.cache[session_id].update(session_update)
 
-        return bytes(AttrDict(**session_update).json(), encoding="utf-8")
+        return session_update.json().encode(encoding="utf-8")
```

### Comparing `otelib-0.2.0/otelib/backends/services/client.py` & `otelib-0.3.0/otelib/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,102 @@
-"""Client for services backend."""
-from otelib.backends.services import (
-    DataResource,
-    Filter,
-    Function,
-    Mapping,
-    Transformation,
-)
+"""OTE Client."""
+from typing import TYPE_CHECKING
 
+from pydantic import AnyHttpUrl, ValidationError, parse_obj_as
 
-# pylint: disable=duplicate-code
-class OTEServiceClient:
-    """The Service version of the OTEClient object representing a remote OTE REST API.
+from otelib.backends.factories import client_factory
+from otelib.backends.utils import Backend, StrategyType
+
+if TYPE_CHECKING:  # pragma: no cover
+    from otelib.backends.strategies import AbstractBaseStrategy
+
+
+class OTEClient:
+    """The OTEClient object representing a remote OTE REST API.
 
     Parameters:
         url (str): The base URL of the OTEAPI Service.
 
     Attributes:
         url (str): The base URL of the OTEAPI Service.
 
     """
 
     def __init__(self, url: str) -> None:
-        """Initiates an OTEAPI Service client.
+        """Initialize an OTE Client.
+
+        Parameters:
+            url: The base URL of the OTE Service (or Python interpreter for local
+                OTEAPI Core usage).
+
+        """
+        try:
+            parse_obj_as(AnyHttpUrl, url)
+        except ValidationError:
+            backend = Backend.PYTHON
+        else:
+            backend = Backend.SERVICES
+
+        self._impl = client_factory(backend)(url)
+
+    @property
+    def url(self) -> str:
+        """The base URL of the OTE Service.
 
-        The `url` is the base URL of the OTEAPI Service.
+        This may also be the Python interpreter for local OTEAPI Core usage.
         """
-        self.url: str = url
+        return self._impl.source
 
-    def create_dataresource(self, **kwargs) -> DataResource:
+    def create_dataresource(self, **config) -> "AbstractBaseStrategy":
         """Create a new data resource.
 
-        Any given keyword arguments are passed on to the `create()` method.
+        Any given keyword arguments are passed on to the `create_strategy()` method.
 
         Returns:
             The newly created data resource.
 
         """
-        data_resource = DataResource(self.url)
-        data_resource.create(**kwargs)
-        return data_resource
+        return self._impl.create_strategy(StrategyType.DATARESOURCE, **config)
 
-    def create_transformation(self, **kwargs) -> Transformation:
-        """Create a new transformation.
+    def create_filter(self, **config) -> "AbstractBaseStrategy":
+        """Create a new filter.
 
-        Any given keyword arguments are passed on to the `create()` method.
+        Any given keyword arguments are passed on to the `create_strategy()` method.
 
         Returns:
-            The newly created transformation.
+            The newly created filter.
 
         """
-        transformation = Transformation(self.url)
-        transformation.create(**kwargs)
-        return transformation
+        return self._impl.create_strategy(StrategyType.FILTER, **config)
 
-    def create_filter(self, **kwargs) -> Filter:
-        """Create a new filter.
+    def create_function(self, **config) -> "AbstractBaseStrategy":
+        """Create a new function.
 
-        Any given keyword arguments are passed on to the `create()` method.
+        Any given keyword arguments are passed on to the `create_strategy()` method.
 
         Returns:
-            The newly created filter.
+            The newly created function.
 
         """
-        filter_ = Filter(self.url)
-        filter_.create(**kwargs)
-        return filter_
+        return self._impl.create_strategy(StrategyType.FUNCTION, **config)
 
-    def create_mapping(self, **kwargs) -> Mapping:
+    def create_mapping(self, **config) -> "AbstractBaseStrategy":
         """Create a new mapping.
 
-        Any given keyword arguments are passed on to the `create()` method.
+        Any given keyword arguments are passed on to the `create_strategy()` method.
 
         Returns:
             The newly created mapping.
 
         """
-        mapping = Mapping(self.url)
-        mapping.create(**kwargs)
-        return mapping
+        return self._impl.create_strategy(StrategyType.MAPPING, **config)
 
-    def create_function(self, **kwargs) -> Function:
-        """Create a new function.
+    def create_transformation(self, **config) -> "AbstractBaseStrategy":
+        """Create a new transformation.
 
-        Any given keyword arguments are passed on to the `create()` method.
+        Any given keyword arguments are passed on to the `create_strategy()` method.
 
         Returns:
-            The newly created function.
+            The newly created transformation.
 
         """
-        function_ = Function(self.url)
-        function_.create(**kwargs)
-        return function_
+        return self._impl.create_strategy(StrategyType.TRANSFORMATION, **config)
```

### Comparing `otelib-0.2.0/otelib/backends/strategies.py` & `otelib-0.3.0/otelib/backends/strategies.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 """Base API for backend strategies."""
+import os
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
+from otelib.backends.utils import StrategyType
 from otelib.pipe import Pipe
 
 if TYPE_CHECKING:  # pragma: no cover
-    from typing import Optional
+    from typing import Optional, Type, Union
+
+    from oteapi.models.genericconfig import GenericConfig
 
 
 class AbstractBaseStrategy(ABC):
     """The abstract base class defining the API for strategies."""
 
+    strategy_name: "Union[StrategyType, str]"
+    strategy_config: "Type[GenericConfig]"
+
+    def __init__(self, source: str) -> None:
+        """Initiates a strategy."""
+        if not source:
+            raise ValueError("source must be provided.")
+
+        self.input_pipe: "Optional[Pipe]" = None
+        self.strategy_id: str = ""
+        self.strategy_name = StrategyType(self.strategy_name)
+
+        # For debugging/testing
+        self.debug = bool(os.getenv("OTELIB_DEBUG", ""))
+        self._session_id: "Optional[str]" = None
+
     @abstractmethod
     def create(self, **kwargs) -> None:
         """Create a strategy.
 
         It should post the configuration for the created strategy.
         """
 
@@ -42,15 +62,14 @@
             session_id: The ID of the session shared by the pipeline.
 
         Returns:
             The response from the OTEAPI Service.
 
         """
 
-    @abstractmethod
     def get(self, session_id: "Optional[str]" = None) -> bytes:
         """Executes a pipeline.
 
         This will call `initialize()` and then the `get()` method on the
         input pipe, which in turn will call the `get()` method on the
         strategy connected to its input and so forth until the beginning
         of the pipeline.
@@ -60,28 +79,49 @@
         Parameters:
             session_id: The ID of the session shared by the pipeline.
 
         Returns:
             The output from `fetch()`.
 
         """
+        if session_id is None:
+            session_id = self._create_session()
+
+        if self.debug:
+            self._session_id = session_id
+
+        self.initialize(session_id)
+        if self.input_pipe:
+            self.input_pipe.get(session_id)
+        return self.fetch(session_id)
+
+    @abstractmethod
+    def _create_session(self) -> str:
+        """Create a new session.
+
+        This method should not be run by a user, hence it is "private".
+        The method is used within the `get()` method and allows a backend to customize
+        its session creation method.
+
+        Returns:
+            The newly created session's ID.
+
+        """
 
-    def _set_input(self, input_pipe: "Optional[Pipe]") -> None:
+    def _set_input(self, input_pipe: Pipe) -> None:
         """Used by `__rshift__` to set the input pipe.
 
         Parameters:
             input_pipe: A pipe representing the strategy that is "piped" into this
                 strategy.
 
         """
-        self.input_pipe = input_pipe  # pylint: disable=attribute-defined-outside-init
+        self.input_pipe = input_pipe
 
-    def __rshift__(
-        self, other: "AbstractBaseStrategy"
-    ) -> "AbstractBaseStrategy":  # type: ignore[override]
+    def __rshift__(self, other: "AbstractBaseStrategy") -> "AbstractBaseStrategy":
         """Implements strategy concatenation using the `>>` symbol.
 
         Parameters:
             other: The next strategy this one is "piping" into.
 
         Returns:
             The next strategy this one is "piped" into.
```

