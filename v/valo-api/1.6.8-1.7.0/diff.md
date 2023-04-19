# Comparing `tmp/valo_api-1.6.8.tar.gz` & `tmp/valo_api-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api-1.6.8.tar", max compression
+gzip compressed data, was "valo_api-1.7.0.tar", max compression
```

## Comparing `valo_api-1.6.8.tar` & `valo_api-1.7.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0     1074 2023-04-06 20:59:56.331739 valo_api-1.6.8/LICENSE
--rw-r--r--   0        0        0     2451 2023-04-06 20:59:56.331739 valo_api-1.6.8/README.md
--rw-r--r--   0        0        0     3135 2023-04-06 20:59:56.335739 valo_api-1.6.8/pyproject.toml
--rw-r--r--   0        0        0      388 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/__init__.py
--rw-r--r--   0        0        0      793 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/config.py
--rw-r--r--   0        0        0     6793 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/__init__.py
--rw-r--r--   0        0        0     8990 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/account_details.py
--rw-r--r--   0        0        0     3369 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/content.py
--rw-r--r--   0        0        0     3508 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/crosshair.py
--rw-r--r--   0        0        0    11005 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/leaderboard.py
--rw-r--r--   0        0        0     3787 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/match_details.py
--rw-r--r--   0        0        0    14140 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/match_history.py
--rw-r--r--   0        0        0    17609 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/mmr_details.py
--rw-r--r--   0        0        0     9551 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/mmr_history.py
--rw-r--r--   0        0        0     8985 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/raw.py
--rw-r--r--   0        0        0     3961 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/status.py
--rw-r--r--   0        0        0     4828 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/store_featured.py
--rw-r--r--   0        0        0     4659 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/store_offers.py
--rw-r--r--   0        0        0     3578 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/version_info.py
--rw-r--r--   0        0        0     3782 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints/website.py
--rw-r--r--   0        0        0     1185 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/exceptions/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/exceptions/rate_limit.py
--rw-r--r--   0        0        0     2069 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/__init__.py
--rw-r--r--   0        0        0      410 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/account_details.py
--rw-r--r--   0        0        0      541 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/competitive_updates_raw.py
--rw-r--r--   0        0        0      858 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/content.py
--rw-r--r--   0        0        0      371 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/error_response.py
--rw-r--r--   0        0        0      917 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/leaderboard.py
--rw-r--r--   0        0        0     5550 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/match_details_raw.py
--rw-r--r--   0        0        0     5996 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/match_history.py
--rw-r--r--   0        0        0      299 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/match_history_raw.py
--rw-r--r--   0        0        0     1317 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/mmr_details.py
--rw-r--r--   0        0        0      628 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/mmr_history.py
--rw-r--r--   0        0        0     1306 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/mmr_raw.py
--rw-r--r--   0        0        0      817 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/status.py
--rw-r--r--   0        0        0     1093 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/store_featured.py
--rw-r--r--   0        0        0      853 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/store_offers.py
--rw-r--r--   0        0        0      157 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/version_info.py
--rw-r--r--   0        0        0      236 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/responses/website.py
--rw-r--r--   0        0        0        0 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/utils/dict_struct.py
--rw-r--r--   0        0        0     3821 2023-04-06 20:59:56.467741 valo_api-1.6.8/valo_api/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-19 19:00:01.506382 valo_api-1.7.0/LICENSE
+-rw-r--r--   0        0        0     2451 2023-04-19 19:00:01.506382 valo_api-1.7.0/README.md
+-rw-r--r--   0        0        0     3115 2023-04-19 19:00:01.510382 valo_api-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/__init__.py
+-rw-r--r--   0        0        0      793 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/config.py
+-rw-r--r--   0        0        0     7593 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     8990 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/account_details.py
+-rw-r--r--   0        0        0     3369 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/content.py
+-rw-r--r--   0        0        0     3508 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/crosshair.py
+-rw-r--r--   0        0        0    11005 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/leaderboard.py
+-rw-r--r--   0        0        0    14178 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/lifetime_matches.py
+-rw-r--r--   0        0        0     3787 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/match_details.py
+-rw-r--r--   0        0        0    14140 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/match_history.py
+-rw-r--r--   0        0        0    17609 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/mmr_details.py
+-rw-r--r--   0        0        0     9551 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/mmr_history.py
+-rw-r--r--   0        0        0     8985 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/raw.py
+-rw-r--r--   0        0        0     3961 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/status.py
+-rw-r--r--   0        0        0     4828 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/store_featured.py
+-rw-r--r--   0        0        0     4659 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/store_offers.py
+-rw-r--r--   0        0        0     3578 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/version_info.py
+-rw-r--r--   0        0        0     3782 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/website.py
+-rw-r--r--   0        0        0     1407 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     2069 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/account_details.py
+-rw-r--r--   0        0        0      541 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/competitive_updates_raw.py
+-rw-r--r--   0        0        0      858 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/content.py
+-rw-r--r--   0        0        0      371 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/error_response.py
+-rw-r--r--   0        0        0      917 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/leaderboard.py
+-rw-r--r--   0        0        0     1175 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/lifetime_match.py
+-rw-r--r--   0        0        0     5550 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_details_raw.py
+-rw-r--r--   0        0        0     5996 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_history.py
+-rw-r--r--   0        0        0      299 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_history_raw.py
+-rw-r--r--   0        0        0     1317 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_details.py
+-rw-r--r--   0        0        0      628 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_history.py
+-rw-r--r--   0        0        0     1306 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_raw.py
+-rw-r--r--   0        0        0      817 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/status.py
+-rw-r--r--   0        0        0     1093 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/store_featured.py
+-rw-r--r--   0        0        0      853 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/store_offers.py
+-rw-r--r--   0        0        0      157 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/version_info.py
+-rw-r--r--   0        0        0      236 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/website.py
+-rw-r--r--   0        0        0        0 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/dict_struct.py
+-rw-r--r--   0        0        0     3821 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-1.7.0/PKG-INFO
```

### Comparing `valo_api-1.6.8/LICENSE` & `valo_api-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/README.md` & `valo_api-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/pyproject.toml` & `valo_api-1.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api"
-version = "1.6.8"
+version = "1.7.0"
 description = "Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPI"
 homepage = "https://github.com/raimannma/ValorantAPI"
 
