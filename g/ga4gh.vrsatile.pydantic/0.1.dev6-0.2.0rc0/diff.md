# Comparing `tmp/ga4gh.vrsatile.pydantic-0.1.dev6.tar.gz` & `tmp/ga4gh.vrsatile.pydantic-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga4gh.vrsatile.pydantic-0.1.dev6.tar", last modified: Tue Dec 13 16:59:38 2022, max compression
+gzip compressed data, was "ga4gh.vrsatile.pydantic-0.2.0rc0.tar", last modified: Wed Apr 19 13:54:03 2023, max compression
```

## Comparing `ga4gh.vrsatile.pydantic-0.1.dev6.tar` & `ga4gh.vrsatile.pydantic-0.2.0rc0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/core_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrs_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrsatile_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.652814 ga4gh.vrsatile.pydantic-0.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-19 13:54:03.652814 ga4gh.vrsatile.pydantic-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-19 13:54:03.652814 ga4gh.vrsatile.pydantic-0.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.648814 ga4gh.vrsatile.pydantic-0.2.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.648814 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.648814 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.652814 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/pydantic/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/pydantic/vrs_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-19 13:53:53.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh/vrsatile/pydantic/vrsatile_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:54:03.652814 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 13:54:03.000000 ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/top_level.txt
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev6/LICENSE` & `ga4gh.vrsatile.pydantic-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev6/PKG-INFO` & `ga4gh.vrsatile.pydantic-0.2.0rc0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.vrsatile.pydantic
-Version: 0.1.dev6
+Version: 0.2.0rc0
 Summary: "Translation of the GA4GH VRS and VRSATILE Schemas to a Pydantic data model"
 Home-page: https://github.com/ga4gh/vrs-pydantic
 Author: Alex H. Wagner
 Author-email: alex.wagner@nationwidechildrens.org
 Keywords: bioinformatics,ga4gh,genomics,hgvs,spdi,variation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,34 +18,49 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vrsatile-pydantic
