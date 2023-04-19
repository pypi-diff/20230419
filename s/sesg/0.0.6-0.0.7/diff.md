# Comparing `tmp/sesg-0.0.6.tar.gz` & `tmp/sesg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.6.tar", max compression
+gzip compressed data, was "sesg-0.0.7.tar", max compression
```

## Comparing `sesg-0.0.6.tar` & `sesg-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.6/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.6/README.md
--rw-r--r--   0        0        0     2801 2023-04-18 16:48:51.447223 sesg-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.6/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.6/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.6/src/sesg/metrics.py
--rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.6/src/sesg/scopus/__init__.py
--rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.6/src/sesg/scopus/api.py
--rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.6/src/sesg/scopus/client.py
--rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.6/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.6/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.6/src/sesg/snowballing.py
--rw-r--r--   0        0        0     6042 2023-04-18 16:47:52.299822 sesg-0.0.6/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 sesg-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.7/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.7/README.md
+-rw-r--r--   0        0        0     2801 2023-04-19 01:32:20.739678 sesg-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.7/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.7/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.7/src/sesg/metrics.py
+-rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.7/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-19 01:30:57.284403 sesg-0.0.7/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.7/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.7/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.7/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.7/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     6042 2023-04-18 16:47:52.299822 sesg-0.0.7/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 sesg-0.0.7/PKG-INFO
```

### Comparing `sesg-0.0.6/LICENSE` & `sesg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/pyproject.toml` & `sesg-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.6"
+version = "0.0.7"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
```

### Comparing `sesg-0.0.6/src/sesg/graph.py` & `sesg-0.0.7/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/metrics.py` & `sesg-0.0.7/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/scopus/api.py` & `sesg-0.0.7/src/sesg/scopus/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         *,
         resets_at: Optional[datetime] = None,
     ) -> None:
         self.resets_at = resets_at
 
 
 class PayloadTooLargeError(Exception):
-    """The response has a status code of 413. Probably the search string is too long."""
+    """The response has a status code of 400. Probably the search string is too long."""
 
 
 def _api_key_is_expired(
     *,
     response: httpx.Response,
 ) -> bool:
     """Checks if a Scopus API key is expired, given the response of a Scopus Request.
@@ -142,15 +142,15 @@
     except (asyncio.TimeoutError, httpx.ConnectError):
         raise TimeoutError()
 
     if _api_key_is_expired(response=response):
         resets_at = _get_api_key_reset_date(response=response)
         raise APIKeyExpiredError(resets_at=resets_at)
 
-    if response.status_code == 413:
+    if response.status_code == 400:
         raise PayloadTooLargeError()
 
     return response
 
 
 def _create_request(
     *,
```

### Comparing `sesg-0.0.6/src/sesg/scopus/client.py` & `sesg-0.0.7/src/sesg/scopus/client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/scopus_client.py` & `sesg-0.0.7/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/search_string.py` & `sesg-0.0.7/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/snowballing.py` & `sesg-0.0.7/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/src/sesg/topic_extraction.py` & `sesg-0.0.7/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.6/PKG-INFO` & `sesg-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.6
+Version: 0.0.7
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

