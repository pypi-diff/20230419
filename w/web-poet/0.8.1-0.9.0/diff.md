# Comparing `tmp/web-poet-0.8.1.tar.gz` & `tmp/web-poet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-poet-0.8.1.tar", last modified: Fri Mar  3 08:18:19 2023, max compression
+gzip compressed data, was "web-poet-0.9.0.tar", last modified: Thu Mar 30 10:56:19 2023, max compression
```

## Comparing `web-poet-0.8.1.tar` & `web-poet-0.9.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-03 08:18:11.000000 web-poet-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-03 08:18:11.000000 web-poet-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-03 08:18:19.797052 web-poet-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-03 08:18:11.000000 web-poet-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 08:18:11.000000 web-poet-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 08:18:19.797052 web-poet-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-03 08:18:11.000000 web-poet-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    40307 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/fixtures/book_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/po_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/a_module.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/an_empty_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/po_lib/an_empty_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/an_empty_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/po_lib/nested_package/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/nested_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib/nested_package/a_nested_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/po_lib_sub/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.793052 web-poet-0.8.1/tests/po_lib_to_return/
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/po_lib_to_return/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_page_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-03-03 08:18:11.000000 web-poet-0.8.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/exceptions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/exceptions/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet/page_inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/page_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/page_inputs/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/serialization/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/serialization/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-03-03 08:18:11.000000 web-poet-0.8.1/web_poet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:18:19.797052 web-poet-0.8.1/web_poet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-03 08:18:19.000000 web-poet-0.8.1/web_poet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.472594 web-poet-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-30 10:56:04.000000 web-poet-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-30 10:56:04.000000 web-poet-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-30 10:56:19.472594 web-poet-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-30 10:56:04.000000 web-poet-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-30 10:56:04.000000 web-poet-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 10:56:19.472594 web-poet-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-30 10:56:04.000000 web-poet-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    40307 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/fixtures/book_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/po_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/a_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/an_empty_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/po_lib/an_empty_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/an_empty_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/po_lib/nested_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/nested_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib/nested_package/a_nested_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/po_lib_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/tests/po_lib_to_return/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/po_lib_to_return/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_page_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-03-30 10:56:04.000000 web-poet-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/web_poet/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/web_poet/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/exceptions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/exceptions/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/web_poet/page_inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/page_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/page_inputs/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.472594 web-poet-0.9.0/web_poet/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/serialization/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/serialization/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.472594 web-poet-0.9.0/web_poet/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-03-30 10:56:04.000000 web-poet-0.9.0/web_poet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:56:19.468594 web-poet-0.9.0/web_poet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 10:56:19.000000 web-poet-0.9.0/web_poet.egg-info/top_level.txt
```

### Comparing `web-poet-0.8.1/LICENSE` & `web-poet-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/PKG-INFO` & `web-poet-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-poet
-Version: 0.8.1
+Version: 0.9.0
 Summary: Zyte's Page Object pattern for web scraping
 Home-page: https://github.com/scrapinghub/web-poet
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `web-poet-0.8.1/README.rst` & `web-poet-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/setup.py` & `web-poet-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.rst") as f:
     long_description = f.read()
 
 
 setup(
     name="web-poet",
-    version="0.8.1",
+    version="0.9.0",
     description="Zyte's Page Object pattern for web scraping",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="opensource@zyte.com",
     url="https://github.com/scrapinghub/web-poet",
     packages=find_packages(include=["web_poet*"]),
```

### Comparing `web-poet-0.8.1/tests/conftest.py` & `web-poet-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/fixtures/book_list.html` & `web-poet-0.9.0/tests/fixtures/book_list.html`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/po_lib/__init__.py` & `web-poet-0.9.0/tests/po_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/po_lib/nested_package/a_nested_module.py` & `web-poet-0.9.0/tests/po_lib/nested_package/a_nested_module.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/po_lib_sub/__init__.py` & `web-poet-0.9.0/tests/po_lib_sub/__init__.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/po_lib_to_return/__init__.py` & `web-poet-0.9.0/tests/po_lib_to_return/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import attrs
 from url_matcher import Patterns
 
