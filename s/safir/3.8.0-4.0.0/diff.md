# Comparing `tmp/safir-3.8.0.tar.gz` & `tmp/safir-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-3.8.0.tar", last modified: Wed Mar 15 21:05:40 2023, max compression
+gzip compressed data, was "safir-4.0.0.tar", last modified: Wed Apr 19 16:56:55 2023, max compression
```

## Comparing `safir-3.8.0.tar` & `safir-4.0.0.tar`

### file list

```diff
@@ -1,120 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.854625 safir-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-15 21:05:28.000000 safir-3.8.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.842625 safir-3.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-15 21:05:28.000000 safir-3.8.0/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-15 21:05:28.000000 safir-3.8.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-15 21:05:28.000000 safir-3.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.842625 safir-3.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-15 21:05:28.000000 safir-3.8.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-15 21:05:28.000000 safir-3.8.0/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-15 21:05:28.000000 safir-3.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-15 21:05:28.000000 safir-3.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-03-15 21:05:28.000000 safir-3.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-15 21:05:28.000000 safir-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-15 21:05:28.000000 safir-3.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-15 21:05:40.854625 safir-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-15 21:05:28.000000 safir-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.842625 safir-3.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-15 21:05:28.000000 safir-3.8.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-15 21:05:28.000000 safir-3.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-03-15 21:05:28.000000 safir-3.8.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-15 21:05:28.000000 safir-3.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.842625 safir-3.8.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-03-15 21:05:28.000000 safir-3.8.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-15 21:05:28.000000 safir-3.8.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-15 21:05:28.000000 safir-3.8.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-15 21:05:28.000000 safir-3.8.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-15 21:05:28.000000 safir-3.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.846625 safir-3.8.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/gcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-03-15 21:05:28.000000 safir-3.8.0/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-03-15 21:05:28.000000 safir-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 21:05:40.854625 safir-3.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.838625 safir-3.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.846625 safir-3.8.0/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.850625 safir-3.8.0/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-15 21:05:28.000000 safir-3.8.0/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.850625 safir-3.8.0/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.850625 safir-3.8.0/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.850625 safir-3.8.0/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-15 21:05:29.000000 safir-3.8.0/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.846625 safir-3.8.0/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-15 21:05:40.000000 safir-3.8.0/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-15 21:05:40.000000 safir-3.8.0/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:05:40.000000 safir-3.8.0/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-15 21:05:40.000000 safir-3.8.0/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 21:05:40.000000 safir-3.8.0/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.850625 safir-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-15 21:05:29.000000 safir-3.8.0/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-15 21:05:29.000000 safir-3.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-03-15 21:05:29.000000 safir-3.8.0/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-15 21:05:29.000000 safir-3.8.0/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.854625 safir-3.8.0/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-15 21:05:29.000000 safir-3.8.0/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-15 21:05:29.000000 safir-3.8.0/tests/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-03-15 21:05:29.000000 safir-3.8.0/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-15 21:05:29.000000 safir-3.8.0/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.854625 safir-3.8.0/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-15 21:05:29.000000 safir-3.8.0/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-03-15 21:05:29.000000 safir-3.8.0/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-15 21:05:29.000000 safir-3.8.0/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-03-15 21:05:29.000000 safir-3.8.0/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-15 21:05:29.000000 safir-3.8.0/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.854625 safir-3.8.0/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-15 21:05:29.000000 safir-3.8.0/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-03-15 21:05:29.000000 safir-3.8.0/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:40.854625 safir-3.8.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:05:29.000000 safir-3.8.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-15 21:05:29.000000 safir-3.8.0/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-15 21:05:29.000000 safir-3.8.0/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-15 21:05:29.000000 safir-3.8.0/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-15 21:05:29.000000 safir-3.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.778174 safir-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 16:56:40.000000 safir-4.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 16:56:40.000000 safir-4.0.0/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 16:56:40.000000 safir-4.0.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 16:56:40.000000 safir-4.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-19 16:56:40.000000 safir-4.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-19 16:56:40.000000 safir-4.0.0/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-19 16:56:40.000000 safir-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-19 16:56:40.000000 safir-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-04-19 16:56:40.000000 safir-4.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 16:56:40.000000 safir-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 16:56:40.000000 safir-4.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-19 16:56:55.778174 safir-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-19 16:56:40.000000 safir-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-19 16:56:40.000000 safir-4.0.0/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-19 16:56:40.000000 safir-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-04-19 16:56:40.000000 safir-4.0.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-19 16:56:40.000000 safir-4.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 16:56:40.000000 safir-4.0.0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-19 16:56:40.000000 safir-4.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.754174 safir-4.0.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.758174 safir-4.0.0/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-19 16:56:40.000000 safir-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:56:55.778174 safir-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.746174 safir-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.770174 safir-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 16:56:40.000000 safir-4.0.0/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 16:56:40.000000 safir-4.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-19 16:56:40.000000 safir-4.0.0/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-19 16:56:40.000000 safir-4.0.0/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.770174 safir-4.0.0/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-19 16:56:40.000000 safir-4.0.0/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 16:56:40.000000 safir-4.0.0/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.746174 safir-4.0.0/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 16:56:40.000000 safir-4.0.0/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-19 16:56:40.000000 safir-4.0.0/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-19 16:56:40.000000 safir-4.0.0/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-19 16:56:40.000000 safir-4.0.0/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-19 16:56:40.000000 safir-4.0.0/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-19 16:56:40.000000 safir-4.0.0/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 16:56:40.000000 safir-4.0.0/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-19 16:56:40.000000 safir-4.0.0/tox.ini
```

### Comparing `safir-3.8.0/.github/workflows/ci.yaml` & `safir-4.0.0/.github/workflows/ci.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -22,29 +22,26 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
 
       - name: Run pre-commit
         uses: pre-commit/action@v3.0.0
 
   test:
 
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
-          - "3.8"
-          - "3.9"
-          - "3.10"
           - "3.11"
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Run tox
         uses: lsst-sqre/run-tox@v1
@@ -64,15 +61,15 @@
 
       - name: Install Graphviz
         run: sudo apt-get install graphviz
 
       - name: Run tox
         uses: lsst-sqre/run-tox@v1
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           tox-envs: "docs,docs-linkcheck"
 
       # Only attempt documentation uploads for tagged releases and pull
       # requests from ticket branches in the same repository.  This avoids
       # version clutter in the docs and failures when a PR doesn't have access
       # to secrets.
       - name: Upload to LSST the Docs
@@ -96,9 +93,9 @@
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v1
         with:
           pypi-token: ${{ secrets.PYPI_SQRE_ADMIN }}
-          python-version: "3.10"
+          python-version: "3.11"
           upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags/') }}
```

### Comparing `safir-3.8.0/.github/workflows/periodic.yaml` & `safir-4.0.0/.github/workflows/periodic.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 jobs:
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
-          - "3.8"
-          - "3.9"
-          - "3.10"
           - "3.11"
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Run tests in tox
         uses: lsst-sqre/run-tox@v1
@@ -40,15 +37,15 @@
 
       - name: Install Graphviz
         run: sudo apt-get install graphviz
 
       - name: Build docs in tox
         uses: lsst-sqre/run-tox@v1
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           tox-envs: "docs,docs-linkcheck"
           use-cache: false
 
   pypi:
     runs-on: ubuntu-latest
 
     steps:
@@ -56,9 +53,9 @@
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v1
         with:
           pypi-token: ""
-          python-version: "3.10"
+          python-version: "3.11"
           upload: false
```

### Comparing `safir-3.8.0/.gitignore` & `safir-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/.pre-commit-config.yaml` & `safir-4.0.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies:
           - toml
 
   - repo: https://github.com/ambv/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
-        args: [-l, '76', -t, py39]
+        args: [-l, '76', -t, py311]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
```

### Comparing `safir-3.8.0/CHANGELOG.md` & `safir-4.0.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,48 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.0.0 (2023-04-19)
+
+### Backwards-incompatible changes
+
+- Safir now requires a minimum Python version of 3.11.
+- `safir.pydantic.validate_exactly_one_of` is now a Pydantic root validator instead of an individual field validator, which simplifies how it should be called.
+- Custom Kubernetes objects are no longer copied before being stored in the Kubernetes mock by `create_namespaced_custom_object`, and no longer automatically get a `metadata.uid` value. This brings handling of custom objects in line with the behavior of other mocked `create_*` and `replace_*` APIs.
+- All objects stored in the Kubernetes mock will be modified to set `api_version`, `kind`, and (where appropriate) `namespace`. If any of those values are set in the object, they are checked for correctness and rejected with `AssertionError` if they don't match the API call and its parameters.
+- The mocked `create_*` Kubernetes APIs now use the name `body` for the parameter containing the API object, instead of using some other name specific to the kind of object. This fixes compatibility with the Python Kubernetes API that this class is mocking.
+
+### New features
+
+- The new `safir.redis.PydanticRedisStorage` class enables you to store Pydantic model objects in Redis.
+  A `safir.redis.EncryptedPydanticRedisStorage` class also encrypts data in Redis.
+  To use the `safir.redis` module, install Safir with the `redis` extra (i.e., `pip install safir[redis]`).
+- Add `safir.fastapi.ClientRequestError` base class for exceptions and the corresponding exception handler `safir.fastapi.client_request_error_handler`. These may be used together to raise structured exceptions and automatically transform them into structured HTTP errors with the correct HTTP status code and an error body compatible with `safir.models.ErrorModel` and FastAPI's own internally-generated errors.
+- Add `safir.slack.webhook.SlackWebException`, which is a child class of `safir.slack.webhook.SlackException` that knows how to capture and report details from an underlying HTTPX exception.
+- Add a `safir.testing.kubernetes.strip_none` helper function that makes it easier to compare Kubernetes objects against expected test data.
+- Add a `get_namespace_objects_for_test` method to the Kubernetes mock to retrieve all objects (of any kind) in a namespace.
+- Add a mock for the `list_nodes` Kubernetes API, which returns data set by a call to the new `set_nodes_for_test` method.
+- Add optional rudimentary namespace tracking to the Kubernetes mock. Namespaces can be created, deleted (which deletes all objects in the namespace), read, and listed. Explicit namespace creation remains optional; if an object is created in a namespace and that namespace does not exist, one will be implicitly created by the mock.
+- Add support for namespaced events (the older core API, not the new events API) to the Kubernetes mock. Newly-created pods with the default initial status post an event by default; otherwise, events must be created by calling the mocked `create_namespaced_event` API. The `list_namespaced_event` API supports watches with timeouts.
+- Add rudimentary support for `NetworkPolicy`, `ResourceQuota`, and `Service` objects to the Kubernetes mock.
+- Add a `safir.github` module for writing GitHub integrations with GidgetHub and Pydantic modeling. `safir.github.GitHubAppClientFactory` helps create authenticated clients for GitHub Apps and app installations. `safir.github.models` contains Pydantic models for GitHub v3 REST API resources. `safir.github.webhooks` contains Pydantic models for GitHub webhook payloads.
+
+### Bug fixes
+
+- Stop adding the `X-Auth-Request-User` header to the OpenAPI schema for routes that use `auth_dependency` or `auth_logger_dependency`.
+
+### Other changes
+
+- The `safir.testing.kubernetes.MockKubernetesApi` mock now has rudimentary API documentation for the Kubernetes APIs that it supports.
+- The documentation for running commands with `tox` has been updated for the new command-line syntax in tox v4.
+
 ## 3.8.0 (2023-03-15)
 
 ### New features
 
 - Add `safir.slack.webhook.SlackWebhookClient` and accompanying models to post a structured message to Slack via an incoming webhook. Add a `safir.slack.blockkit.SlackException` base class that can be used to create exceptions with supplemental metadata that can be sent to Slack as a formatted alert.
 - Add a FastAPI route class (`safir.slack.webhook.SlackRouteErrorHandler`) that reports all uncaught exceptions to Slack using an incoming webhook.
 - Add `safir.datetime.format_datetime_for_logging` to convert a `datetime` object into an easily human-readable representation.
@@ -132,15 +166,15 @@
 - When logging in JSON format, use `severity` instead of `level` for the log level for compatibility with Google Log Explorer.
 - In the FastAPI `logger_dependency`, add log information about the incoming requst in a format compatible with Google Log Explorer.
 
 ## 2.2.0 (2021-11-09)
 
 ### Bug fixes
 
-- Restore previous `http_client_dependency` behavior by enabling following redirects by default. This adjusts for the change of defaults in httpx 0.20.0.
+- Restore previous `http_client_dependency` behavior by enabling following redirects by default. This adjusts for the change of defaults in HTTPX 0.20.0.
 
 ## 2.1.1 (2021-10-29)
 
 ### Other changes
 
 - Require structlog 21.2.0 and adjust logger configuration of exception handling for the expectations of that version.
 
