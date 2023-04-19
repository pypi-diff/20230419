# Comparing `tmp/adafruit-circuitpython-wiznet5k-2.4.0.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.4.0.tar", last modified: Mon Mar 20 21:24:17 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.4.1.tar", last modified: Wed Apr 19 17:52:22 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-2.4.0.tar` & `adafruit-circuitpython-wiznet5k-2.4.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.071248 adafruit-circuitpython-wiznet5k-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.075248 adafruit-circuitpython-wiznet5k-2.4.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.075248 adafruit-circuitpython-wiznet5k-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.075248 adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.075248 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-20 21:24:17.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-20 21:24:17.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 21:24:17.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-20 21:24:17.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-20 21:24:17.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44913 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-20 21:23:59.000000 adafruit-circuitpython-wiznet5k-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:24:17.079248 adafruit-circuitpython-wiznet5k-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/tests/extract_unique_dns_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/tests/test_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/tests/test_dns_server_nonbreaking_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-20 21:24:08.000000 adafruit-circuitpython-wiznet5k-2.4.0/tests/test_parse_dns_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44913 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/extract_unique_dns_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dns_server_nonbreaking_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_parse_dns_function.py
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/.gitignore` & `adafruit-circuitpython-wiznet5k-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/.pylintrc` & `adafruit-circuitpython-wiznet5k-2.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-2.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/LICENSE` & `adafruit-circuitpython-wiznet5k-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.4.0
+Version: 2.4.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/README.rst` & `adafruit-circuitpython-wiznet5k-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.4.0
+Version: 2.4.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     if TYPE_CHECKING:
         from circuitpython_typing import WriteableBuffer
         import busio
         import digitalio
 except ImportError:
     pass
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files 24% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 _DNS_SERVERS = 6
 _DHCP_SERVER_ID = 54
 _T1_VAL = 58
 _T2_VAL = 59
 _LEASE_TIME = 51
 _OPT_END = 255
 
