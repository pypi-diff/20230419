# Comparing `tmp/iqm-cortex-cli-3.5.tar.gz` & `tmp/iqm-cortex-cli-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-3.5.tar", last modified: Thu Apr 13 08:39:21 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-3.6.tar", last modified: Wed Apr 19 12:19:06 2023, max compression
```

## Comparing `iqm-cortex-cli-3.5.tar` & `iqm-cortex-cli-3.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.303268 iqm-cortex-cli-3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.307268 iqm-cortex-cli-3.5/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    40133 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/src/cortex_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 08:39:21.000000 iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20504 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/circuit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_logout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_auth_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:39:21.311268 iqm-cortex-cli-3.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/qasm_qubit_placement.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/resources/valid_circuit_qasm_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 08:38:44.000000 iqm-cortex-cli-3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.289602 iqm-cortex-cli-3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.273602 iqm-cortex-cli-3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.277602 iqm-cortex-cli-3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-19 12:19:06.289602 iqm-cortex-cli-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.281602 iqm-cortex-cli-3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.273602 iqm-cortex-cli-3.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.281602 iqm-cortex-cli-3.6/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.281602 iqm-cortex-cli-3.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:19:06.289602 iqm-cortex-cli-3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.273602 iqm-cortex-cli-3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.285602 iqm-cortex-cli-3.6/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40133 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/src/cortex_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.285602 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 12:19:06.000000 iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.289602 iqm-cortex-cli-3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20504 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/circuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:19:06.289602 iqm-cortex-cli-3.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/qasm_qubit_placement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/valid_circuit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/valid_circuit.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/valid_circuit_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/resources/valid_circuit_qasm_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-19 12:18:16.000000 iqm-cortex-cli-3.6/tox.ini
```

### Comparing `iqm-cortex-cli-3.5/.github/workflows/ci.yml` & `iqm-cortex-cli-3.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/.github/workflows/publish.yml` & `iqm-cortex-cli-3.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-3.6/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/CHANGELOG.rst` & `iqm-cortex-cli-3.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 3.6
+============
+
+* Upgrade to IQMClient version 12.0 `#42 <https://github.com/iqm-finland/cortex-cli/pull/42>`_
+
 Version 3.5
 ===========
 
 * Allow user to update a temporary password in ``auth login`` command. `#41 <https://github.com/iqm-finland/cortex-cli/pull/41>`_
 
 Version 3.4
 ===========
