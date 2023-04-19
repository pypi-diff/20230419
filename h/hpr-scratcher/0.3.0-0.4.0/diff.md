# Comparing `tmp/hpr_scratcher-0.3.0.tar.gz` & `tmp/hpr_scratcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpr_scratcher-0.3.0.tar", max compression
+gzip compressed data, was "hpr_scratcher-0.4.0.tar", max compression
```

## Comparing `hpr_scratcher-0.3.0.tar` & `hpr_scratcher-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2305 2023-04-18 22:15:57.692034 hpr_scratcher-0.3.0/README.md
--rwxr-xr-x   0        0        0     9028 2023-04-18 22:13:50.352941 hpr_scratcher-0.3.0/hpr_scratcher/__init__.py
--rw-r--r--   0        0        0      479 2023-04-18 22:14:52.764472 hpr_scratcher-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 hpr_scratcher-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2336 2023-04-19 11:24:59.572726 hpr_scratcher-0.4.0/README.md
+-rwxr-xr-x   0        0        0    10374 2023-04-19 11:20:15.796092 hpr_scratcher-0.4.0/hpr_scratcher/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-19 11:25:06.053113 hpr_scratcher-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 hpr_scratcher-0.4.0/PKG-INFO
```

### Comparing `hpr_scratcher-0.3.0/README.md` & `hpr_scratcher-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 ```json
 {
   "term": {
     "command": "kitty --class kitty-dropterm",
     "class": "kitty-dropterm",
     "offset": 800,
     "animation": "fromTop",
+    "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "class": "pavucontrol",
-    "animation": "fromTop",
-    "offset": 1200
+    "animation": "fromTop"
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
 ## Options
@@ -65,48 +65,55 @@
 
 _TODO_:
 
 - `fromBottom`
 - `fromLeft`
 - `fromRight`
 
-### offset
+### offset (optional)
 
 number of pixels for the animation.
 
 ### class
 
 class of the created window
 
-### unfocus
+### unfocus (optional)
 
 allow to hide the window when the focus is lost when set to "hide"
 
+### margin (optional)
+
+number of pixels for the margin
+
 # Changelog
 
-# 0.3.0 (WIP)
+# 0.4.0
+
+- the offset is now optional
+- the margin can be configured now
+- FIX: fast repetition of show/hide sequences
+- FIX: automatic hide on focus lost doesn't trigger before the window takes the focus
+
+# 0.3.0
 
 - add animation (only "fromTop" now, but can be switched off)
 - pid used in most commands (more reliable)
 - FIX: stop pinning the windows
 - FIX: debug traces
 - FIX: close processes on exit (should be configurable ?)
 
 # 0.2.0
 
-- reload command
+- add a "reload" command re-reading the configuration
 - allow automatic hiding on focus
 
 # 0.1.0
 
 - first version, close to no options
 
 # TODO
 
-- Add some period of grace after a dropdown is shown, so the window can't be closed by unfocus in the fist X seconds
-- Better handling of fast repetitions
 - Allow different "poles" for scratchpads instead of always sliding from the top
-- Make the usage of an explicit offset not needed
-- study avoiding the usage of classes to track the windows (once registered)
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

### Comparing `hpr_scratcher-0.3.0/hpr_scratcher/__init__.py` & `hpr_scratcher-0.4.0/hpr_scratcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,24 +45,26 @@
 class Scratch:
     def __init__(self, uid, opts):
         self.uid = uid
         self.pid = 0
         self.conf = opts
         self.visible = False
         self.just_created = True
+        self.clientInfo = {}
 
 
 class ScratchpadManager:
     server: asyncio.Server
     event_reader: asyncio.StreamReader
     stopped = False
 
     def __init__(self):
         self.procs = {}
         self.scratches = {}
+        self.transitioning_scratches = set()
         self.load_config()
 
     def load_config(self, reload=False):
         config = json.loads(
             open(os.path.expanduser(CONFIG_FILE), encoding="utf-8").read()
         )
         old_scratches = self.scratches
@@ -86,14 +88,35 @@
             for name, scratch in self.scratches.items()
         }
         for name, proc in self.procs.items():
             self.scratches[name].pid = proc.pid
 
     # event handlers:
 
+    async def event_moveworkspace(self, params):
+        pass
+
+    async def event_openlayer(self, params):
+        pass
+
+    async def event_closelayer(self, params):
+        pass
+
+    async def event_changefloatingmode(self, params):
+        pass
+
+    async def event_activelayout(self, params):
+        pass
+
+    async def event_urgent(self, params):
+        pass
+
+    async def event_closewindow(self, params):  # winid
+        pass
+
     async def event_fullscreen(self, params):
         pass
 
     async def event_workspace(self, params):
         pass
 
     async def event_destroyworkspace(self, params):
@@ -101,35 +124,39 @@
 
     async def event_createworkspace(self, params):
         pass
 
     async def event_focusedmon(self, params):
         pass
 
+    async def event_activewindowv2(self, params):
+        pass
+
     async def event_openwindow(self, params):
         addr, wrkspc, kls, title = params.split(",", 3)
         if wrkspc == "special":
             item = self.scratches_by_class.get(kls)
             if item and item.just_created:
                 await self.run_hide(item.uid, force=True)
                 item.just_created = False
 
