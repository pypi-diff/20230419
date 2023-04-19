# Comparing `tmp/apiron-7.0.0.tar.gz` & `tmp/apiron-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiron-7.0.0.tar", last modified: Wed Dec  7 23:32:14 2022, max compression
+gzip compressed data, was "apiron-7.1.0.tar", last modified: Wed Apr 19 14:09:40 2023, max compression
```

## Comparing `apiron-7.0.0.tar` & `apiron-7.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.067115 apiron-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2022-12-07 23:32:05.000000 apiron-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       60 2022-12-07 23:32:05.000000 apiron-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-07 23:32:14.067115 apiron-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2461 2022-12-07 23:32:05.000000 apiron-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-12-07 23:32:05.000000 apiron-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2426 2022-12-07 23:32:14.067115 apiron-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-07 23:32:05.000000 apiron-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/src/apiron/
--rw-r--r--   0 runner    (1001) docker     (122)      550 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9372 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/src/apiron/endpoint/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/endpoint/json.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/endpoint/streaming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/endpoint/stub.py
--rw-r--r--   0 runner    (1001) docker     (122)      531 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/src/apiron/service/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/service/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      898 2022-12-07 23:32:05.000000 apiron-7.0.0/src/apiron/service/discoverable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/src/apiron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-07 23:32:14.000000 apiron-7.0.0/src/apiron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      717 2022-12-07 23:32:14.000000 apiron-7.0.0/src/apiron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-07 23:32:14.000000 apiron-7.0.0/src/apiron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-12-07 23:32:14.000000 apiron-7.0.0/src/apiron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-07 23:32:14.000000 apiron-7.0.0/src/apiron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.063115 apiron-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:14.067115 apiron-7.0.0/tests/service/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/service/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/service/test_discoverable.py
--rw-r--r--   0 runner    (1001) docker     (122)    10412 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7207 2022-12-07 23:32:05.000000 apiron-7.0.0/tests/test_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-19 14:09:30.000000 apiron-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 14:09:30.000000 apiron-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-19 14:09:40.819875 apiron-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-19 14:09:30.000000 apiron-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 14:09:30.000000 apiron-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-19 14:09:40.819875 apiron-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:09:30.000000 apiron-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.815875 apiron-7.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.815875 apiron-7.1.0/src/apiron/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/src/apiron/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/endpoint/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/endpoint/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/endpoint/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/src/apiron/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-19 14:09:30.000000 apiron-7.1.0/src/apiron/service/discoverable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/src/apiron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-19 14:09:40.000000 apiron-7.1.0/src/apiron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-19 14:09:40.000000 apiron-7.1.0/src/apiron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:09:40.000000 apiron-7.1.0/src/apiron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 14:09:40.000000 apiron-7.1.0/src/apiron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 14:09:40.000000 apiron-7.1.0/src/apiron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:40.819875 apiron-7.1.0/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/service/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/service/test_discoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-19 14:09:30.000000 apiron-7.1.0/tests/test_endpoint.py
```

### Comparing `apiron-7.0.0/LICENSE` & `apiron-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/PKG-INFO` & `apiron-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiron
-Version: 7.0.0
+Version: 7.1.0
 Summary: apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 Home-page: https://github.com/ithaka/apiron
 Author: Ithaka Harbors, Inc.
 Author-email: opensource@ithaka.org
 License: MIT
 Project-URL: Documentation, https://apiron.readthedocs.io
 Project-URL: Source, https://github.com/ithaka/apiron
```

### Comparing `apiron-7.0.0/README.md` & `apiron-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/setup.cfg` & `apiron-7.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apiron
-version = 7.0.0
+version = 7.1.0
 description = apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 author = Ithaka Harbors, Inc.
 author_email = opensource@ithaka.org
 url = https://github.com/ithaka/apiron
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
@@ -67,15 +67,15 @@
 precision = 2
 show_missing = True
 skip_covered = True
 
 [coverage:paths]
 source = 
 	src
-	.tox/*/site-packages
+	.tox/**/site-packages
 
 [tool:pytest]
 testpaths = tests
 addopts = -ra --strict-markers --cov
 xfail_strict = True
 
 [tox:tox]
