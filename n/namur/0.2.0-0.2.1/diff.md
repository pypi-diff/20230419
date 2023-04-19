# Comparing `tmp/namur-0.2.0.tar.gz` & `tmp/namur-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namur-0.2.0.tar", max compression
+gzip compressed data, was "namur-0.2.1.tar", max compression
```

## Comparing `namur-0.2.0.tar` & `namur-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-13 16:47:34.221371 namur-0.2.0/LICENSE
--rw-r--r--   0        0        0     8089 2023-03-13 16:47:34.221371 namur-0.2.0/README.md
--rw-r--r--   0        0        0      416 2023-03-13 16:47:34.221371 namur-0.2.0/namur/__init__.py
--rw-r--r--   0        0        0      477 2023-03-13 16:47:34.221371 namur-0.2.0/namur/exceptions.py
--rw-r--r--   0        0        0     1330 2023-03-13 16:47:34.221371 namur-0.2.0/namur/models.py
--rw-r--r--   0        0        0     5949 2023-03-13 16:47:34.221371 namur-0.2.0/namur/namur.py
--rw-r--r--   0        0        0        0 2023-03-13 16:47:34.221371 namur-0.2.0/namur/py.typed
--rw-r--r--   0        0        0     3794 2023-03-13 16:47:47.837504 namur-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9599 1970-01-01 00:00:00.000000 namur-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-19 10:56:14.412161 namur-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8059 2023-04-19 10:56:14.412161 namur-0.2.1/README.md
+-rw-r--r--   0        0        0      416 2023-04-19 10:56:14.416161 namur-0.2.1/namur/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-19 10:56:14.416161 namur-0.2.1/namur/exceptions.py
+-rw-r--r--   0        0        0     1330 2023-04-19 10:56:14.416161 namur-0.2.1/namur/models.py
+-rw-r--r--   0        0        0     5949 2023-04-19 10:56:14.416161 namur-0.2.1/namur/namur.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:56:14.416161 namur-0.2.1/namur/py.typed
+-rw-r--r--   0        0        0     3827 2023-04-19 10:56:28.452284 namur-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9569 1970-01-01 00:00:00.000000 namur-0.2.1/PKG-INFO
```

### Comparing `namur-0.2.0/LICENSE` & `namur-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `namur-0.2.0/README.md` & `namur-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![GitHub Release][releases-shield]][releases]
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
-[![Forks][forks-shield]][forks-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
@@ -194,16 +194,16 @@
 [build-url]: https://github.com/klaasnicolaas/python-namur/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-namur/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-namur/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-namur.svg
 [commits-url]: https://github.com/klaasnicolaas/python-namur/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-namur/branch/main/graph/badge.svg?token=AMVI2EVPR0
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-namur
-[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/python-namur.svg
-[forks-url]: https://github.com/klaasnicolaas/python-namur/network/members
+[downloads-shield]: https://img.shields.io/pypi/dm/namur
+[downloads-url]: https://pypistats.org/packages/namur
 [issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-namur.svg
 [issues-url]: https://github.com/klaasnicolaas/python-namur/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-namur.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-namur.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/4beb1bcd3473c5344432/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-namur/maintainability
```

### Comparing `namur-0.2.0/namur/models.py` & `namur-0.2.1/namur/models.py`

 * *Files identical despite different names*

### Comparing `namur-0.2.0/namur/namur.py` & `namur-0.2.1/namur/namur.py`

 * *Files identical despite different names*

### Comparing `namur-0.2.0/pyproject.toml` & `namur-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "namur"
-version = "0.2.0"
+version = "0.2.1"
 description = "Asynchronous Python client providing Open Data information of Namur"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-namur"
 repository = "https://github.com/klaasnicolaas/python-namur"
@@ -25,37 +25,37 @@
     { include = "namur" }
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
-pytz = "^2022.7.1"
+pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-namur/issues"
 Changelog = "https://github.com/klaasnicolaas/python-namur/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.255"
+ruff = ">=0.0.243,<0.0.262"
 aresponses = "^2.1.6"
 black = ">=22.10,<24.0"
 blacken-docs = "^1.13.0"
 codespell = "^2.2.4"
 coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.2"
+mypy = ">=1.0,<1.3"
 pre-commit = "^3.1.1"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.17.0"
 pytest = "^7.2.2"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 yamllint = "^1.29.0"
 covdefaults = "^2.3.0"
-types-pytz = "^2022.7.1.2"
+types-pytz = ">=2022.7.1.2,<2024.0.0.0"
 
 [tool.black]
 target-version = ['py39']
 
 [tool.coverage.paths]
 source = ["namur"]
```

### Comparing `namur-0.2.0/PKG-INFO` & `namur-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namur
-Version: 0.2.0
+Version: 0.2.1
 Summary: Asynchronous Python client providing Open Data information of Namur
 Home-page: https://github.com/klaasnicolaas/python-namur
 License: MIT
 Keywords: open,data,platform,namur,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
+Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-namur/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-namur/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-namur
 Project-URL: Repository, https://github.com/klaasnicolaas/python-namur
 Description-Content-Type: text/markdown
 
@@ -39,15 +39,15 @@
 [![GitHub Release][releases-shield]][releases]
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
-[![Forks][forks-shield]][forks-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
 
 [![Code Quality][code-quality-shield]][code-quality]
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
@@ -228,16 +228,16 @@
 [build-url]: https://github.com/klaasnicolaas/python-namur/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-namur/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-namur/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-namur.svg
 [commits-url]: https://github.com/klaasnicolaas/python-namur/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-namur/branch/main/graph/badge.svg?token=AMVI2EVPR0
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-namur
-[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/python-namur.svg
-[forks-url]: https://github.com/klaasnicolaas/python-namur/network/members
+[downloads-shield]: https://img.shields.io/pypi/dm/namur
+[downloads-url]: https://pypistats.org/packages/namur
 [issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-namur.svg
 [issues-url]: https://github.com/klaasnicolaas/python-namur/issues
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-namur.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-namur.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/4beb1bcd3473c5344432/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-namur/maintainability
```

