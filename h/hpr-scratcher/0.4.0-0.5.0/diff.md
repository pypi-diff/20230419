# Comparing `tmp/hpr_scratcher-0.4.0.tar.gz` & `tmp/hpr_scratcher-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpr_scratcher-0.4.0.tar", max compression
+gzip compressed data, was "hpr_scratcher-0.5.0.tar", max compression
```

## Comparing `hpr_scratcher-0.4.0.tar` & `hpr_scratcher-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2336 2023-04-19 11:24:59.572726 hpr_scratcher-0.4.0/README.md
--rwxr-xr-x   0        0        0    10374 2023-04-19 11:20:15.796092 hpr_scratcher-0.4.0/hpr_scratcher/__init__.py
--rw-r--r--   0        0        0      479 2023-04-19 11:25:06.053113 hpr_scratcher-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 hpr_scratcher-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2957 2023-04-19 15:25:07.637443 hpr_scratcher-0.5.0/README.md
+-rwxr-xr-x   0        0        0    13721 2023-04-19 15:10:02.799997 hpr_scratcher-0.5.0/hpr_scratcher/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-19 15:24:57.870300 hpr_scratcher-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 hpr_scratcher-0.5.0/PKG-INFO
```

### Comparing `hpr_scratcher-0.4.0/README.md` & `hpr_scratcher-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,24 @@
 
 - copy and rename the `__init__.py` file to some accessible path, do not forget to add +x to it
 
 # Features
 
 - Allow showing & hiding sliding scratchpads
 - Allow auto-hide when the focus is lost
+- Supports optional animation from top, bottom, left or right
+- Reload config without restart
 
 # Usage
 
+As an example, defining two scratchpads:
+
+- _term_ which would be a kitty terminal on upper part of the screen
+- _volume_ which would be a pavucontrol window on the right part of the screen
+
 In your `hyprland.conf` add something like this:
 
 ```ini
 exec-once = hpr-scratcher
 
 # Repeat this for each scratchpad you need
 bind = $mainMod,V,exec,hpr-scratcher toggle volume
@@ -33,64 +40,74 @@
 ```
 
 Then in $HOME/.config/hypr/scratchpads.json add:
 
 ```json
 {
   "term": {
-    "command": "kitty --class kitty-dropterm",
-    "class": "kitty-dropterm",
-    "offset": 800,
+    "command": "kitty",
     "animation": "fromTop",
     "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
-    "class": "pavucontrol",
-    "animation": "fromTop"
+    "animation": "fromRight"
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
-## Options
+## Command-line options
 
-### animation
+- `reload` : reloads the configuration file
+- `toggle <scratchpad name>` : toggle the given scratchpad
+- `show <scratchpad name>` : show the given scratchpad
+- `hide <scratchpad name>` : hide the given scratchpad
 
-Type of animation to use
+Note: with no argument it runs the daemon (doesn't fork in the background)
 
-- `null` / `""`
-- `"fromTop"`
+## Scratchpad Options
 
-_TODO_:
+### animation
 
-- `fromBottom`
-- `fromLeft`
-- `fromRight`
+Type of animation to use
+
+- `null` / `""` / not defined
+- "fromTop"
+- "fromBottom"
+- "fromLeft"
+- "fromRight"
 
 ### offset (optional)
 
 number of pixels for the animation.
 
-### class
-
-class of the created window
-
 ### unfocus (optional)
 
 allow to hide the window when the focus is lost when set to "hide"
 
 ### margin (optional)
 
 number of pixels for the margin
 
 # Changelog
 
+# 0.5.0
+
+- windows can slide from any direction now (values for "animation" property):
+  - `fromTop`
+  - `fromBottom`
+  - `fromLeft`
+  - `fromRight`
+- make "class" option obsolete
+- FIX: code reloading
+- FIX: misc improvements
+
 # 0.4.0
 
 - the offset is now optional
 - the margin can be configured now
 - FIX: fast repetition of show/hide sequences
 - FIX: automatic hide on focus lost doesn't trigger before the window takes the focus
 
@@ -109,11 +126,10 @@
 
 # 0.1.0
 
 - first version, close to no options
 
 # TODO
 
-- Allow different "poles" for scratchpads instead of always sliding from the top
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

### Comparing `hpr_scratcher-0.4.0/PKG-INFO` & `hpr_scratcher-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpr-scratcher
-Version: 0.4.0
+Version: 0.5.0
 Summary: A scratchpad manager for hyprland
 Home-page: https://github.com/hyprland-community/hpr-scratcher
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,17 +23,24 @@
 
 - copy and rename the `__init__.py` file to some accessible path, do not forget to add +x to it
 
 # Features
 
 - Allow showing & hiding sliding scratchpads
 - Allow auto-hide when the focus is lost
