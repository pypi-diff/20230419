# Comparing `tmp/alerts_in_ua-0.2.4-py3-none-any.whl.zip` & `tmp/alerts_in_ua-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 8468 bytes, number of entries: 13
--rw-r--r--  2.0 unx      123 b- defN 23-Feb-14 20:19 alerts_in_ua/__init__.py
--rw-r--r--  2.0 unx     1413 b- defN 23-Feb-13 10:07 alerts_in_ua/alert.py
--rw-r--r--  2.0 unx     2733 b- defN 23-Feb-13 10:45 alerts_in_ua/alerts.py
--rw-r--r--  2.0 unx     3275 b- defN 23-Feb-14 08:45 alerts_in_ua/async_client.py
--rw-r--r--  2.0 unx     3041 b- defN 23-Feb-14 09:15 alerts_in_ua/client.py
+Zip file size: 10183 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      123 b- defN 23-Apr-10 21:09 alerts_in_ua/__init__.py
+-rw-r--r--  2.0 unx      936 b- defN 23-Apr-10 20:53 alerts_in_ua/air_raid_alert_oblast_status.py
+-rw-r--r--  2.0 unx     2701 b- defN 23-Apr-10 20:59 alerts_in_ua/air_raid_alert_oblast_statuses.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-Apr-10 20:00 alerts_in_ua/alert.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Apr-10 20:00 alerts_in_ua/alerts.py
+-rw-r--r--  2.0 unx     3679 b- defN 23-Apr-10 20:47 alerts_in_ua/async_client.py
+-rw-r--r--  2.0 unx     3425 b- defN 23-Apr-10 20:48 alerts_in_ua/client.py
 -rw-r--r--  2.0 unx      310 b- defN 23-Feb-14 08:45 alerts_in_ua/errors.py
 -rw-r--r--  2.0 unx      713 b- defN 23-Feb-13 10:12 alerts_in_ua/ua_date_parser.py
 -rw-r--r--  2.0 unx      167 b- defN 23-Feb-13 20:38 alerts_in_ua/user_agent.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Feb-14 20:20 alerts_in_ua-0.2.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5677 b- defN 23-Feb-14 20:20 alerts_in_ua-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-14 20:20 alerts_in_ua-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-14 20:20 alerts_in_ua-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1062 b- defN 23-Feb-14 20:20 alerts_in_ua-0.2.4.dist-info/RECORD
-13 files, 19686 bytes uncompressed, 6692 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-19 09:41 alerts_in_ua-0.2.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5677 b- defN 23-Apr-19 09:41 alerts_in_ua-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 09:41 alerts_in_ua-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-19 09:41 alerts_in_ua-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1265 b- defN 23-Apr-19 09:41 alerts_in_ua-0.2.5.dist-info/RECORD
+15 files, 24568 bytes uncompressed, 8075 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
 Filename: alerts_in_ua/__init__.py
 Comment: 
 
+Filename: alerts_in_ua/air_raid_alert_oblast_status.py
+Comment: 
+
+Filename: alerts_in_ua/air_raid_alert_oblast_statuses.py
+Comment: 
+
 Filename: alerts_in_ua/alert.py
 Comment: 
 
 Filename: alerts_in_ua/alerts.py
 Comment: 
 
 Filename: alerts_in_ua/async_client.py
@@ -18,23 +24,23 @@
 
 Filename: alerts_in_ua/ua_date_parser.py
 Comment: 
 
 Filename: alerts_in_ua/user_agent.py
 Comment: 
 
-Filename: alerts_in_ua-0.2.4.dist-info/LICENSE.txt
+Filename: alerts_in_ua-0.2.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: alerts_in_ua-0.2.4.dist-info/METADATA
+Filename: alerts_in_ua-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: alerts_in_ua-0.2.4.dist-info/WHEEL
+Filename: alerts_in_ua-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: alerts_in_ua-0.2.4.dist-info/top_level.txt
+Filename: alerts_in_ua-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: alerts_in_ua-0.2.4.dist-info/RECORD
+Filename: alerts_in_ua-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alerts_in_ua/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 from .client import Client
 from .async_client import AsyncClient
 
 __all__ = ['Client','AsyncClient']
```

## alerts_in_ua/alert.py

```diff
@@ -12,16 +12,17 @@
         self.location_type = data.get("location_type")
         self.started_at = UaDateParser.parse_date(data.get("started_at"))
         self.finished_at = UaDateParser.parse_date(data.get("finished_at"))
         self.updated_at = UaDateParser.parse_date(data.get("updated_at"))
         self.alert_type = data.get("alert_type")
         self.location_uid = data.get("location_uid")
         self.location_oblast = data.get("location_oblast")
+        self.location_oblast_uid = data.get("location_oblast_uid")
         self.location_raion = data.get("location_raion")
         self.notes = data.get("notes")
         self.calculated = data.get("calculated")
 
 
     def is_finished(self) -> bool:
         return self.finished_at is not None
     def __repr__(self):
