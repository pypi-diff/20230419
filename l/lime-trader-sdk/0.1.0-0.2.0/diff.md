# Comparing `tmp/lime_trader_sdk-0.1.0.tar.gz` & `tmp/lime_trader_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime_trader_sdk-0.1.0.tar", max compression
+gzip compressed data, was "lime_trader_sdk-0.2.0.tar", max compression
```

## Comparing `lime_trader_sdk-0.1.0.tar` & `lime_trader_sdk-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      815 2023-04-13 00:39:09.183928 lime_trader_sdk-0.1.0/README.md
--rw-r--r--   0        0        0       86 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/api/__init__.py
--rw-r--r--   0        0        0     7861 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/api/api_client.py
--rw-r--r--   0        0        0     4552 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/api/authenticated_api_client.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/async_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/async_trader/api/__init__.py
--rw-r--r--   0        0        0     2104 2023-04-13 00:39:09.184928 lime_trader_sdk-0.1.0/lime_trader/async_trader/api/async_api_client.py
--rw-r--r--   0        0        0     2091 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/api/async_authenticated_api_client.py
--rw-r--r--   0        0        0     2282 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/async_client.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/__init__.py
--rw-r--r--   0        0        0     4805 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_account_client.py
--rw-r--r--   0        0        0     4470 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_market_data_client.py
--rw-r--r--   0        0        0     3097 2023-04-13 00:39:09.185928 lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_trading_client.py
--rw-r--r--   0        0        0     7787 2023-04-13 00:39:09.186928 lime_trader_sdk-0.1.0/lime_trader/client.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.186928 lime_trader_sdk-0.1.0/lime_trader/clients/__init__.py
--rw-r--r--   0        0        0     6775 2023-04-13 00:39:09.186928 lime_trader_sdk-0.1.0/lime_trader/clients/account_client.py
--rw-r--r--   0        0        0     4341 2023-04-13 00:39:09.186928 lime_trader_sdk-0.1.0/lime_trader/clients/account_feed_client.py
--rw-r--r--   0        0        0     8195 2023-04-13 00:39:09.186928 lime_trader_sdk-0.1.0/lime_trader/clients/market_data_client.py
--rw-r--r--   0        0        0     2260 2023-04-13 00:39:09.187928 lime_trader_sdk-0.1.0/lime_trader/clients/market_data_feed_client.py
--rw-r--r--   0        0        0     5211 2023-04-13 00:39:09.187928 lime_trader_sdk-0.1.0/lime_trader/clients/trading_client.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.188928 lime_trader_sdk-0.1.0/lime_trader/constants/__init__.py
--rw-r--r--   0        0        0     1707 2023-04-13 00:39:09.188928 lime_trader_sdk-0.1.0/lime_trader/constants/urls.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.189928 lime_trader_sdk-0.1.0/lime_trader/converters/__init__.py
--rw-r--r--   0        0        0      979 2023-04-13 00:39:09.189928 lime_trader_sdk-0.1.0/lime_trader/converters/abstract_converter.py
--rw-r--r--   0        0        0     2088 2023-04-13 00:39:09.189928 lime_trader_sdk-0.1.0/lime_trader/converters/cattr_converter.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.189928 lime_trader_sdk-0.1.0/lime_trader/exceptions/__init__.py
--rw-r--r--   0        0        0      446 2023-04-13 00:39:09.189928 lime_trader_sdk-0.1.0/lime_trader/exceptions/api_error.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.190929 lime_trader_sdk-0.1.0/lime_trader/handlers/__init__.py
--rw-r--r--   0        0        0     5360 2023-04-13 00:39:09.190929 lime_trader_sdk-0.1.0/lime_trader/handlers/account_feed_handler.py
--rw-r--r--   0        0        0     3272 2023-04-13 00:39:09.190929 lime_trader_sdk-0.1.0/lime_trader/handlers/market_data_feed_handler.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/__init__.py
--rw-r--r--   0        0        0     8409 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/accounts.py
--rw-r--r--   0        0        0      294 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/errors.py
--rw-r--r--   0        0        0     6134 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/market.py
--rw-r--r--   0        0        0     2311 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/page.py
--rw-r--r--   0        0        0     3054 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/token_storage.py
--rw-r--r--   0        0        0     5148 2023-04-13 00:39:09.191928 lime_trader_sdk-0.1.0/lime_trader/models/trading.py
--rw-r--r--   0        0        0        0 2023-04-13 00:39:09.192929 lime_trader_sdk-0.1.0/lime_trader/utils/__init__.py
--rw-r--r--   0        0        0     1275 2023-04-13 00:39:09.193929 lime_trader_sdk-0.1.0/lime_trader/utils/date_utils.py
--rw-r--r--   0        0        0     1480 2023-04-13 00:39:09.193929 lime_trader_sdk-0.1.0/lime_trader/utils/logging_utils.py
--rw-r--r--   0        0        0     1405 2023-04-13 00:39:09.193929 lime_trader_sdk-0.1.0/lime_trader/utils/pagination.py
--rw-r--r--   0        0        0      649 2023-04-13 00:39:09.195929 lime_trader_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      815 2023-04-19 18:06:04.914359 lime_trader_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0       86 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/__init__.py
+-rw-r--r--   0        0        0     7868 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/api_client.py
+-rw-r--r--   0        0        0     4552 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/authenticated_api_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/__init__.py
+-rw-r--r--   0        0        0     2104 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_api_client.py
+-rw-r--r--   0        0        0     2091 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_authenticated_api_client.py
+-rw-r--r--   0        0        0     2282 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/async_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/__init__.py
+-rw-r--r--   0        0        0     4805 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_account_client.py
+-rw-r--r--   0        0        0     4470 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_market_data_client.py
+-rw-r--r--   0        0        0     3097 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_trading_client.py
+-rw-r--r--   0        0        0     7787 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/__init__.py
+-rw-r--r--   0        0        0     6775 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/account_client.py
+-rw-r--r--   0        0        0     4341 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/account_feed_client.py
+-rw-r--r--   0        0        0     8195 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/market_data_client.py
+-rw-r--r--   0        0        0     2260 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/market_data_feed_client.py
+-rw-r--r--   0        0        0     5211 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/clients/trading_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/constants/__init__.py
+-rw-r--r--   0        0        0     1707 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/constants/urls.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/__init__.py
+-rw-r--r--   0        0        0      979 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/abstract_converter.py
+-rw-r--r--   0        0        0     2088 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/cattr_converter.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/exceptions/__init__.py
+-rw-r--r--   0        0        0      446 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/exceptions/api_error.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/__init__.py
+-rw-r--r--   0        0        0     5360 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/account_feed_handler.py
+-rw-r--r--   0        0        0     3272 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/market_data_feed_handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/__init__.py
+-rw-r--r--   0        0        0     8409 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/accounts.py
+-rw-r--r--   0        0        0      294 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/errors.py
+-rw-r--r--   0        0        0     6134 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/market.py
+-rw-r--r--   0        0        0     2311 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/page.py
+-rw-r--r--   0        0        0     3054 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/token_storage.py
+-rw-r--r--   0        0        0     5148 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/trading.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/__init__.py
+-rw-r--r--   0        0        0     1275 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/date_utils.py
+-rw-r--r--   0        0        0     1480 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/logging_utils.py
+-rw-r--r--   0        0        0     1405 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/pagination.py
+-rw-r--r--   0        0        0      649 2023-04-19 18:06:04.921360 lime_trader_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.2.0/PKG-INFO
```

### Comparing `lime_trader_sdk-0.1.0/README.md` & `lime_trader_sdk-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/api/api_client.py` & `lime_trader_sdk-0.2.0/lime_trader/api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,15 @@
         """
         if path.url.startswith("http://"):
             scheme = "https" if self._use_https else "http"
         elif path.url.startswith("ws://"):
             scheme = "wss" if self._use_wss else "ws"
         else:
             raise Exception("Invalid urls specified!")
-        url = Url(scheme=scheme, path=self._base_url.path + path.path, host=self._base_url.hostname).url
-
+        url = Url(scheme=scheme, path=(self._base_url.path or '') + path.path, host=self._base_url.hostname).url
         return url.format(**self._converter.dump_to_dict(path_params))
 
     def post_form(self, url: Url, path_params: dict[str, Any], data: Any, headers: dict[str, str],
                   response_schema: Type[T]) -> T:
         """
         Executes POST request with form data
