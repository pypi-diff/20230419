# Comparing `tmp/py_clob_client-0.5.0.tar.gz` & `tmp/py_clob_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_clob_client-0.5.0.tar", last modified: Tue Apr  4 18:13:59 2023, max compression
+gzip compressed data, was "py_clob_client-0.6.0.tar", last modified: Wed Apr 19 16:51:51 2023, max compression
```

## Comparing `py_clob_client-0.5.0.tar` & `py_clob_client-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.550304 py_clob_client-0.5.0/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.5.0/LICENSE
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-04 18:13:59.550147 py_clob_client-0.5.0/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.5.0/README.md
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.546309 py_clob_client-0.5.0/py_clob_client/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.5.0/py_clob_client/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    14414 2023-03-31 18:04:55.000000 py_clob_client-0.5.0/py_clob_client/client.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2269 2023-03-31 18:04:55.000000 py_clob_client-0.5.0/py_clob_client/clob_types.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      645 2023-03-31 18:04:55.000000 py_clob_client-0.5.0/py_clob_client/endpoints.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/exceptions.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.547297 py_clob_client-0.5.0/py_clob_client/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/headers/headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.547538 py_clob_client-0.5.0/py_clob_client/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.5.0/py_clob_client/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3850 2023-03-31 18:04:55.000000 py_clob_client-0.5.0/py_clob_client/http_helpers/helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.548241 py_clob_client-0.5.0/py_clob_client/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3356 2023-01-27 20:18:52.000000 py_clob_client-0.5.0/py_clob_client/order_builder/builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.5.0/py_clob_client/order_builder/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.5.0/py_clob_client/order_builder/helpers.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/signer.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.548720 py_clob_client-0.5.0/py_clob_client/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.5.0/py_clob_client/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/signing/eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/signing/hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/py_clob_client/signing/model.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      949 2023-03-14 17:04:59.000000 py_clob_client-0.5.0/py_clob_client/utilities.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.547081 py_clob_client-0.5.0/py_clob_client.egg-info/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-04 18:13:59.000000 py_clob_client-0.5.0/py_clob_client.egg-info/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1226 2023-04-04 18:13:59.000000 py_clob_client-0.5.0/py_clob_client.egg-info/SOURCES.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-04-04 18:13:59.000000 py_clob_client-0.5.0/py_clob_client.egg-info/dependency_links.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-04-04 18:13:59.000000 py_clob_client-0.5.0/py_clob_client.egg-info/requires.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-04-04 18:13:59.000000 py_clob_client-0.5.0/py_clob_client.egg-info/top_level.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-04-04 18:13:59.550349 py_clob_client-0.5.0/setup.cfg
--rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-04-04 18:13:49.000000 py_clob_client-0.5.0/setup.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.548934 py_clob_client-0.5.0/tests/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/__init__.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.549140 py_clob_client-0.5.0/tests/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/headers/test_headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.549337 py_clob_client-0.5.0/tests/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2384 2023-03-31 18:04:55.000000 py_clob_client-0.5.0/tests/http_helpers/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.549652 py_clob_client-0.5.0/tests/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    13512 2023-03-14 17:04:59.000000 py_clob_client-0.5.0/tests/order_builder/test_builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-01-27 20:18:52.000000 py_clob_client-0.5.0/tests/order_builder/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-04 18:13:59.549949 py_clob_client-0.5.0/tests/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/signing/test_eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.5.0/tests/signing/test_hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    11906 2023-03-14 17:04:59.000000 py_clob_client-0.5.0/tests/test_utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.999919 py_clob_client-0.6.0/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/LICENSE
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-19 16:51:50.999780 py_clob_client-0.6.0/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.6.0/README.md
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.994408 py_clob_client-0.6.0/py_clob_client/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    15509 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/client.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2467 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/clob_types.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      674 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/endpoints.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/exceptions.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995353 py_clob_client-0.6.0/py_clob_client/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/headers/headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995634 py_clob_client-0.6.0/py_clob_client/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3850 2023-03-31 18:04:55.000000 py_clob_client-0.6.0/py_clob_client/http_helpers/helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.996471 py_clob_client-0.6.0/py_clob_client/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3995 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/order_builder/builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.6.0/py_clob_client/order_builder/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.6.0/py_clob_client/order_builder/helpers.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signer.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.997275 py_clob_client-0.6.0/py_clob_client/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/model.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1040 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995148 py_clob_client-0.6.0/py_clob_client.egg-info/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1247 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/SOURCES.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/dependency_links.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/requires.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/top_level.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-04-19 16:51:50.999966 py_clob_client-0.6.0/setup.cfg
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/setup.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.997751 py_clob_client-0.6.0/tests/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/__init__.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998068 py_clob_client-0.6.0/tests/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/headers/test_headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998319 py_clob_client-0.6.0/tests/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2384 2023-03-31 18:04:55.000000 py_clob_client-0.6.0/tests/http_helpers/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998900 py_clob_client-0.6.0/tests/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    30909 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/tests/order_builder/test_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-01-27 20:18:52.000000 py_clob_client-0.6.0/tests/order_builder/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.999564 py_clob_client-0.6.0/tests/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/test_eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/test_hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1172 2023-04-12 18:14:06.000000 py_clob_client-0.6.0/tests/test_client.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    33747 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/tests/test_utilities.py
```

### Comparing `py_clob_client-0.5.0/LICENSE` & `py_clob_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/PKG-INFO` & `py_clob_client-0.6.0/py_clob_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_clob_client
-Version: 0.5.0
+Name: py-clob-client
+Version: 0.6.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py_clob_client Version: 0.5.0 Summary: Python
+Metadata-Version: 2.1 Name: py-clob-client Version: 0.6.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.5.0/README.md` & `py_clob_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/client.py` & `py_clob_client-0.6.0/py_clob_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,26 @@
     PRICE,
     TIME,
     TRADES,
     GET_TRADE_NOTIFICATIONS,
     DROP_TRADE_NOTIFICATIONS,
     GET_BALANCE_ALLOWANCE,
     IS_ORDER_SCORING,