-        return f"Alert({{'id': {self.id!r}, 'location_title': {self.location_title!r}, 'location_type': {self.location_type!r}, 'started_at': {self.started_at!r}, 'finished_at': {self.finished_at!r}, 'updated_at': {self.updated_at!r}, 'alert_type': {self.alert_type!r}, 'location_uid': {self.location_uid!r}, 'location_oblast': {self.location_oblast!r}, 'location_raion': {self.location_raion!r}, 'notes': {self.notes!r}, 'calculated': {self.calculated!r}}}"
+        return f"Alert({{'id': {self.id!r}, 'location_title': {self.location_title!r}, 'location_type': {self.location_type!r}, 'started_at': {self.started_at!r}, 'finished_at': {self.finished_at!r}, 'updated_at': {self.updated_at!r}, 'alert_type': {self.alert_type!r}, 'location_uid': {self.location_uid!r}, 'location_oblast': {self.location_oblast!r}, 'location_oblast_uid': {self.location_oblast_uid!r}, 'location_raion': {self.location_raion!r}, 'notes': {self.notes!r}, 'calculated': {self.calculated!r}}}"
```

## alerts_in_ua/alerts.py

```diff
@@ -37,14 +37,17 @@
 
     def get_alerts_by_location_type(self, location_type: str) -> List[Alert]:
         return self.filter('location_type',location_type)
 
     def get_alerts_by_oblast(self, oblast_title: str) -> List[Alert]:
         return self.filter('location_oblast',oblast_title)
 
+    def get_alerts_by_oblast_uid(self, oblast_uid: str) -> List[Alert]:
+        return self.filter('location_oblast_uid',oblast_uid)
+
     def get_alerts_by_location_uid(self, location_uid: str) -> List[Alert]:
         return self.filter('location_uid',location_uid)
 
     def get_air_raid_alerts(self) -> List[Alert]:
         return self.get_alerts_by_alert_type('air_raid')
 
     def get_artillery_shelling_alerts(self) -> List[Alert]:
```

## alerts_in_ua/async_client.py

```diff
@@ -1,13 +1,13 @@
 import aiohttp
-from .errors import UnauthorizedError, RateLimitError, InternalServerError, ForbiddenError
+from .errors import UnauthorizedError, RateLimitError, InternalServerError, ForbiddenError, ApiError
 from .alert import Alert
 from .alerts import Alerts
 from .user_agent import UserAgent
-
+from .air_raid_alert_oblast_statuses import AirRaidAlertOblastStatuses
 class AsyncClient:
     REQUEST_TIMEOUT = 5
     API_BASE_URL = "https://api.alerts.in.ua"
 
     def __init__(self, token: str):
         self.token = token
         self.base_url = "/v1/"
@@ -72,10 +72,13 @@
                         message = "Too many requests: Rate limit exceeded"
                     raise RateLimitError(message)
                 elif response.status == 500:
                     raise InternalServerError("Internal server error")
                 else:
                     raise ApiError(f"Unknown error. HTTP Code:{response.status}")
 
-    async def get_active_alerts(self, use_cache=True):
+    async def get_active_alerts(self, use_cache=True) -> Alerts:
         data = await self._request("alerts/active.json", use_cache=use_cache)
         return Alerts(data)
+    async def get_air_raid_alert_statuses_by_oblast(self, oblast_level_only=False, use_cache=True) -> AirRaidAlertOblastStatuses:
+        data = await self._request("iot/active_air_raid_alerts_by_oblast.json", use_cache=use_cache)
+        return AirRaidAlertOblastStatuses(data,oblast_level_only=oblast_level_only)
```

## alerts_in_ua/client.py

```diff
@@ -1,13 +1,14 @@
 import requests
-from .errors import UnauthorizedError, RateLimitError, InternalServerError, ForbiddenError
+from .errors import UnauthorizedError, RateLimitError, InternalServerError, ForbiddenError, ApiError
 from .alert import Alert
 from .alerts import Alerts
 from .user_agent import UserAgent
 from typing import List, Dict, Union
+from .air_raid_alert_oblast_statuses import AirRaidAlertOblastStatuses
 
 class Client:
     REQUEST_TIMEOUT = 5
     API_BASE_URL = "https://api.alerts.in.ua"
     def __init__(self, token: str):
         self.token = token
         self.base_url = Client.API_BASE_URL + "/v1/"
@@ -73,8 +74,11 @@
             elif response.status_code == 500:
                 raise InternalServerError("Internal server error")
             else:
                 raise ApiError(f"Unknown error. HTTP Code:{response.status_code}")
 
     def get_active_alerts(self, use_cache=True) -> Alerts:
         data = self._request("alerts/active.json", use_cache=use_cache)
