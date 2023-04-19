# Comparing `tmp/pdbp-1.3.0.tar.gz` & `tmp/pdbp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.3.0.tar", last modified: Wed Apr 19 04:39:09 2023, max compression
+gzip compressed data, was "pdbp-1.3.1.tar", last modified: Wed Apr 19 18:40:42 2023, max compression
```

## Comparing `pdbp-1.3.0.tar` & `pdbp-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.717706 pdbp-1.3.0/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.3.0/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.3.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.3.0/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.3.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6454 2023-04-19 04:39:09.717765 pdbp-1.3.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4438 2023-04-19 04:33:33.000000 pdbp-1.3.0/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.3.0/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-19 04:39:09.717948 pdbp-1.3.0/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-19 04:33:33.000000 pdbp-1.3.0/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.716884 pdbp-1.3.0/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.3.0/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.717606 pdbp-1.3.0/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6454 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    52503 2023-04-19 04:33:33.000000 pdbp-1.3.0/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.433124 pdbp-1.3.1/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.3.1/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.3.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.3.1/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.3.1/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.3.1/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6294 2023-04-19 18:40:42.433176 pdbp-1.3.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4278 2023-04-19 18:37:55.000000 pdbp-1.3.1/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.3.1/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-19 18:40:42.433332 pdbp-1.3.1/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-19 18:37:55.000000 pdbp-1.3.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.432404 pdbp-1.3.1/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.3.1/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.433027 pdbp-1.3.1/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6294 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    52815 2023-04-19 18:37:55.000000 pdbp-1.3.1/src/pdbp.py
```

### Comparing `pdbp-1.3.0/.gitignore` & `pdbp-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.0/CODE_OF_CONDUCT.md` & `pdbp-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.0/CONTRIBUTING.md` & `pdbp-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.0/LICENSE` & `pdbp-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.0/PKG-INFO` & `pdbp-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.3.0
+Version: 1.3.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -103,17 +103,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbp-1.3.0/README.md` & `pdbp-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbp-1.3.0/setup.py` & `pdbp-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.3.0",
+    version="1.3.1",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
```

### Comparing `pdbp-1.3.0/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.3.1/src/pdbp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.3.0
+Version: 1.3.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -103,17 +103,14 @@
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
     pdb.DefaultConfig.filename_color = pdb.Color.blue
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
     pdb.DefaultConfig.truncate_long_lines = True
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
```

### Comparing `pdbp-1.3.0/src/pdbp.py` & `pdbp-1.3.1/src/pdbp.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,30 +247,28 @@
 
     def ensure_file_can_write_unicode(self, f):
         # Wrap with an encoder, but only if not already wrapped.
         if (not hasattr(f, "stream")
                 and getattr(f, "encoding", False)
                 and f.encoding.lower() != "utf-8"):
             f = codecs.getwriter("utf-8")(getattr(f, "buffer", f))
-
         return f
 
     def _disable_pytest_capture_maybe(self):
         try:
-            import py.test
-            # Force raising of ImportError if pytest is not installed.
-            py.test.config
+            import pytest
+            import _pytest
+            pytest.Config
+            _pytest.config
         except (ImportError, AttributeError):
-            return
+            return  # pytest is not installed
         try:
-            capman = py.test.config.pluginmanager.getplugin("capturemanager")
-            capman.suspendcapture()
-        except KeyError:
-            pass
-        except AttributeError:
+            capman = _pytest.capture.CaptureManager("global")
+            capman.stop_global_capturing()
+        except (KeyError, AttributeError, Exception):
             pass
 
     def interaction(self, frame, traceback):
         # Restore the previous signal handler at the Pdb+ prompt.
         if getattr(pdb.Pdb, "_previous_sigint_handler", None):
             try:
                 signal.signal(signal.SIGINT, pdb.Pdb._previous_sigint_handler)
@@ -1053,15 +1051,22 @@
     ):
         if self.sticky:
             return
         frame_index = frame_index if frame_index is not None else self.curindex
         frame, lineno = frame_lineno
         colored_index = Color.set(self.config.stack_color, frame_index)
         if frame is self.curframe:
-            print("[%s] >" % colored_index, file=self.stdout, end=" ")
+            indicator = " >"
+            color = self.config.regular_line_color
+            if self.has_traceback:
+                color = self.config.exc_line_color
+                if frame_index == len(self.stack) - 1:
+                    color = self.config.pm_cur_line_color
+            ind = setbgcolor(indicator, color)
+            print("[%s]%s" % (colored_index, ind), file=self.stdout, end=" ")
         else:
             print("[%s]  " % colored_index, file=self.stdout, end=" ")
         stack_entry = self.format_stack_entry(frame_lineno, prompt_prefix)
         print(stack_entry, file=self.stdout)
         if not self.sticky:
             print(file=self.stdout, end="\n\033[F")
             if (
```

