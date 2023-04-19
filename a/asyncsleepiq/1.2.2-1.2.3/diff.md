# Comparing `tmp/asyncsleepiq-1.2.2.tar.gz` & `tmp/asyncsleepiq-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncsleepiq-1.2.2.tar", last modified: Fri Apr  1 20:51:21 2022, max compression
+gzip compressed data, was "asyncsleepiq-1.2.3.tar", last modified: Fri Apr  1 21:14:08 2022, max compression
```

## Comparing `asyncsleepiq-1.2.2.tar` & `asyncsleepiq-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 20:51:21.826717 asyncsleepiq-1.2.2/
--rw-rw-r--   0 home      (1000) home      (1000)     3765 2022-04-01 20:51:21.826717 asyncsleepiq-1.2.2/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)     2882 2022-02-21 16:48:25.000000 asyncsleepiq-1.2.2/README.md
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 20:51:21.826717 asyncsleepiq-1.2.2/asyncsleepiq/
--rw-rw-r--   0 home      (1000) home      (1000)      436 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/__init__.py
--rw-rw-r--   0 home      (1000) home      (1000)     1922 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/actuator.py
--rw-rw-r--   0 home      (1000) home      (1000)     8376 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.2/asyncsleepiq/api.py
--rw-rw-r--   0 home      (1000) home      (1000)     2290 2022-03-20 20:56:29.000000 asyncsleepiq-1.2.2/asyncsleepiq/asyncsleepiq.py
--rw-rw-r--   0 home      (1000) home      (1000)     2567 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/bed.py
--rw-rw-r--   0 home      (1000) home      (1000)     1214 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/consts.py
--rw-rw-r--   0 home      (1000) home      (1000)      272 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.2/asyncsleepiq/exceptions.py
--rw-rw-r--   0 home      (1000) home      (1000)     7130 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/foundation.py
--rw-rw-r--   0 home      (1000) home      (1000)     1542 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.2/asyncsleepiq/light.py
--rw-rw-r--   0 home      (1000) home      (1000)     1573 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/preset.py
--rw-rw-r--   0 home      (1000) home      (1000)        0 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.2/asyncsleepiq/py.typed
--rw-rw-r--   0 home      (1000) home      (1000)     2419 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq/sleeper.py
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 20:51:21.826717 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/
--rw-rw-r--   0 home      (1000) home      (1000)     3765 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)      484 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/SOURCES.txt
--rw-rw-r--   0 home      (1000) home      (1000)        1 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/dependency_links.txt
--rw-rw-r--   0 home      (1000) home      (1000)       36 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/requires.txt
--rw-rw-r--   0 home      (1000) home      (1000)       13 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.2/asyncsleepiq.egg-info/top_level.txt
--rw-rw-r--   0 home      (1000) home      (1000)       38 2022-04-01 20:51:21.826717 asyncsleepiq-1.2.2/setup.cfg
--rw-rw-r--   0 home      (1000) home      (1000)      703 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.2/setup.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 21:14:08.283027 asyncsleepiq-1.2.3/
+-rw-rw-r--   0 home      (1000) home      (1000)     3765 2022-04-01 21:14:08.283027 asyncsleepiq-1.2.3/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)     2882 2022-02-21 16:48:25.000000 asyncsleepiq-1.2.3/README.md
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 21:14:08.283027 asyncsleepiq-1.2.3/asyncsleepiq/
+-rw-rw-r--   0 home      (1000) home      (1000)      436 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/__init__.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1938 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/actuator.py
+-rw-rw-r--   0 home      (1000) home      (1000)     8376 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.3/asyncsleepiq/api.py
+-rw-rw-r--   0 home      (1000) home      (1000)     2290 2022-03-20 20:56:29.000000 asyncsleepiq-1.2.3/asyncsleepiq/asyncsleepiq.py
+-rw-rw-r--   0 home      (1000) home      (1000)     2586 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/bed.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1298 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/consts.py
+-rw-rw-r--   0 home      (1000) home      (1000)      272 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.3/asyncsleepiq/exceptions.py
+-rw-rw-r--   0 home      (1000) home      (1000)     7130 2022-04-01 20:51:21.000000 asyncsleepiq-1.2.3/asyncsleepiq/foundation.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1542 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.3/asyncsleepiq/light.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1599 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/preset.py
+-rw-rw-r--   0 home      (1000) home      (1000)        0 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.3/asyncsleepiq/py.typed
+-rw-rw-r--   0 home      (1000) home      (1000)     2535 2022-04-01 21:14:04.000000 asyncsleepiq-1.2.3/asyncsleepiq/sleeper.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-04-01 21:14:08.283027 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/
+-rw-rw-r--   0 home      (1000) home      (1000)     3765 2022-04-01 21:14:08.000000 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)      484 2022-04-01 21:14:08.000000 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/SOURCES.txt
+-rw-rw-r--   0 home      (1000) home      (1000)        1 2022-04-01 21:14:08.000000 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/dependency_links.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       36 2022-04-01 21:14:08.000000 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/requires.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       13 2022-04-01 21:14:08.000000 asyncsleepiq-1.2.3/asyncsleepiq.egg-info/top_level.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       38 2022-04-01 21:14:08.283027 asyncsleepiq-1.2.3/setup.cfg
+-rw-rw-r--   0 home      (1000) home      (1000)      703 2022-03-04 17:14:23.000000 asyncsleepiq-1.2.3/setup.py
```

### Comparing `asyncsleepiq-1.2.2/PKG-INFO` & `asyncsleepiq-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.2.2
+Version: 1.2.3
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Description: # AsyncSleepIQ
```

### Comparing `asyncsleepiq-1.2.2/README.md` & `asyncsleepiq-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/actuator.py` & `asyncsleepiq-1.2.3/asyncsleepiq/actuator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Actuator representation for SleepIQ API."""
 from __future__ import annotations
 
 from typing import Any
 
 from .api import SleepIQAPI
-from .consts import ACTUATORS_FULL, SIDES_FULL, End, Side
+from .consts import ACTUATORS_FULL, SIDES_FULL, SIDES_SHORT, End, Side
 
 
 class SleepIQActuator:
     """Actuator representation for SleepIQ API."""
 
     def __init__(
         self, api: SleepIQAPI, bed_id: str, side: Side, actuator: End
@@ -20,29 +20,29 @@
         self.side_full = SIDES_FULL[side]
         self.actuator = actuator
         self.actuator_full = ACTUATORS_FULL[actuator]
         self.position = 0
 
     def __str__(self) -> str:
         """Return string representation."""
-        return f"SleepIQActuator[{self.actuator_full} {self.side_full}], position={self.position}"
+        return f"SleepIQActuator[{self.actuator_full} {self.side}], position={self.position}"
 
     def __repr__(self) -> str:
         """Return string representation."""
-        return f"SleepIQActuator[{self.actuator_full} {self.side_full}], position={self.position}"
+        return f"SleepIQActuator[{self.actuator_full} {self.side}], position={self.position}"
 
     async def set_position(self, position: int, slow_speed: bool = False) -> None:
         """Set the position of an actuator through the API."""
         if position < 0 or position > 100:
             raise ValueError("Invalid position, must be between 0 and 100")
         if position == self.position:
             return
         data = {
             "position": position,
-            "side": self.side,
+            "side": SIDES_SHORT[self.side],
             "actuator": self.actuator,
             "speed": 1 if slow_speed else 0,
         }
         await self._api.put(f"bed/{self.bed_id}/foundation/adjustment/micro", data)
 
     async def update(self, data: dict[str, Any]) -> None:
         """Update the position of an actuator from the API."""
```

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/api.py` & `asyncsleepiq-1.2.3/asyncsleepiq/api.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/asyncsleepiq.py` & `asyncsleepiq-1.2.3/asyncsleepiq/asyncsleepiq.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/bed.py` & `asyncsleepiq-1.2.3/asyncsleepiq/bed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Bed object from SleepIQ API."""
 from __future__ import annotations
 
 from typing import Any
 
 from .api import SleepIQAPI