+    GET_TICK_SIZE,
 )
 from .clob_types import (
     ApiCreds,
     FilterParams,
     OrderArgs,
     RequestArgs,
     TradeNotificationParams,
     OrderBookSummary,
     BalanceAllowanceParams,
     OrderScoringParams,
+    TickSize,
 )
 from .exceptions import PolyException
 from .http_helpers.helpers import (
     add_query_params,
     delete,
     get,
     post,
@@ -51,14 +53,15 @@
 )
 from py_order_utils.config import get_contract_config
 from .constants import L0, L1, L1_AUTH_UNAVAILABLE, L2, L2_AUTH_UNAVAILABLE
 from .utilities import (
     parse_raw_orderbook_summary,
     generate_orderbook_summary_hash,
     order_to_json,
+    is_tick_size_smaller,
 )
 
 
 class ClobClient:
     def __init__(
         self,
         host,
@@ -86,14 +89,15 @@
         self.mode = self._get_client_mode()
         if chain_id:
             self.contract_config = get_contract_config(chain_id)
         if self.signer:
             self.builder = OrderBuilder(
                 self.signer, sig_type=signature_type, funder=funder
             )
+        self.__tick_sizes = {}
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def get_address(self):
         """
         Returns the public address of the signer
         """
         return self.signer.address() if self.signer else None
@@ -221,22 +225,48 @@
 
     def get_price(self, token_id, side):
         """
         Get the market price for the given market
         """
         return get("{}{}?token_id={}&side={}".format(self.host, PRICE, token_id, side))
 
-    def create_order(self, order_args: OrderArgs):
+    def get_tick_size(self, token_id: str) -> TickSize:
+        if token_id in self.__tick_sizes:
+            return self.__tick_sizes[token_id]
+
+        result = get("{}{}?token_id={}".format(self.host, GET_TICK_SIZE, token_id))
+        self.__tick_sizes[token_id] = result["minimum_tick_size"]
+
+        return self.__tick_sizes[token_id]
+
+    def __resolve_tick_size(
+        self, token_id: str, tick_size: TickSize = None
+    ) -> TickSize:
+        min_tick_size = self.get_tick_size(token_id)
+        if tick_size is not None:
+            if is_tick_size_smaller(tick_size, min_tick_size):
+                raise Exception(
+                    "invalid tick size ("
+                    + tick_size
+                    + "), minimum for the market is "
+                    + min_tick_size,
+                )
+        else:
+            tick_size = min_tick_size
+        return tick_size
+
+    def create_order(self, order_args: OrderArgs, tick_size: TickSize = None):
         """
         Creates and signs an order
         Level 2 Auth required
         """
         self.assert_level_2_auth()
 
-        return self.builder.create_order(order_args)
+        tick_size = self.__resolve_tick_size(order_args.token_id, tick_size)
+        return self.builder.create_order(order_args, tick_size)
 
     def post_order(self, order, orderType: OrderType = OrderType.GTC):
         """
         Posts the order
         """
         self.assert_level_2_auth()
         body = order_to_json(order, self.creds.api_key, orderType)
```

### Comparing `py_clob_client-0.5.0/py_clob_client/clob_types.py` & `py_clob_client-0.6.0/py_clob_client/clob_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import Any
 from dataclasses import dataclass, asdict
 from json import dumps
+from typing import Literal
 
 from .constants import ZERO_ADDRESS
 
 
 @dataclass
 class ApiCreds:
     api_key: str
@@ -128,7 +129,20 @@
     FOK = "FOK"
     GTD = "GTD"
 
 
 @dataclass
 class OrderScoringParams:
     orderId: str
+
+
+TickSize = Literal["0.1", "0.01", "0.001", "0.0001"]
+
+
+@dataclass
+class RoundConfig:
+    price: float
+    size: float
+    amount: float
+
+
+TickSizes: dict[str, TickSize]
```

### Comparing `py_clob_client-0.5.0/py_clob_client/endpoints.py` & `py_clob_client-0.6.0/py_clob_client/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 MID_POINT = "/midpoint"
 PRICE = "/price"
 GET_LAST_TRADE_PRICE = "/last-trade-price"
 GET_TRADE_NOTIFICATIONS = "/trade-notifications"
 DROP_TRADE_NOTIFICATIONS = "/drop-trade-notifications"
 GET_BALANCE_ALLOWANCE = "/balance-allowance"
 IS_ORDER_SCORING = "/order-scoring"
+GET_TICK_SIZE = "/tick-size"
```

### Comparing `py_clob_client-0.5.0/py_clob_client/exceptions.py` & `py_clob_client-0.6.0/py_clob_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/headers/headers.py` & `py_clob_client-0.6.0/py_clob_client/headers/headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/http_helpers/helpers.py` & `py_clob_client-0.6.0/py_clob_client/http_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/order_builder/builder.py` & `py_clob_client-0.6.0/py_clob_client/order_builder/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,23 @@
     round_normal,
     decimal_places,
     round_up,
 )
 from .constants import BUY, SELL
 
 from ..signer import Signer