-        return Alerts(data)
+        return Alerts(data)
+    def get_air_raid_alert_statuses_by_oblast(self, oblast_level_only=False, use_cache=True) -> AirRaidAlertOblastStatuses:
+        data = self._request("iot/active_air_raid_alerts_by_oblast.json", use_cache=use_cache)
+        return AirRaidAlertOblastStatuses(data,oblast_level_only=oblast_level_only)
```

## Comparing `alerts_in_ua-0.2.4.dist-info/LICENSE.txt` & `alerts_in_ua-0.2.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `alerts_in_ua-0.2.4.dist-info/METADATA` & `alerts_in_ua-0.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerts-in-ua
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library for alerts.in.ua API
 Home-page: https://github.com/alerts-ua/alerts-in-ua-py
 Author: Ukrzen Team
 Author-email: api@alerts.in.ua
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `alerts_in_ua-0.2.4.dist-info/RECORD` & `alerts_in_ua-0.2.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-alerts_in_ua/__init__.py,sha256=kFSYqkHOGGXbQ7Sc6d-ijEpw5pct0uPxrkb-J46Akx8,123
-alerts_in_ua/alert.py,sha256=bt-FOdBGNzbwp19A8KN0WLzgvGIQFxQc5Cmu-4CLzyI,1413
-alerts_in_ua/alerts.py,sha256=dI_DPlwRX0aHddmpcBr70cjBCIa_mCVV9wQeU4Pu46w,2733
-alerts_in_ua/async_client.py,sha256=llMO_Ckb9UsTYZmtfb4UZKhenvG2SKAqy4OHLh8NORo,3275
-alerts_in_ua/client.py,sha256=nTVIZgPoJhpgCnxDLWe8ZB1b4y53Mi9QYGR-tu-Gkrw,3041
+alerts_in_ua/__init__.py,sha256=UM6P8aocbnrCmF2Gia3Vybonp_e0CSZrzcnrFvOQEUA,123
+alerts_in_ua/air_raid_alert_oblast_status.py,sha256=2BOSVREL497hrVot5vUi4qR_6GF2GMqKKYvWLJXYyFo,936
+alerts_in_ua/air_raid_alert_oblast_statuses.py,sha256=tOSoYz8RZ6-9mX7qh3asp0JJuevQHMQZzqGqoCFIRe0,2701
+alerts_in_ua/alert.py,sha256=iW9bTseurKjvLXrq2r1kopR67rlVv-pQttuwDGeo_KQ,1533
+alerts_in_ua/alerts.py,sha256=IruMhy94Rwr1OC6XHIkSfbtFjf2A6VSnlldEQixzApw,2867
+alerts_in_ua/async_client.py,sha256=uPk4ZKgnX1xXls7btOX8d37rqdz4oV07oliksvTC1Yg,3679
+alerts_in_ua/client.py,sha256=2ZbdTGagSYSWUkJOEwH_GugLkp10x-MF0x_BleKskdQ,3425
 alerts_in_ua/errors.py,sha256=sxb5iPl2M_SC6RKz16jNSmgQ_P9Db-kA8I6dj0VqPlg,310
 alerts_in_ua/ua_date_parser.py,sha256=8MrckVsSe0wHk_SGEETO6LK6s8A0YQ0RhH6xswski5g,713
 alerts_in_ua/user_agent.py,sha256=-qu2Cng5ZMaflrtclccZaxG6QZxTnkYbQiVT5jaScsw,167
-alerts_in_ua-0.2.4.dist-info/LICENSE.txt,sha256=zN5JNSULOzNf0YhIwcbBUFQ4ZrXN3t1gPWF6yqHxdpw,1067
-alerts_in_ua-0.2.4.dist-info/METADATA,sha256=9dWPD9THR-qaqW76ITXtsUkoPD96WyusZuNuZI47lkA,5677
-alerts_in_ua-0.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-alerts_in_ua-0.2.4.dist-info/top_level.txt,sha256=ID8v6qr4Y2AKvMy7IJoD13YcLyqS4LYrpaZnLY2TqLs,13
-alerts_in_ua-0.2.4.dist-info/RECORD,,
+alerts_in_ua-0.2.5.dist-info/LICENSE.txt,sha256=zN5JNSULOzNf0YhIwcbBUFQ4ZrXN3t1gPWF6yqHxdpw,1067
+alerts_in_ua-0.2.5.dist-info/METADATA,sha256=xMNaWvXSHixfoCaMn8kW9ZRbHFLqAbq1zni8ZeUPGh0,5677
+alerts_in_ua-0.2.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+alerts_in_ua-0.2.5.dist-info/top_level.txt,sha256=ID8v6qr4Y2AKvMy7IJoD13YcLyqS4LYrpaZnLY2TqLs,13
+alerts_in_ua-0.2.5.dist-info/RECORD,,
```

