# Comparing `tmp/adafruit-circuitpython-httpserver-2.4.0.tar.gz` & `tmp/adafruit-circuitpython-httpserver-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-2.4.0.tar", last modified: Mon Apr  3 15:30:35 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-2.5.0.tar", last modified: Wed Apr 19 17:03:25 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-2.4.0.tar` & `adafruit-circuitpython-httpserver-2.5.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.769618 adafruit-circuitpython-httpserver-2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.761618 adafruit-circuitpython-httpserver-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.761618 adafruit-circuitpython-httpserver-2.4.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.761618 adafruit-circuitpython-httpserver-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.761618 adafruit-circuitpython-httpserver-2.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-03 15:30:35.769618 adafruit-circuitpython-httpserver-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.765618 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-03 15:30:35.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-03 15:30:35.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:30:35.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-03 15:30:35.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 15:30:35.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.765618 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.765618 adafruit-circuitpython-httpserver-2.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.765618 adafruit-circuitpython-httpserver-2.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:30:35.769618 adafruit-circuitpython-httpserver-2.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_simple_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_simple_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-03 15:30:28.000000 adafruit-circuitpython-httpserver-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-03 15:30:16.000000 adafruit-circuitpython-httpserver-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:30:35.769618 adafruit-circuitpython-httpserver-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.719733 adafruit-circuitpython-httpserver-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.723733 adafruit-circuitpython-httpserver-2.5.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.723733 adafruit-circuitpython-httpserver-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.723733 adafruit-circuitpython-httpserver-2.5.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.723733 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-19 17:03:25.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 17:03:25.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:03:25.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 17:03:25.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 17:03:25.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_simple_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_simple_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-19 17:03:18.000000 adafruit-circuitpython-httpserver-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 17:03:08.000000 adafruit-circuitpython-httpserver-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:03:25.727733 adafruit-circuitpython-httpserver-2.5.0/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-2.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/.gitignore` & `adafruit-circuitpython-httpserver-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-2.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/.pylintrc` & `adafruit-circuitpython-httpserver-2.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-2.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/LICENSE` & `adafruit-circuitpython-httpserver-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-2.5.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-2.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-2.5.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/PKG-INFO` & `adafruit-circuitpython-httpserver-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 2.4.0
+Version: 2.5.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/README.rst` & `adafruit-circuitpython-httpserver-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 2.4.0
+Version: 2.5.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/methods.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/mime_type.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/mime_type.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/response.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         self._response_already_sent = True
 
     def send_file(
         self,
         filename: str = "index.html",
         root_path: str = "./",
         buffer_size: int = 1024,
+        head_only: bool = False,
     ) -> None:
         """
         Send response with content of ``filename`` located in ``root_path``.
         Implicitly calls ``_send_headers`` before sending the file content.
         File is send split into ``buffer_size`` parts.
 
         Should be called **only once** per response.
@@ -193,17 +194,18 @@
             return
 
         self._send_headers(
             content_type=MIMEType.from_file_name(filename),
             content_length=file_length,
         )
 
-        with open(root_path + filename, "rb") as file:
-            while bytes_read := file.read(buffer_size):
-                self._send_bytes(self.request.connection, bytes_read)
+        if not head_only:
+            with open(root_path + filename, "rb") as file:
+                while bytes_read := file.read(buffer_size):
+                    self._send_bytes(self.request.connection, bytes_read)
         self._response_already_sent = True
 
     def send_chunk(self, chunk: str = "") -> None:
         """
         Sends chunk of response.
 
         Should be used **only** inside
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/route.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             @server.route("/example/<my_parameter>", HTTPMethod.GET)
             def route_func(request, my_parameter):
                 ...
                 request.path == "/example/123" # True
                 my_parameter == "123" # True
         """
         if not self._routes:
-            raise ValueError("No routes added")
+            return None
 
         found_route, _route = False, None
 
         for _route in self._routes:
             matches, url_parameters_values = _route.match(route)
 
             if matches:
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,20 +163,24 @@
                 )
 
                 # If a handler for route exists and is callable, call it.
                 if handler is not None and callable(handler):
                     handler(request)
 
                 # If no handler exists and request method is GET, try to serve a file.
-                elif handler is None and request.method == HTTPMethod.GET:
+                elif handler is None and request.method in (
+                    HTTPMethod.GET,
+                    HTTPMethod.HEAD,
+                ):
                     filename = "index.html" if request.path == "/" else request.path
                     HTTPResponse(request).send_file(
                         filename=filename,
                         root_path=self.root_path,
                         buffer_size=self.request_buffer_size,
+                        head_only=(request.method == HTTPMethod.HEAD),
                     )
                 else:
                     HTTPResponse(
                         request, status=CommonHTTPStatus.BAD_REQUEST_400
                     ).send()
 
         except OSError as ex:
```

### Comparing `adafruit-circuitpython-httpserver-2.4.0/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-2.5.0/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-2.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/docs/api.rst` & `adafruit-circuitpython-httpserver-2.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/docs/conf.py` & `adafruit-circuitpython-httpserver-2.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/docs/examples.rst` & `adafruit-circuitpython-httpserver-2.5.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/docs/index.rst` & `adafruit-circuitpython-httpserver-2.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_simple_poll.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_simple_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_simple_serve.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_simple_serve.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-2.5.0/examples/httpserver_url_parameters.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-2.4.0/pyproject.toml` & `adafruit-circuitpython-httpserver-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "2.4.0"
+version = "2.5.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