```

### Comparing `iqm-cortex-cli-3.5/DEVELOPMENT.rst` & `iqm-cortex-cli-3.6/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/LICENSE.rst` & `iqm-cortex-cli-3.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/PKG-INFO` & `iqm-cortex-cli-3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 3.5
+Version: 3.6
 Summary: CLI for executing quantum circuits
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-3.5/README.rst` & `iqm-cortex-cli-3.6/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/Makefile` & `iqm-cortex-cli-3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_static/images/favicon.ico` & `iqm-cortex-cli-3.6/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_static/images/logo.png` & `iqm-cortex-cli-3.6/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-3.6/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-3.6/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_templates/page.html` & `iqm-cortex-cli-3.6/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/_templates/versioning.html` & `iqm-cortex-cli-3.6/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/docs/conf.py` & `iqm-cortex-cli-3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/pyproject.toml` & `iqm-cortex-cli-3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 changelog = "https://github.com/iqm-finland/cortex-cli/blob/main/CHANGELOG.rst"
 
 [project.optional-dependencies]
 # Add here additional requirements for extra features, to install with:
 # `pip install iqm-cortex-cli[testing,docs,dev]`
 circuit = [
     "cirq-iqm >= 11.0, < 12.0",
-    "iqm-client >= 11.4, < 12.0"
+    "iqm-client >= 12.0, < 13.0"
 ]
 dev = [
     "tox == 3.25.1"
 ]
 testing = [
     "black == 22.10.0",
     "isort == 5.10.1",
```

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/__init__.py` & `iqm-cortex-cli-3.6/src/cortex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/auth.py` & `iqm-cortex-cli-3.6/src/cortex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/circuit.py` & `iqm-cortex-cli-3.6/src/cortex_cli/circuit.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-3.6/src/cortex_cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/models.py` & `iqm-cortex-cli-3.6/src/cortex_cli/models.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-3.6/src/cortex_cli/token_manager.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/cortex_cli/utils.py` & `iqm-cortex-cli-3.6/src/cortex_cli/utils.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 3.5
+Version: 3.6
 Summary: CLI for executing quantum circuits
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-3.5/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-3.6/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tag-from-pipeline.sh` & `iqm-cortex-cli-3.6/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/auth_test.py` & `iqm-cortex-cli-3.6/tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/circuit_test.py` & `iqm-cortex-cli-3.6/tests/circuit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         )
     verify(requests).post(
         iqm_server_url + '/jobs',
         json=ANY(dict),
         headers={'Expect': '100-Continue', 'User-Agent': expected_user_agent},
         timeout=ANY(int),
     )
-    verify(requests, times=2).get(
+    verify(requests, times=3).get(
         iqm_server_url + f'/jobs/{existing_run}',
         headers={'User-Agent': expected_user_agent},
         timeout=ANY(int),
     )
     unstub()
```

### Comparing `iqm-cortex-cli-3.5/tests/conftest.py` & `iqm-cortex-cli-3.6/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,17 +198,21 @@
     Prepare for job submission requests.
     """
     success_submit_result = {'id': str(existing_run)}
     success_submit_response = mock({'status_code': 201, 'text': json.dumps(success_submit_result)})
     when(success_submit_response).json().thenReturn(success_submit_result)
     when(requests).post(f'{iqm_server_url}/jobs', ...).thenReturn(success_submit_response)
 
-    running_result = {'status': 'pending', 'metadata': {'request': {'shots': 42, 'circuits': []}}}
-    running_response = mock({'status_code': 200, 'text': json.dumps(running_result)})
-    when(running_response).json().thenReturn(running_result)
+    running_result = {'status': 'pending compilation', 'metadata': {'request': {'shots': 42, 'circuits': []}}}
+    pending_compilation_response = mock({'status_code': 200, 'text': json.dumps(running_result)})
+    when(pending_compilation_response).json().thenReturn(running_result)
+
+    running_result['status'] = 'pending execution'
+    pending_execution_response = mock({'status_code': 200, 'text': json.dumps(running_result)})
+    when(pending_execution_response).json().thenReturn(running_result)
 
     if valid_circuit_qasm_result_file is not None:
         with open(valid_circuit_qasm_result_file, 'r', encoding='utf-8') as file:
             success_get_result = json.loads(file.read())
     else:
         success_get_result = {
             'status': 'ready',
@@ -221,17 +225,17 @@
                 },
                 'calibration_set_id': str(calibration_set_id) if calibration_set_id is not None else None,
             },
         }
     success_get_response = mock({'status_code': 200, 'text': json.dumps(success_get_result)})
     when(success_get_response).json().thenReturn(success_get_result)
 
-    when(requests).get(f'{iqm_server_url}/jobs/{existing_run}', ...).thenReturn(running_response).thenReturn(
-        success_get_response
-    )
+    when(requests).get(f'{iqm_server_url}/jobs/{existing_run}', ...).thenReturn(
+        pending_compilation_response
+    ).thenReturn(pending_execution_response).thenReturn(success_get_response)
 
 
 def expect_token_is_valid(token: str, result: bool = True):
     """
     Prepare for token_is_valid call
     """
     when(auth).token_is_valid(token).thenReturn(result)
```

### Comparing `iqm-cortex-cli-3.5/tests/cortex_cli_auth_login_test.py` & `iqm-cortex-cli-3.6/tests/cortex_cli_auth_login_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/cortex_cli_auth_logout_test.py` & `iqm-cortex-cli-3.6/tests/cortex_cli_auth_logout_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/cortex_cli_auth_status_test.py` & `iqm-cortex-cli-3.6/tests/cortex_cli_auth_status_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/cortex_cli_init_test.py` & `iqm-cortex-cli-3.6/tests/cortex_cli_init_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/cortex_cli_test.py` & `iqm-cortex-cli-3.6/tests/cortex_cli_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/resources/tokens.json` & `iqm-cortex-cli-3.6/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/resources/valid_circuit_2.json` & `iqm-cortex-cli-3.6/tests/resources/valid_circuit_2.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/resources/valid_circuit_qasm_result.json` & `iqm-cortex-cli-3.6/tests/resources/valid_circuit_qasm_result.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tests/token_manager_test.py` & `iqm-cortex-cli-3.6/tests/token_manager_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-3.5/tox.ini` & `iqm-cortex-cli-3.6/tox.ini`

 * *Files identical despite different names*