-from ..clob_types import OrderArgs
+from ..clob_types import OrderArgs, TickSize, RoundConfig
+from typing import Tuple
+
+ROUNDING_CONFIG: Tuple[TickSize, RoundConfig] = {
+    "0.1": RoundConfig(price=1, size=2, amount=3),
+    "0.01": RoundConfig(price=2, size=2, amount=4),
+    "0.001": RoundConfig(price=3, size=2, amount=5),
+    "0.0001": RoundConfig(price=4, size=2, amount=6),
+}
 
 
 class OrderBuilder:
     def __init__(self, signer: Signer, sig_type=None, funder=None):
         self.signer = signer
 
         # Signature type used sign orders, defaults to EOA type
@@ -36,52 +44,57 @@
         self.order_builder = UtilsOrderBuild(
             self.contract_config.exchange, self.signer.get_chain_id(), self.signer
         )
 
     def _get_contract_config(self, chain_id: int):
         return get_contract_config(chain_id)
 
-    def get_order_amounts(self, side: str, size: float, price: float):
-        raw_price = round_normal(price, 2)
+    def get_order_amounts(
+        self, side: str, size: float, price: float, round_config: RoundConfig
+    ):
+        raw_price = round_normal(price, round_config.price)
 
         if side == BUY:
-            raw_taker_amt = round_down(size, 2)
+            raw_taker_amt = round_down(size, round_config.size)
 
             raw_maker_amt = raw_taker_amt * raw_price
-            if decimal_places(raw_maker_amt) > 4:
-                raw_maker_amt = round_up(raw_maker_amt, 8)
-                if decimal_places(raw_maker_amt) > 4:
-                    raw_maker_amt = round_down(raw_maker_amt, 4)
+            if decimal_places(raw_maker_amt) > round_config.amount:
+                raw_maker_amt = round_up(raw_maker_amt, round_config.amount + 4)
+                if decimal_places(raw_maker_amt) > round_config.amount:
+                    raw_maker_amt = round_down(raw_maker_amt, round_config.amount)
 
             maker_amount = to_token_decimals(raw_maker_amt)
             taker_amount = to_token_decimals(raw_taker_amt)
 
             return UtilsBuy, maker_amount, taker_amount
         elif side == SELL:
-            raw_maker_amt = round_down(size, 2)
+            raw_maker_amt = round_down(size, round_config.size)
 
             raw_taker_amt = raw_maker_amt * raw_price