-from web_poet import Injectable, ItemPage, Returns, field, handle_urls, item_from_fields
+from web_poet import Injectable, ItemPage, Returns, field, handle_urls
 
 
 @attrs.define
 class Product:
     name: str
     price: float
 
@@ -180,17 +180,17 @@
     """
 
     expected_instead_of = None
     expected_patterns = Patterns(["example.com"])
     expected_to_return = Product
     expected_meta = {}
 
-    @field
+    @property
     def name(self) -> str:
         return "name"
 
-    @field
+    @property
     def price(self) -> float:
         return 12.99
 
     async def to_item(self) -> Product:
-        return await item_from_fields(self, item_cls=Product)
+        return Product(name=self.name, price=self.price)
```

### Comparing `web-poet-0.8.1/tests/test_example.py` & `web-poet-0.9.0/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_exceptions.py` & `web-poet-0.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_fields.py` & `web-poet-0.9.0/tests/test_fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import random
+from typing import Callable, List
 
 import attrs
 import pytest
 
 from tests.po_lib_to_return import (
     CustomProductPage,
     CustomProductPageDataTypeOnly,
@@ -16,53 +17,53 @@
     ProductMoreFields,
     ProductPage,
     ProductSimilar,
     SimilarProductPage,
 )
 from web_poet import (
     HttpResponse,
-    Injectable,
     ItemPage,
+    WebPage,
     field,
     item_from_fields,
     item_from_fields_sync,
 )
-from web_poet.fields import get_fields_dict
+from web_poet.fields import FieldsMixin, get_fields_dict
 
 
 @attrs.define
 class Item:
     name: str
     price: str
 
 
 @attrs.define
 class Page(ItemPage[Item]):
     response: HttpResponse
 
     @field
-    def name(self):  # noqa: D102
+    def name(self):
         return self.response.css("title ::text").get()
 
     @field
-    async def price(self):  # noqa: D102
+    async def price(self):
         await asyncio.sleep(0.01)
         return "$123"
 
 
 @attrs.define
 class InvalidPage(ItemPage[Item]):
     response: HttpResponse
 
     @field
-    def name(self):  # noqa: D102
+    def name(self):
         return self.response.css("title ::text").get()
 
     @field
-    def unknown_attribute(self):  # noqa: D102
+    def unknown_attribute(self):
         return "foo"
 
 
 EXAMPLE_RESPONSE = HttpResponse(
     "http://example.com",
     body=b"<html><head><title>Hello!</title></html>",
 )
@@ -90,50 +91,50 @@
         await page.to_item()
 
 
 def test_item_from_fields_sync() -> None:
     @attrs.define
     class Page(ItemPage):
         @field
-        def name(self):  # noqa: D102
+        def name(self):
             return "name"
 
-        def to_item(self):  # noqa: D102
+        def to_item(self):
             return item_from_fields_sync(self, dict)
 
     page = Page()
     assert page.to_item() == dict(name="name")
 
 
 def test_field_non_callable() -> None:
     with pytest.raises(TypeError):
 
         @attrs.define
         class Page(ItemPage):
             # https://github.com/python/mypy/issues/1362#issuecomment-438246775
             @field  # type: ignore
             @property
-            def name(self):  # noqa: D102
+            def name(self):
                 return "name"
 
-            def to_item(self):  # noqa: D102
+            def to_item(self):
                 return item_from_fields_sync(self, dict)
 
 
 def test_field_classmethod() -> None:
     with pytest.raises(TypeError):
 
         @attrs.define
         class Page(ItemPage):
             @field
             @classmethod
-            def name(cls):  # noqa: D102
+            def name(cls):
                 return "name"
 
-            def to_item(self):  # noqa: D102
+            def to_item(self):
                 return item_from_fields_sync(self, dict)
 
 
 @pytest.mark.asyncio
 async def test_field_order() -> None:
     class DictItemPage(Page):
         async def to_item(self):
@@ -155,15 +156,15 @@
             return item_from_fields_sync(self)
 
     page = Page()
     assert page.to_item() == {"name": "Name"}
 
 
 def test_field_cache_sync() -> None:
-    class Page:
+    class Page(ItemPage):
         _n_called_1 = 0
         _n_called_2 = 0
 
         def __init__(self, name):
             self.name = name
 
         @field(cached=True)
@@ -183,15 +184,15 @@
 
         assert page.n_called_2 == (1, page.name)
         assert page.n_called_2 == (2, page.name)
 
 
 @pytest.mark.asyncio
 async def test_field_cache_async() -> None:
-    class Page:
+    class Page(ItemPage):
         _n_called_1 = 0
         _n_called_2 = 0
 
         def __init__(self, name):
             self.name = name
 
         @field(cached=True)
@@ -211,15 +212,15 @@
 
         assert await page.n_called_2 == (1, page.name)
         assert await page.n_called_2 == (2, page.name)
 
 
 @pytest.mark.asyncio
 async def test_field_cache_async_locked() -> None:
-    class Page:
+    class Page(ItemPage):
         _n_called = 0
 
         @field(cached=True)
         async def n_called(self):
             await asyncio.sleep(random.randint(0, 10) / 100.0)
             self._n_called += 1
             return self._n_called
@@ -253,39 +254,39 @@
     page = ExtendedPage2(response=EXAMPLE_RESPONSE)
     item = await page.to_item()
     assert item == Item(name="Hello!", price="$123")
 
 
 def test_skip_nonitem_fields() -> None:
     @attrs.define
-    class SyncPage(Injectable):
+    class SyncPage(ItemPage):
         response: HttpResponse
 
         @field
-        def name(self):  # noqa: D102
+        def name(self):
             return self.response.css("title ::text").get()
 
         @field
-        def price(self):  # noqa: D102
+        def price(self):
             return "$123"
 
-        def to_item(self):  # noqa: D102
+        def to_item(self) -> Item:  # type: ignore[override]
             return item_from_fields_sync(self, Item)
 
     class ExtendedPage(SyncPage):
         @field
         def new_attribute(self):
             return "foo"
 
     page = ExtendedPage(response=EXAMPLE_RESPONSE)
     with pytest.raises(TypeError, match="unexpected keyword argument 'new_attribute'"):
         page.to_item()
 
     class ExtendedPage2(ExtendedPage):
-        def to_item(self) -> Item:
+        def to_item(self) -> Item:  # type: ignore[override]
             return item_from_fields_sync(self, Item, skip_nonitem_fields=True)
 
     page = ExtendedPage2(response=EXAMPLE_RESPONSE)
     item = page.to_item()
     assert item == Item(name="Hello!", price="$123")
 
 
@@ -351,14 +352,31 @@
     assert get_fields_dict(Page)["field3"].meta is None
     assert list(get_fields_dict(Page)) == ["field1", "field3"]
 
     assert get_fields_dict(Page2)["field3"].meta == {"foo": "bar"}
     assert list(get_fields_dict(Page2)) == ["field1", "field3", "field2"]
 
 
+def test_field_subclassing_super() -> None:
+    class Page(ItemPage):
+        @field
+        def field1(self):
+            return 1
+
+    class Page2(Page):
+        @field
+        def field1(self):
+            return super().field1 + 1
+
+    page = Page()
+    assert page.field1 == 1
+    page2 = Page2()
+    assert page2.field1 == 2
+
+
 def test_field_subclassing_from_to_item() -> None:
     # to_item() should be the same since it was not overridden from the
     # subclass.
     class PageToItem(ItemPage):
         def to_item(self):
             return {"field1": 1, "field2": 2, "field3": 3, "field4": 4}
 
@@ -479,46 +497,251 @@
 def test_field_processors_sync() -> None:
     def proc1(s):
         return s + "x"
 
     @attrs.define
     class Page(ItemPage):
         @field(out=[str.strip, proc1])
-        def name(self):  # noqa: D102
+        def name(self):
             return "  name\t "
 
     page = Page()
     assert page.name == "namex"
 
 
 @pytest.mark.asyncio
 async def test_field_processors_async() -> None:
     def proc1(s):
         return s + "x"
 
     @attrs.define
     class Page(ItemPage):
         @field(out=[str.strip, proc1])
-        async def name(self):  # noqa: D102
+        async def name(self):
             return "  name\t "
 
     page = Page()
     assert await page.name == "namex"
 
 
+def test_field_processors_inheritance() -> None:
+    def proc1(s):
+        return s + "x"
+
+    class BasePage(ItemPage):
+        @field(out=[str.strip, proc1])
+        def name(self):
+            return "  name\t "
+
+    class Page(BasePage):
+        @field(out=[str.strip])
+        def name(self):
+            return "  name\t "
+
+    base_page = BasePage()
+    assert base_page.name == "namex"
+    page = Page()
+    assert page.name == "name"
+
+
+def test_field_processors_page() -> None:
+    def proc1(s, page):
+        return page.prefix + s + "x"
+
+    class Page(ItemPage):
+        @field(out=[str.strip, proc1])
+        def name(self):
+            return "  name\t "
+
+        @field
+        def prefix(self):
+            return "prefix: "
+
+    page = Page()
+    assert page.name == "prefix: namex"
+
+
+def test_field_processors_multiple_pages() -> None:
+    def proc(value, page):
+        return page.body + value
+
+    class Page(WebPage):
+        @field
+        def body(self):
+            return self.response.text
+
+        @field(out=[proc])
+        def processed(self):
+            return "suffix"
+
+    page1 = Page(response=HttpResponse("https://example.com", b"page1"))
+    page2 = Page(response=HttpResponse("https://example.com", b"page2"))
+    assert page1.body == "page1"
+    assert page1.processed == "page1suffix"
+    assert page2.body == "page2"
+    assert page2.processed == "page2suffix"
+
+
+def test_field_processors_circular() -> None:
+    def proc1(s, page):
+        return s + page.b
+
+    def proc2(s, page):
+        return s + page.a
+
+    class Page(ItemPage):
+        @field(out=[proc1])
+        def a(self):
+            return "a"
+
+        @field(out=[proc2])
+        def b(self):
+            return "b"
+
+    page = Page()
+    with pytest.raises(RecursionError):
+        page.a
+    with pytest.raises(RecursionError):
+        page.b
+
+
+def test_field_processors_default() -> None:
+    @attrs.define
+    class BasePage(ItemPage):
+        class Processors:
+            name = [str.strip]
+
+        @field
+        def name(self):
+            return "  name\t "
+
+    class Page(BasePage):
+        pass
+
+    base_page = BasePage()
+    assert base_page.name == "name"
+
+    page = Page()
+    assert page.name == "name"
+
+
+def test_field_processors_override() -> None:
+    def proc1(s):
+        return s + "x"
+
+    class BasePage(ItemPage):
+        class Processors:
+            f1: List[Callable] = [str.strip]
+            f2 = [str.strip]
+            f3 = [str.strip]
+            f4: List[Callable] = [str.strip]
+            f5: List[Callable] = [str.strip]
+
+        @field
+        def f1(self):
+            return "  f1\t "
+
+        @field(out=[])
+        def f2(self):
+            return "  f2\t "
+
+        @field
+        def f3(self):
+            return "  f3\t "
+
+        @field
+        def f4(self):
+            return "  f4\t "
+
+        @field
+        def f5(self):
+            return "  f5\t "
+
+    class Page(BasePage):
+        class Processors(BasePage.Processors):
+            f1 = [proc1]
+            f4 = BasePage.Processors.f4 + [proc1]
+
+        @field(out=BasePage.Processors.f5 + [proc1])
+        def f5(self):
+            return "  f5\t "
+
+    base_page = BasePage()
+    assert base_page.f1 == "f1"
+    assert base_page.f2 == "  f2\t "
+    assert base_page.f3 == "f3"
+    assert base_page.f4 == "f4"
+    assert base_page.f5 == "f5"
+
+    page = Page()
+    assert page.f1 == "  f1\t x"
+    assert page.f2 == "  f2\t "
+    assert page.f3 == "f3"
+    assert page.f4 == "f4x"
+    assert page.f5 == "f5x"
+
+
+def test_field_processors_super() -> None:
+    class BasePage(ItemPage):
+        class Processors:
+            name = [str.strip]
+            desc = [str.strip]
+
+        @field
+        def name(self):
+            return "name "
+
+        @field
+        def desc(self):
+            return "desc "
+
+    class Page(BasePage):
+        class Processors(BasePage.Processors):
+            name: List[Callable] = []
+
+        @field
+        def name(self):
+            base_name = super().name
+            return base_name + "2 "
+
+    class Page2(Page):
+        class Processors(Page.Processors):
+            name: List[Callable] = []
+            desc: List[Callable] = []
+
+        @field
+        def desc(self):
+            base_desc = super().desc
+            return base_desc + "2 "
+
+    base_page = BasePage()
+    assert base_page.name == "name"
+    page = Page()
+    assert page.name == "name 2 "
+    page2 = Page2()
+    assert page2.desc == "desc 2 "
+
+
 def test_field_mixin() -> None:
     class A(ItemPage):
         @field
         def a(self):
             return None
 
-    class Mixin:
+    class Mixin(FieldsMixin):
         @field
         def mixin(self):
             return None
 
     class B(Mixin, A):
         @field
         def b(self):
             return None
 
+    class C(Mixin, A):
+        @field
+        def c(self):
+            return None
+
+    assert set(get_fields_dict(A)) == {"a"}
     assert set(get_fields_dict(B)) == {"a", "b", "mixin"}
+    assert set(get_fields_dict(C)) == {"a", "c", "mixin"}
```

### Comparing `web-poet-0.8.1/tests/test_mixins.py` & `web-poet-0.9.0/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_page_inputs.py` & `web-poet-0.9.0/tests/test_page_inputs.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_pages.py` & `web-poet-0.9.0/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_requests.py` & `web-poet-0.9.0/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_rules.py` & `web-poet-0.9.0/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_serialization.py` & `web-poet-0.9.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_testing.py` & `web-poet-0.9.0/tests/test_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     )
     _assert_fixture_files(base_dir / "custom")
     Fixture.save(base_dir, inputs=[book_list_html_response], item=item, meta=meta)
     _assert_fixture_files(base_dir / "test-2", expected_meta=meta)
 
 
 class MyItemPage(WebPage):
-    async def to_item(self) -> dict:  # noqa: D102
+    async def to_item(self) -> dict:
         return {"foo": "bar"}
 
 
 class MyItemPage2(WebPage):
-    async def to_item(self) -> dict:  # noqa: D102
+    async def to_item(self) -> dict:
         return {"foo": None}
 
 
 def _save_fixture(pytester, page_cls, page_inputs, expected):
     base_dir = pytester.path / "fixtures" / get_fq_class_name(page_cls)
     return Fixture.save(base_dir, inputs=page_inputs, item=expected)
 
@@ -196,15 +196,15 @@
         metadata=MetadataLocalTime(
             dateDownloaded=date_str, dateDownloadedLocal=date_local_str  # type: ignore[call-arg]
         ),
     )
 
 
 class DateItemPage(WebPage):
-    async def to_item(self) -> Item:  # noqa: D102
+    async def to_item(self) -> Item:
         date = datetime.datetime.now().astimezone()
         return _get_product_item(date)
 
 
 def _assert_frozen_item(
     frozen_time: datetime.datetime,
     pytester: pytest.Pytester,
@@ -271,15 +271,15 @@
     _assert_frozen_item(frozen_time, pytester, book_list_html_response)
 
 
 @attrs.define
 class ClientPage(WebPage):
     client: HttpClient
 
-    async def to_item(self) -> dict:  # noqa: D102
+    async def to_item(self) -> dict:
         resp1 = await self.client.get("http://books.toscrape.com/1.html")
         resp2 = await self.client.post("http://books.toscrape.com/2.html", body=b"post")
         return {"foo": "bar", "additional": [resp1.body.decode(), resp2.body.decode()]}
 
 
 def test_httpclient(pytester, book_list_html_response) -> None:
     url1 = "http://books.toscrape.com/1.html"
@@ -335,15 +335,15 @@
     result.assert_outcomes(failed=1, skipped=3)
 
 
 @attrs.define
 class ClientExceptionPage(WebPage):
     client: HttpClient
 
-    async def to_item(self) -> dict:  # noqa: D102
+    async def to_item(self) -> dict:
         msg = ""
         try:
             await self.client.get("http://books.toscrape.com/1.html")
         except HttpResponseError as ex:
             msg = ex.args[0]
         return {"foo": "bar", "exception": msg}
```

### Comparing `web-poet-0.8.1/tests/test_url.py` & `web-poet-0.9.0/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/tests/test_utils.py` & `web-poet-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/__init__.py` & `web-poet-0.9.0/web_poet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     HttpResponse,
     HttpResponseBody,
     HttpResponseHeaders,
     PageParams,
     RequestUrl,
     ResponseUrl,
 )
-from .pages import Injectable, ItemPage, ItemWebPage, Returns, WebPage
+from .pages import Injectable, ItemPage, ItemWebPage, Returns, WebPage, validates_input
 from .requests import request_downloader_var
 from .rules import (
     ApplyRule,
     OverrideRule,
     PageObjectRegistry,
     RulesRegistry,
     consume_modules,
```

### Comparing `web-poet-0.8.1/web_poet/_base.py` & `web-poet-0.9.0/web_poet/_base.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/_typing.py` & `web-poet-0.9.0/web_poet/_typing.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/example.py` & `web-poet-0.9.0/web_poet/example.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/exceptions/core.py` & `web-poet-0.9.0/web_poet/exceptions/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,37 +9,44 @@
 
 if TYPE_CHECKING:
     from web_poet import HttpRequest
 
 
 __all__ = [
     "RequestDownloaderVarError",
+    "PageObjectAction",
     "Retry",
+    "UseFallback",
+    "NoSavedHttpResponse",
 ]
 
 
 class RequestDownloaderVarError(Exception):
     """The ``web_poet.request_downloader_var`` had its contents accessed but there
     wasn't any value set during the time requests are executed.
 
     See the documentation section about :ref:`setting up the contextvars <setup-contextvars>`
     to learn more about this.
     """
 
-    pass
 
+class PageObjectAction(ValueError):
+    """Base class for exceptions that can be raised from a page object to
+    indicate something to be done about that page object."""
 
-class Retry(ValueError):
+
+class Retry(PageObjectAction):
     """The page object found that the input data is partial or empty, and a