-# Packet buffer
-_BUFF = bytearray(318)
+# Packet buffer size
+_BUFF_SIZE = const(318)
 
 
 class DHCP:
     """W5k DHCP Client implementation."""
 
     # pylint: disable=too-many-arguments, too-many-instance-attributes, invalid-name
     def __init__(
@@ -162,195 +162,194 @@
         """
         Assemble and send a DHCP message packet to a socket.
 
         :param int state: DHCP Message state.
         :param float time_elapsed: Number of seconds elapsed since DHCP process started
         :param bool renew: Set True for renew and rebind, defaults to False
         """
-        _BUFF[:] = b"\x00" * len(_BUFF)
+        buff = bytearray(_BUFF_SIZE)
         # OP
-        _BUFF[0] = _DHCP_BOOT_REQUEST
+        buff[0] = _DHCP_BOOT_REQUEST
         # HTYPE
-        _BUFF[1] = _DHCP_HTYPE10MB
+        buff[1] = _DHCP_HTYPE10MB
         # HLEN
-        _BUFF[2] = _DHCP_HLENETHERNET
+        buff[2] = _DHCP_HLENETHERNET
         # HOPS
-        _BUFF[3] = _DHCP_HOPS
+        buff[3] = _DHCP_HOPS
 
         # Transaction ID (xid)
         self._initial_xid = htonl(self._transaction_id)
         self._initial_xid = self._initial_xid.to_bytes(4, "big")
-        _BUFF[4:8] = self._initial_xid
+        buff[4:8] = self._initial_xid
 
         # seconds elapsed
-        _BUFF[8] = (int(time_elapsed) & 0xFF00) >> 8
-        _BUFF[9] = int(time_elapsed) & 0x00FF
+        buff[8] = (int(time_elapsed) & 0xFF00) >> 8
+        buff[9] = int(time_elapsed) & 0x00FF
 
         # flags
         flags = htons(0x8000)
         flags = flags.to_bytes(2, "big")
-        _BUFF[10] = flags[1]
-        _BUFF[11] = flags[0]
+        buff[10] = flags[1]
+        buff[11] = flags[0]
 
         # NOTE: Skipping ciaddr/yiaddr/siaddr/giaddr
         # as they're already set to 0.0.0.0
         # Except when renewing, then fill in ciaddr
         if renew:
-            _BUFF[12:16] = bytes(self.local_ip)
+            buff[12:16] = bytes(self.local_ip)
 
         # chaddr
-        _BUFF[28:34] = self._mac_address
+        buff[28:34] = self._mac_address
 
         # NOTE:  192 octets of 0's, BOOTP legacy
 
         # Magic Cookie
-        _BUFF[236:240] = _MAGIC_COOKIE
+        buff[236:240] = _MAGIC_COOKIE
 
         # Option - DHCP Message Type
-        _BUFF[240] = 53
-        _BUFF[241] = 0x01
-        _BUFF[242] = state
+        buff[240] = 53
+        buff[241] = 0x01
+        buff[242] = state
 
         # Option - Client Identifier
-        _BUFF[243] = 61
+        buff[243] = 61
         # Length
-        _BUFF[244] = 0x07
+        buff[244] = 0x07
         # HW Type - ETH
-        _BUFF[245] = 0x01
+        buff[245] = 0x01
         # Client MAC Address
         for mac, val in enumerate(self._mac_address):
-            _BUFF[246 + mac] = val
+            buff[246 + mac] = val
 
         # Option - Host Name
-        _BUFF[252] = 12
+        buff[252] = 12
         hostname_len = len(self._hostname)
         after_hostname = 254 + hostname_len
-        _BUFF[253] = hostname_len
-        _BUFF[254:after_hostname] = self._hostname
+        buff[253] = hostname_len
+        buff[254:after_hostname] = self._hostname
 
         if state == _DHCP_REQUEST and not renew:
             # Set the parsed local IP addr
-            _BUFF[after_hostname] = 50
-            _BUFF[after_hostname + 1] = 0x04
-            _BUFF[after_hostname + 2 : after_hostname + 6] = bytes(self.local_ip)
+            buff[after_hostname] = 50
+            buff[after_hostname + 1] = 0x04
+            buff[after_hostname + 2 : after_hostname + 6] = bytes(self.local_ip)
             # Set the parsed dhcp server ip addr
-            _BUFF[after_hostname + 6] = 54
-            _BUFF[after_hostname + 7] = 0x04
-            _BUFF[after_hostname + 8 : after_hostname + 12] = bytes(self.dhcp_server_ip)
+            buff[after_hostname + 6] = 54
+            buff[after_hostname + 7] = 0x04
+            buff[after_hostname + 8 : after_hostname + 12] = bytes(self.dhcp_server_ip)
 
-        _BUFF[after_hostname + 12] = 55
-        _BUFF[after_hostname + 13] = 0x06
+        buff[after_hostname + 12] = 55
+        buff[after_hostname + 13] = 0x06
         # subnet mask
-        _BUFF[after_hostname + 14] = 1
+        buff[after_hostname + 14] = 1
         # routers on subnet
-        _BUFF[after_hostname + 15] = 3
+        buff[after_hostname + 15] = 3
         # DNS
-        _BUFF[after_hostname + 16] = 6
+        buff[after_hostname + 16] = 6
         # domain name
-        _BUFF[after_hostname + 17] = 15
+        buff[after_hostname + 17] = 15
         # renewal (T1) value
-        _BUFF[after_hostname + 18] = 58
+        buff[after_hostname + 18] = 58
         # rebinding (T2) value
-        _BUFF[after_hostname + 19] = 59
-        _BUFF[after_hostname + 20] = 255
+        buff[after_hostname + 19] = 59
+        buff[after_hostname + 20] = 255
 
         # Send DHCP packet
-        self._sock.send(_BUFF)
+        self._sock.send(buff)
 
     # pylint: disable=too-many-branches, too-many-statements
     def parse_dhcp_response(
         self,
     ) -> Tuple[int, bytearray]:
         """Parse DHCP response from DHCP server.
 
         :return Tuple[int, bytearray]: DHCP packet type and ID.
         """
-        global _BUFF  # pylint: disable=global-statement
         # store packet in buffer
-        _BUFF = bytearray(self._sock.recv(len(_BUFF)))
+        buff = bytearray(self._sock.recv(_BUFF_SIZE))
         if self._debug:
-            print("DHCP Response: ", _BUFF)
+            print("DHCP Response: ", buff)
 
         # -- Parse Packet, FIXED -- #
         # Validate OP
-        if _BUFF[0] != _DHCP_BOOT_REPLY:
+        if buff[0] != _DHCP_BOOT_REPLY:
             raise RuntimeError(
                 "Malformed Packet - \
             DHCP message OP is not expected BOOT Reply."
             )
 
-        xid = _BUFF[4:8]
+        xid = buff[4:8]
         if bytes(xid) != self._initial_xid:
             raise ValueError("DHCP response ID mismatch.")
 
-        self.local_ip = tuple(_BUFF[16:20])
+        self.local_ip = tuple(buff[16:20])
         # Check that there is a server ID.
-        if _BUFF[28:34] == b"\x00\x00\x00\x00\x00\x00":
+        if buff[28:34] == b"\x00\x00\x00\x00\x00\x00":
             raise ValueError("No DHCP server ID in the response.")
 
-        if _BUFF[236:240] != _MAGIC_COOKIE:
+        if buff[236:240] != _MAGIC_COOKIE:
             raise ValueError("No DHCP Magic Cookie in the response.")
 
         # -- Parse Packet, VARIABLE -- #
         ptr = 240
-        while _BUFF[ptr] != _OPT_END:
-            if _BUFF[ptr] == _MSG_TYPE:
+        while buff[ptr] != _OPT_END:
+            if buff[ptr] == _MSG_TYPE:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += opt_len
-                msg_type = _BUFF[ptr]
+                msg_type = buff[ptr]
                 ptr += 1
-            elif _BUFF[ptr] == _SUBNET_MASK:
+            elif buff[ptr] == _SUBNET_MASK:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self.subnet_mask = tuple(_BUFF[ptr : ptr + opt_len])
+                self.subnet_mask = tuple(buff[ptr : ptr + opt_len])
                 ptr += opt_len
-            elif _BUFF[ptr] == _DHCP_SERVER_ID:
+            elif buff[ptr] == _DHCP_SERVER_ID:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self.dhcp_server_ip = tuple(_BUFF[ptr : ptr + opt_len])
+                self.dhcp_server_ip = tuple(buff[ptr : ptr + opt_len])
                 ptr += opt_len
-            elif _BUFF[ptr] == _LEASE_TIME:
+            elif buff[ptr] == _LEASE_TIME:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self._lease_time = int.from_bytes(_BUFF[ptr : ptr + opt_len], "big")
+                self._lease_time = int.from_bytes(buff[ptr : ptr + opt_len], "big")
                 ptr += opt_len
-            elif _BUFF[ptr] == _ROUTERS_ON_SUBNET:
+            elif buff[ptr] == _ROUTERS_ON_SUBNET:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self.gateway_ip = tuple(_BUFF[ptr : ptr + 4])
+                self.gateway_ip = tuple(buff[ptr : ptr + 4])
                 ptr += opt_len
-            elif _BUFF[ptr] == _DNS_SERVERS:
+            elif buff[ptr] == _DNS_SERVERS:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self.dns_server_ip = tuple(_BUFF[ptr : ptr + 4])
+                self.dns_server_ip = tuple(buff[ptr : ptr + 4])
                 ptr += opt_len  # still increment even though we only read 1 addr.
-            elif _BUFF[ptr] == _T1_VAL:
+            elif buff[ptr] == _T1_VAL:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self._t1 = int.from_bytes(_BUFF[ptr : ptr + opt_len], "big")
+                self._t1 = int.from_bytes(buff[ptr : ptr + opt_len], "big")
                 ptr += opt_len
-            elif _BUFF[ptr] == _T2_VAL:
+            elif buff[ptr] == _T2_VAL:
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
-                self._t2 = int.from_bytes(_BUFF[ptr : ptr + opt_len], "big")
+                self._t2 = int.from_bytes(buff[ptr : ptr + opt_len], "big")
                 ptr += opt_len
-            elif _BUFF[ptr] == 0:
+            elif buff[ptr] == 0:
                 break
             else:
                 # We're not interested in this option
                 ptr += 1
-                opt_len = _BUFF[ptr]
+                opt_len = buff[ptr]
                 ptr += 1
                 # no-op
                 ptr += opt_len
 
         if self._debug:
             print(
                 "Msg Type: {}\nSubnet Mask: {}\nDHCP Server IP: {}\nDNS Server IP: {}\
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 
 import time
 from random import getrandbits
 from micropython import const
-import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
 _QUERY_FLAG = const(0x00)
 _OPCODE_STANDARD_QUERY = const(0x00)
 _RECURSION_DESIRED_FLAG = 1 << 8
 
 _TYPE_A = const(0x0001)
 _CLASS_IN = const(0x0001)
@@ -225,18 +224,19 @@
         """
         :param adafruit_wiznet5k.WIZNET5K: Ethernet network connection.
         :param Union[str, Tuple[int, int, int, int]]: IP address of the DNS server.
         :param bool debug: Enable debugging messages, defaults to False.
         """
         self._debug = debug
         self._iface = iface
-        socket.set_interface(iface)
-        self._sock = socket.socket(type=socket.SOCK_DGRAM)
-        self._sock.settimeout(1)
-        self._dns_server = dns_address
+        self._dns_server = (
+            self._iface.unpretty_ip(dns_address)
+            if isinstance(dns_address, str)
+            else dns_address
+        )
         self._query_id = 0  # Request ID.
         self._query_length = 0  # Length of last query.
 
     def gethostbyname(self, hostname: bytes) -> Union[int, bytes]:
         """
         DNS look up of a host name.
 
@@ -247,39 +247,37 @@
 
         if self._dns_server is None:
             return _INVALID_SERVER
         # build DNS request packet
         self._query_id, self._query_length, buffer = _build_dns_query(hostname)
 
         # Send DNS request packet
-        self._sock.bind(("", _DNS_PORT))
-        self._sock.connect((self._dns_server, _DNS_PORT))
+        dns_socket = self._iface.get_socket()
+        self._iface.socket_connect(
+            dns_socket, bytes(self._dns_server), _DNS_PORT, conn_mode=0x02
+        )
         _debug_print(debug=self._debug, message="* DNS: Sending request packet...")
-        self._sock.send(buffer)
+        self._iface.socket_write(dns_socket, buffer)
 
         # Read and parse the DNS response
         ipaddress = -1
         for _ in range(5):
             #  wait for a response
             socket_timeout = time.monotonic() + 1.0
-            packet_size = self._sock._available()  # pylint: disable=protected-access
-            while packet_size == 0:
-                packet_size = (
-                    self._sock._available()  # pylint: disable=protected-access
-                )
+            while not self._iface.socket_available(dns_socket, 0x02):
                 if time.monotonic() > socket_timeout:
                     _debug_print(
                         debug=self._debug,
                         message="* DNS ERROR: Did not receive DNS response (socket timeout).",
                     )
-                    self._sock.close()
-                    return -1
+                    self._iface.socket_close(dns_socket)
+                    raise RuntimeError("Failed to resolve hostname!")
                 time.sleep(0.05)
             # recv packet into buf
-            buffer = self._sock.recv(512)  # > UDP payload length
+            _, buffer = self._iface.read_udp(dns_socket, 512)
             _debug_print(
                 debug=self._debug,
                 message="DNS Packet Received: {}".format(buffer),
             )
             try:
                 ipaddress = _parse_dns_response(
                     response=buffer,
@@ -290,9 +288,9 @@
                 break
             except ValueError as error:
                 _debug_print(
                     debug=self._debug,
                     message="* DNS ERROR: Failed to resolve DNS response, retrying…\n"
                     "    ({}).".format(error.args[0]),
                 )
-        self._sock.close()
+        self._iface.socket_close(dns_socket)
         return ipaddress
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 import time
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
-# __version__ = "2.4.0"
+# __version__ = "2.4.1"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 
 class NTP:
     """Wiznet5k NTP Client."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,16 @@
         only some of the data was transmitted, the application needs to attempt
         delivery of the remaining data.
 
         :param bytearray data: Data to send to the socket.
 
         :return int: Number of bytes sent.
         """
-        bytes_sent = _the_interface.socket_write(self._socknum, data, self._timeout)
+        timeout = 0 if self._timeout is None else self._timeout
+        bytes_sent = _the_interface.socket_write(self._socknum, data, timeout)
         gc.collect()
         return bytes_sent
 
     @_check_socket_closed
     def sendto(self, data: bytearray, *flags_and_or_address: any) -> int:
         """
         Send data to the socket. The socket should not be connected to a remote socket, since the
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/docs/api.rst` & `adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/docs/conf.py` & `adafruit-circuitpython-wiznet5k-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/docs/index.rst` & `adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/pyproject.toml` & `adafruit-circuitpython-wiznet5k-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "2.4.0"
+version = "2.4.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/tests/extract_unique_dns_responses.py` & `adafruit-circuitpython-wiznet5k-2.4.1/tests/extract_unique_dns_responses.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/tests/test_dhcp.py` & `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/tests/test_dns_server_nonbreaking_changes.py` & `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dns_server_nonbreaking_changes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.0/tests/test_parse_dns_function.py` & `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_parse_dns_function.py`

 * *Files identical despite different names*