-            if decimal_places(raw_taker_amt) > 4:
-                raw_taker_amt = round_up(raw_taker_amt, 8)
-                if decimal_places(raw_taker_amt) > 4:
-                    raw_taker_amt = round_down(raw_taker_amt, 4)
+            if decimal_places(raw_taker_amt) > round_config.amount:
+                raw_taker_amt = round_up(raw_taker_amt, round_config.amount + 4)
+                if decimal_places(raw_taker_amt) > round_config.amount:
+                    raw_taker_amt = round_down(raw_taker_amt, round_config.amount)
 
             maker_amount = to_token_decimals(raw_maker_amt)
             taker_amount = to_token_decimals(raw_taker_amt)
 
             return UtilsSell, maker_amount, taker_amount
         else:
             raise ValueError(f"order_args.side must be '{BUY}' or '{SELL}'")
 
-    def create_order(self, order_args: OrderArgs) -> SignedOrder:
+    def create_order(self, order_args: OrderArgs, tick_size: TickSize) -> SignedOrder:
         """
         Creates and signs an order
         """
         side, maker_amount, taker_amount = self.get_order_amounts(
-            order_args.side, order_args.size, order_args.price
+            order_args.side,
+            order_args.size,
+            order_args.price,
+            ROUNDING_CONFIG[tick_size],
         )
 
         data = OrderData(
             maker=self.funder,
             taker=order_args.taker,
             tokenId=order_args.token_id,
             makerAmount=maker_amount,
```

### Comparing `py_clob_client-0.5.0/py_clob_client/order_builder/helpers.py` & `py_clob_client-0.6.0/py_clob_client/order_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/signer.py` & `py_clob_client-0.6.0/py_clob_client/signer.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/signing/eip712.py` & `py_clob_client-0.6.0/py_clob_client/signing/eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/signing/hmac.py` & `py_clob_client-0.6.0/py_clob_client/signing/hmac.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/py_clob_client/utilities.py` & `py_clob_client-0.6.0/py_clob_client/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hashlib
-import json
 
-from .clob_types import OrderBookSummary, OrderSummary
+from .clob_types import OrderBookSummary, OrderSummary, TickSize
 
 
 def parse_raw_orderbook_summary(raw_obs: any) -> OrderBookSummary:
     bids = []
     for bid in raw_obs["bids"]:
         bids.append(OrderSummary(size=bid["size"], price=bid["price"]))
 
@@ -29,7 +28,11 @@
     hash = hashlib.sha1(str(orderbook.json).encode("utf-8")).hexdigest()
     orderbook.hash = hash
     return hash
 
 
 def order_to_json(order, owner, orderType) -> dict:
     return {"order": order.dict(), "owner": owner, "orderType": orderType}
+
+
+def is_tick_size_smaller(a: TickSize, b: TickSize) -> bool:
+    return float(a) < float(b)
```

### Comparing `py_clob_client-0.5.0/py_clob_client.egg-info/PKG-INFO` & `py_clob_client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-clob-client
-Version: 0.5.0
+Name: py_clob_client
+Version: 0.6.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-clob-client Version: 0.5.0 Summary: Python
+Metadata-Version: 2.1 Name: py_clob_client Version: 0.6.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.5.0/py_clob_client.egg-info/SOURCES.txt` & `py_clob_client-0.6.0/py_clob_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 py_clob_client/order_builder/constants.py
 py_clob_client/order_builder/helpers.py
 py_clob_client/signing/__init__.py
 py_clob_client/signing/eip712.py
 py_clob_client/signing/hmac.py
 py_clob_client/signing/model.py
 tests/__init__.py
+tests/test_client.py
 tests/test_utilities.py
 tests/headers/__init__.py
 tests/headers/test_headers.py
 tests/http_helpers/__init__.py
 tests/http_helpers/test_helpers.py
 tests/order_builder/__init__.py
 tests/order_builder/test_builder.py
```

### Comparing `py_clob_client-0.5.0/setup.py` & `py_clob_client-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_clob_client",
-    version="0.5.0",
+    version="0.6.0",
     author="Polymarket Engineering",
     author_email="engineering@polymarket.com",
     maintainer="Polymarket Engineering",
     maintainer_email="engineering@polymarket.com",
     description="Python client for the Polymarket CLOB",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py_clob_client-0.5.0/tests/headers/test_headers.py` & `py_clob_client-0.6.0/tests/headers/test_headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/tests/http_helpers/test_helpers.py` & `py_clob_client-0.6.0/tests/http_helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/tests/signing/test_eip712.py` & `py_clob_client-0.6.0/tests/signing/test_eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.5.0/tests/signing/test_hmac.py` & `py_clob_client-0.6.0/tests/signing/test_hmac.py`

 * *Files identical despite different names*

