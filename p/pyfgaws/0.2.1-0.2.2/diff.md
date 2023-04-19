# Comparing `tmp/pyfgaws-0.2.1.tar.gz` & `tmp/pyfgaws-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfgaws-0.2.1.tar", last modified: Wed Apr 19 14:01:02 2023, max compression
+gzip compressed data, was "pyfgaws-0.2.2.tar", last modified: Wed Apr 19 14:08:22 2023, max compression
```

## Comparing `pyfgaws-0.2.1.tar` & `pyfgaws-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.1/LICENSE
--rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.1/LICENSE
--rw-r--r--   0        0        0     2480 2022-06-14 04:40:34.280516 pyfgaws-0.2.1/README.md
--rw-r--r--   0        0        0       58 2022-06-02 20:36:50.013456 pyfgaws-0.2.1/pyfgaws/__init__.py
--rw-r--r--   0        0        0     1926 2023-03-10 00:49:14.418971 pyfgaws-0.2.1/pyfgaws/__main__.py
--rw-r--r--   0        0        0       81 2022-06-02 20:37:10.604331 pyfgaws-0.2.1/pyfgaws/batch/__init__.py
--rw-r--r--   0        0        0    21455 2023-03-10 00:49:14.419264 pyfgaws-0.2.1/pyfgaws/batch/api.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014080 pyfgaws-0.2.1/pyfgaws/batch/tests/__init__.py
--rw-r--r--   0        0        0     5802 2023-03-10 00:49:14.419509 pyfgaws-0.2.1/pyfgaws/batch/tests/test_api.py
--rw-r--r--   0        0        0    12325 2023-04-19 14:00:10.882084 pyfgaws-0.2.1/pyfgaws/batch/tools.py
--rw-r--r--   0        0        0     1137 2022-06-02 20:36:50.014555 pyfgaws-0.2.1/pyfgaws/core/__init__.py
--rw-r--r--   0        0        0     1295 2022-06-02 20:36:50.014672 pyfgaws-0.2.1/pyfgaws/core/logging.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014769 pyfgaws-0.2.1/pyfgaws/core/tests/__init__.py
--rw-r--r--   0        0        0      988 2022-06-02 20:36:50.014891 pyfgaws-0.2.1/pyfgaws/core/tests/test_core.py
--rw-r--r--   0        0        0      106 2022-06-02 20:36:50.015044 pyfgaws-0.2.1/pyfgaws/logs/__init__.py
--rw-r--r--   0        0        0     2309 2023-03-10 00:49:14.419917 pyfgaws-0.2.1/pyfgaws/logs/api.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.015263 pyfgaws-0.2.1/pyfgaws/logs/tests/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-10 00:49:14.420126 pyfgaws-0.2.1/pyfgaws/logs/tests/test_api.py
--rw-r--r--   0        0        0     1303 2023-03-10 00:49:14.420356 pyfgaws-0.2.1/pyfgaws/logs/tools.py
--rw-r--r--   0        0        0     1711 2023-03-10 00:49:14.420575 pyfgaws-0.2.1/pyfgaws/tests/__init__.py
--rw-r--r--   0        0        0     2132 2023-03-10 00:49:14.420771 pyfgaws-0.2.1/pyfgaws/tests/test_main.py
--rw-r--r--   0        0        0     1329 2023-04-19 14:00:43.396323 pyfgaws-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3620 2023-04-19 14:01:02.576784 pyfgaws-0.2.1/setup.py
--rw-r--r--   0        0        0     3706 2023-04-19 14:01:02.577065 pyfgaws-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2480 2022-06-14 04:40:34.280516 pyfgaws-0.2.2/README.md
+-rw-r--r--   0        0        0       58 2022-06-02 20:36:50.013456 pyfgaws-0.2.2/pyfgaws/__init__.py
+-rw-r--r--   0        0        0     1926 2023-03-10 00:49:14.418971 pyfgaws-0.2.2/pyfgaws/__main__.py
+-rw-r--r--   0        0        0       81 2022-06-02 20:37:10.604331 pyfgaws-0.2.2/pyfgaws/batch/__init__.py
+-rw-r--r--   0        0        0    21455 2023-03-10 00:49:14.419264 pyfgaws-0.2.2/pyfgaws/batch/api.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014080 pyfgaws-0.2.2/pyfgaws/batch/tests/__init__.py
+-rw-r--r--   0        0        0     5802 2023-03-10 00:49:14.419509 pyfgaws-0.2.2/pyfgaws/batch/tests/test_api.py
+-rw-r--r--   0        0        0    12329 2023-04-19 14:07:30.347014 pyfgaws-0.2.2/pyfgaws/batch/tools.py
+-rw-r--r--   0        0        0     1137 2022-06-02 20:36:50.014555 pyfgaws-0.2.2/pyfgaws/core/__init__.py
+-rw-r--r--   0        0        0     1295 2022-06-02 20:36:50.014672 pyfgaws-0.2.2/pyfgaws/core/logging.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014769 pyfgaws-0.2.2/pyfgaws/core/tests/__init__.py
+-rw-r--r--   0        0        0      988 2022-06-02 20:36:50.014891 pyfgaws-0.2.2/pyfgaws/core/tests/test_core.py
+-rw-r--r--   0        0        0      106 2022-06-02 20:36:50.015044 pyfgaws-0.2.2/pyfgaws/logs/__init__.py
+-rw-r--r--   0        0        0     2309 2023-03-10 00:49:14.419917 pyfgaws-0.2.2/pyfgaws/logs/api.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.015263 pyfgaws-0.2.2/pyfgaws/logs/tests/__init__.py
+-rw-r--r--   0        0        0     3165 2023-03-10 00:49:14.420126 pyfgaws-0.2.2/pyfgaws/logs/tests/test_api.py
+-rw-r--r--   0        0        0     1303 2023-03-10 00:49:14.420356 pyfgaws-0.2.2/pyfgaws/logs/tools.py
+-rw-r--r--   0        0        0     1711 2023-03-10 00:49:14.420575 pyfgaws-0.2.2/pyfgaws/tests/__init__.py
+-rw-r--r--   0        0        0     2132 2023-03-10 00:49:14.420771 pyfgaws-0.2.2/pyfgaws/tests/test_main.py
+-rw-r--r--   0        0        0     1329 2023-04-19 14:07:44.400893 pyfgaws-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3620 2023-04-19 14:08:22.220405 pyfgaws-0.2.2/setup.py
+-rw-r--r--   0        0        0     3706 2023-04-19 14:08:22.220697 pyfgaws-0.2.2/PKG-INFO
```

### Comparing `pyfgaws-0.2.1/LICENSE` & `pyfgaws-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/README.md` & `pyfgaws-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/__main__.py` & `pyfgaws-0.2.2/pyfgaws/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/batch/api.py` & `pyfgaws-0.2.2/pyfgaws/batch/api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/batch/tests/test_api.py` & `pyfgaws-0.2.2/pyfgaws/batch/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/batch/tools.py` & `pyfgaws-0.2.2/pyfgaws/batch/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                        `--queue` option
     """
     logger = logging.getLogger(__name__)
     assert (
         job_ids is not None or queue is not None
     ), "Either --job-ids or --queue must be specified"
     assert job_ids is None or queue is None, "Both --job-ids or --queue cannot be specified"
-    assert queue is None or not monitor_queue, "--queue must be used with --monitor-queue"
+    assert not monitor_queue or queue is not None, "--queue must be used with --monitor-queue"
 
     client: batch.Client = boto3.client(
         service_name="batch", region_name=region_name  # type: ignore
     )
 
     # get the list of batch jobs from job ids.  If using a queue, the job ids will be retrieved
     # later
```

### Comparing `pyfgaws-0.2.1/pyfgaws/core/__init__.py` & `pyfgaws-0.2.2/pyfgaws/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/core/logging.py` & `pyfgaws-0.2.2/pyfgaws/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/core/tests/test_core.py` & `pyfgaws-0.2.2/pyfgaws/core/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/logs/api.py` & `pyfgaws-0.2.2/pyfgaws/logs/api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/logs/tests/test_api.py` & `pyfgaws-0.2.2/pyfgaws/logs/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/logs/tools.py` & `pyfgaws-0.2.2/pyfgaws/logs/tools.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/tests/__init__.py` & `pyfgaws-0.2.2/pyfgaws/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyfgaws/tests/test_main.py` & `pyfgaws-0.2.2/pyfgaws/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.1/pyproject.toml` & `pyfgaws-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfgaws"
-version = "0.2.1"
+version = "0.2.2"
 description = "Tools and python libraries for working with AWS."
 authors = ["Nils Homer", "Tim Fennell"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fulcrumgenomics/pyfgaws"
 repository = "https://github.com/fulcrumgenomics/pyfgaws"
 keywords = ["aws", "bioinformatics"]
```

### Comparing `pyfgaws-0.2.1/setup.py` & `pyfgaws-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'namegenerator>=1.0.6,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['fgaws-tools = pyfgaws.__main__:main']}
 
 setup_kwargs = {
     'name': 'pyfgaws',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Tools and python libraries for working with AWS.',
     'long_description': '\n[![Language][language-badge]][language-link]\n[![Code Style][code-style-badge]][code-style-link]\n[![Type Checked][type-checking-badge]][type-checking-link]\n[![PEP8][pep-8-badge]][pep-8-link]\n[![Code Coverage][code-coverage-badge]][code-coverage-link]\n[![License][license-badge]][license-link]\n\n---\n\n[![Python package][python-package-badge]][python-package-link]\n[![PyPI version][pypi-badge]][pypi-link]\n[![PyPI download total][pypi-downloads-badge]][pypi-downloads-link]\n\n---\n\n[language-badge]:       http://img.shields.io/badge/language-python-brightgreen.svg\n[language-link]:        http://www.python.org/\n[code-style-badge]:     https://img.shields.io/badge/code%20style-black-000000.svg\n[code-style-link]:      https://black.readthedocs.io/en/stable/ \n[type-checking-badge]:  http://www.mypy-lang.org/static/mypy_badge.svg\n[type-checking-link]:   http://mypy-lang.org/\n[pep-8-badge]:          https://img.shields.io/badge/code%20style-pep8-brightgreen.svg\n[pep-8-link]:           https://www.python.org/dev/peps/pep-0008/\n[code-coverage-badge]:  https://codecov.io/gh/fulcrumgenomics/pyfgaws/branch/main/graph/badge.svg\n[code-coverage-link]:   https://codecov.io/gh/fulcrumgenomics/pyfgaws\n[license-badge]:        http://img.shields.io/badge/license-MIT-blue.svg\n[license-link]:         https://github.com/fulcrumgenomics/pyfgaws/blob/main/LICENSE\n[python-package-badge]: https://github.com/fulcrumgenomics/pyfgaws/workflows/Python%20package/badge.svg\n[python-package-link]:  https://github.com/fulcrumgenomics/pyfgaws/actions?query=workflow%3A%22Python+package%22\n[pypi-badge]:           https://badge.fury.io/py/pyfgaws.svg\n[pypi-link]:            https://pypi.python.org/pypi/pyfgaws\n[pypi-downloads-badge]: https://img.shields.io/pypi/dm/pyfgaws\n[pypi-downloads-link]:  https://pypi.python.org/pypi/pyfgaws\n\n# pyfgaws\n\n`pip install pyfgaws`\n\n**Requires python 3.8**\n\n# Getting Setup\n\nConda is used to install a specific version of python and [poetry][poetry-link]\nwhich is then used to manage the python development environment.  If not already installed, install \n[miniconda from the latest platform-appropriate installer](miniconda-link). Then run:\n\n```\nconda create -n pyfgaws -c conda-forge -c bioconda --file conda-requirements.txt\n```\n\nThen activate the new environment and install the toolkit:\n\n```\nconda activate pyfgaws\npoetry install\n```\n\n[miniconda-link]: https://docs.conda.io/en/latest/miniconda.html\n[poetry-link]:    https://github.com/python-poetry/poetry\n',
     'author': 'Nils Homer',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fulcrumgenomics/pyfgaws',
```

### Comparing `pyfgaws-0.2.1/PKG-INFO` & `pyfgaws-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfgaws
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools and python libraries for working with AWS.
 Home-page: https://github.com/fulcrumgenomics/pyfgaws
 License: MIT
 Keywords: aws,bioinformatics
 Author: Nils Homer
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