@@ -194,13 +228,13 @@
 - Fix duplicated log output when logging is configured multiple times.
 
 ## 0.1.0 (2020-02-26)
 
 ### New features
 
 - The first release of Safir featuring:
-  
+
   - `safir.http` for adding an `aiohttp.ClientSession` to your application.
   - `safir.logging` for configuring structlog loggers.
   - `safir.metadata` helps your gather and structure metadata about your application for publishing on metadata endpoints.
   - `safir.middleware` includes a logging middleware that adds a logger with bound context about the request to your Request object.
   - Documentation about these features and a tutorial for starting a new application with the `roundtable_aiohttp_bot` template.
```

### Comparing `safir-3.8.0/LICENSE` & `safir-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/PKG-INFO` & `safir-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 3.8.0
+Version: 4.0.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,33 +26,31 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://safir.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/safir
 Project-URL: Change log, https://safir.lsst.io/changelog.html
 Project-URL: Issue tracker, https://github.com/lsst-sqre/safir/issues
 Keywords: rubin,lsst
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: arq
 Provides-Extra: db
 Provides-Extra: dev
 Provides-Extra: gcs
 Provides-Extra: kubernetes
+Provides-Extra: redis
 License-File: LICENSE
 
 # Safir
 
 Safir is Rubin Observatory's library for building [FastAPI](https://fastapi.tiangolo.com/) services for the [Rubin Science Platform (Phalanx)](https://github.com/lsst-sqre/phalanx) and [Roundtable](https://github.com/lsst-sqre/roundtable) Kubernetes clusters.
 Safir is developed, maintained, and field tested by the SQuaRE team.
```

### Comparing `safir-3.8.0/README.md` & `safir-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/api.rst` & `safir-4.0.0/docs/api.rst`

 * *Files 23% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 .. automodapi:: safir.arq
    :include-all-objects:
 
 .. automodapi:: safir.asyncio
    :include-all-objects:
 
 .. automodapi:: safir.database
+   :include-all-objects:
 
 .. automodapi:: safir.datetime
+   :include-all-objects:
 
 .. automodapi:: safir.dependencies.arq
    :include-all-objects:
 
 .. automodapi:: safir.dependencies.db_session
    :include-all-objects:
 
@@ -26,17 +28,29 @@
 
 .. automodapi:: safir.dependencies.http_client
    :include-all-objects:
 
 .. automodapi:: safir.dependencies.logger
    :include-all-objects:
 
+.. automodapi:: safir.fastapi
+   :include-all-objects:
+
 .. automodapi:: safir.gcs
    :include-all-objects:
 
+.. automodapi:: safir.github
+   :include-all-objects:
+
+.. automodapi:: safir.github.models
+   :include-all-objects:
+
+.. automodapi:: safir.github.webhooks
+   :include-all-objects:
+
 .. automodapi:: safir.kubernetes
    :include-all-objects:
 
 .. automodapi:: safir.logging
    :include-all-objects:
 
 .. automodapi:: safir.metadata
@@ -50,20 +64,28 @@
 
 .. automodapi:: safir.middleware.x_forwarded
    :include-all-objects:
 
 .. automodapi:: safir.pydantic
    :include-all-objects:
 
+.. automodapi:: safir.redis
+   :include-all-objects:
+   :inherited-members:
+
 .. automodapi:: safir.slack.blockkit
+   :include-all-objects:
 
 .. automodapi:: safir.slack.webhook
+   :include-all-objects:
 
 .. automodapi:: safir.testing.gcs
    :include-all-objects:
 
 .. automodapi:: safir.testing.kubernetes
    :include-all-objects:
 
 .. automodapi:: safir.testing.slack
+   :include-all-objects:
 
 .. automodapi:: safir.testing.uvicorn
+   :include-all-objects:
```

### Comparing `safir-3.8.0/docs/changelog.md` & `safir-4.0.0/docs/changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,48 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.0.0 (2023-04-19)
+
+### Backwards-incompatible changes
+
+- Safir now requires a minimum Python version of 3.11.
+- `safir.pydantic.validate_exactly_one_of` is now a Pydantic root validator instead of an individual field validator, which simplifies how it should be called.
+- Custom Kubernetes objects are no longer copied before being stored in the Kubernetes mock by `create_namespaced_custom_object`, and no longer automatically get a `metadata.uid` value. This brings handling of custom objects in line with the behavior of other mocked `create_*` and `replace_*` APIs.
+- All objects stored in the Kubernetes mock will be modified to set `api_version`, `kind`, and (where appropriate) `namespace`. If any of those values are set in the object, they are checked for correctness and rejected with `AssertionError` if they don't match the API call and its parameters.
+- The mocked `create_*` Kubernetes APIs now use the name `body` for the parameter containing the API object, instead of using some other name specific to the kind of object. This fixes compatibility with the Python Kubernetes API that this class is mocking.
+
+### New features
+
+- The new `safir.redis.PydanticRedisStorage` class enables you to store Pydantic model objects in Redis.
+  A `safir.redis.EncryptedPydanticRedisStorage` class also encrypts data in Redis.
+  To use the `safir.redis` module, install Safir with the `redis` extra (i.e., `pip install safir[redis]`).
+- Add `safir.fastapi.ClientRequestError` base class for exceptions and the corresponding exception handler `safir.fastapi.client_request_error_handler`. These may be used together to raise structured exceptions and automatically transform them into structured HTTP errors with the correct HTTP status code and an error body compatible with `safir.models.ErrorModel` and FastAPI's own internally-generated errors.
+- Add `safir.slack.webhook.SlackWebException`, which is a child class of `safir.slack.webhook.SlackException` that knows how to capture and report details from an underlying HTTPX exception.
+- Add a `safir.testing.kubernetes.strip_none` helper function that makes it easier to compare Kubernetes objects against expected test data.
+- Add a `get_namespace_objects_for_test` method to the Kubernetes mock to retrieve all objects (of any kind) in a namespace.
+- Add a mock for the `list_nodes` Kubernetes API, which returns data set by a call to the new `set_nodes_for_test` method.
+- Add optional rudimentary namespace tracking to the Kubernetes mock. Namespaces can be created, deleted (which deletes all objects in the namespace), read, and listed. Explicit namespace creation remains optional; if an object is created in a namespace and that namespace does not exist, one will be implicitly created by the mock.
+- Add support for namespaced events (the older core API, not the new events API) to the Kubernetes mock. Newly-created pods with the default initial status post an event by default; otherwise, events must be created by calling the mocked `create_namespaced_event` API. The `list_namespaced_event` API supports watches with timeouts.
+- Add rudimentary support for `NetworkPolicy`, `ResourceQuota`, and `Service` objects to the Kubernetes mock.
+- Add a `safir.github` module for writing GitHub integrations with GidgetHub and Pydantic modeling. `safir.github.GitHubAppClientFactory` helps create authenticated clients for GitHub Apps and app installations. `safir.github.models` contains Pydantic models for GitHub v3 REST API resources. `safir.github.webhooks` contains Pydantic models for GitHub webhook payloads.
+
+### Bug fixes
+
+- Stop adding the `X-Auth-Request-User` header to the OpenAPI schema for routes that use `auth_dependency` or `auth_logger_dependency`.
+
+### Other changes
+
+- The `safir.testing.kubernetes.MockKubernetesApi` mock now has rudimentary API documentation for the Kubernetes APIs that it supports.
+- The documentation for running commands with `tox` has been updated for the new command-line syntax in tox v4.
+
 ## 3.8.0 (2023-03-15)
 
 ### New features
 
 - Add `safir.slack.webhook.SlackWebhookClient` and accompanying models to post a structured message to Slack via an incoming webhook. Add a `safir.slack.blockkit.SlackException` base class that can be used to create exceptions with supplemental metadata that can be sent to Slack as a formatted alert.
 - Add a FastAPI route class (`safir.slack.webhook.SlackRouteErrorHandler`) that reports all uncaught exceptions to Slack using an incoming webhook.
 - Add `safir.datetime.format_datetime_for_logging` to convert a `datetime` object into an easily human-readable representation.
@@ -132,15 +166,15 @@
 - When logging in JSON format, use `severity` instead of `level` for the log level for compatibility with Google Log Explorer.
 - In the FastAPI `logger_dependency`, add log information about the incoming requst in a format compatible with Google Log Explorer.
 
 ## 2.2.0 (2021-11-09)
 
 ### Bug fixes
 
-- Restore previous `http_client_dependency` behavior by enabling following redirects by default. This adjusts for the change of defaults in httpx 0.20.0.
+- Restore previous `http_client_dependency` behavior by enabling following redirects by default. This adjusts for the change of defaults in HTTPX 0.20.0.
 
 ## 2.1.1 (2021-10-29)
 
 ### Other changes
 
 - Require structlog 21.2.0 and adjust logger configuration of exception handling for the expectations of that version.
 
@@ -194,13 +228,13 @@
 - Fix duplicated log output when logging is configured multiple times.
 
 ## 0.1.0 (2020-02-26)
 
 ### New features
 
 - The first release of Safir featuring:
-  
+
   - `safir.http` for adding an `aiohttp.ClientSession` to your application.
   - `safir.logging` for configuring structlog loggers.
   - `safir.metadata` helps your gather and structure metadata about your application for publishing on metadata endpoints.
   - `safir.middleware` includes a logging middleware that adds a logger with bound context about the request to your Request object.
   - Documentation about these features and a tutorial for starting a new application with the `roundtable_aiohttp_bot` template.
```

### Comparing `safir-3.8.0/docs/dev/development.rst` & `safir-4.0.0/docs/dev/development.rst`

 * *Files 1% similar despite different names*

```diff
@@ -65,43 +65,43 @@
 Running tests
 =============
 
 To test the library, run tox_, which tests the library the same way that the CI workflow does:
 
 .. code-block:: sh
 
-   tox
+   tox run
 
 To see a listing of test environments, run:
 
 .. code-block:: sh
 
-   tox -av
+   tox list
 
 tox will start a PostgreSQL container, which is required for some tests.
 
 To run a specific test or list of tests, you can add test file names (and any other pytest_ options) after ``--`` when executing the ``py`` tox environment.
 For example:
 
 .. code-block:: sh
 
-   tox -e py -- tests/database_test.py
+   tox run -e py -- tests/database_test.py
 
 .. _dev-build-docs:
 
 Building documentation
 ======================
 
 Documentation is built with Sphinx_:
 
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 
 .. code-block:: sh
 
-   tox -e docs
+   tox run -e docs
 
 The build documentation is located in the :file:`docs/_build/html` directory.
 
 .. _dev-change-log:
 
 Updating the change log
 =======================
@@ -144,15 +144,15 @@
 
 Code
 ----
 
 - The code style follows :pep:`8`, though in practice lean on Black and isort to format the code for you.
 
 - Use :pep:`484` type annotations.
-  The ``tox -e typing`` test environment, which runs mypy_, ensures that the project's types are consistent.
+  The ``tox run -e typing`` test environment, which runs mypy_, ensures that the project's types are consistent.
 
 - Write tests for Pytest_.
 
 Documentation
 -------------
 
 - Follow the `LSST DM User Documentation Style Guide`_, which is primarily based on the `Google Developer Style Guide`_.
```

### Comparing `safir-3.8.0/docs/dev/release.rst` & `safir-4.0.0/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/index.rst` & `safir-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/user-guide/arq.rst` & `safir-4.0.0/docs/user-guide/arq.rst`

 * *Files 1% similar despite different names*

```diff
@@ -94,25 +94,25 @@
 The :file:`src/yourapp/worker/main.py` module looks like:
 
 .. code-block:: python
 
     from __future__ import annotations
 
     import uuid
-    from typing import Any, Dict
+    from typing import Any
 
     import httpx
     import structlog
     from safir.logging import configure_logging
 
     from ..config import config
     from .functions import function_a, function_b
 
 
-    async def startup(ctx: Dict[Any, Any]) -> None:
+    async def startup(ctx: dict[Any, Any]) -> None:
         """Runs during worker start-up to set up the worker context."""
         configure_logging(
             profile=config.profile,
             log_level=config.log_level,
             name="yourapp",
         )
         logger = structlog.get_logger("yourapp")
@@ -123,15 +123,15 @@
         http_client = httpx.AsyncClient()
         ctx["http_client"] = http_client
 
         ctx["logger"] = logger
         logger.info("Worker start up complete")
 
 
-    async def shutdown(ctx: Dict[Any, Any]) -> None:
+    async def shutdown(ctx: dict[Any, Any]) -> None:
         """Runs during worker shutdown to cleanup resources."""
         if "logger" in ctx.keys():
             logger = ctx["logger"]
         else:
             logger = structlog.get_logger("yourapp")
         logger.info("Running worker shutdown.")
 