```

### Comparing `lime_trader_sdk-0.1.0/lime_trader/api/authenticated_api_client.py` & `lime_trader_sdk-0.2.0/lime_trader/api/authenticated_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/api/async_api_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/api/async_authenticated_api_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_authenticated_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/async_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/async_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_account_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_market_data_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_market_data_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/async_trader/clients/async_trading_client.py` & `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/client.py` & `lime_trader_sdk-0.2.0/lime_trader/client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/clients/account_client.py` & `lime_trader_sdk-0.2.0/lime_trader/clients/account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/clients/account_feed_client.py` & `lime_trader_sdk-0.2.0/lime_trader/clients/account_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/clients/market_data_client.py` & `lime_trader_sdk-0.2.0/lime_trader/clients/market_data_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/clients/market_data_feed_client.py` & `lime_trader_sdk-0.2.0/lime_trader/clients/market_data_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/clients/trading_client.py` & `lime_trader_sdk-0.2.0/lime_trader/clients/trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/constants/urls.py` & `lime_trader_sdk-0.2.0/lime_trader/constants/urls.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/converters/abstract_converter.py` & `lime_trader_sdk-0.2.0/lime_trader/converters/abstract_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/converters/cattr_converter.py` & `lime_trader_sdk-0.2.0/lime_trader/converters/cattr_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/handlers/account_feed_handler.py` & `lime_trader_sdk-0.2.0/lime_trader/handlers/account_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/handlers/market_data_feed_handler.py` & `lime_trader_sdk-0.2.0/lime_trader/handlers/market_data_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/models/accounts.py` & `lime_trader_sdk-0.2.0/lime_trader/models/accounts.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/models/market.py` & `lime_trader_sdk-0.2.0/lime_trader/models/market.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/models/page.py` & `lime_trader_sdk-0.2.0/lime_trader/models/page.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/models/token_storage.py` & `lime_trader_sdk-0.2.0/lime_trader/models/token_storage.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/models/trading.py` & `lime_trader_sdk-0.2.0/lime_trader/models/trading.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/utils/date_utils.py` & `lime_trader_sdk-0.2.0/lime_trader/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/utils/logging_utils.py` & `lime_trader_sdk-0.2.0/lime_trader/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/lime_trader/utils/pagination.py` & `lime_trader_sdk-0.2.0/lime_trader/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.1.0/pyproject.toml` & `lime_trader_sdk-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lime-trader-sdk"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python wrapper for Lime Trader REST API (https://docs.lime.co/trader/)"
 authors = ["Lime Financial <support@lime.co>"]
 readme = "README.md"
 packages = [{include = "lime_trader"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `lime_trader_sdk-0.1.0/PKG-INFO` & `lime_trader_sdk-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-trader-sdk
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python wrapper for Lime Trader REST API (https://docs.lime.co/trader/)
 Author: Lime Financial
 Author-email: support@lime.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