+- Supports optional animation from top, bottom, left or right
+- Reload config without restart
 
 # Usage
 
+As an example, defining two scratchpads:
+
+- _term_ which would be a kitty terminal on upper part of the screen
+- _volume_ which would be a pavucontrol window on the right part of the screen
+
 In your `hyprland.conf` add something like this:
 
 ```ini
 exec-once = hpr-scratcher
 
 # Repeat this for each scratchpad you need
 bind = $mainMod,V,exec,hpr-scratcher toggle volume
@@ -48,64 +55,74 @@
 ```
 
 Then in $HOME/.config/hypr/scratchpads.json add:
 
 ```json
 {
   "term": {
-    "command": "kitty --class kitty-dropterm",
-    "class": "kitty-dropterm",
-    "offset": 800,
+    "command": "kitty",
     "animation": "fromTop",
     "margin": 50,
     "unfocus": "hide"
   },
   "volume": {
     "command": "pavucontrol",
-    "class": "pavucontrol",
-    "animation": "fromTop"
+    "animation": "fromRight"
   }
 }
 ```
 
 And you'll be able to toggle pavucontrol with MOD + V.
 
-## Options
+## Command-line options
 
-### animation
+- `reload` : reloads the configuration file
+- `toggle <scratchpad name>` : toggle the given scratchpad
+- `show <scratchpad name>` : show the given scratchpad
+- `hide <scratchpad name>` : hide the given scratchpad
 
-Type of animation to use
+Note: with no argument it runs the daemon (doesn't fork in the background)
 
-- `null` / `""`
-- `"fromTop"`
+## Scratchpad Options
 
-_TODO_:
+### animation
 
-- `fromBottom`
-- `fromLeft`
-- `fromRight`
+Type of animation to use
+
+- `null` / `""` / not defined
+- "fromTop"
+- "fromBottom"
+- "fromLeft"
+- "fromRight"
 
 ### offset (optional)
 
 number of pixels for the animation.
 
-### class
-
-class of the created window
-
 ### unfocus (optional)
 
 allow to hide the window when the focus is lost when set to "hide"
 
 ### margin (optional)
 
 number of pixels for the margin
 
 # Changelog
 
+# 0.5.0
+
+- windows can slide from any direction now (values for "animation" property):
+  - `fromTop`
+  - `fromBottom`
+  - `fromLeft`
+  - `fromRight`
+- make "class" option obsolete
+- FIX: code reloading
+- FIX: misc improvements
+
 # 0.4.0
 
 - the offset is now optional
 - the margin can be configured now
 - FIX: fast repetition of show/hide sequences
 - FIX: automatic hide on focus lost doesn't trigger before the window takes the focus
 
@@ -124,12 +141,11 @@
 
 # 0.1.0
 
 - first version, close to no options
 
 # TODO
 
-- Allow different "poles" for scratchpads instead of always sliding from the top
 - Allow auto-restart of applications (if closed)
   - Allow closing the app on unfocus
 - Move to socket instead of hyprctl when possible
```