-Translation of the GA4GH [VRS v1.2.0](https://vrs.ga4gh.org/en/1.2.0) and [VRSATILE](https://vrsatile.readthedocs.io/en/latest/) schemas to a Pydantic data model
+Translation of the GA4GH [VRS](https://vrs.ga4gh.org/en/stable/) and [VRSATILE](https://vrsatile.readthedocs.io/en/latest/) schemas to a Pydantic data model
 
-# Developer instructions
+The ga4gh/vrsatile/pydantic repo depends on VRS and VRSATILE models, and therefore each ga4gh.vrsatile.pydantic package on PyPI uses a particular version of VRS and VRSATILE. The correspondences between the packages may be summarized as:
 
-To install vrstaile-pydantic:
+| ga4gh.vrsatile.pydantic branch | ga4gh.vrsatile.pydantic version | VRS version | VRSATILE version |
+| ---- | --- | --- | --- |
+| vrs-1.2 *(no longer being updated)* | 0.0.X | [1.2.X](https://github.com/ga4gh/vrs/tree/1.2) | [main](https://github.com/ga4gh/vrsatile/tree/main) |
+| metaschema-update | 0.1.X | [metaschema-update](https://github.com/ga4gh/vrs/tree/metaschema-update) | [metaschema-update](https://github.com/ga4gh/vrsatile/tree/metaschema-update)
+| main | 0.2.X | [1.3.X](https://github.com/ga4gh/vrs/tree/1.3) | [main](https://github.com/ga4gh/vrsatile/tree/main)
+
+## Installation
+
+vrsatile-pydantic is available via PyPI:
 ```commandline
 pip install ga4gh.vrsatile.pydantic
 ```
 
+## Developer Instructions
+
 Following are sections include instructions specifically for developers.
 
+### Installation
+
 For a development install, we recommend using Pipenv. See the
 [pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
 for direction on installing pipenv in your compute environment.
 
-Once installed, from the project root dir, just run:
+Once installed, clone the repo and initialize the environment:
 
 ```commandline
-pipenv lock
-pipenv sync
+git clone https://github.com/ga4gh/vrsatile-pydantic
+cd vrsatile-pydantic
+pipenv shell
+pipenv update
+pipenv install --dev
 ```
 
 ### Init coding style tests
 
 Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
 
 We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
@@ -59,15 +74,14 @@
 
 Before first commit run:
 
 ```commandline
 pre-commit install
 ```
 
-
 ### Running unit tests
 
 Running unit tests is as easy as pytest.
 
 ```commandline
-pipenv run pytest
+pipenv run pytest tests
 ```
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev6/setup.cfg` & `ga4gh.vrsatile.pydantic-0.2.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO` & `ga4gh.vrsatile.pydantic-0.2.0rc0/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.vrsatile.pydantic
-Version: 0.1.dev6
+Version: 0.2.0rc0
 Summary: "Translation of the GA4GH VRS and VRSATILE Schemas to a Pydantic data model"
 Home-page: https://github.com/ga4gh/vrs-pydantic
 Author: Alex H. Wagner
 Author-email: alex.wagner@nationwidechildrens.org
 Keywords: bioinformatics,ga4gh,genomics,hgvs,spdi,variation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,34 +18,49 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vrsatile-pydantic
-Translation of the GA4GH [VRS v1.2.0](https://vrs.ga4gh.org/en/1.2.0) and [VRSATILE](https://vrsatile.readthedocs.io/en/latest/) schemas to a Pydantic data model
+Translation of the GA4GH [VRS](https://vrs.ga4gh.org/en/stable/) and [VRSATILE](https://vrsatile.readthedocs.io/en/latest/) schemas to a Pydantic data model
 
-# Developer instructions
+The ga4gh/vrsatile/pydantic repo depends on VRS and VRSATILE models, and therefore each ga4gh.vrsatile.pydantic package on PyPI uses a particular version of VRS and VRSATILE. The correspondences between the packages may be summarized as:
 
-To install vrstaile-pydantic:
+| ga4gh.vrsatile.pydantic branch | ga4gh.vrsatile.pydantic version | VRS version | VRSATILE version |
+| ---- | --- | --- | --- |
+| vrs-1.2 *(no longer being updated)* | 0.0.X | [1.2.X](https://github.com/ga4gh/vrs/tree/1.2) | [main](https://github.com/ga4gh/vrsatile/tree/main) |
+| metaschema-update | 0.1.X | [metaschema-update](https://github.com/ga4gh/vrs/tree/metaschema-update) | [metaschema-update](https://github.com/ga4gh/vrsatile/tree/metaschema-update)
+| main | 0.2.X | [1.3.X](https://github.com/ga4gh/vrs/tree/1.3) | [main](https://github.com/ga4gh/vrsatile/tree/main)
+
+## Installation
+
+vrsatile-pydantic is available via PyPI:
 ```commandline
 pip install ga4gh.vrsatile.pydantic
 ```
 
+## Developer Instructions
+
 Following are sections include instructions specifically for developers.
 
+### Installation
+
 For a development install, we recommend using Pipenv. See the
 [pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
 for direction on installing pipenv in your compute environment.
 
-Once installed, from the project root dir, just run:
+Once installed, clone the repo and initialize the environment:
 
 ```commandline
-pipenv lock
-pipenv sync
+git clone https://github.com/ga4gh/vrsatile-pydantic
+cd vrsatile-pydantic
+pipenv shell
+pipenv update
+pipenv install --dev
 ```
 
 ### Init coding style tests
 
 Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
 
 We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
@@ -59,15 +74,14 @@
 
 Before first commit run:
 
 ```commandline
 pre-commit install
 ```
 
-
 ### Running unit tests
 
 Running unit tests is as easy as pytest.
 
 ```commandline
-pipenv run pytest
+pipenv run pytest tests
 ```
```