-from .consts import SIDES_FULL
+from .consts import SIDES_FULL, Side
 from .foundation import SleepIQFoundation
 from .sleeper import SleepIQSleeper
 
 
 class SleepIQBed:
     """Bed object from SleepIQ API."""
 
@@ -18,15 +18,15 @@
 
         self.name = data["name"]
         self.id = data["bedId"]
         self.mac_addr = data["macAddress"]
         self.paused = False
         self.sleepers = [
             SleepIQSleeper(api, self.id, data[f"sleeper{SIDES_FULL[side]}Id"], side)
-            for side in SIDES_FULL
+            for side in [Side.LEFT, Side.RIGHT]
             if data.get(f"sleeper{SIDES_FULL[side]}Id")
         ]
         self.foundation = SleepIQFoundation(api, self.id)
 
         self.model = "Unknown"
         if "model" in data:
             self.model = data["model"]
```

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/consts.py` & `asyncsleepiq-1.2.3/asyncsleepiq/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,17 @@
     WAVE = 3
 
 MASSAGE_MODES = [Mode.OFF, Mode.SOOTHE, Mode.REVITILIZE, Mode.WAVE]
 
 class Side(str, enum.Enum):
     LEFT = "L"
     RIGHT = "R"
-    NONE = "R"
-SIDES_FULL = {Side.LEFT: "Left", Side.RIGHT: "Right"}
+    NONE = "-"
+SIDES_SHORT = {Side.LEFT: "L", Side.RIGHT: "R", Side.NONE: "R"}
+SIDES_FULL = {Side.LEFT: "Left", Side.RIGHT: "Right", Side.NONE: "Right"}
 
 FOUNDATION_TYPES = ["single", "splitHead", "splitKing", "easternKing"]
 
 class End(str, enum.Enum):
     HEAD = "H"
     FOOT = "F"
 ACTUATORS_FULL = {End.HEAD: "Head", End.FOOT: "Foot"}
```

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/foundation.py` & `asyncsleepiq-1.2.3/asyncsleepiq/foundation.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/light.py` & `asyncsleepiq-1.2.3/asyncsleepiq/light.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/preset.py` & `asyncsleepiq-1.2.3/asyncsleepiq/preset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Foundation preset setting from SleepIQ API."""
 from __future__ import annotations
 
 from typing import Any
 from .api import SleepIQAPI
-from .consts import BED_PRESETS, NO_PRESET, SIDES_FULL, Side
+from .consts import BED_PRESETS, NO_PRESET, SIDES_FULL, SIDES_SHORT, Side
 
 class SleepIQPreset:
     """Foundation preset setting from SleepIQ API."""
 
     def __init__(self, api: SleepIQAPI, bed_id: str, side: Side) -> None:
         """Initialize preset setting."""
         self._api = api
@@ -32,15 +32,15 @@
         #
         if preset == NO_PRESET:
             return
         if preset not in BED_PRESETS:
             raise ValueError("Invalid preset")
         data = {
             "preset": BED_PRESETS[preset], 
-            "side": self.side,
+            "side": SIDES_SHORT[self.side],
             "speed": 1 if slow_speed else 0
         }
         await self._api.put("bed/" + self.bed_id + "/foundation/preset", data)
 
     async def update(self, data: dict[str, Any]) -> None:
         """Update the position of an actuator from the API."""
         self.preset = data[f"fsCurrentPositionPreset{self.side_full}"]
```

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq/sleeper.py` & `asyncsleepiq-1.2.3/asyncsleepiq/sleeper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Sleeper representation for SleepIQ API."""
 from __future__ import annotations
 
 from .api import SleepIQAPI
