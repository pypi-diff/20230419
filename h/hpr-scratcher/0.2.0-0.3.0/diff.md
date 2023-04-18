# Comparing `tmp/hpr_scratcher-0.2.0.tar.gz` & `tmp/hpr_scratcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpr_scratcher-0.2.0.tar", max compression
+gzip compressed data, was "hpr_scratcher-0.3.0.tar", max compression
```

## Comparing `hpr_scratcher-0.2.0.tar` & `hpr_scratcher-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1473 2023-04-18 17:24:49.959974 hpr_scratcher-0.2.0/README.md
--rwxr-xr-x   0        0        0     8173 2023-04-18 17:21:39.069206 hpr_scratcher-0.2.0/hpr_scratcher/__init__.py
--rw-r--r--   0        0        0      479 2023-04-18 17:27:36.040522 hpr_scratcher-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 hpr_scratcher-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2305 2023-04-18 22:15:57.692034 hpr_scratcher-0.3.0/README.md
+-rwxr-xr-x   0        0        0     9028 2023-04-18 22:13:50.352941 hpr_scratcher-0.3.0/hpr_scratcher/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-18 22:14:52.764472 hpr_scratcher-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 hpr_scratcher-0.3.0/PKG-INFO
```

### Comparing `hpr_scratcher-0.2.0/README.md` & `hpr_scratcher-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -36,28 +36,77 @@
 
 ```json
 {
   "term": {
     "command": "kitty --class kitty-dropterm",
     "class": "kitty-dropterm",
     "offset": 800,
+    "animation": "fromTop",
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "class": "pavucontrol",
+    "animation": "fromTop",
     "offset": 1200
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
+## Options
+
+### animation
+
+Type of animation to use
+
+- `null` / `""`
+- `"fromTop"`
+
+_TODO_:
+
+- `fromBottom`
+- `fromLeft`
+- `fromRight`
+
+### offset
+
+number of pixels for the animation.
+
+### class
+
+class of the created window
+
+### unfocus
+
+allow to hide the window when the focus is lost when set to "hide"
+
+# Changelog
+
+# 0.3.0 (WIP)
+
+- add animation (only "fromTop" now, but can be switched off)
+- pid used in most commands (more reliable)
+- FIX: stop pinning the windows
+- FIX: debug traces
+- FIX: close processes on exit (should be configurable ?)
+
+# 0.2.0
+
+- reload command
+- allow automatic hiding on focus
+
+# 0.1.0
+
+- first version, close to no options
+
 # TODO
 
+- Add some period of grace after a dropdown is shown, so the window can't be closed by unfocus in the fist X seconds
 - Better handling of fast repetitions
 - Allow different "poles" for scratchpads instead of always sliding from the top
 - Make the usage of an explicit offset not needed
 - study avoiding the usage of classes to track the windows (once registered)
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

### Comparing `hpr_scratcher-0.2.0/hpr_scratcher/__init__.py` & `hpr_scratcher-0.3.0/hpr_scratcher/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         if client.get("class") == name:
             return client
 
 
 class Scratch:
     def __init__(self, uid, opts):
         self.uid = uid
+        self.pid = 0
         self.conf = opts
         self.visible = False
         self.just_created = True
 
 
 class ScratchpadManager:
     server: asyncio.Server
@@ -80,17 +81,34 @@
                 stdin=subprocess.DEVNULL,
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 shell=True,
             )
             for name, scratch in self.scratches.items()
         }
+        for name, proc in self.procs.items():
+            self.scratches[name].pid = proc.pid
 
     # event handlers:
 
+    async def event_fullscreen(self, params):
+        pass
+
+    async def event_workspace(self, params):
+        pass
+
+    async def event_destroyworkspace(self, params):
+        pass
+
+    async def event_createworkspace(self, params):
+        pass
+
+    async def event_focusedmon(self, params):
+        pass
+
     async def event_openwindow(self, params):
         addr, wrkspc, kls, title = params.split(",", 3)
         if wrkspc == "special":
             item = self.scratches_by_class.get(kls)
             if item and item.just_created:
                 await self.run_hide(item.uid, force=True)
                 item.just_created = False
@@ -132,18 +150,20 @@
         if not item:
             print(f"{uid} is not configured")
             return
         if not item.visible and not force:
             print(f"{uid} is already hidden")
             return
         item.visible = False
-        kls = item.conf["class"]
-        hyprctl(f"movewindowpixel 0 -{item.conf['offset']},^({kls})$")
-        await asyncio.sleep(0.2)
-        hyprctl(f"movetoworkspacesilent special,^({kls})$")
+        pid = "pid:%d" % item.pid
+        if item.conf.get("animation"):
+            # TODO: handle different directions
+            hyprctl(f"movewindowpixel 0 -{item.conf['offset']},{pid}")
+            await asyncio.sleep(0.2)
+        hyprctl(f"movetoworkspacesilent special,{pid}")
 
     async def run_show(self, uid, force=False):
         uid = uid.strip()
         item = self.scratches.get(uid)
 
         if not item:
             print(f"{uid} is not configured")