-    request retry may provide better input.
+    request retry may provide better input."""
 
-    See :ref:`retries`.
-    """
 
-    pass
+class UseFallback(PageObjectAction):
+    """The page object cannot extract data from the input, but the input seems
+    valid, so an alternative data extraction implementation for the same item
+    type may succeed."""
 
 
 class NoSavedHttpResponse(AssertionError):
     """Indicates that there is no saved response for this request.
 
     Can only be raised when a :class:`~.HttpClient` instance is used to
     get saved responses.
```

### Comparing `web-poet-0.8.1/web_poet/exceptions/http.py` & `web-poet-0.9.0/web_poet/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/fields.py` & `web-poet-0.9.0/web_poet/fields.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 ``web_poet.fields`` is a module with helpers for putting extraction logic
 into separate Page Object methods / properties.
 """
 import inspect
 from contextlib import suppress
 from functools import update_wrapper, wraps
-from typing import Callable, Dict, List, Optional, Type, TypeVar
+from typing import Callable, Dict, List, Optional, Tuple, Type, TypeVar
 
 import attrs
 from itemadapter import ItemAdapter
 
 from web_poet.utils import cached_method, ensure_awaitable
 
 _FIELDS_INFO_ATTRIBUTE_READ = "_web_poet_fields_info"
 _FIELDS_INFO_ATTRIBUTE_WRITE = "_web_poet_fields_info_temp"
