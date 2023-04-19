# Comparing `tmp/aga-0.9.0.tar.gz` & `tmp/aga-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aga-0.9.0.tar", max compression
+gzip compressed data, was "aga-0.9.1.tar", max compression
```

## Comparing `aga-0.9.0.tar` & `aga-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-10 06:03:46.975747 aga-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     4905 2022-09-10 06:03:46.975747 aga-0.9.0/README.md
--rw-r--r--   0        0        0     2174 2022-09-10 06:03:46.975747 aga-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      428 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/__init__.py
--rw-r--r--   0        0        0      623 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/checks.py
--rw-r--r--   0        0        0      136 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/cli/__init__.py
--rw-r--r--   0        0        0     8112 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/cli/app.py
--rw-r--r--   0        0        0      937 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/cli/ui.py
--rw-r--r--   0        0        0     9592 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/config.py
--rw-r--r--   0        0        0    27325 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/core.py
--rw-r--r--   0        0        0     4752 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/defaults.toml
--rw-r--r--   0        0        0     1548 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/gradescope/__init__.py
--rw-r--r--   0        0        0     4389 2022-09-10 06:03:46.975747 aga-0.9.0/src/aga/gradescope/into_zip.py
--rw-r--r--   0        0        0     1287 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/main.py
--rw-r--r--   0        0        0     5051 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/metadata.py
--rw-r--r--   0        0        0      177 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/resources/__init__.py
--rwxr-xr-x   0        0        0      125 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/resources/run_autograder
--rw-r--r--   0        0        0      878 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/resources/setup.py
--rw-r--r--   0        0        0      463 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/resources/setup.sh
--rw-r--r--   0        0        0     3438 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/gradescope/schema.py
--rw-r--r--   0        0        0     6879 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/loader.py
--rw-r--r--   0        0        0      540 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/prize.py
--rw-r--r--   0        0        0        0 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/py.typed
--rw-r--r--   0        0        0     9137 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/runner.py
--rw-r--r--   0        0        0     4527 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/score.py
--rw-r--r--   0        0        0     1109 2022-09-10 06:03:46.979747 aga-0.9.0/src/aga/util.py
--rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 aga-0.9.0/setup.py
--rw-r--r--   0        0        0     5748 1970-01-01 00:00:00.000000 aga-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-12 01:16:04.498031 aga-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     4905 2022-09-12 01:16:04.498031 aga-0.9.1/README.md
+-rw-r--r--   0        0        0     2174 2022-09-12 01:16:04.502032 aga-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      428 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/__init__.py
+-rw-r--r--   0        0        0      623 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/checks.py
+-rw-r--r--   0        0        0      136 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/cli/__init__.py
+-rw-r--r--   0        0        0     8112 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/cli/app.py
+-rw-r--r--   0        0        0      937 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/cli/ui.py
+-rw-r--r--   0        0        0     9592 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/config.py
+-rw-r--r--   0        0        0    27547 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/core.py
+-rw-r--r--   0        0        0     4752 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/defaults.toml
+-rw-r--r--   0        0        0     1548 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/__init__.py
+-rw-r--r--   0        0        0     4389 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/into_zip.py
+-rw-r--r--   0        0        0     1287 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/main.py
+-rw-r--r--   0        0        0     5051 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/metadata.py
+-rw-r--r--   0        0        0      177 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/resources/__init__.py
+-rwxr-xr-x   0        0        0      125 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/resources/run_autograder
+-rw-r--r--   0        0        0      878 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/resources/setup.py
+-rw-r--r--   0        0        0      463 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/resources/setup.sh
+-rw-r--r--   0        0        0     3438 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/gradescope/schema.py
+-rw-r--r--   0        0        0     6879 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/loader.py
+-rw-r--r--   0        0        0      540 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/prize.py
+-rw-r--r--   0        0        0        0 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/py.typed
+-rw-r--r--   0        0        0     9137 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/runner.py
+-rw-r--r--   0        0        0     4527 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/score.py
+-rw-r--r--   0        0        0     1109 2022-09-12 01:16:04.502032 aga-0.9.1/src/aga/util.py
+-rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 aga-0.9.1/setup.py
+-rw-r--r--   0        0        0     5748 1970-01-01 00:00:00.000000 aga-0.9.1/PKG-INFO
```

### Comparing `aga-0.9.0/LICENSE.md` & `aga-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/README.md` & `aga-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/pyproject.toml` & `aga-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aga"
-version = "0.9.0"
+version = "0.9.1"
 description = "aga grades assignments"
 authors = ["Riley Shahar <riley.shahar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nihilistkitten/aga"
 repository = "https://github.com/nihilistkitten/aga"
 documentation = "https://aga.readthedocs.io"
```

### Comparing `aga-0.9.0/src/aga/checks.py` & `aga-0.9.1/src/aga/checks.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/cli/app.py` & `aga-0.9.1/src/aga/cli/app.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/cli/ui.py` & `aga-0.9.1/src/aga/cli/ui.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/config.py` & `aga-0.9.1/src/aga/config.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/core.py` & `aga-0.9.1/src/aga/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import timedelta
 from itertools import product
 from typing import (
     Any,
     Callable,
+    Dict,
     Generic,
+    List,
     Optional,
+    Sequence,
     TypeVar,
-    Dict,
-    List,
     overload,
-    Sequence,
 )
 from unittest import TestCase, TestSuite
 from unittest.mock import patch
 
 from .checks import with_captured_stdout
 from .config import AgaConfig, AgaTestConfig
 from .score import Prize, ScoredPrize, ScoreInfo, compute_scores
@@ -215,15 +215,21 @@
         if isinstance(expected, str) and isinstance(got, str):
             diff_explanation = metadata.config.diff_explanation_msg
             diff = text_diff(got, expected)
         else:
             diff_explanation = ""
             diff = ""
 
-        self.assertEqual(
+        if isinstance(expected, float) and isinstance(got, (float, int)):
+            comparator = self.assertAlmostEqual  # type: ignore
+
+        else:
+            comparator = self.assertEqual  # type: ignore
+
+        comparator(  # type: ignore
             got,
             expected,
             msg=msg_format.format(
                 input=repr(self),
                 expected=repr(expected),
                 output=repr(got),
                 diff_explanation=diff_explanation,
```

### Comparing `aga-0.9.0/src/aga/defaults.toml` & `aga-0.9.1/src/aga/defaults.toml`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/gradescope/__init__.py` & `aga-0.9.1/src/aga/gradescope/__init__.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/gradescope/into_zip.py` & `aga-0.9.1/src/aga/gradescope/into_zip.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/gradescope/main.py` & `aga-0.9.1/src/aga/gradescope/main.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/gradescope/metadata.py` & `aga-0.9.1/src/aga/gradescope/metadata.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/gradescope/resources/setup.py` & `aga-0.9.1/src/aga/gradescope/resources/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 it from PyPI.
 """
 
 from setuptools import setup  # type: ignore
 
 setup(
     name="aga",
-    version="0.9.0",
+    version="0.9.1",
     install_requires=[
         "dataclasses-json >= 0.5.6",
         "dill >= 0.3.4",
         "gradescope-utils >= 0.4.0",
         "typer >= 0.4.0",
         "dacite >= ^1.6.0",
         "toml >= ^0.10.2",
```

### Comparing `aga-0.9.0/src/aga/gradescope/schema.py` & `aga-0.9.1/src/aga/gradescope/schema.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/loader.py` & `aga-0.9.1/src/aga/loader.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/prize.py` & `aga-0.9.1/src/aga/prize.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/runner.py` & `aga-0.9.1/src/aga/runner.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/score.py` & `aga-0.9.1/src/aga/score.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/src/aga/util.py` & `aga-0.9.1/src/aga/util.py`

 * *Files identical despite different names*

### Comparing `aga-0.9.0/setup.py` & `aga-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'types-toml>=0.10.8,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['aga = aga.cli:aga_app']}
 
 setup_kwargs = {
     'name': 'aga',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'aga grades assignments',
     'long_description': '<div align="center">\n\n# aga grades assignments\n\n[![tests](https://github.com/nihilistkitten/aga/workflows/tests/badge.svg)](https://github.com/nihilistkitten/aga/actions?workflow=tests)\n[![lints](https://github.com/nihilistkitten/aga/workflows/lints/badge.svg)](https://github.com/nihilistkitten/aga/actions?workflow=lints)\n[![Codecov](https://codecov.io/gh/nihilistkitten/aga/branch/main/graph/badge.svg)](https://codecov.io/gh/nihilistkitten/aga)\n[![PyPI](https://img.shields.io/pypi/v/aga.svg)](https://pypi.org/project/aga/)\n[![Read the Docs](https://readthedocs.org/projects/aga/badge/)](https://aga.readthedocs.io/)\n[![License](https://img.shields.io/github/license/nihilistkitten/aga)](https://choosealicense.com/licenses/mit/)\n\n</div>\n\n**aga** (**a**ga **g**rades **a**ssignments) is a tool for easily producing autograders for python programming assignments, originally developed for Reed College\'s CS1 course.\n\n## Motivation\n\nUnlike traditional software testing, where there is likely no _a priori_ known-correct implementation, there is always such an implementation (or one can be easily written by course staff) in homework grading. Therefore, applying traditional software testing frameworks to homework grading is limited. Relying on reference implementations (what aga calls _golden solutions_) has several benefits:\n\n1. Reliability: having a reference solution gives a second layer of confirmation for the correctness of expected outputs. Aga supports _golden tests_, which function as traditional unit tests of the golden solution.\n2. Test case generation: many complex test cases can easily be generated via the reference solution, instead of needing to work out the expected output by hand. Aga supports generating test cases from inputs without explcitly referring to an expected output, and supports collecting test cases from python generators.\n3. Property testing: unit testing libraries like [hypothesis](https://hypothesis.readthedocs.io) allow testing large sets of arbitrary inputs for certain properties, and identifying simple inputs which reproduce violations of those properties. This is traditionally unreliable, because identifying specific properties to test is difficult. In homework grading, the property can simply be "the input matches the golden solution\'s output." Support for hypothesis is a [long-term goal](https://github.com/nihilistkitten/aga/issues/32) of aga.\n\n## Installation\n\nInstall from pip:\n\n```bash\npip install aga\n```\n\nor with the python dependency manager of your choice (I like [poetry](https://github.com/python-poetry/poetry)), for example:\n\n```bash\ncurl -sSL https://install.python-poetry.org | python3 -\necho "cd into aga repo"\ncd aga\npoetry install && poetry shell\n```\n\n## Example\n\nIn `square.py` (or any python file), write:\n\n```python\nfrom aga import problem, test_case, test_cases\n\n@test_cases([-3, 100])\n@test_case(2, aga_expect=4)\n@test_case(-2, aga_expect=4)\n@problem()\ndef square(x: int) -> int:\n    """Square x."""\n    return x * x\n```\n\nThen run `aga gen square.py` from the directory with `square.py`. This will generate a ZIP file suitable for upload to Gradescope.\n\n## Usage\n\nAga relies on the notion of a _golden solution_ to a given problem which is known to be correct. The main work of the library is to compare the output of this golden solution on some family of test inputs against the output of a student submission. To that end, aga integrates with frontends: existing classroom software which allow submission of student code. Currently, only Gradescope is supported.\n\nTo use aga:\n\n1. Write a golden solution to some programming problem.\n2. Decorate this solution with the `problem` decorator.\n3. Decorate this problem with any number of `test_case` decorators, which take arbitrary positional or keyword arguments and pass them verbatim to the golden and submitted functions.\n4. Generate the autograder using the CLI: `aga gen <file_name>`.\n\nThe `test_case` decorator may optionally take a special keyword argument called `aga_expect`. This allows easy testing of the golden solution: aga will not successfully produce an autograder unless the golden solution\'s output matches the `aga_expect`. You should use these as sanity checks to ensure your golden solution is implemented correctly.\n\nFor more info, see the [tutorial](https://aga.readthedocs.io/en/stable/tutorial.html).\n\nFor complete documentation, including configuring problem and test case metadata, see the [API reference](https://aga.readthedocs.io/en/stable/reference.html).\n\nFor CLI documentation, run `aga --help`, or access the docs [online](https://aga.readthedocs.io/en/stable/cli.html).\n\n## Contributing\n\nBug reports, feature requests, and pull requests are all welcome. For details on our test suite, development environment, and more, see the [developer documentation](https://aga.readthedocs.io/en/stable/development.html).\n\n<!-- vim:set tw=0: -->\n',
     'author': 'Riley Shahar',
     'author_email': 'riley.shahar@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nihilistkitten/aga',
```

### Comparing `aga-0.9.0/PKG-INFO` & `aga-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aga
-Version: 0.9.0
+Version: 0.9.1
 Summary: aga grades assignments
 Home-page: https://github.com/nihilistkitten/aga
 License: MIT
 Author: Riley Shahar
 Author-email: riley.shahar@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