-from .consts import SIDES_FULL, Side
+from .consts import SIDES_FULL, SIDES_SHORT, Side
 
 
 class SleepIQSleeper:
     """Sleeper representation for SleepIQ API."""
 
     def __init__(
         self, api: SleepIQAPI, bed_id: str, sleeper_id: str, side: Side
@@ -38,23 +38,29 @@
         await self.api.put("sleeper/" + self.sleeper_id + "/calibrate")
 
     async def set_sleepnumber(self, setting: int) -> None:
         """Set sleep number 5-100 (multiple of 5)."""
         if 0 > setting or setting > 100:
             raise ValueError("Invalid SleepNumber, must be between 0 and 100")
         setting = int(round(setting / 5)) * 5
-        data = {"sleepNumber": setting, "side": self.side}
+        data = {
+            "sleepNumber": setting, 
+            "side": SIDES_SHORT[self.side],
+        }
         await self.api.put("bed/" + self.bed_id + "/sleepNumber", data)
 
     async def set_favsleepnumber(self, setting: int) -> None:
         """Set favorite sleep number 5-100 (multiple of 5)."""
         if 0 > setting or setting > 100:
             raise ValueError("Invalid SleepNumber, must be between 0 and 100")
         setting = int(round(setting / 5)) * 5
-        data = {"side": self.side, "sleepNumberFavorite": setting}
+        data = {
+            "side": SIDES_SHORT[self.side],
+            "sleepNumberFavorite": setting,
+        }
         await self.api.put("bed/" + self.bed_id + "/sleepNumberFavorite", data)
         await self.fetch_favsleepnumber()
 
     async def fetch_favsleepnumber(self) -> None:
         """Update fav_sleep_number from API."""
         json = await self.api.get("bed/" + self.bed_id + "/sleepNumberFavorite")
         self.fav_sleep_number = json["sleepNumberFavorite" + self.side_full]
```

### Comparing `asyncsleepiq-1.2.2/asyncsleepiq.egg-info/PKG-INFO` & `asyncsleepiq-1.2.3/asyncsleepiq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.2.2
+Version: 1.2.3
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Description: # AsyncSleepIQ
```

### Comparing `asyncsleepiq-1.2.2/setup.py` & `asyncsleepiq-1.2.3/setup.py`

 * *Files identical despite different names*