```

### Comparing `apiron-7.0.0/src/apiron/__init__.py` & `apiron-7.1.0/src/apiron/__init__.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/client.py` & `apiron-7.1.0/src/apiron/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,29 +133,37 @@
 
 def _get_guaranteed_session(session: Optional[requests.Session]) -> requests.Session:
     if session:
         return session
     return requests.Session()
 
 
+def _get_retry_spec(endpoint: apiron.Endpoint, retry_spec: Optional[retry.Retry] = None) -> retry.Retry:
+    return retry_spec or endpoint.retry_spec or DEFAULT_RETRY
+
+
+def _get_timeout_spec(endpoint: apiron.Endpoint, timeout_spec: Optional[Timeout] = None) -> Timeout:
+    return timeout_spec or endpoint.timeout_spec or DEFAULT_TIMEOUT
+
+
 def call(
     service: apiron.Service,
     endpoint: apiron.Endpoint,
     method: Optional[str] = None,
     session: Optional[requests.Session] = None,
     params: Optional[Dict[str, Any]] = None,
     data: Optional[Dict[str, Any]] = None,
     files: Optional[Dict[str, str]] = None,
     json: Optional[Dict[str, Any]] = None,
     headers: Optional[Dict[str, Any]] = None,
     cookies: Optional[Dict[str, Any]] = None,
     auth: Optional[Any] = None,
     encoding: Optional[str] = None,
-    retry_spec: retry.Retry = DEFAULT_RETRY,
-    timeout_spec: Timeout = DEFAULT_TIMEOUT,
+    retry_spec: Optional[retry.Retry] = None,
+    timeout_spec: Optional[Timeout] = None,
     logger: Optional[logging.Logger] = None,
     allow_redirects: bool = True,
     return_raw_response_object: Optional[bool] = None,
     **kwargs,
 ):
     """
     :param Service service:
@@ -196,19 +204,19 @@
     :param str encoding:
         The codec to use when decoding the response.
         Default behavior is to have ``requests`` guess the codec.
         (default ``None``)
     :param urllib3.util.retry.Retry retry_spec:
         (optional)
         An override of the retry behavior for this call.
-        (default ``Retry(total=1, connect=1, read=1, status_forcelist=[500-level status codes])``)
+        (default ``None``)
     :param Timeout timeout_spec:
         (optional)
         An override of the timeout behavior for this call.
-        (default ``Timeout(connection_timeout=1, read_timeout=3)``)
+        (default ``None``)
     :param logging.Logger logger:
         (optional)
         An existing logger for logging from the proper caller for better correlation
     :param bool allow_redirects:
         (optional)
         Enable/disable GET/OPTIONS/POST/PUT/PATCH/DELETE/HEAD redirection
         (default ``True``)
@@ -225,15 +233,18 @@
     :raises requests.ConnectionError:
         if retry threshold exceeded due to connection or request timeouts
     """
     logger = logger or LOGGER
 
     managing_session = not session
     guaranteed_session = _get_guaranteed_session(session)
-    adapted_session = _adapt_session(guaranteed_session, adapters.HTTPAdapter(max_retries=retry_spec))
+
+    retry_spec_to_use = _get_retry_spec(endpoint, retry_spec)
+
+    adapted_session = _adapt_session(guaranteed_session, adapters.HTTPAdapter(max_retries=retry_spec_to_use))
 
     method = method or endpoint.default_method
 
     auth = auth or getattr(session, "auth", None) or service.auth
 
     request = _build_request_object(
         adapted_session,
@@ -248,17 +259,19 @@
         cookies=cookies,
         auth=auth,
         **kwargs,
     )
 
     logger.info("%s %s", method, request.url)
 
