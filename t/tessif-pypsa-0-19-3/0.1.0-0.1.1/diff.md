# Comparing `tmp/tessif_pypsa_0_19_3-0.1.0.tar.gz` & `tmp/tessif_pypsa_0_19_3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessif_pypsa_0_19_3-0.1.0.tar", max compression
+gzip compressed data, was "tessif_pypsa_0_19_3-0.1.1.tar", max compression
```

## Comparing `tessif_pypsa_0_19_3-0.1.0.tar` & `tessif_pypsa_0_19_3-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-02-28 15:29:39.811832 tessif_pypsa_0_19_3-0.1.0/LICENSE
--rw-r--r--   0        0        0     5814 2023-02-28 15:29:39.811832 tessif_pypsa_0_19_3-0.1.0/README.rst
--rw-r--r--   0        0        0     1597 2023-02-28 15:29:39.811832 tessif_pypsa_0_19_3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      202 2023-02-28 15:29:39.811832 tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/__init__.py
--rw-r--r--   0        0        0     1603 2023-02-28 15:29:39.811832 tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/optimize.py
--rw-r--r--   0        0        0    85337 2023-02-28 15:29:39.815832 tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/post_process.py
--rw-r--r--   0        0        0    65712 2023-02-28 15:29:39.815832 tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/transform.py
--rw-r--r--   0        0        0     6772 1970-01-01 00:00:00.000000 tessif_pypsa_0_19_3-0.1.0/setup.py
--rw-r--r--   0        0        0     6694 1970-01-01 00:00:00.000000 tessif_pypsa_0_19_3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-19 16:47:13.660583 tessif_pypsa_0_19_3-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5814 2023-04-19 16:47:13.660583 tessif_pypsa_0_19_3-0.1.1/README.rst
+-rw-r--r--   0        0        0     1597 2023-04-19 16:47:13.664583 tessif_pypsa_0_19_3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-19 16:47:13.664583 tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-19 16:47:13.664583 tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/optimize.py
+-rw-r--r--   0        0        0    85337 2023-04-19 16:47:13.664583 tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/post_process.py
+-rw-r--r--   0        0        0    65712 2023-04-19 16:47:13.664583 tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/transform.py
+-rw-r--r--   0        0        0     6772 1970-01-01 00:00:00.000000 tessif_pypsa_0_19_3-0.1.1/setup.py
+-rw-r--r--   0        0        0     6694 1970-01-01 00:00:00.000000 tessif_pypsa_0_19_3-0.1.1/PKG-INFO
```

### Comparing `tessif_pypsa_0_19_3-0.1.0/LICENSE` & `tessif_pypsa_0_19_3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tessif_pypsa_0_19_3-0.1.0/README.rst` & `tessif_pypsa_0_19_3-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `tessif_pypsa_0_19_3-0.1.0/pyproject.toml` & `tessif_pypsa_0_19_3-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tessif-pypsa-0-19-3"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tessif-Plugin for providing pypsa version 0.19.3 support."
 authors = ["Mathias Ammon <tz3ma.coding@use.startmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/tZ3ma/tessif_pypsa_0_19_3"
 homepage = "https://github.com/tZ3ma/tessif_pypsa_0_19_3"
 keywords = ["Tessif", "Tessif-PyPSA", "ESSMOS", "optimization", "energy supply system modelling"]
```

### Comparing `tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/optimize.py` & `tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/optimize.py`

 * *Files identical despite different names*

### Comparing `tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/post_process.py` & `tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/post_process.py`

 * *Files identical despite different names*

### Comparing `tessif_pypsa_0_19_3-0.1.0/src/tessif_pypsa_0_19_3/transform.py` & `tessif_pypsa_0_19_3-0.1.1/src/tessif_pypsa_0_19_3/transform.py`

 * *Files identical despite different names*