@@ -152,49 +172,51 @@
         if item.visible and not force:
             print(f"{uid} is already visible")
             return
 
         item.visible = True
         monitor = get_focused_monitor()
         assert monitor
-        kls = item.conf["class"]
-        client = get_client_by_class(kls)
+        client = get_client_by_class(item.conf["class"])
         assert client
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = monitor["width"]
 
         offset = client["at"][1]
-        if offset > -1:
-            print(f"Huhu, didn't expect this! offset={offset}")
+        if offset > -1 and DEBUG:
+            print(f"....didn't expect this! offset={offset}")
+
+        pid = "pid:%d" % item.pid
 
         client_width = client["size"][0]
         margin_x = int((mon_width - client_width) / 2) + mon_x
         wrkspc = monitor["activeWorkspace"]["id"]
-        hyprctl(f"movetoworkspace {wrkspc},^({kls})$")
-        hyprctl(f"pin ^({kls})$")
-        hyprctl(f"movewindowpixel exact {margin_x} {mon_y + MARGIN},^({kls})$")
-        hyprctl(f"focuswindow ^({kls})$")
+        hyprctl(f"movetoworkspacesilent {wrkspc},{pid}")
+        if item.conf.get("animation"):
+            # TODO: handle directions
+            hyprctl(f"movewindowpixel exact {margin_x} {mon_y + MARGIN},{pid}")
+        hyprctl(f"focuswindow {pid}")
 
     # Async loops & handlers (dispatchers):
 
     async def read_events_loop(self):
         while not self.stopped:
             data = (await self.event_reader.readline()).decode()
             if not data:
                 print("Reader starved")
                 return
             cmd, params = data.split(">>")
             full_name = f"event_{cmd}"
             if hasattr(self, full_name):
                 if DEBUG:
-                    print("EVT", full_name, params)
+                    print(f"EVT {full_name}({params.strip()})")
                 await getattr(self, full_name)(params)
             else:
-                print("unknown event:", cmd, "///", params)
+                print(f"unknown event: {cmd} ({params.strip()})")
 
     async def read_command(self, reader, writer):
         data = (await reader.readline()).decode()
         if not data:
             print("Server starved")
             return
         if data == "exit\n":
@@ -209,22 +231,30 @@
             args = []
         else:
             cmd = args[0]
             args = args[1:]
         full_name = f"run_{cmd}"
         if hasattr(self, full_name):
             if DEBUG:
-                print("CMD:", full_name, args)
+                print(f"CMD: {full_name}({args})")
             await getattr(self, full_name)(*args)
         else:
             print("Unknown command:", cmd)
 
     async def serve(self):
-        async with self.server:
-            await self.server.serve_forever()
+        try:
+            async with self.server:
+                await self.server.serve_forever()
+        finally:
+            for scratch in self.scratches:
+                proc = self.procs[scratch]
+                proc.terminate()
+                await asyncio.sleep(0.1)
+                proc.kill()
+                proc.wait()
 
     async def run(self):
         await asyncio.gather(
             asyncio.create_task(self.serve()),
             asyncio.create_task(self.read_events_loop()),
         )
```

### Comparing `hpr_scratcher-0.2.0/PKG-INFO` & `hpr_scratcher-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpr-scratcher
-Version: 0.2.0
+Version: 0.3.0
 Summary: A scratchpad manager for hyprland
 Home-page: https://github.com/hyprland-community/hpr-scratcher
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,28 +51,77 @@
 
 ```json
 {
   "term": {
     "command": "kitty --class kitty-dropterm",
     "class": "kitty-dropterm",
     "offset": 800,
+    "animation": "fromTop",
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
     "class": "pavucontrol",
+    "animation": "fromTop",
     "offset": 1200
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
+## Options
+
+### animation
+
+Type of animation to use
+
+- `null` / `""`
+- `"fromTop"`
+
+_TODO_:
+
+- `fromBottom`
+- `fromLeft`
+- `fromRight`
+
+### offset
+
+number of pixels for the animation.
+
+### class
+
+class of the created window
+
+### unfocus
+
+allow to hide the window when the focus is lost when set to "hide"
+
+# Changelog
+
+# 0.3.0 (WIP)
+
+- add animation (only "fromTop" now, but can be switched off)
+- pid used in most commands (more reliable)
+- FIX: stop pinning the windows
+- FIX: debug traces
+- FIX: close processes on exit (should be configurable ?)
+
+# 0.2.0
+
+- reload command
+- allow automatic hiding on focus
+
+# 0.1.0
+
+- first version, close to no options
+
 # TODO
 
+- Add some period of grace after a dropdown is shown, so the window can't be closed by unfocus in the fist X seconds
 - Better handling of fast repetitions
 - Allow different "poles" for scratchpads instead of always sliding from the top
 - Make the usage of an explicit offset not needed
 - study avoiding the usage of classes to track the windows (once registered)
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