@@ -168,35 +168,37 @@
 Using the arq dependency in endpoint handlers
 ---------------------------------------------
 
 The `safir.dependencies.arq.arq_dependency` dependency provides your FastAPI endpoint handlers with an `ArqQueue` client that you can use to add jobs (`ArqQueue.enqueue`) to the queue, and get metadata (`ArqQueue.get_job_metadata`) and results (`ArqQueue.get_job_result`) from the queue:
 
 .. code-block:: python
 
+    from typing import Any
+
     from fastapi import Depends, HTTPException
     from safir.arq import ArqQueue
     from safir.dependencies.arq import arq_dependency
 
 
     @app.post("/jobs")
     async def post_job(
         arq_queue: ArqQueue = Depends(arq_dependency),
         a: str = "hello",
         b: int = 42,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Create a job."""
         job = await arq_queue.enqueue("test_task", a, a_number=b)
         return {"job_id": job.id}
 
 
     @app.get("/jobs/{job_id}")
     async def get_job(
         job_id: str,
         arq_queue: ArqQueue = Depends(arq_dependency),
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Get metadata about a job."""
         try:
             job = await arq_queue.get_job_metadata(
                 job_id, queue_name=queue_name
             )
         except JobNotFound:
             raise HTTPException(status_code=404)
```

### Comparing `safir-3.8.0/docs/user-guide/database.rst` & `safir-4.0.0/docs/user-guide/database.rst`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,39 @@
 
 To drop and recreate all of the tables, pass the ``reset=True`` option to `~safir.database.initialize_database`.
 
 Note that `~safir.database.initialize_database` returns a `~sqlalchemy.ext.asyncio.AsyncEngine` object for the newly-initialized database.
 This can be used to perform any further application-specific database initialization that is required, such as adding default table entries.
 Put any such code before the ``await engine.dispose()`` call.
 
+Using non-default PostgreSQL schemas
+------------------------------------
+
+Occasionally it's convenient for multiple applications to share the same database but use separate collections of tables.
+PostgreSQL supports serving multiple schemas (in the sense of a namespace of tables) from the same database, and SQLAlchemy supports specifying the PostgreSQL schema for a given collection of tables.
+
+The normal way to do this in SQLAlchemy is to modify the `~sqlalchemy.orm.DeclarativeBase` subclass used by the table definitions to specify a non-default schema.
+For example:
+
+.. code-block:: python
+
+   from sqlalchemy import MetaData
+   from sqlalchemy.orm import DeclarativeBase
+
+   from ..config import config
+
+
+   class Base(DeclarativeBase):
+       metadata = MetaData(schema=config.database_schema)
+
+If ``config.database_schema`` is `None`, the default schema will be used; otherwise, SQLAlchemy will use the specified schema instead of the default one.
+
+Safir supports this in database initialization by creating a non-default schema if one is set.
+If the ``schema`` attribute is set (via code like the above) on the SQLAlchemy metadata passed to the ``schema`` parameter of `~safir.database.initialize_database`, it will create that schema in the PostgreSQL database if it does not already exist.
+
 Running database initialization on pod startup
 ----------------------------------------------
 
 The recommended pattern for Safir-based applications that use a database is to initialize the database every time the pod has been restarted.
 Since initialization does nothing if the schema already exists, this is safe to do.
 It only wastes a bit of time during normal startup.
 This allows the application to be deployed on a new cluster without any special initialization step.
@@ -292,15 +317,15 @@
 
 Then, initialize the database in a test fixture.
 The simplest way to do this is to add a call to `~safir.database.initialize_database` to the ``app`` fixture.
 For example:
 
 .. code-block:: python
 
-   from typing import AsyncIterator
+   from collections.abc import AsyncIterator
 
    import pytest_asyncio
    from asgi_lifespan import LifespanManager
    from fastapi import FastAPI
    from safir.database import create_database_engine, initialize_database
 
    from application import main
```

### Comparing `safir-3.8.0/docs/user-guide/datetime.rst` & `safir-4.0.0/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/user-guide/gafaelfawr.rst` & `safir-4.0.0/docs/user-guide/gafaelfawr.rst`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 The value of the header should be the username of the user the test is simulating.
 Optionally, if a test will be simulating many requests from the same authenticated user, this header can be added as a default header sent by the client.
 This is most easily done by defining a fixture, as follows.
 (This fixture assumes the FastAPI application under test is available via another fixture named ``app``.)
 
 .. code-block:: python
 
-   from typing import AsyncIterator
+   from collections.abc import AsyncIterator
 
    import pytest_asyncio
    from fastapi import FastAPI
    from httpx import AsyncClient
 
 
    @pytest_asyncio.fixture
```

### Comparing `safir-3.8.0/docs/user-guide/gcs.rst` & `safir-4.0.0/docs/user-guide/gcs.rst`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,18 @@
 Testing signed URLs
 -------------------
 
 Applications that want to run tests with the mock GCS API should define a fixture (in ``conftest.py``) as follows:
 
 .. code-block:: python
 
+   from collections.abc import Iterator
    from datetime import timedelta
-   from typing import Iterator
 
    import pytest
-
    from safir.testing.gcs import MockStorageClient, patch_google_storage
 
 
    @pytest.fixture
    def mock_gcs() -> Iterator[MockStorageClient]:
        yield from patch_google_storage(
            expected_expiration=timedelta(hours=1), bucket_name="some-bucket"
```

### Comparing `safir-3.8.0/docs/user-guide/http-client.rst` & `safir-4.0.0/docs/user-guide/http-client.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################
-Using the httpx client
+Using the HTTPX client
 ######################
 
 Safir helps you manage a single ``httpx.AsyncClient`` for your application.
-Using a single HTTP client improves performance by reusing connections.
+Using a single HTTPX_ client improves performance by reusing connections.
 
 Setting up the httpx.AsyncClient
 ================================
 
 The ``httpx.AsyncClient`` will be dyanmically created during application startup.
 Nothing further is needed apart from importing the dependency.
 However, it must be closed during application shutdown or a warning will be generated.
```

### Comparing `safir-3.8.0/docs/user-guide/ivoa.rst` & `safir-4.0.0/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/user-guide/logging.rst` & `safir-4.0.0/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/docs/user-guide/pydantic.rst` & `safir-4.0.0/docs/user-guide/pydantic.rst`

 * *Files 4% similar despite different names*

```diff
@@ -82,26 +82,23 @@
        docker: Optional[DockerConfig] = None
        ghcr: Optional[GHCRConfig] = None
 
 The intent here is that only one of those two configurations will be present: either Docker or GitHub Container Registry.
 However, Pydantic has no native way to express that, and the above model will accept input where neither or both of those attributes are set.
 
 Safir provides a function, `~safir.pydantic.validate_exactly_one_of`, designed for this case.
-It takes a list of fields, of which exactly one must be set, and builds a validation function that checks this property of the model.
+It takes a list of fields, of which exactly one must be set, and builds a root validator function that checks this property of the model.
 
 So, in the above example, the full class would be:
 
 .. code-block:: python
 
    class Model(BaseModel):
        docker: Optional[DockerConfig] = None
        ghcr: Optional[GHCRConfig] = None
 
-       _validate_type = validator("ghcr", always=True, allow_reuse=True)(
+       _validate_type = root_validator(allow_reuse=True)(
            validate_exactly_one_of("docker", "ghcr")
        )
 
 Note the syntax, which is a little odd since it is calling a decorator on the results of a function builder.
-
-The argument to `~pydantic.validator` must always be the last of the possible attributes that may be set, ensuring that any other attributes have been seen when the validator runs.
-``always=True`` must be set to ensure the validator runs regardless of which attribute is set.
 ``allow_reuse=True`` must be set due to limitations in Pydantic.
```

### Comparing `safir-3.8.0/docs/user-guide/set-up-from-template.rst` & `safir-4.0.0/docs/user-guide/set-up-from-template.rst`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 =========================
 
 The Python code generated by the template is good, but there may be minor formatting issues related to line length and your application's chosen name.
 You can format the code and by running tox_:
 
 .. prompt:: bash
 
-   tox -e lint
+   tox run -e lint
    git commit -a
 
 6. Push to GitHub
 =================
 
 Now `create your application's repository on GitHub <https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository>`__ and push to it.
 
@@ -133,49 +133,49 @@
 
    pytest
 
 An even better, and more robust approach is with tox:
 
 .. prompt:: bash
 
-   tox
+   tox run
 
 Tox runs several test steps, each in their own virtual environment.
 To learn about these test steps:
 
 .. prompt:: bash
 
-   tox -av
+   tox list
 
 For example, to only run mypy to check type annotations:
 
 .. prompt:: bash
 
-   tox -e typing
+   tox run -e typing
 
 Or to only lint the code (and reformat it):
 
 .. prompt:: bash
 
-   tox -e lint
+   tox run -e lint
 
 To run all the default test steps, but in parallel:
 
 .. prompt:: bash
 
-   tox -p auto
+   tox run-parallel -p auto
 
 9. Try the local development server
 ===================================
 
 In addition to running tests, tox is also configured with a command to spin up a development server:
 
 .. prompt:: bash
 
-   tox -e run
+   tox run -e run
 
 In another shell, send an HTTP GET request to the development server:
 
 .. prompt:: bash
 
    curl http://localhost:8000/ | python -m json.tool
```

### Comparing `safir-3.8.0/docs/user-guide/slack-webhook.rst` & `safir-4.0.0/docs/user-guide/slack-webhook.rst`

 * *Files 11% similar despite different names*

```diff
@@ -156,14 +156,55 @@
            )
            return message
 
 .. warning::
 
    The full exception message (although not the traceback) is sent to Slack, so it should not contain any sensitive information, security keys, or similar data.
 
+Reporting HTTPX exceptions
+--------------------------
+
+A common source of exceptions in Safir applications are exceptions raised by HTTPX_ while making calls to other web services.
+Safir provides a base class for those exceptions, `~safir.slack.blockkit.SlackWebException`, which behaves the same as `~safir.slack.blockkit.SlackException` but captures additional information from the underlying HTTPX exception.
+
+The advantages of `~safir.slack.blockkit.SlackWebException` over using `~safir.slack.blockkit.SlackException` directly, possibly with the text of the HTTPX exception, are:
+
+- If the exception is due to an error returned by the remote server, the stringification of the exception, and the main Slack message if posted to Slack, always includes the URL, method, and status code.
+  (You therefore will want to override the ``__str__`` method if your URLs may contain secret data that should not be sent in Slack alerts, such as Slack webhook URLs.)
+- The body of any reply is included in the stringification and in a block of the Slack message.
+  (Again, override this behavior if the bodies of error replies may include secrets that should not be sent to Slack.)
+- For other exceptions, the stringification and main Slack message include both the type and the stringification of the underlying exception.
+- Where possible, the URL and method are included in a field in the Slack message.
+
+The normal way to use this class or exception classes derived from it is to call the class method ``from_exception``, passing in the underlying HTTPX exception.
+For example:
+
+.. code-block:: python
+
+   from httpx import AsyncClient, HTTPError
+   from safir.slack.blockkit import SlackWebException
+
+
+   class FooServiceError(SlackWebException):
+       """An error occurred sending a request to the foo service."""
+
+
+   async def do_something(client: AsyncClient) -> None:
+       # ... set up some request to the foo service ...
+       try:
+           r = await client.get(url)
+           r.raise_for_status()
+       except HTTPError as e:
+           raise FooServiceError.from_exception(e) from e
+
+Note the ``from e`` clause when raising the derived exception, which tells Python to include the backtraces from both exceptions.
+Higher-level code may then catch this exception and post it to Slack if desired.
+
+As with `~safir.slack.blockkit.SlackException`, a username may be provided as a second argument to ``from_exception`` or set later by catching the exception, setting its ``user`` attribute, and re-raising it.
+
 .. _slack-uncaught-exceptions:
 
 Reporting uncaught exceptions to a Slack webhook
 ================================================
 
 The above exception reporting mechanism only works with exceptions that were caught by the application code.
 Uncaught exceptions are a common problem for most web applications and indicate some unanticipated error case.
```

### Comparing `safir-3.8.0/docs/user-guide/uvicorn.rst` & `safir-4.0.0/docs/user-guide/uvicorn.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ########################################
 Starting an app with Uvicorn for testing
 ########################################
 
-Normally, testing of FastAPI apps should be done by passing the app to ``httpx.AsyncClient`` and using httpx's built-in support for sending requests directly to an ASGI application.
+Normally, testing of FastAPI apps should be done by passing the app to ``httpx.AsyncClient`` and using HTTPX's built-in support for sending requests directly to an ASGI application.
 To do this, use the ``client`` fixture provided by the ``fastapi_safir_app`` template (see :ref:`create-from-template`).
 
 However, in some test scenarios it may be necessary for the app being tested to respond to regular HTTP requests, such as for Selenium_ testing with a browser.
 Testing integration with Uvicorn_ also requires running the app with Uvicorn.
 
 .. _Selenium: https://selenium-python.readthedocs.io/
```

### Comparing `safir-3.8.0/docs/user-guide/x-forwarded.rst` & `safir-4.0.0/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/pyproject.toml` & `safir-4.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,29 @@
 readme= "README.md"
 keywords = [
     "rubin",
     "lsst",
 ]
 # https://pypi.org/classifiers/
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 dependencies = [
+    "cryptography",
     "fastapi",
+    "gidgethub",
     "httpx>=0.20.0",
     "pydantic",
     "starlette",
     "structlog>=21.2.0",
 ]
 dynamic = ["version"]
 
@@ -48,25 +47,30 @@
     "mypy",
     "pre-commit",
     "psycopg2",
     "pytest",
     "pytest-asyncio",
     "respx",
     "sqlalchemy[mypy]",
+    "types-redis",
     "uvicorn",
     # documentation
     "documenteer[guide]>=0.7.0b2",
+    "autodoc_pydantic",
 ]
 gcs = [
     "google-auth",
     "google-cloud-storage"
 ]
 kubernetes = [
     "kubernetes_asyncio"
 ]