### Comparing `tessif_pypsa_0_19_3-0.1.0/setup.py` & `tessif_pypsa_0_19_3-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyomo<6.0.0', 'pypsa==0.19.3', 'tessif>=0.0.24']
 
 setup_kwargs = {
     'name': 'tessif-pypsa-0-19-3',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Tessif-Plugin for providing pypsa version 0.19.3 support.',
     'long_description': 'tessif-pypsa-0-19-3\n====================================================================================================\n\n|PyPI| |Python Version| |License| |Status|\n\n|Stable Release| |Develop Release|\n\n|Read the Docs| |Tests| |Safety| |Pylinting| |Flake8 Linting| |Pre-Commit|\n\n|Codecov| |Codacy| |Codeclimate| |Scrutinizer|\n\n|pre-commit| |Black| |Pylint| |Flake8|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/tessif-pypsa-0-19-3.svg\n   :target: https://pypi.org/project/tessif-pypsa-0-19-3/\n   :alt: PyPI\n\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/tessif-pypsa-0-19-3\n   :target: https://pypi.org/project/tessif-pypsa-0-19-3\n   :alt: Python Version\n\n.. |License| image:: https://img.shields.io/pypi/l/tessif-pypsa-0-19-3\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n\n.. |Status| image:: https://badgen.net/badge/status/alpha/d8624d\n   :target: https://pypi.org/project/tessif-pypsa-0-19-3/\n   :alt: Status\n\n.. |Stable Release| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Stable-PyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Stable-PyPI-Release\n   :alt: Stable PyPI Release Workflow Status\n\n.. |Develop Release| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Develop-TestPyPI-Release/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Develop-TestPyPI-Release\n   :alt: Develop TestPyPI Release Workflow Status\n\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/tessif-pypsa-0-19-3/latest.svg?label=Read%20the%20Docs\n   :target: https://tessif-pypsa-0-19-3.readthedocs.io/\n   :alt: Read the documentation at https://tessif-pypsa-0-19-3.readthedocs.io/\n\n.. |Tests| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Tests-and-Coverage/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Tests-and-Coverage\n   :alt: Tests Workflow Status\n\n.. |Safety| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Safety/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Safety\n   :alt: Safety Workflow Status\n\n.. |Pylinting| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Pylinting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Pylinting\n   :alt: Pylint Workflow Status\n\n.. |Flake8 Linting| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Flake8-Linting/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Flake8-Linting\n   :alt: Flake8-Linting Workflow Status\n\n.. |Pre-Commit| image:: https://github.com/tZ3ma/tessif-pypsa-0-19-3/workflows/Pre-Commit/badge.svg\n   :target: https://github.com/tZ3ma/tessif-pypsa-0-19-3/actions?workflow=Pre-Commit\n   :alt: Pre-Commit Workflow Status\n\n.. |Codecov| image:: https://codecov.io/gh/tZ3ma/tessif-pypsa-0-19-3/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/tZ3ma/tessif-pypsa-0-19-3\n   :alt: Codecov\n\n.. |Codacy| image:: https://app.codacy.com/project/badge/Grade/b278433bb9224147a2e6231d783b62e4\n   :target: https://app.codacy.com/gh/tZ3ma/tessif-pypsa-0-19-3/dashboard\n   :alt: Codacy Code Quality Status\n\n.. |Codeclimate| image:: https://api.codeclimate.com/v1/badges/ff119252f0bb7f40aecb/maintainability\n   :target: https://codeclimate.com/github/tZ3ma/tessif-pypsa-0-19-3/maintainability\n   :alt: Maintainability\n\n.. |Scrutinizer| image:: https://scrutinizer-ci.com/g/tZ3ma/tessif-pypsa-0-19-3/badges/quality-score.png?b=main\n   :target: https://scrutinizer-ci.com/g/tZ3ma/tessif-pypsa-0-19-3/\n   :alt: Scrutinizer Code Quality\n\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. |Pylint| image:: https://img.shields.io/badge/linting-pylint-yellowgreen\n   :target: https://github.com/PyCQA/pylint\n   :alt: Package uses pylint\n\n.. |Flake8| image:: https://img.shields.io/badge/linting-flake8-yellogreen\n   :target: https://github.com/pycqa/flake8\n   :alt: Package uses flake8\n\n\nTessif-Plugin for including the software-tool oemof version 4.4.\n\nInstallation\n------------\n\nPlease see the `Installation Guide`_ (`Github Repo Link`_) for details.\n\n\nUsage\n-----\n\nPlease see the `Worklow Reference <Workflow-Guide_>`_ (`Github Repo Link`_) for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_ (`Github Repo Link`_).\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_ (`Github Repo Link`_),\n*tessif-pypsa-0-19-3* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\nCredits\n-------\n\nThis project was created using the `Mathias Ammon <tZ3ma>`_ tweaked version of the\nHypermodern-Python_ project foundation proposed by `Claudio Jolowicz <cj>`_.\n\n.. _Hypermodern-Python: https://cjolowicz.github.io/posts/hypermodern-python-01-setup/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _cj: https://github.com/cjolowicz\n\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n\n.. _file an issue: https://github.com/tZ3ma/tessif-pypsa-0-19-3/issues\n.. _pip: https://pip.pypa.io/\n\n.. _tZ3ma: https://github.com/tZ3ma\n.. working on github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Installation Guide: docs/source/getting_started/installation.rst\n.. _Workflow-Guide: docs/source/developer_guide/workflows.rst\n\n.. _Github Repo Link: https://github.com/tZ3ma/tessif-pypsa-0-19-3\n',
     'author': 'Mathias Ammon',
     'author_email': 'tz3ma.coding@use.startmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tZ3ma/tessif_pypsa_0_19_3',
```

### Comparing `tessif_pypsa_0_19_3-0.1.0/PKG-INFO` & `tessif_pypsa_0_19_3-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tessif-pypsa-0-19-3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tessif-Plugin for providing pypsa version 0.19.3 support.
 Home-page: https://github.com/tZ3ma/tessif_pypsa_0_19_3
 License: MIT
 Keywords: Tessif,Tessif-PyPSA,ESSMOS,optimization,energy supply system modelling
 Author: Mathias Ammon
 Author-email: tz3ma.coding@use.startmail.com
 Requires-Python: >=3.8,<4.0
```