+    timeout_spec_to_use = _get_timeout_spec(endpoint, timeout_spec)
+
     response = adapted_session.send(
         request,
-        timeout=(timeout_spec.connection_timeout, timeout_spec.read_timeout),
+        timeout=(timeout_spec_to_use.connection_timeout, timeout_spec_to_use.read_timeout),
         stream=getattr(endpoint, "streaming", False),
         allow_redirects=allow_redirects,
         proxies=adapted_session.proxies or service.proxies,
     )
 
     logger.info(
         "%d %s%s",
```

### Comparing `apiron-7.0.0/src/apiron/endpoint/endpoint.py` & `apiron-7.1.0/src/apiron/endpoint/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import logging
 import string
 import sys
 import warnings
 from functools import partial, update_wrapper
 from typing import Optional, Any, Callable, Dict, Iterable, List, TypeVar, Union, TYPE_CHECKING
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     if sys.version_info >= (3, 10):
         from typing import Concatenate, ParamSpec
     else:
         from typing_extensions import Concatenate, ParamSpec
 
     from apiron.service import Service
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
 import requests
+from urllib3.util import retry
 
-from apiron import client
+from apiron import client, Timeout
 from apiron.exceptions import UnfulfilledParameterException
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _create_caller(
@@ -51,14 +52,16 @@
     def __init__(
         self,
         path: str = "/",
         default_method: str = "GET",
         default_params: Optional[Dict[str, Any]] = None,
         required_params: Optional[Iterable[str]] = None,
         return_raw_response_object: bool = False,
+        timeout_spec: Optional[Timeout] = None,
+        retry_spec: Optional[retry.Retry] = None,
     ):
         """
         :param str path:
             The URL path for this endpoint, without the protocol or domain
         :param str default_method:
             (Default ``'GET'``)
             The default method to use when calling this endpoint.
@@ -68,14 +71,22 @@
         :param required_params:
             An iterable of required parameter names.
             Calling an endpoint without its required parameters raises an exception.
         :param bool return_raw_response_object:
             Whether to return a :class:`requests.Response` object or call :func:`format_response` on it first.
             This can be overridden when calling the endpoint.
             (Default ``False``)
+        :param Timeout timeout_spec:
+            (optional)
+            An override of the timeout behavior for calls to this endpoint.
+            (default ``None``)
+        :param urllib3.util.retry.Retry retry_spec:
+            (optional)
+            An override of the retry behavior for calls to this endpoint.
+            (default ``None``)
         """
         self.default_method = default_method
 
         if "?" in path:
             warnings.warn(
                 f"Endpoint path ('{path}') may contain query parameters. "
                 f"Use the default_params or required_params attributes in the initialization of this endpoint, "
@@ -83,14 +94,16 @@
                 stacklevel=3,
             )
 
         self.path = path
         self.default_params = default_params or {}
         self.required_params = required_params or set()
         self.return_raw_response_object = return_raw_response_object
+        self.timeout_spec = timeout_spec
+        self.retry_spec = retry_spec
 
     def format_response(self, response: requests.Response) -> Union[str, Dict[str, Any], Iterable[bytes]]:
         """
         Extracts the appropriate type of response data from a :class:`requests.Response` object
 
         :param requests.Response response:
             The original response from :mod:`requests`
```

### Comparing `apiron-7.0.0/src/apiron/endpoint/json.py` & `apiron-7.1.0/src/apiron/endpoint/json.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/endpoint/streaming.py` & `apiron-7.1.0/src/apiron/endpoint/streaming.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/endpoint/stub.py` & `apiron-7.1.0/src/apiron/endpoint/stub.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/exceptions.py` & `apiron-7.1.0/src/apiron/exceptions.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/service/base.py` & `apiron-7.1.0/src/apiron/service/base.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron/service/discoverable.py` & `apiron-7.1.0/src/apiron/service/discoverable.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/src/apiron.egg-info/PKG-INFO` & `apiron-7.1.0/src/apiron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiron
-Version: 7.0.0
+Version: 7.1.0
 Summary: apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 Home-page: https://github.com/ithaka/apiron
 Author: Ithaka Harbors, Inc.
 Author-email: opensource@ithaka.org
 License: MIT
 Project-URL: Documentation, https://apiron.readthedocs.io
 Project-URL: Source, https://github.com/ithaka/apiron
```

### Comparing `apiron-7.0.0/src/apiron.egg-info/SOURCES.txt` & `apiron-7.1.0/src/apiron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/tests/service/test_base.py` & `apiron-7.1.0/tests/service/test_base.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/tests/service/test_discoverable.py` & `apiron-7.1.0/tests/service/test_discoverable.py`

 * *Files identical despite different names*

### Comparing `apiron-7.0.0/tests/test_client.py` & `apiron-7.1.0/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from unittest import mock
 
 import pytest
+from urllib3.util import retry
 
-from apiron import client, NoHostsAvailableException
+from apiron import client, NoHostsAvailableException, Timeout
 
 
 @pytest.fixture
 def mock_response():
     response = mock.Mock()
     response.history = []
     return response
 
 
 @pytest.fixture
 def mock_endpoint():
     endpoint = mock.Mock()
     endpoint.required_headers = {}
     endpoint.get_formatted_path.return_value = "/foo/"
+    endpoint.timeout_spec = None
+    endpoint.retry_spec = None
     del endpoint.stub_response
     return endpoint
 
 
 @pytest.fixture
 def mock_logger():
     return mock.Mock()
@@ -230,14 +233,81 @@
     session.send.return_value = mock_response
 
     client.call(service, mock_endpoint, session=session, logger=mock_logger, encoding="FAKE-CODEC")
 
     assert "FAKE-CODEC" == mock_response.encoding
 
 
+@mock.patch("apiron.client._build_request_object")
+@mock.patch("apiron.client._adapt_session")
+@mock.patch("requests.Session", autospec=True)
+def test_call_uses_configured_endpoint_timeout_spec(
+    MockSession, mock_adapt_session, mock_build_request_object, mock_response, mock_endpoint, mock_logger
+):
+    service = mock.Mock()
+    service.get_hosts.return_value = ["http://host1.biz"]
+    service.required_headers = {}
+
+    session = MockSession()
+    session.send.return_value = mock_response
+
+    request = mock.Mock()
+    mock_build_request_object.return_value = request
+    mock_endpoint.timeout_spec = Timeout(connection_timeout=1_000, read_timeout=1_000)
+
+    mock_session = MockSession()
+    mock_session.send.return_value = mock_response
+    mock_session.proxies = {}
+    mock_session.auth = ()
+    mock_adapt_session.return_value = mock_session
+
+    client.call(service, mock_endpoint, session=mock_session, logger=mock_logger)
+
+    session.send.assert_called_once_with(
+        request,
+        timeout=(1_000, 1_000),
+        stream=mock_endpoint.streaming,
+        allow_redirects=True,
+        proxies=service.proxies,
+    )
+
+
+@mock.patch("apiron.client._build_request_object")
+@mock.patch("apiron.client.adapters.HTTPAdapter", autospec=True)
+@mock.patch("requests.Session", autospec=True)
+def test_call_uses_configured_endpoint_retry_spec(
+    MockSession, MockAdapter, mock_build_request_object, mock_response, mock_endpoint, mock_logger
+):
+    service = mock.Mock()
+    service.get_hosts.return_value = ["http://host1.biz"]
+    service.required_headers = {}
+
+    session = MockSession()
+    session.send.return_value = mock_response
+
+    request = mock.Mock()
+    mock_build_request_object.return_value = request
+    retry_spec = retry.Retry(
+        total=42,
+        connect=42,
+        read=42,
+        status_forcelist=[500],
+    )
+    mock_endpoint.retry_spec = retry_spec
+
+    mock_session = MockSession()
+    mock_session.send.return_value = mock_response
+    mock_session.proxies = {}
+    mock_session.auth = ()
+
+    client.call(service, mock_endpoint, session=mock_session, logger=mock_logger)
+
+    MockAdapter.assert_called_once_with(max_retries=retry_spec)
+
+
 def test_build_request_object_raises_no_host_exception():
     service = mock.Mock()
     service.get_hosts.return_value = []
 
     with pytest.raises(NoHostsAvailableException):
         client._build_request_object(mock.Mock(), service, mock.Mock())
```

### Comparing `apiron-7.0.0/tests/test_endpoint.py` & `apiron-7.1.0/tests/test_endpoint.py`

 * *Files identical despite different names*