+redis = [
+    "redis>=4.2.0rc1,!=4.5.2", # https://github.com/redis/redis-py/issues/2633
+]
 
 [[project.authors]]
 name = "Association of Universities for Research in Astronomy, Inc. (AURA)"
 email = "sqre-admin@lists.lsst.org"
 
 [project.urls]
 Homepage = "https://safir.lsst.io"
@@ -104,15 +108,15 @@
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:"
 ]
 
 [tool.black]
 line-length = 79
-target-version = ['py37']
+target-version = ["py311"]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
   | \.tox
   | \.venv
@@ -121,23 +125,26 @@
   | dist
 )/
 '''
 # Use single-quoted strings so TOML treats the string like a Python r-string
 # Multi-line strings are implicitly treated by black as regular expressions
 
 [tool.isort]
-include_trailing_comma = true
-multi_line_output = 3
+profile = "black"
+line_length = 79
 known_first_party = ["safir", "tests"]
 skip = ["docs/conf.py"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 filterwarnings = [
     "ignore:'cgi' is deprecated:DeprecationWarning:google.cloud.storage.blob",
+    # Google modules call a deprecated pkg_resources API.
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
+    "ignore:.*pkg_resources\\.declare_namespace:DeprecationWarning",
 ]
 python_files = [
     "tests/*.py",
     "tests/*/*.py"
 ]
 
 [tool.mypy]
@@ -146,11 +153,18 @@
 ignore_missing_imports = true
 local_partial_types = true
 no_implicit_reexport = true
 plugins = [
     "pydantic.mypy",
     "sqlalchemy.ext.mypy.plugin",
 ]
+show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
```

### Comparing `safir-3.8.0/src/safir/__init__.py` & `safir-4.0.0/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/src/safir/arq.py` & `safir-4.0.0/src/safir/arq.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import abc
 import uuid
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Optional, Self
 
 from arq import create_pool
 from arq.connections import ArqRedis, RedisSettings
 from arq.constants import default_queue_name as arq_default_queue_name
 from arq.jobs import Job, JobStatus
 
 __all__ = [
@@ -35,28 +35,28 @@
 
     Attributes
     ----------
     job_id
         The job ID, or `None` if the job ID is not known in this context.
     """
 
-    def __init__(self, message: str, job_id: Optional[str]) -> None:
+    def __init__(self, message: str, job_id: str | None) -> None:
         super().__init__(message)
         self._job_id = job_id
 
     @property
-    def job_id(self) -> Optional[str]:
+    def job_id(self) -> str | None:
         """The job ID, or `None` if the job ID is not known in this context."""
         return self._job_id
 
 
 class JobNotQueued(ArqJobError):
     """The job was not successfully queued."""
 
-    def __init__(self, job_id: Optional[str]) -> None:
+    def __init__(self, job_id: str | None) -> None:
         super().__init__(
             f"Job was not queued because it already exists. id={job_id}",
             job_id,
         )
 
 
 class JobNotFound(ArqJobError):
@@ -118,18 +118,18 @@
 
     id: str
     """The `~arq.jobs.Job` identifier."""
 
     name: str
     """The task name."""
 
-    args: Tuple[Any, ...]
+    args: tuple[Any, ...]
     """The positional arguments to the task function."""
 
-    kwargs: Dict[str, Any]
+    kwargs: dict[str, Any]
     """The keyword arguments to the task function."""
 
     enqueue_time: datetime
     """Time when the job was added to the queue."""
 
     status: JobStatus
     """Status of the job.
@@ -144,15 +144,15 @@
     - ``not_found`` (the job cannot be found)
     """
 
     queue_name: str
     """Name of the queue this job belongs to."""
 
     @classmethod
-    async def from_job(cls, job: Job) -> JobMetadata:
+    async def from_job(cls, job: Job) -> Self:
         """Initialize JobMetadata from an arq Job.
 
         Raises
         ------
         JobNotFound
             Raised if the job is not found
         """
@@ -226,15 +226,15 @@
     exception was raised.
     """
 
     result: Any
     """The job's result."""
 
     @classmethod
-    async def from_job(cls, job: Job) -> JobResult:
+    async def from_job(cls, job: Job) -> Self:
         """Initialize the `JobResult` from an arq `~arq.jobs.Job`.
 
         Raises
         ------
         JobNotFound
             Raised if the job is not found
         JobResultUnavailable
@@ -395,15 +395,15 @@
 
     @classmethod
     async def initialize(
         cls,
         redis_settings: RedisSettings,
         *,
         default_queue_name: str = arq_default_queue_name,
-    ) -> RedisArqQueue:
+    ) -> Self:
         """Initialize a RedisArqQueue from Redis settings."""
         pool = await create_pool(
             redis_settings, default_queue_name=default_queue_name
         )
         return cls(pool)
 
     async def enqueue(
@@ -448,22 +448,22 @@
 class MockArqQueue(ArqQueue):
     """A mocked queue for testing API services."""
 
     def __init__(
         self, *, default_queue_name: str = arq_default_queue_name
     ) -> None:
         super().__init__(default_queue_name=default_queue_name)
-        self._job_metadata: Dict[str, Dict[str, JobMetadata]] = {
+        self._job_metadata: dict[str, dict[str, JobMetadata]] = {
             self.default_queue_name: {}
         }
-        self._job_results: Dict[str, Dict[str, JobResult]] = {
+        self._job_results: dict[str, dict[str, JobResult]] = {
             self.default_queue_name: {}
         }
 
-    def _resolve_queue_name(self, queue_name: Optional[str]) -> str:
+    def _resolve_queue_name(self, queue_name: str | None) -> str:
         return queue_name or self.default_queue_name
 
     async def enqueue(
         self,
         task_name: str,
         *task_args: Any,
         _queue_name: Optional[str] = None,
```

### Comparing `safir-3.8.0/src/safir/asyncio.py` & `safir-4.0.0/src/safir/asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utility functions for asyncio code."""
 
 from __future__ import annotations
 
 import asyncio
+from collections.abc import Callable, Coroutine
 from functools import wraps
-from typing import Any, Callable, Coroutine, TypeVar
+from typing import Any, TypeVar
 
 T = TypeVar("T")
 
 __all__ = ["run_with_asyncio"]
 
 
 def run_with_asyncio(
```

### Comparing `safir-3.8.0/src/safir/database.py` & `safir-4.0.0/src/safir/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class DatabaseInitializationError(Exception):
     """Database initialization failed."""
 
 
 def _build_database_url(
-    url: str, password: Optional[str], *, is_async: bool
+    url: str, password: str | None, *, is_async: bool
 ) -> str:
     """Build the authenticated URL for the database.
 
     Parameters
     ----------
     url
         Database connection URL, not including the password.
@@ -87,15 +87,15 @@
 
 
 @overload
 def datetime_from_db(time: None) -> None:
     ...
 
 
-def datetime_from_db(time: Optional[datetime]) -> Optional[datetime]:
+def datetime_from_db(time: datetime | None) -> datetime | None:
     """Add the UTC time zone to a naive datetime from the database.
 
     Parameters
     ----------
     time
         The naive datetime from the database, or `None`.
 
@@ -118,15 +118,15 @@
 
 
 @overload
 def datetime_to_db(time: None) -> None:
     ...
 
 
-def datetime_to_db(time: Optional[datetime]) -> Optional[datetime]:
+def datetime_to_db(time: datetime | None) -> datetime | None:
     """Strip time zone for storing a datetime in the database.
 
     Parameters
     ----------
     time
         The timezone-aware `~datetime.datetime` in the UTC time zone, or
         `None`.
@@ -143,15 +143,15 @@
     if time.tzinfo != timezone.utc:
         raise ValueError(f"datetime {time} not in UTC")
     return time.replace(tzinfo=None)
 
 
 def create_database_engine(
     url: str,
-    password: Optional[str],
+    password: str | None,
     *,
     isolation_level: Optional[str] = None,
 ) -> AsyncEngine:
     """Create a new async database engine.
 
     Parameters
     ----------
@@ -242,15 +242,15 @@
     async with session.begin():
         await session.execute(statement.limit(1))
         return session
 
 
 def create_sync_session(
     url: str,
-    password: Optional[str],
+    password: str | None,
     logger: Optional[BoundLogger] = None,
     *,
     isolation_level: Optional[str] = None,
     statement: Optional[Select] = None,
 ) -> scoped_session:
     """Create a new sync database session.
```

### Comparing `safir-3.8.0/src/safir/datetime.py` & `safir-4.0.0/src/safir/datetime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Date and time manipulation utility functions."""
 
 from __future__ import annotations
 
 from datetime import datetime, timezone
-from typing import Optional, overload
+from typing import overload
 
 __all__ = [
     "current_datetime",
     "format_datetime_for_logging",
     "isodatetime",
     "parse_isodatetime",
 ]
@@ -49,17 +49,15 @@
 
 
 @overload
 def format_datetime_for_logging(timestamp: None) -> None:
     ...
 
 
-def format_datetime_for_logging(
-    timestamp: Optional[datetime],
-) -> Optional[str]:
+def format_datetime_for_logging(timestamp: datetime | None) -> str | None:
     """Format a datetime for logging and human readabilty.
 
     Parameters
     ----------
     timestamp
         Object to format. Must be in UTC or timezone-naive (in which case it's
         assumed to be in UTC).
@@ -109,15 +107,15 @@
         The provided timestamp was not in UTC.
     """
     if timestamp.tzinfo not in (None, timezone.utc):
         raise ValueError("Datetime {timestamp} not in UTC")
     return timestamp.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
-def parse_isodatetime(time_string: str) -> Optional[datetime]:
+def parse_isodatetime(time_string: str) -> datetime | None:
     """Parse a string in a standard ISO date format.
 
     Parameters
     ----------
     time_string
         Date and time formatted as an ISO 8601 date and time using ``Z`` as
         the time zone.  This is the same format produced by `isodatetime` and
```

### Comparing `safir-3.8.0/src/safir/dependencies/arq.py` & `safir-4.0.0/src/safir/dependencies/arq.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     tasks to the worker pool.
     """
 
     def __init__(self) -> None:
         self._arq_queue: Optional[ArqQueue] = None
 
     async def initialize(
-        self, *, mode: ArqMode, redis_settings: Optional[RedisSettings]
+        self, *, mode: ArqMode, redis_settings: RedisSettings | None
     ) -> None:
         """Initialize the dependency (call during the FastAPI start-up event).
 
         Parameters
         ----------
         mode
             The mode to operate the queue dependency in. With
```

### Comparing `safir-3.8.0/src/safir/dependencies/db_session.py` & `safir-4.0.0/src/safir/dependencies/db_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Manage an async database session."""
 
-from typing import AsyncIterator, Optional
+from collections.abc import AsyncIterator
+from typing import Optional
 
 from sqlalchemy.ext.asyncio import AsyncEngine, async_scoped_session
 
 from ..database import create_async_session, create_database_engine
 
 __all__ = ["DatabaseSessionDependency", "db_session_dependency"]
 
@@ -62,15 +63,15 @@
         if self._engine:
             await self._engine.dispose()
             self._engine = None
 
     async def initialize(
         self,
         url: str,
-        password: Optional[str],
+        password: str | None,
         *,
         isolation_level: Optional[str] = None,
     ) -> None:
         """Initialize the session dependency.
 
         Parameters
         ----------
```

### Comparing `safir-3.8.0/src/safir/dependencies/gafaelfawr.py` & `safir-4.0.0/src/safir/dependencies/gafaelfawr.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 __all__ = [
     "auth_dependency",
     "auth_logger_dependency",
 ]
 
 
-async def auth_dependency(x_auth_request_user: str = Header(...)) -> str:
+async def auth_dependency(
+    x_auth_request_user: str = Header(..., include_in_schema=False)
+) -> str:
     """Retrieve authentication information from HTTP headers.
 
     Intended for use with applications protected by Gafaelfawr, this retrieves
     authentication information from headers added to the incoming request by
     the Gafaelfawr ``auth_request`` NGINX subhandler.
     """
     return x_auth_request_user
```

### Comparing `safir-3.8.0/src/safir/dependencies/http_client.py` & `safir-4.0.0/src/safir/dependencies/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "HTTPClientDependency",
     "http_client_dependency",
 ]
 
 DEFAULT_HTTP_TIMEOUT = 20.0
 """Default timeout (in seconds) for outbound HTTP requests.
 
-The default httpx timeout has proven too short in practice for calls to, for
+The default HTTPX timeout has proven too short in practice for calls to, for
 example, GitHub for authorization verification. Increase the default to 20
 seconds. Users of this dependency can always lower it if needed.
 """
 
 
 class HTTPClientDependency:
     """Provides an ``httpx.AsyncClient`` as a dependency.
```

### Comparing `safir-3.8.0/src/safir/dependencies/logger.py` & `safir-4.0.0/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/src/safir/gcs.py` & `safir-4.0.0/src/safir/gcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utilities for interacting with Google Cloud Storage."""
 
 from __future__ import annotations
 
 from datetime import timedelta
-from typing import Optional
 from urllib.parse import urlparse
 
 import google.auth
 from google.auth import impersonated_credentials
 from google.cloud import storage
 
 __all__ = ["SignedURLService"]
@@ -45,15 +44,15 @@
         self, service_account: str, lifetime: timedelta = timedelta(hours=1)
     ) -> None:
         self._lifetime = lifetime
         self._service_account = service_account
         self._gcs = storage.Client()
         self._credentials, _ = google.auth.default()
 
-    def signed_url(self, uri: str, mime_type: Optional[str]) -> str:
+    def signed_url(self, uri: str, mime_type: str | None) -> str:
         """Generate signed URL for a given storage object.
 
         Parameters
         ----------
         uri
             URI for the storage object.  This must start with ``s3://`` and
             use the S3 URI syntax to specify bucket and blob of a Google
```

### Comparing `safir-3.8.0/src/safir/kubernetes.py` & `safir-4.0.0/src/safir/kubernetes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 import os
 
 from kubernetes_asyncio import config
 
+__all__ = ["initialize_kubernetes"]
+
 
 async def initialize_kubernetes() -> None:
     """Load the Kubernetes configuration.
 
     This has to be run once per process and should be run during application
     startup.  This function handles Kubernetes configuration independent of
     any given Kubernetes client so that clients can be created for each
```

### Comparing `safir-3.8.0/src/safir/logging.py` & `safir-4.0.0/src/safir/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 import re
 import sys
 from enum import Enum
-from typing import Any, List, Optional, Union
+from typing import Any, Optional
 
 import structlog
 from structlog.stdlib import add_log_level
 from structlog.types import EventDict
 
 __all__ = [
     "LogLevel",
@@ -88,16 +88,16 @@
     event_dict["severity"] = severity
     return event_dict
 
 
 def configure_logging(
     *,
     name: str,
-    profile: Union[Profile, str] = Profile.production,
-    log_level: Union[LogLevel, str] = LogLevel.INFO,
+    profile: Profile | str = Profile.production,
+    log_level: LogLevel | str = LogLevel.INFO,
     add_timestamp: bool = False,
 ) -> None:
     """Configure logging and structlog.
 
     Parameters
     ----------
     name
@@ -163,15 +163,15 @@
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(logging.Formatter("%(message)s"))
     logger = logging.getLogger(name)
     logger.handlers = []
     logger.addHandler(stream_handler)
     logger.setLevel(log_level.value)
 
-    processors: List[Any] = [
+    processors: list[Any] = [
         structlog.stdlib.filter_by_level,
         structlog.stdlib.add_logger_name,
         structlog.stdlib.PositionalArgumentsFormatter(),
     ]
     if add_timestamp:
         processors.append(structlog.processors.TimeStamper(fmt="iso"))
     processors.extend(
@@ -243,15 +243,15 @@
     event_dict["httpRequest"]["requestMethod"] = method
     event_dict["httpRequest"]["requestUrl"] = url
     event_dict["httpRequest"]["status"] = match.group(2)
     return event_dict
 
 
 def configure_uvicorn_logging(
-    log_level: Union[LogLevel, str] = LogLevel.INFO,
+    log_level: LogLevel | str = LogLevel.INFO,
 ) -> None:
     """Set up logging.
 
     This configures Uvicorn to use structlog for output formatting and
     installs a custom processor to parse its access log messages into
     additional log context that matches the format of Google log messages.
     This helps Google's Cloud Logging system understand the logs. Access logs
```

### Comparing `safir-3.8.0/src/safir/metadata.py` & `safir-4.0.0/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/src/safir/middleware/ivoa.py` & `safir-4.0.0/src/safir/middleware/ivoa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Middleware for IVOA services."""
 
-from typing import Awaitable, Callable
+from collections.abc import Awaitable, Callable
 from urllib.parse import urlencode
 
 from fastapi import Request, Response
 from starlette.middleware.base import BaseHTTPMiddleware
 
 __all__ = ["CaseInsensitiveQueryMiddleware"]
```

### Comparing `safir-3.8.0/src/safir/middleware/x_forwarded.py` & `safir-4.0.0/src/safir/middleware/x_forwarded.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Update the request based on ``X-Forwarded-For`` headers."""
 
 from __future__ import annotations
 
+from collections.abc import Awaitable, Callable
 from ipaddress import _BaseAddress, _BaseNetwork, ip_address
-from typing import Awaitable, Callable, List, Optional
+from typing import Optional
 
 from fastapi import FastAPI, Request, Response
 from starlette.middleware.base import BaseHTTPMiddleware
 
 __all__ = ["XForwardedMiddleware"]
 
 
@@ -34,15 +35,15 @@
     proxies
         The networks of the trusted proxies.  If not specified, defaults to
         the empty list, which means only the immediately upstream proxy will
         be trusted.
     """
 
     def __init__(
-        self, app: FastAPI, *, proxies: Optional[List[_BaseNetwork]] = None
+        self, app: FastAPI, *, proxies: Optional[list[_BaseNetwork]] = None
     ) -> None:
         super().__init__(app)
         if proxies:
             self.proxies = proxies
         else:
             self.proxies = []
 
@@ -104,15 +105,15 @@
 
         # Rather than one entry per hop, NGINX seems to add only a single
         # X-Forwarded-Host header with the original hostname.
         request.state.forwarded_host = self._get_forwarded_host(request)
 
         return await call_next(request)
 
-    def _get_forwarded_for(self, request: Request) -> List[_BaseAddress]:
+    def _get_forwarded_for(self, request: Request) -> list[_BaseAddress]:
         """Retrieve the ``X-Forwarded-For`` entries from the request.
 
         Parameters
         ----------
         request
             The incoming request.
 
@@ -128,15 +129,15 @@
             return []
         return [
             ip_address(addr)
             for addr in (a.strip() for a in forwarded_for_str[0].split(","))
             if addr
         ]
 
-    def _get_forwarded_host(self, request: Request) -> Optional[str]:
+    def _get_forwarded_host(self, request: Request) -> str | None:
         """Retrieve the ``X-Forwarded-Host`` header.
 
         Parameters
         ----------
         request
             The incoming request.
 
@@ -149,15 +150,15 @@
             so act as if there are no headers.
         """
         forwarded_host = request.headers.getlist("X-Forwarded-Host")
         if not forwarded_host or len(forwarded_host) > 1:
             return None
         return forwarded_host[0].strip()
 
-    def _get_forwarded_proto(self, request: Request) -> List[str]:
+    def _get_forwarded_proto(self, request: Request) -> list[str]:
         """Retrieve the ``X-Forwarded-Proto`` entries from the request.
 
         Parameters
         ----------
         request
             The incoming request.
```

### Comparing `safir-3.8.0/src/safir/models.py` & `safir-4.0.0/src/safir/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -----
 FastAPI does not appear to export its error response model in a usable form,
 so define a copy of it so that we can reference it in API definitions to
 generate good documentation.
 """
 
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import BaseModel, Field
 
 __all__ = [
     "ErrorDetail",
     "ErrorLocation",
     "ErrorModel",
@@ -31,20 +31,20 @@
     path = "path"
     query = "query"
 
 
 class ErrorDetail(BaseModel):
     """The detail of the error message."""
 
-    loc: Optional[List[str]] = Field(
+    loc: Optional[list[str]] = Field(
         None, title="Location", example=["area", "field"]
     )
 
     msg: str = Field(..., title="Message", example="Some error messge")
 
     type: str = Field(..., title="Error type", example="some_code")
 
 
 class ErrorModel(BaseModel):
     """A structured API error message."""
 
-    detail: List[ErrorDetail] = Field(..., title="Detail")
+    detail: list[ErrorDetail] = Field(..., title="Detail")
```

### Comparing `safir-3.8.0/src/safir/pydantic.py` & `safir-4.0.0/src/safir/pydantic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """Utility functions for Pydantic models."""
 
 from __future__ import annotations
 
+from collections.abc import Callable
 from datetime import datetime, timezone
-from typing import AbstractSet, Any, Callable, Dict, Mapping, Optional, Union
+from typing import Any, ParamSpec, TypeVar
 
 from pydantic import BaseModel
 
-# From Pydantic internals, so copy them here so that we can use them.  See the
-# comment in CamelCaseModel about better ways to copy type signatures from
-# Pydantic without duplicating code, possible in Python 3.10.
-AbstractSetIntStr = AbstractSet[Union[int, str]]
-MappingIntStrAny = Mapping[Union[int, str], Any]
+P = ParamSpec("P")
+T = TypeVar("T")
 
 __all__ = [
     "CamelCaseModel",
     "normalize_datetime",
     "normalize_isodatetime",
     "to_camel_case",
     "validate_exactly_one_of",
 ]
 
 
-def normalize_datetime(
-    v: Optional[Union[int, datetime]]
-) -> Optional[datetime]:
+def normalize_datetime(v: int | datetime | None) -> datetime | None:
     """Pydantic validator for datetime fields.
 
     Supports `~datetime.datetime` fields given in either any format supported
     by Pydantic natively, or in seconds since epoch (which Pydantic doesn't
     support).  This validator ensures that datetimes are always stored in the
     model as timezone-aware UTC datetimes.
 
@@ -67,15 +63,15 @@
         return datetime.fromtimestamp(v, tz=timezone.utc)
     elif v.tzinfo and v.tzinfo.utcoffset(v) is not None:
         return v.astimezone(timezone.utc)
     else:
         return v.replace(tzinfo=timezone.utc)
 
 
-def normalize_isodatetime(v: Optional[str]) -> Optional[datetime]:
+def normalize_isodatetime(v: str | None) -> datetime | None:
     """Pydantic validator for datetime fields in ISO format.
 
     This validator requires the ISO 8601 date and time format with ``Z`` as
     the time zone (``YYYY-MM-DDTHH:MM:SSZ``).  This format is compatible with
     Kubernetes and the ISO UWS standard and is the same format produced by
     `safir.datetime.isodatetime`.  It should be used when the ambiguous
     formats supported by Pydantic by default (such as dates and times without
@@ -155,95 +151,75 @@
     Alternately, inherit from `~safir.pydantic.CamelCaseModel`, which is
     derived from `pydantic.BaseModel` with those settings added.
     """
     components = string.split("_")
     return components[0] + "".join(c.title() for c in components[1:])
 
 
+def _copy_type(
+    parent: Callable[P, T]
+) -> Callable[[Callable[..., T]], Callable[P, T]]:
+    """Copy the type of a parent method.
+
+    Used to avoid duplicating the prototype of `pydantic.BaseModel.dict` and
+    `pydantic.BaseModel.json` when overriding them in `CamelCaseModel`.
+
+    Parameters
+    ----------
+    parent
+        Method from which to copy a type signature.
+
+    Returns
+    -------
+    Callable
+        Decorator that will replace the type signature of a function with the
+        type signature of its parent.
+    """
+    return lambda x: x
+
+
 class CamelCaseModel(BaseModel):
     """`pydantic.BaseModel` configured to accept camel-case input.
 
     This is a convenience class identical to `~pydantic.BaseModel` except with
     an alias generator configured so that it can be initialized with either
     camel-case or snake-case keys. Model exports with ``dict`` or ``json``
     also default to exporting in camel-case.
     """
 
     class Config:
         alias_generator = to_camel_case
         allow_population_by_field_name = True
 
-    # A better solution for typing that wouldn't require copying the arguments
-    # from Pydantic and therefore would be more future-proof would be to use
-    # ParamSpec plus a decorator to copy the signature from the overridden
-    # method. ParamSpec requires Python 3.10 and Safir currently supports
-    # versions as old as Python 3.8, so that approach isn't yet usable.
-
-    def dict(
-        self,
-        *,
-        include: Optional[Union[AbstractSetIntStr, MappingIntStrAny]] = None,
-        exclude: Optional[Union[AbstractSetIntStr, MappingIntStrAny]] = None,
-        by_alias: bool = True,
-        skip_defaults: Optional[bool] = None,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ) -> Dict[str, Any]:
+    @_copy_type(BaseModel.dict)
+    def dict(self, **kwargs: Any) -> dict[str, Any]:
         """Export the model as a dictionary.
 
         Overridden to change the default of ``by_alias`` from `False` to
         `True`, so that by default the exported dictionary uses camel-case.
         """
-        return super().dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-        )
-
-    def json(
-        self,
-        *,
-        include: Optional[Union[AbstractSetIntStr, MappingIntStrAny]] = None,
-        exclude: Optional[Union[AbstractSetIntStr, MappingIntStrAny]] = None,
-        by_alias: bool = True,
-        skip_defaults: Optional[bool] = None,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: Optional[Callable[[Any], Any]] = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
+        if "by_alias" not in kwargs:
+            kwargs["by_alias"] = True
+        return super().dict(**kwargs)
+
+    @_copy_type(BaseModel.json)
+    def json(self, **kwargs: Any) -> str:
         """Export the model as JSON.
 
         Overridden to change the default of ``by_alias`` from `False` to
         `True`, so that by default the exported dictionary uses camel-case.
         """
-        return super().json(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-            encoder=encoder,
-            models_as_dict=models_as_dict,
-            **dumps_kwargs,
-        )
+        if "by_alias" not in kwargs:
+            kwargs["by_alias"] = True
+        return super().json(**kwargs)
 
 
 def validate_exactly_one_of(
     *settings: str,
-) -> Callable[[Any, Dict[str, Any]], Any]:
+) -> Callable[[type, dict[str, Any]], dict[str, Any]]:
     """Generate a validator imposing a one and only one constraint.
 
     Sometimes, models have a set of attributes of which one and only one may
     be set. Ideally this is represented properly in the type system, but
     occasionally it's more convenient to use a validator. This is a validator
     generator that can produce a validator function that ensures one and only
     one of an arbitrary set of attributes must be set.
@@ -253,28 +229,28 @@
     *settings
         List of names of attributes, of which one and only one must be set.
         At least two attribute names must be listed.
 
     Returns
     -------
     Callable
-        The validator.
+        The root validator.
 
     Examples
     --------
     Use this inside a Pydantic class as a validator as follows:
 
     .. code-block:: python
 
        class Foo(BaseModel):
            foo: Optional[str] = None
            bar: Optional[str] = None
            baz: Optional[str] = None
 
-           _validate_options = validator("baz", always=True, allow_reuse=True)(
+           _validate_options = root_validator(allow_reuse=True)(
                validate_exactly_one_of("foo", "bar", "baz")
            )
 
     The attribute listed as the first argument to the ``validator`` call must
     be the last attribute in the model definition so that any other attributes
     have already been seen.
     """
@@ -283,19 +259,19 @@
         raise ValueError(msg)
 
     if len(settings) == 2:
         options = f"{settings[0]} and {settings[1]}"
     else:
         options = ", ".join(settings[:-1]) + ", and " + settings[-1]
 
-    def validator(v: Any, values: Dict[str, Any]) -> Any:
-        seen = v is not None
+    def validator(cls: type, values: dict[str, Any]) -> dict[str, Any]:
+        seen = False
         for setting in settings:
             if setting in values and values[setting] is not None:
                 if seen:
                     raise ValueError(f"only one of {options} may be given")
                 seen = True
         if not seen:
             raise ValueError(f"one of {options} must be given")
-        return v
+        return values
 
     return validator
```

### Comparing `safir-3.8.0/src/safir/slack/blockkit.py` & `safir-4.0.0/src/safir/slack/blockkit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """Slack Block Kit message models."""
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Optional, Self
 
+from httpx import HTTPError, HTTPStatusError, RequestError
 from pydantic import BaseModel, validator
 
 from safir.datetime import current_datetime, format_datetime_for_logging
 
 __all__ = [
     "SlackBaseBlock",
     "SlackBaseField",
     "SlackCodeBlock",
     "SlackCodeField",
     "SlackException",
     "SlackMessage",
     "SlackTextBlock",
     "SlackTextField",
+    "SlackWebException",
 ]
 
 
 class SlackBaseBlock(BaseModel, metaclass=ABCMeta):
     """Base class for any Slack Block Kit block."""
 
+    max_formatted_length: ClassVar[int] = 3000
+    """Maximum length of formatted output, imposed by Slack.
+
+    Intended to be overridden by child classes that need to impose different
+    maximum lengths.
+    """
+
     @abstractmethod
-    def to_slack(self) -> Dict[str, Any]:
+    def to_slack(self) -> dict[str, Any]:
         """Convert to a Slack Block Kit block.
 
         Returns
         -------
         dict
             A Slack Block Kit block suitable for including in the ``fields``
             or ``text`` section of a ``blocks`` element.
@@ -50,22 +59,15 @@
     text: str
     """Text of the field as normal text.
 
     This is always marked as vertabim, so channel mentions or @-mentions of
     users will not be treated as special.
     """
 
-    max_formatted_length: ClassVar[int] = 3000
-    """Maximum length of formatted output, imposed by Slack.
-
-    Intended to be overridden by child classes that need to impose different
-    maximum lengths.
-    """
-
-    def to_slack(self) -> Dict[str, Any]:
+    def to_slack(self) -> dict[str, Any]:
         """Convert to a Slack Block Kit block.
 
         Returns
         -------
         dict
             A Slack Block Kit block suitable for including in the ``fields``
             or ``text`` section of a ``blocks`` element.
@@ -85,22 +87,15 @@
 
     heading: str
     """Heading of the field (shown in bold)."""
 
     code: str
     """Text of the field as a code block."""
 
-    max_formatted_length: ClassVar[int] = 3000
-    """Maximum length of formatted output, imposed by Slack.
-
-    Intended to be overridden by child classes that need to impose different
-    maximum lengths.
-    """
-
-    def to_slack(self) -> Dict[str, Any]:
+    def to_slack(self) -> dict[str, Any]:
         """Convert to a Slack Block Kit block.
 
         Returns
         -------
         dict
             A Slack Block Kit block suitable for including in the ``fields``
             or ``text`` section of a ``blocks`` element.
@@ -112,15 +107,15 @@
         text = f"{heading}```\n{code}\n```"
         return {"type": "mrkdwn", "text": text, "verbatim": True}
 
 
 class SlackBaseField(SlackBaseBlock):
     """Base class for Slack Block Kit blocks for the ``fields`` section."""
 
-    max_formatted_length = 2000
+    max_formatted_length: ClassVar[int] = 2000
 
 
 class SlackTextField(SlackTextBlock, SlackBaseField):
     """One field in a Slack message with a heading and text body.
 
     Intended for use in the ``fields`` portion of a Block Kit message. If the
     formatted output is longer than 2000 characters, it will be truncated to
@@ -162,47 +157,47 @@
 
     Verbatim messages in Slack don't expand channel references or create user
     notifications. This is the default, but can be set to `False` to allow
     any such elements in the message to be recognized by Slack. Do not set
     this to `False` with untrusted input.
     """
 
-    fields: List[SlackBaseField] = []
+    fields: list[SlackBaseField] = []
     """Short key/value fields to include in the message (at most 10)."""
 
-    blocks: List[SlackBaseBlock] = []
+    blocks: list[SlackBaseBlock] = []
     """Additional text blocks to include in the message (after fields)."""
 
-    attachments: List[SlackBaseBlock] = []
+    attachments: list[SlackBaseBlock] = []
     """Longer sections to include as attachments.
 
     Notes
     -----
     Slack has marked attachments as legacy and warns that future changes may
     reduce their visibility or utility. Unfortunately, there is no other way
     to attach possibly-long text where Slack will hide long content by default
     but allow the user to expand it. We therefore continue to use attachments
     for long text for want of a better alternative.
     """
 
     @validator("fields")
-    def _validate_fields(cls, v: List[SlackBaseField]) -> List[SlackBaseField]:
+    def _validate_fields(cls, v: list[SlackBaseField]) -> list[SlackBaseField]:
         """Check constraints on fields.
 
         Slack imposes a maximum of 10 items in a ``fields`` array. Also ensure
         that no fields are actually attachments, since in that case they may
         not be truncated to the correct length. (The type system we're using
         doesn't allow Pydantic to check this directly.)
         """
         if len(v) > 10:
             msg = f"Slack does not allow more than 10 fields ({len(v)} seen)"
             raise ValueError(msg)
         return v
 
-    def to_slack(self) -> Dict[str, Any]:
+    def to_slack(self) -> dict[str, Any]:
         """Convert to a Slack Block Kit message.
 
         Returns
         -------
         dict
             A Slack Block Kit data structure suitable for serializing to
             JSON and sending to Slack.
@@ -274,23 +269,135 @@
 
         Returns
         -------
         SlackMessage
             Slack message suitable for posting with `SlackClient`.
         """
         failed_at = format_datetime_for_logging(self.failed_at)
-        fields = [
+        fields: list[SlackBaseField] = [
             SlackTextField(heading="Exception type", text=type(self).__name__),
             SlackTextField(heading="Failed at", text=failed_at),
         ]
         if self.user:
             fields.append(SlackTextField(heading="User", text=self.user))
         return SlackMessage(message=str(self), fields=fields)
 
 
+class SlackWebException(SlackException):
+    """Parent class of exceptions arising from HTTPX_ failures.
+
+    Captures additional information from any HTTPX_ exception.  Intended to be
+    subclassed.  Subclasses may wish to override the ``to_slack`` method.
+
+    Parameters
+    ----------
+    message
+        Exception string value, which is the default Slack message.
+    failed_at
+        When the exception happened. Omit to use the current time.
+    method
+        Method of request.
+    url
+        URL of the request.
+    user
+        Username on whose behalf the request is being made.
+    status
+        Status code of failure, if any.
+    body
+        Body of failure message, if any.
+    """
+
+    @classmethod
+    def from_exception(
+        cls, exc: HTTPError, user: Optional[str] = None
+    ) -> Self:
+        """Create an exception from an HTTPX_ exception.
+
+        Parameters
+        ----------
+        exc
+            Exception from HTTPX.
+        user
+            User on whose behalf the request is being made, if known.
+
+        Returns
+        -------
+        SlackWebException
+            Newly-constructed exception.
+        """
+        if isinstance(exc, HTTPStatusError):
+            status = exc.response.status_code
+            method = exc.request.method
+            message = f"Status {status} from {method} {exc.request.url}"
+            return cls(
+                message,
+                method=exc.request.method,
+                url=str(exc.request.url),
+                user=user,
+                status=status,
+                body=exc.response.text,
+            )
+        else:
+            message = f"{type(exc).__name__}: {str(exc)}"
+            if isinstance(exc, RequestError):
+                return cls(
+                    message,
+                    method=exc.request.method,
+                    url=str(exc.request.url),
+                    user=user,
+                )
+            else:
+                return cls(message, user=user)
+
+    def __init__(
+        self,
+        message: str,
+        *,
+        failed_at: Optional[datetime] = None,
+        method: Optional[str] = None,
+        url: Optional[str] = None,
+        user: Optional[str] = None,
+        status: Optional[int] = None,
+        body: Optional[str] = None,
+    ) -> None:
+        self.message = message
+        self.method = method
+        self.url = url
+        self.status = status
+        self.body = body
+        super().__init__(message, user, failed_at=failed_at)
+
+    def __str__(self) -> str:
+        result = self.message
+        if self.body:
+            result += f"\nBody:\n{self.body}\n"
+        return result
+
+    def to_slack(self) -> SlackMessage:
+        """Convert to a Slack message for Slack alerting.
+
+        Returns
+        -------
+        SlackMessage
+            Slack message suitable for posting as an alert.
+        """
+        message = super().to_slack()
+        message.message = self.message
+        if self.url:
+            if self.method:
+                text = f"{self.method} {self.url}"
+            else:
+                text = self.url
+            message.blocks.append(SlackTextField(heading="URL", text=text))
+        if self.body:
+            block = SlackCodeBlock(heading="Response", code=self.body)
+            message.blocks.append(block)
+        return message
+
+
 def _format_and_truncate_at_end(string: str, max_length: int) -> str:
     """Format a string for Slack, truncating at the end.
 
     Slack prohibits text blocks longer than a varying number of characters
     depending on where they are in the message. If this constraint is not met,
     the whole mesage is rejected with an HTTP error. Truncate a potentially
     long message at the end.
```

### Comparing `safir-3.8.0/src/safir/slack/webhook.py` & `safir-4.0.0/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/src/safir/testing/gcs.py` & `safir-4.0.0/src/safir/testing/gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Mock Google Cloud Storage API for testing."""
 
 from __future__ import annotations
 
+from collections.abc import Iterator
 from datetime import datetime, timedelta, timezone
 from io import BufferedReader
 from pathlib import Path
-from typing import Any, Iterator, Optional
+from typing import Any, Optional
 from unittest.mock import Mock, patch
 
 from google.cloud import storage
 
 __all__ = [
     "MockBlob",
     "MockBucket",
```

### Comparing `safir-3.8.0/src/safir/testing/slack.py` & `safir-4.0.0/src/safir/testing/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Mock Slack server for testing Slack messaging."""
 
 from __future__ import annotations
 
 import json
-from typing import Any, Dict, List
+from typing import Any
 
 import respx
 from httpx import Request, Response
 
 __all__ = ["MockSlackWebhook", "mock_slack_webhook"]
 
 
@@ -20,15 +20,15 @@
         Messages that have been posted to the webhook so far.
     url
         URL that the mock has been configured to listen on.
     """
 
     def __init__(self, url: str) -> None:
         self.url = url
-        self.messages: List[Dict[str, Any]] = []
+        self.messages: list[dict[str, Any]] = []
 
     def post_webhook(self, request: Request) -> Response:
         """Callback called whenever a Slack message is posted.
 
         The provided message is stored in the messages attribute.
 
         Parameters
```

### Comparing `safir-3.8.0/src/safir/testing/uvicorn.py` & `safir-4.0.0/src/safir/testing/uvicorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utiility functions for managing an external Uvicorn test process.
 
-Normally, ASGI apps are tested via the built-in support in httpx for running
+Normally, ASGI apps are tested via the built-in support in HTTPX for running
 an ASGI app directly. However, sometimes the app has to be spawned in a
 separate process so that it can be accessed over HTTP, such as when testing it
 with Selenium or when testing Uvicorn integration. This module provides
 utility functions to aid with that test setup.
 """
 
 from __future__ import annotations
@@ -13,15 +13,15 @@
 import logging
 import os
 import socket
 import subprocess
 import time
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 
 __all__ = [
     "ServerNotListeningError",
     "UvicornProcess",
     "spawn_uvicorn",
 ]
 
@@ -80,15 +80,15 @@
 def spawn_uvicorn(
     *,
     working_directory: str | Path,
     app: Optional[str] = None,
     factory: Optional[str] = None,
     capture: bool = False,
     timeout: float = 5.0,
-    env: Optional[Dict[str, str]] = None,
+    env: Optional[dict[str, str]] = None,
 ) -> UvicornProcess:
     """Spawn an ASGI app as a separate Uvicorn process.
 
     The current working directory will always be added to the Python path, so
     ``app`` and ``factory`` can point to modules found relative to the current
     working directory, or relative to the ``working_directory`` parameter.
```

### Comparing `safir-3.8.0/src/safir.egg-info/PKG-INFO` & `safir-4.0.0/src/safir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 3.8.0
+Version: 4.0.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,33 +26,31 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://safir.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/safir
 Project-URL: Change log, https://safir.lsst.io/changelog.html
 Project-URL: Issue tracker, https://github.com/lsst-sqre/safir/issues
 Keywords: rubin,lsst
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: arq
 Provides-Extra: db
 Provides-Extra: dev
 Provides-Extra: gcs
 Provides-Extra: kubernetes
+Provides-Extra: redis
 License-File: LICENSE
 
 # Safir
 
 Safir is Rubin Observatory's library for building [FastAPI](https://fastapi.tiangolo.com/) services for the [Rubin Science Platform (Phalanx)](https://github.com/lsst-sqre/phalanx) and [Roundtable](https://github.com/lsst-sqre/roundtable) Kubernetes clusters.
 Safir is developed, maintained, and field tested by the SQuaRE team.
```

### Comparing `safir-3.8.0/src/safir.egg-info/SOURCES.txt` & `safir-4.0.0/src/safir.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -28,42 +28,54 @@
 docs/user-guide/gafaelfawr.rst
 docs/user-guide/gcs.rst
 docs/user-guide/http-client.rst
 docs/user-guide/index.rst
 docs/user-guide/ivoa.rst
 docs/user-guide/kubernetes.rst
 docs/user-guide/logging.rst
+docs/user-guide/pydantic-redis.rst
 docs/user-guide/pydantic.rst
 docs/user-guide/set-up-from-template.rst
 docs/user-guide/slack-webhook.rst
 docs/user-guide/uvicorn.rst
 docs/user-guide/x-forwarded.rst
+docs/user-guide/github-apps/api-resources.rst
+docs/user-guide/github-apps/create-a-github-client.rst
+docs/user-guide/github-apps/handling-webhooks.rst
+docs/user-guide/github-apps/index.rst
+docs/user-guide/github-apps/webhook-models.rst
 src/safir/__init__.py
 src/safir/arq.py
 src/safir/asyncio.py
 src/safir/database.py
 src/safir/datetime.py
+src/safir/fastapi.py
 src/safir/gcs.py
 src/safir/kubernetes.py
 src/safir/logging.py
 src/safir/metadata.py
 src/safir/models.py
 src/safir/py.typed
 src/safir/pydantic.py
+src/safir/redis.py
 src/safir.egg-info/PKG-INFO
 src/safir.egg-info/SOURCES.txt
 src/safir.egg-info/dependency_links.txt
 src/safir.egg-info/requires.txt
 src/safir.egg-info/top_level.txt
 src/safir/dependencies/__init__.py
 src/safir/dependencies/arq.py
 src/safir/dependencies/db_session.py
 src/safir/dependencies/gafaelfawr.py
 src/safir/dependencies/http_client.py
 src/safir/dependencies/logger.py
+src/safir/github/__init__.py
+src/safir/github/_client.py
+src/safir/github/models.py
+src/safir/github/webhooks.py
 src/safir/middleware/__init__.py
 src/safir/middleware/ivoa.py
 src/safir/middleware/x_forwarded.py
 src/safir/slack/__init__.py
 src/safir/slack/blockkit.py
 src/safir/slack/webhook.py
 src/safir/testing/__init__.py
@@ -72,26 +84,37 @@
 src/safir/testing/slack.py
 src/safir/testing/uvicorn.py
 tests/__init__.py
 tests/asyncio_test.py
 tests/conftest.py
 tests/database_test.py
 tests/datetime_test.py
+tests/fastapi_test.py
 tests/gcs_test.py
+tests/kubernetes_test.py
 tests/logging_test.py
 tests/metadata_test.py
 tests/models_test.py
 tests/pydantic_test.py
+tests/redis_test.py
 tests/safir_test.py
 tests/dependencies/__init__.py
 tests/dependencies/arq_test.py
 tests/dependencies/db_session_test.py
 tests/dependencies/gafaelfawr_test.py
 tests/dependencies/http_client_test.py
 tests/dependencies/logger_test.py
+tests/github/__init__.py
+tests/github/webhooks_test.py
+tests/github/data/webhooks/check_run_created.json
+tests/github/data/webhooks/check_suite_completed.json
+tests/github/data/webhooks/installation.json
+tests/github/data/webhooks/installation_repositories.json
+tests/github/data/webhooks/pull_request_event.json
+tests/github/data/webhooks/push_event.json
 tests/middleware/__init__.py
 tests/middleware/ivoa_test.py
 tests/middleware/x_forwarded_test.py
 tests/slack/__init__.py
 tests/slack/blockkit_test.py
 tests/slack/webhook_test.py
 tests/testing/__init__.py
```

### Comparing `safir-3.8.0/tests/database_test.py` & `safir-4.0.0/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tests/datetime_test.py` & `safir-4.0.0/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tests/dependencies/arq_test.py` & `safir-4.0.0/tests/dependencies/arq_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test `safir.dependencies.arq`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import pytest
 from arq.constants import default_queue_name
 from asgi_lifespan import LifespanManager
 from fastapi import Depends, FastAPI, HTTPException
 from httpx import AsyncClient
 
@@ -18,15 +18,15 @@
 async def test_arq_dependency_mock() -> None:
     """Test the arq dependency entirely through the MockArqQueue."""
     app = FastAPI()
 
     @app.post("/")
     async def post_job(
         arq_queue: MockArqQueue = Depends(arq_dependency),
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Create a job."""
         job = await arq_queue.enqueue("test_task", "hello", a_number=42)
         return {
             "job_id": job.id,
             "job_status": job.status,
             "job_name": job.name,
             "job_args": job.args,
@@ -35,15 +35,15 @@
         }
 
     @app.get("/jobs/{job_id}")
     async def get_metadata(
         job_id: str,
         queue_name: Optional[str] = None,
         arq_queue: MockArqQueue = Depends(arq_dependency),
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Get metadata about a job."""
         try:
             job = await arq_queue.get_job_metadata(
                 job_id, queue_name=queue_name
             )
         except JobNotFound:
             raise HTTPException(status_code=404)
@@ -57,15 +57,15 @@
         }
 
     @app.get("/results/{job_id}")
     async def get_result(
         job_id: str,
         queue_name: Optional[str] = None,
         arq_queue: MockArqQueue = Depends(arq_dependency),
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Get the results for a job."""
         try:
             job_result = await arq_queue.get_job_result(
                 job_id, queue_name=queue_name
             )
         except (JobNotFound, JobResultUnavailable) as e:
             raise HTTPException(status_code=404, detail=str(e))
```

### Comparing `safir-3.8.0/tests/dependencies/db_session_test.py` & `safir-4.0.0/tests/dependencies/db_session_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests for the database session dependency."""
 
 from __future__ import annotations
 
 import os
-from typing import List
 
 import pytest
 import structlog
 from fastapi import Depends, FastAPI
 from httpx import AsyncClient
 from sqlalchemy import Column, String
 from sqlalchemy.ext.asyncio import async_scoped_session
@@ -53,15 +52,15 @@
     ) -> None:
         async with session.begin():
             session.add(User(username="foo"))
 
     @app.get("/list")
     async def get_list(
         session: async_scoped_session = Depends(db_session_dependency),
-    ) -> List[str]:
+    ) -> list[str]:
         async with session.begin():
             result = await session.scalars(select(User.username))
             return list(result.all())
 
     async with AsyncClient(app=app, base_url="https://example.com") as client:
         r = await client.get("/list")
         assert r.status_code == 200
```

### Comparing `safir-3.8.0/tests/dependencies/gafaelfawr_test.py` & `safir-4.0.0/tests/dependencies/gafaelfawr_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Test the Gafaelfawr auth FastAPI dependencies."""
 
 from __future__ import annotations
 
 import json
-from typing import Dict
 from unittest.mock import ANY
 
 import pytest
 from _pytest.logging import LogCaptureFixture
 from fastapi import Depends, FastAPI
 from httpx import AsyncClient
 from structlog.stdlib import BoundLogger
@@ -20,15 +19,15 @@
 
 
 @pytest.mark.asyncio
 async def test_auth_dependency() -> None:
     app = FastAPI()
 
     @app.get("/")
-    async def handler(user: str = Depends(auth_dependency)) -> Dict[str, str]:
+    async def handler(user: str = Depends(auth_dependency)) -> dict[str, str]:
         return {"user": user}
 
     async with AsyncClient(app=app, base_url="https://example.com") as client:
         r = await client.get("/")
         assert r.status_code == 422
 
         r = await client.get("/", headers={"X-Auth-Request-User": "someuser"})
@@ -41,15 +40,15 @@
     configure_logging(name="myapp", profile="production", log_level="info")
 
     app = FastAPI()
 
     @app.get("/")
     async def handler(
         logger: BoundLogger = Depends(auth_logger_dependency),
-    ) -> Dict[str, str]:
+    ) -> dict[str, str]:
         logger.info("something")
         return {}
 
     caplog.clear()
     async with AsyncClient(app=app, base_url="https://example.com") as client:
         r = await client.get("/", headers={"User-Agent": ""})
         assert r.status_code == 422
```

### Comparing `safir-3.8.0/tests/dependencies/http_client_test.py` & `safir-4.0.0/tests/dependencies/http_client_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """Test the HTTP client FastAPI dependency."""
 
 from __future__ import annotations
 
-from typing import Dict, List
-
 import pytest
 import respx
 from asgi_lifespan import LifespanManager
 from fastapi import Depends, FastAPI
 from httpx import AsyncClient
 
 from safir.dependencies.http_client import http_client_dependency
 
 
 @pytest.fixture
-def non_mocked_hosts() -> List[str]:
+def non_mocked_hosts() -> list[str]:
     return ["example.com"]
 
 
 @pytest.mark.asyncio
 async def test_http_client(respx_mock: respx.Router) -> None:
     app = FastAPI()
     respx_mock.get("https://www.google.com").respond(200)
 
     @app.get("/")
     async def handler(
         http_client: AsyncClient = Depends(http_client_dependency),
-    ) -> Dict[str, str]:
+    ) -> dict[str, str]:
         assert isinstance(http_client, AsyncClient)
         await http_client.get("https://www.google.com")
         return {}
 
     @app.on_event("shutdown")
     async def shutdown_event() -> None:
         await http_client_dependency.aclose()
```

### Comparing `safir-3.8.0/tests/dependencies/logger_test.py` & `safir-4.0.0/tests/dependencies/logger_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """Test the logger FastAPI dependency."""
 
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Dict
 from unittest.mock import ANY
 
 import pytest
+from _pytest.logging import LogCaptureFixture
 from fastapi import Depends, FastAPI
 from httpx import AsyncClient
 from structlog.stdlib import BoundLogger
 
 from safir.dependencies.logger import logger_dependency
 from safir.logging import configure_logging
 from safir.middleware.x_forwarded import XForwardedMiddleware
 
-if TYPE_CHECKING:
-    from _pytest.logging import LogCaptureFixture
-
 
 @pytest.mark.asyncio
 async def test_logger(caplog: LogCaptureFixture) -> None:
     configure_logging(name="myapp", profile="production", log_level="info")
 
     app = FastAPI()
 
     @app.get("/")
     async def handler(
         logger: BoundLogger = Depends(logger_dependency),
-    ) -> Dict[str, str]:
+    ) -> dict[str, str]:
         logger.info("something", param="value")
         return {}
 
     caplog.clear()
     async with AsyncClient(app=app, base_url="http://example.com") as client:
         r = await client.get(
             "/", headers={"User-Agent": "some-user-agent/1.0"}
@@ -61,15 +58,15 @@
 
     app = FastAPI()
     app.add_middleware(XForwardedMiddleware)
 
     @app.get("/")
     async def handler(
         logger: BoundLogger = Depends(logger_dependency),
-    ) -> Dict[str, str]:
+    ) -> dict[str, str]:
         logger.info("something", param="value")
         return {}
 
     caplog.clear()
     async with AsyncClient(app=app, base_url="http://example.com") as client:
         r = await client.get(
             "/",
```

### Comparing `safir-3.8.0/tests/gcs_test.py` & `safir-4.0.0/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tests/logging_test.py` & `safir-4.0.0/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tests/metadata_test.py` & `safir-4.0.0/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tests/middleware/ivoa_test.py` & `safir-4.0.0/tests/middleware/ivoa_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Test IVOA middleware."""
 
 from __future__ import annotations
 
-from typing import Dict
-
 import pytest
 from fastapi import FastAPI
 from httpx import AsyncClient
 
 from safir.middleware.ivoa import CaseInsensitiveQueryMiddleware
 
 
@@ -19,15 +17,15 @@
 
 
 @pytest.mark.asyncio
 async def test_case_insensitive() -> None:
     app = build_app()
 
     @app.get("/")
-    async def handler(param: str) -> Dict[str, str]:
+    async def handler(param: str) -> dict[str, str]:
         return {"param": param}
 
     async with AsyncClient(app=app, base_url="https://example.com") as client:
         r = await client.get("/", params={"param": "foo"})
         assert r.status_code == 200
         assert r.json() == {"param": "foo"}
```

### Comparing `safir-3.8.0/tests/middleware/x_forwarded_test.py` & `safir-4.0.0/tests/middleware/x_forwarded_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Test ``X-Forwarded-For`` middleware."""
 
 from __future__ import annotations
 
 from ipaddress import _BaseNetwork, ip_network
-from typing import Dict, List, Optional
+from typing import Optional
 
 import pytest
 from fastapi import FastAPI, Request
 from httpx import AsyncClient
 
 from safir.middleware.x_forwarded import XForwardedMiddleware
 
 
-def build_app(proxies: Optional[List[_BaseNetwork]] = None) -> FastAPI:
+def build_app(proxies: Optional[list[_BaseNetwork]] = None) -> FastAPI:
     """Construct a test FastAPI app with the middleware registered."""
     app = FastAPI()
     app.add_middleware(XForwardedMiddleware, proxies=proxies)
     return app
 
 
 @pytest.mark.asyncio
 async def test_ok() -> None:
     app = build_app([ip_network("11.0.0.0/8")])
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert request.client
         assert request.client.host == "10.10.10.10"
         assert request.state.forwarded_host == "foo.example.com"
         assert request.url == "https://foo.example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -45,15 +45,15 @@
 
 
 @pytest.mark.asyncio
 async def test_defaults() -> None:
     app = build_app()
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert request.client
         assert request.client.host == "192.168.0.1"
         assert request.state.forwarded_host == "foo.example.com"
         assert request.url == "http://example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -69,15 +69,15 @@
 
 
 @pytest.mark.asyncio
 async def test_no_forwards() -> None:
     app = build_app([ip_network("127.0.0.1")])
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert not request.state.forwarded_host
         assert request.client
         assert request.client.host == "127.0.0.1"
         assert request.url == "http://example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -86,15 +86,15 @@
 
 
 @pytest.mark.asyncio
 async def test_all_filtered() -> None:
     app = build_app([ip_network("10.0.0.0/8")])
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert request.client
         assert request.client.host == "10.10.10.10"
         assert request.state.forwarded_host == "foo.example.com"
         assert request.url == "https://example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -110,15 +110,15 @@
 
 
 @pytest.mark.asyncio
 async def test_one_proto() -> None:
     app = build_app([ip_network("11.11.11.11")])
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert request.client
         assert request.client.host == "10.10.10.10"
         assert request.state.forwarded_host == "foo.example.com"
         assert request.url == "https://example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -134,15 +134,15 @@
 
 
 @pytest.mark.asyncio
 async def test_no_proto_or_host() -> None:
     app = build_app([ip_network("11.11.11.11")])
 
     @app.get("/")
-    async def handler(request: Request) -> Dict[str, str]:
+    async def handler(request: Request) -> dict[str, str]:
         assert not request.state.forwarded_host
         assert request.client
         assert request.client.host == "10.10.10.10"
         assert request.url == "http://example.com/"
         return {}
 
     async with AsyncClient(app=app, base_url="http://example.com") as client:
@@ -152,15 +152,15 @@
     assert r.status_code == 200
 
 
 @pytest.mark.asyncio
 async def test_too_many_headers() -> None:
     """Test handling of duplicate headers.
 
-    httpx doesn't allow passing in duplicate headers, so we cannot test end to
+    HTTPX doesn't allow passing in duplicate headers, so we cannot test end to
     end.  Instead, test by generating a mock request and then calling the
     underling middleware functions directly.
     """
     state = {
         "type": "http",
         "headers": [
             ("X-Forwarded-For", "10.10.10.10"),
```

### Comparing `safir-3.8.0/tests/pydantic_test.py` & `safir-4.0.0/tests/pydantic_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tests for Pydantic utility functions."""
 
 from __future__ import annotations
 
 import json
 from datetime import datetime, timedelta, timezone
+from typing import Optional
 
 import pytest
+from pydantic import BaseModel, ValidationError, root_validator
 
 from safir.pydantic import (
     CamelCaseModel,
     normalize_datetime,
     normalize_isodatetime,
     to_camel_case,
     validate_exactly_one_of,
@@ -89,32 +91,44 @@
     assert not data.replace_403
     assert data.foo_bar_baz == "something"
     assert snake_data.dict() == data.dict()
     assert snake_data.json() == data.json()
 
 
 def test_validate_exactly_one_of() -> None:
-    values = {"foo": 4, "bar": None}
-    validate_exactly_one_of("foo", "bar")(None, values)
+    class Model(BaseModel):
+        foo: Optional[int] = None
+        bar: Optional[int] = None
+        baz: Optional[int] = None
+
+        _validate_type = root_validator(allow_reuse=True)(
+            validate_exactly_one_of("foo", "bar", "baz")
+        )
+
+    Model.parse_obj({"foo": 4, "bar": None})
+    Model.parse_obj({"baz": 4})
+    Model.parse_obj({"bar": 4})
+    Model.parse_obj({"foo": None, "bar": 4})
 
-    values = {"foo": 4}
-    validate_exactly_one_of("foo", "bar", "baz")(None, values)
+    with pytest.raises(ValidationError) as excinfo:
+        Model.parse_obj({"foo": 4, "bar": 3, "baz": None})
+    assert "only one of foo, bar, and baz may be given" in str(excinfo.value)
+
+    with pytest.raises(ValidationError) as excinfo:
+        Model.parse_obj({"foo": None, "baz": None})
+    assert "one of foo, bar, and baz must be given" in str(excinfo.value)
 
-    validate_exactly_one_of("foo", "bar")(4, {})
-    validate_exactly_one_of("foo", "bar")(4, {"foo": None})
+    class TwoModel(BaseModel):
+        foo: Optional[int] = None
+        bar: Optional[int] = None
+
+        _validate_type = root_validator(allow_reuse=True)(
+            validate_exactly_one_of("foo", "bar")
+        )
 
-    with pytest.raises(ValueError) as excinfo:
-        validate_exactly_one_of("foo", "bar")(3, values)
+    with pytest.raises(ValidationError) as excinfo:
+        TwoModel.parse_obj({"foo": 3, "bar": 4})
     assert "only one of foo and bar may be given" in str(excinfo.value)
 
-    with pytest.raises(ValueError) as excinfo:
-        validate_exactly_one_of("foo", "bar")(None, {})
+    with pytest.raises(ValidationError) as excinfo:
+        TwoModel.parse_obj({})
     assert "one of foo and bar must be given" in str(excinfo.value)
-
-    values = {"foo": 4, "bar": 3}
-    with pytest.raises(ValueError) as excinfo:
-        validate_exactly_one_of("foo", "bar", "baz")(None, values)
-    assert "only one of foo, bar, and baz may be given" in str(excinfo.value)
-
-    with pytest.raises(ValueError) as excinfo:
-        validate_exactly_one_of("foo", "bar", "baz")(None, {"foo": None})
-    assert "one of foo, bar, and baz must be given" in str(excinfo.value)
```

### Comparing `safir-3.8.0/tests/slack/webhook_test.py` & `safir-4.0.0/tests/slack/webhook_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     @router.get("/known")
     async def get_known() -> None:
         raise OtherAppError("Slack exception")
 
     app = FastAPI()
     app.include_router(router)
 
-    # We need a custom httpx configuration to disable raising server
+    # We need a custom HTTPX configuration to disable raising server
     # exceptions so that we can inspect the resulting error handling.
     transport = ASGITransport(
         app=app,  # type: ignore[arg-type]
         raise_app_exceptions=False,
     )
 
     # Run the test.
```

### Comparing `safir-3.8.0/tests/testing/gcs_test.py` & `safir-4.0.0/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-3.8.0/tox.ini` & `safir-4.0.0/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -18,27 +18,40 @@
     --host=127.0.0.1 --quiet --no-align --tuples-only \
     -1 --command="SELECT 1"
 healthcheck_timeout = 1
 healthcheck_retries = 30
 healthcheck_interval = 1
 healthcheck_start_period = 1
 
+[docker:redis]
+image = redis:latest
+ports =
+    6379:6379/tcp
+healthcheck_cmd =
+    redis-cli ping
+healthcheck_timeout = 1
+healthcheck_retries = 30
+healthcheck_interval = 1
+healthcheck_start_period = 1
+
 [testenv]
 description = Run pytest against {envname}.
 extras =
     arq
     db
     dev
     gcs
     kubernetes
+    redis
 
 [testenv:py]
 description = Run pytest with PostgreSQL via Docker.
 docker =
     postgres
+    redis
 commands =
     coverage run -m pytest {posargs}
 setenv =
     TEST_DATABASE_URL = postgresql://safir@127.0.0.1/safir
     TEST_DATABASE_PASSWORD = INSECURE@%PASSWORD/
 
 [testenv:coverage-report]
```