@@ -33,23 +33,22 @@
 Pillow = "^9.2.0"
 msgspec = ">=0.12,<0.15"
 asyncio = {version = "^3.4.3", optional = true, extras = ["speedups"]}
 aiohttp = {version = "^3.8.3", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
-black = {version = "^23.1.0", allow-prereleases = true}
-darglint = "^1.8.1"
+black = {version = "^23.3.0", allow-prereleases = true}
 isort = "^5.12.0"
 mypy = ">=0.991,<1.3"
 mypy-extensions = ">=0.4.3,<1.1.0"
-pre-commit = "^3.2.0"
+pre-commit = "^3.2.2"
 pydocstyle = "^6.3.0"
-pylint = "^2.17.0"
-pytest = "^7.2.2"
+pylint = "^2.17.2"
+pytest = "^7.3.1"
 hypothesis = "^6.61.0"
 pyupgrade = "^3.3.1"
 safety = "^2.3.5"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.0.0"
 Sphinx = ">=5.3,<7.0"
 sphinxcontrib-applehelp = "^1.0.2"
```

### Comparing `valo_api-1.6.8/valo_api/config.py` & `valo_api-1.7.0/valo_api/config.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/__init__.py` & `valo_api-1.7.0/valo_api/endpoints/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from valo_api.endpoints.content import get_content, get_content_v1
 from valo_api.endpoints.crosshair import get_crosshair, get_crosshair_v1
 from valo_api.endpoints.leaderboard import (
     get_leaderboard,
     get_leaderboard_v1,
     get_leaderboard_v2,
 )
+from valo_api.endpoints.lifetime_matches import (
+    get_lifetime_matches_by_name,
+    get_lifetime_matches_by_name_v1,
+    get_lifetime_matches_by_puuid,
+    get_lifetime_matches_by_puuid_v1,
+)
 from valo_api.endpoints.match_details import get_match_details, get_match_details_v2
 from valo_api.endpoints.match_history import (
     get_match_history_by_name,
     get_match_history_by_name_v3,
     get_match_history_by_puuid,
     get_match_history_by_puuid_v3,
 )
@@ -85,14 +91,18 @@
     "get_leaderboard_v1",
     "get_leaderboard_v2",
     "get_leaderboard",
     "get_raw_data_v1",
     "get_raw_data",
     "get_crosshair_v1",
     "get_crosshair",
+    "get_lifetime_matches_by_name_v1",
+    "get_lifetime_matches_by_name",
+    "get_lifetime_matches_by_puuid_v1",
+    "get_lifetime_matches_by_puuid",
 ]
 
 try:
     from valo_api.endpoints.account_details import (
         get_account_details_by_name_async,
         get_account_details_by_name_v1_async,
         get_account_details_by_puuid_async,
@@ -101,14 +111,20 @@
     from valo_api.endpoints.content import get_content_async, get_content_v1_async
     from valo_api.endpoints.crosshair import get_crosshair_async, get_crosshair_v1_async
     from valo_api.endpoints.leaderboard import (
         get_leaderboard_async,
         get_leaderboard_v1_async,
         get_leaderboard_v2_async,
     )
+    from valo_api.endpoints.lifetime_matches import (
+        get_lifetime_matches_by_name_async,
+        get_lifetime_matches_by_name_v1_async,
+        get_lifetime_matches_by_puuid_async,
+        get_lifetime_matches_by_puuid_v1_async,
+    )
     from valo_api.endpoints.match_details import (
         get_match_details_async,
         get_match_details_v2_async,
     )
     from valo_api.endpoints.match_history import (
         get_match_history_by_name_async,
         get_match_history_by_name_v3_async,
@@ -186,11 +202,15 @@
             "get_leaderboard_v1_async",
             "get_leaderboard_v2_async",
             "get_leaderboard_async",
             "get_raw_data_v1_async",
             "get_raw_data_async",
             "get_crosshair_v1_async",
             "get_crosshair_async",
+            "get_lifetime_matches_by_name_v1_async",
+            "get_lifetime_matches_by_name_async",
+            "get_lifetime_matches_by_puuid_v1_async",
+            "get_lifetime_matches_by_puuid_async",
         ]
     )
 except ImportError:
     pass