-    async def event_activewindowv2(self, params):
-        pass
-
     async def event_activewindow(self, params):
         klass, _ = params.rstrip().split(",", 1)
         item = self.scratches_by_class.get(klass)
         if item:
             if item.just_created:
                 await self.run_hide(item.uid)
                 item.just_created = False
         else:
             for uid, scratch in self.scratches.items():
-                if scratch.visible and scratch.conf.get("unfocus") == "hide":
+                if (
+                    scratch.visible
+                    and scratch.conf.get("unfocus") == "hide"
+                    and scratch.uid not in self.transitioning_scratches
+                ):
                     await self.run_hide(uid)
 
     # command handlers
 
     async def run_reload(self):
         self.load_config(reload=True)
 
@@ -153,17 +180,29 @@
         if not item.visible and not force:
             print(f"{uid} is already hidden")
             return
         item.visible = False
         pid = "pid:%d" % item.pid
         if item.conf.get("animation"):
             # TODO: handle different directions
-            hyprctl(f"movewindowpixel 0 -{item.conf['offset']},{pid}")
+            offset = item.conf.get("offset")
+            if offset is None:
+                if "size" not in item.clientInfo:
+                    client = get_client_by_class(item.conf["class"])
+                    assert client
+                    item.clientInfo.update(client)
+
+                offset = int(1.3 * item.clientInfo["size"][1])
+
+            hyprctl(f"movewindowpixel 0 -{offset},{pid}")
+            if uid in self.transitioning_scratches:
+                return  # abort sequence
             await asyncio.sleep(0.2)
-        hyprctl(f"movetoworkspacesilent special,{pid}")
+        if uid not in self.transitioning_scratches:
+            hyprctl(f"movetoworkspacesilent special,{pid}")
 
     async def run_show(self, uid, force=False):
         uid = uid.strip()
         item = self.scratches.get(uid)
 
         if not item:
             print(f"{uid} is not configured")
@@ -174,32 +213,37 @@
             return
 
         item.visible = True
         monitor = get_focused_monitor()
         assert monitor
         client = get_client_by_class(item.conf["class"])
         assert client
+        item.clientInfo.update(client)
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = monitor["width"]
 
         offset = client["at"][1]
         if offset > -1 and DEBUG:
             print(f"....didn't expect this! offset={offset}")
 
         pid = "pid:%d" % item.pid
 
         client_width = client["size"][0]
         margin_x = int((mon_width - client_width) / 2) + mon_x
         wrkspc = monitor["activeWorkspace"]["id"]
+        self.transitioning_scratches.add(uid)
         hyprctl(f"movetoworkspacesilent {wrkspc},{pid}")
         if item.conf.get("animation"):
+            margin = item.conf.get("margin", MARGIN)
             # TODO: handle directions
-            hyprctl(f"movewindowpixel exact {margin_x} {mon_y + MARGIN},{pid}")
+            hyprctl(f"movewindowpixel exact {margin_x} {mon_y + margin},{pid}")
         hyprctl(f"focuswindow {pid}")
+        await asyncio.sleep(0.2)
+        self.transitioning_scratches.discard(uid)
 
     # Async loops & handlers (dispatchers):
 
     async def read_events_loop(self):
         while not self.stopped:
             data = (await self.event_reader.readline()).decode()
             if not data:
```

### Comparing `hpr_scratcher-0.3.0/PKG-INFO` & `hpr_scratcher-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpr-scratcher
-Version: 0.3.0
+Version: 0.4.0
 Summary: A scratchpad manager for hyprland
 Home-page: https://github.com/hyprland-community/hpr-scratcher
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,21 +52,21 @@
 ```json
 {
   "term": {
     "command": "kitty --class kitty-dropterm",
     "class": "kitty-dropterm",
     "offset": 800,
     "animation": "fromTop",
+    "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "class": "pavucontrol",
-    "animation": "fromTop",
-    "offset": 1200
+    "animation": "fromTop"
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
 ## Options
@@ -80,49 +80,56 @@
 
 _TODO_:
 
 - `fromBottom`
 - `fromLeft`
 - `fromRight`
 
-### offset
+### offset (optional)
 
 number of pixels for the animation.
 
 ### class
 
 class of the created window
 
-### unfocus
+### unfocus (optional)
 
 allow to hide the window when the focus is lost when set to "hide"
 
+### margin (optional)
+
+number of pixels for the margin
+
 # Changelog
 
-# 0.3.0 (WIP)
+# 0.4.0
+
+- the offset is now optional
+- the margin can be configured now
+- FIX: fast repetition of show/hide sequences
+- FIX: automatic hide on focus lost doesn't trigger before the window takes the focus
+
+# 0.3.0
 
 - add animation (only "fromTop" now, but can be switched off)
 - pid used in most commands (more reliable)
 - FIX: stop pinning the windows
 - FIX: debug traces
 - FIX: close processes on exit (should be configurable ?)
 
 # 0.2.0
 
-- reload command
+- add a "reload" command re-reading the configuration
 - allow automatic hiding on focus
 
 # 0.1.0
 
 - first version, close to no options
 
 # TODO
 
-- Add some period of grace after a dropdown is shown, so the window can't be closed by unfocus in the fist X seconds
-- Better handling of fast repetitions
 - Allow different "poles" for scratchpads instead of always sliding from the top
-- Make the usage of an explicit offset not needed
-- study avoiding the usage of classes to track the windows (once registered)
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