+_FIELD_METHODS_ATTRIBUTE = "_web_poet_field_methods"
 
 
 @attrs.define
 class FieldInfo:
     """Information about a field"""
 
     #: name of the field
@@ -36,20 +37,24 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         # To support fields, we must ensure that fields dict is not shared
         # between subclasses, i.e. a decorator in a subclass doesn't affect
         # the base class. This is done by making decorator write to a
         # temporary location, and then merging it all on subclass creation.
         this_class_fields = getattr(cls, _FIELDS_INFO_ATTRIBUTE_WRITE, {})
-        base_class_fields = getattr(cls, _FIELDS_INFO_ATTRIBUTE_READ, {})
-        if base_class_fields or this_class_fields:
-            fields = {**base_class_fields, **this_class_fields}
+        base_fields = {}
+        for base_class in cls.__bases__:
+            fields = getattr(base_class, _FIELDS_INFO_ATTRIBUTE_READ, {})
+            base_fields.update(fields)
+        if base_fields or this_class_fields:
+            fields = {**base_fields, **this_class_fields}
             setattr(cls, _FIELDS_INFO_ATTRIBUTE_READ, fields)
             with suppress(AttributeError):
                 delattr(cls, _FIELDS_INFO_ATTRIBUTE_WRITE)
+        setattr(cls, _FIELD_METHODS_ATTRIBUTE, {})
 
 
 def field(
     method=None,
     *,
     cached: bool = False,
     meta: Optional[dict] = None,
@@ -73,49 +78,86 @@
 
     class _field:
         def __init__(self, method):
             if not callable(method):
                 raise TypeError(
                     f"@field decorator must be used on methods, {method!r} is decorated instead"
                 )
-            method = self._processed(method)
-            if cached:
-                self.unbound_method = cached_method(method)
-            else:
-                self.unbound_method = method
+            self.original_method = method
+            self.name: Optional[str] = None
 
         def __set_name__(self, owner, name):
+            self.name = name
             if not hasattr(owner, _FIELDS_INFO_ATTRIBUTE_WRITE):
                 setattr(owner, _FIELDS_INFO_ATTRIBUTE_WRITE, {})
 
             field_info = FieldInfo(name=name, meta=meta, out=out)
             getattr(owner, _FIELDS_INFO_ATTRIBUTE_WRITE)[name] = field_info
 
         def __get__(self, instance, owner=None):
-            return self.unbound_method(instance)
+            # We use the original method and the out arg from the field and
+            # the Processors class from the instance class, so caching needs to
+            # take into account the instance class and the field object. So we
+            # use the field object id() as a key when caching the method in
+            # the instance class.
+            cache_key = id(self)
+            method = self._get_processed_method(owner, cache_key)
+            if method is None:
+                if out is not None:
+                    processor_functions = out
+                elif hasattr(owner, "Processors"):
+                    processor_functions = getattr(owner.Processors, self.name, [])
+                else:
+                    processor_functions = []
+                processors: List[Tuple[Callable, bool]] = []
+                for processor_function in processor_functions:
+                    sig = inspect.signature(processor_function)
+                    processors.append((processor_function, "page" in sig.parameters))
+                method = self._processed(self.original_method, processors)
+                if cached:
+                    method = cached_method(method)
+                self._set_processed_method(owner, cache_key, method)
+
+            return method(instance)
+
+        @staticmethod
+        def _get_processed_method(cls, key):
+            return getattr(cls, _FIELD_METHODS_ATTRIBUTE).get(key)
 
         @staticmethod
-        def _process(value):
-            for processor in out:
-                value = processor(value)
+        def _set_processed_method(cls, key, method):
+            getattr(cls, _FIELD_METHODS_ATTRIBUTE)[key] = method
+
+        @staticmethod
+        def _process(value, page, processors):
+            for processor, takes_page in processors:
+                if takes_page:
+                    value = processor(value, page=page)
+                else:
+                    value = processor(value)
             return value
 
-        def _processed(self, method):
+        @staticmethod
+        def _processed(method, processors):
             """Returns a wrapper for method that calls processors on its result"""
-            if not out:
-                return method
             if inspect.iscoroutinefunction(method):
 
-                async def processed(*args, **kwargs):
-                    return self._process(await method(*args, **kwargs))
+                async def processed(page):
+                    validation_item = page._validate_input()
+                    if validation_item is not None:
+                        return getattr(validation_item, method.__name__)
+                    return _field._process(await method(page), page, processors)
 
             else:
 
-                def processed(*args, **kwargs):
-                    return self._process(method(*args, **kwargs))
+                def processed(page):
+                    validation_item = page._validate_input()
+                    if validation_item is not None:
+                        return getattr(validation_item, method.__name__)
+                    return _field._process(method(page), page, processors)
 
             return wraps(method)(processed)
 
     if method is not None:
         # @field syntax
         res = _field(method)
         update_wrapper(res, method)
```

### Comparing `web-poet-0.8.1/web_poet/mixins.py` & `web-poet-0.9.0/web_poet/mixins.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/page_inputs/client.py` & `web-poet-0.9.0/web_poet/page_inputs/client.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/page_inputs/http.py` & `web-poet-0.9.0/web_poet/page_inputs/http.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/page_inputs/url.py` & `web-poet-0.9.0/web_poet/page_inputs/url.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/requests.py` & `web-poet-0.9.0/web_poet/requests.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/rules.py` & `web-poet-0.9.0/web_poet/rules.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/serialization/api.py` & `web-poet-0.9.0/web_poet/serialization/api.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/serialization/functions.py` & `web-poet-0.9.0/web_poet/serialization/functions.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/testing/__main__.py` & `web-poet-0.9.0/web_poet/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/testing/fixture.py` & `web-poet-0.9.0/web_poet/testing/fixture.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/testing/pytest.py` & `web-poet-0.9.0/web_poet/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/testing/utils.py` & `web-poet-0.9.0/web_poet/testing/utils.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet/utils.py` & `web-poet-0.9.0/web_poet/utils.py`

 * *Files identical despite different names*

### Comparing `web-poet-0.8.1/web_poet.egg-info/PKG-INFO` & `web-poet-0.9.0/web_poet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-poet
-Version: 0.8.1
+Version: 0.9.0
 Summary: Zyte's Page Object pattern for web scraping
 Home-page: https://github.com/scrapinghub/web-poet
 Author: Zyte Group Ltd
 Author-email: opensource@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `web-poet-0.8.1/web_poet.egg-info/SOURCES.txt` & `web-poet-0.9.0/web_poet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/test_example.py
 tests/test_exceptions.py
 tests/test_fields.py
+tests/test_input_validation.py
 tests/test_mixins.py
 tests/test_page_inputs.py
 tests/test_pages.py
 tests/test_requests.py
 tests/test_rules.py
 tests/test_serialization.py
 tests/test_testing.py
```