```

### Comparing `valo_api-1.6.8/valo_api/endpoints/account_details.py` & `valo_api-1.7.0/valo_api/endpoints/account_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/content.py` & `valo_api-1.7.0/valo_api/endpoints/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/crosshair.py` & `valo_api-1.7.0/valo_api/endpoints/crosshair.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/leaderboard.py` & `valo_api-1.7.0/valo_api/endpoints/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/match_details.py` & `valo_api-1.7.0/valo_api/endpoints/match_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/match_history.py` & `valo_api-1.7.0/valo_api/endpoints/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/mmr_details.py` & `valo_api-1.7.0/valo_api/endpoints/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/mmr_history.py` & `valo_api-1.7.0/valo_api/endpoints/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/raw.py` & `valo_api-1.7.0/valo_api/endpoints/raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/status.py` & `valo_api-1.7.0/valo_api/endpoints/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/store_featured.py` & `valo_api-1.7.0/valo_api/endpoints/store_featured.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/store_offers.py` & `valo_api-1.7.0/valo_api/endpoints/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/version_info.py` & `valo_api-1.7.0/valo_api/endpoints/version_info.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints/website.py` & `valo_api-1.7.0/valo_api/endpoints/website.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/endpoints_config.py` & `valo_api-1.7.0/valo_api/endpoints_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,8 +16,15 @@
 
     MMR_HISTORY_BY_PUUID = "/valorant/{version}/by-puuid/mmr-history/{region}/{puuid}"
     MMR_HISTORY_BY_NAME = "/valorant/{version}/mmr-history/{region}/{name}/{tag}"
 
     MATCH_HISTORY_BY_PUUID = "/valorant/{version}/by-puuid/matches/{region}/{puuid}"
     MATCH_HISTORY_BY_NAME = "/valorant/{version}/matches/{region}/{name}/{tag}"
 
+    LIFETIME_MATCHES_BY_PUUID = (
+        "/valorant/{version}/by-puuid/lifetime/matches/{region}/{puuid}"
+    )
+    LIFETIME_MATCHES_BY_NAME = (
+        "/valorant/{version}/lifetime/matches/{region}/{name}/{tag}"
+    )
+
     CROSSHAIR = "/valorant/{version}/crosshair/generate"
```

### Comparing `valo_api-1.6.8/valo_api/exceptions/rate_limit.py` & `valo_api-1.7.0/valo_api/exceptions/rate_limit.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/exceptions/valo_api_exception.py` & `valo_api-1.7.0/valo_api/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/competitive_updates_raw.py` & `valo_api-1.7.0/valo_api/responses/competitive_updates_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/content.py` & `valo_api-1.7.0/valo_api/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/leaderboard.py` & `valo_api-1.7.0/valo_api/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/match_details_raw.py` & `valo_api-1.7.0/valo_api/responses/match_details_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/match_history.py` & `valo_api-1.7.0/valo_api/responses/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/mmr_details.py` & `valo_api-1.7.0/valo_api/responses/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/mmr_history.py` & `valo_api-1.7.0/valo_api/responses/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/mmr_raw.py` & `valo_api-1.7.0/valo_api/responses/mmr_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/status.py` & `valo_api-1.7.0/valo_api/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/store_featured.py` & `valo_api-1.7.0/valo_api/responses/store_featured.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/responses/store_offers.py` & `valo_api-1.7.0/valo_api/responses/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/valo_api/utils/fetch_endpoint.py` & `valo_api-1.7.0/valo_api/utils/fetch_endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.6.8/PKG-INFO` & `valo_api-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valo-api
-Version: 1.6.8
+Version: 1.7.0
 Summary: Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api
 Home-page: https://github.com/raimannma/ValorantAPI
 License: MIT
 Author: Manuel Raimann
 Author-email: raimannma@outlook.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

