# Comparing `tmp/codeframe-0.2.3.tar.gz` & `tmp/codeframe-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.2.3.tar", last modified: Tue Apr 18 14:42:20 2023, max compression
+gzip compressed data, was "codeframe-0.2.5.tar", last modified: Wed Apr 19 10:45:36 2023, max compression
```

## Comparing `codeframe-0.2.3.tar` & `codeframe-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.187620 codeframe-0.2.3/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:42:20.183620 codeframe-0.2.3/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1916 2023-04-14 15:32:36.000000 codeframe-0.2.3/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    37453 2023-04-18 14:41:28.000000 codeframe-0.2.3/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2023-04-14 15:32:36.000000 codeframe-0.2.3/codeframe/prj_utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-18 14:42:19.000000 codeframe-0.2.3/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:42:20.183620 codeframe-0.2.3/codeframe.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-18 14:42:20.000000 codeframe-0.2.3/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-18 14:42:20.187620 codeframe-0.2.3/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2023-04-14 15:32:36.000000 codeframe-0.2.3/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 10:45:36.474887 codeframe-0.2.5/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-19 10:45:36.474887 codeframe-0.2.5/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1916 2023-04-14 15:32:36.000000 codeframe-0.2.5/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 10:45:36.474887 codeframe-0.2.5/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    38414 2023-04-19 10:45:11.000000 codeframe-0.2.5/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 10:45:36.474887 codeframe-0.2.5/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-04-14 15:32:36.000000 codeframe-0.2.5/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2023-04-14 15:32:36.000000 codeframe-0.2.5/codeframe/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2023-04-14 15:32:36.000000 codeframe-0.2.5/codeframe/prj_utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 10:45:36.474887 codeframe-0.2.5/codeframe.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-19 10:45:36.000000 codeframe-0.2.5/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-19 10:45:36.474887 codeframe-0.2.5/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2023-04-14 15:32:36.000000 codeframe-0.2.5/setup.py
```

### Comparing `codeframe-0.2.3/PKG-INFO` & `codeframe-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.2.3
+Version: 0.2.5
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `codeframe-0.2.3/README.md` & `codeframe-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.3/bin/codeframe` & `codeframe-0.2.5/bin/codeframe`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     print("             [OK]")
 
 
 
 
 
 def create_unit_keyb(proj):
-    result="""#!/usr/bin/env python3
+    result1="""#!/usr/bin/env python3
 
 # from {proj}.version import __version__
 from fire import Fire
 import threading
 import time
 from console import fg,bg,fx
 
@@ -285,14 +285,21 @@
     def __init__(self,  name='keyboard-input-thread', ending=None):
         '''
         Restart itself as thread
         '''
         self.block = False
         self.ending = ending
         self.cursor = 0
+"""
+
+
+
+    result2 = """
+        self.history = {} # dict with past commands
+        self.history_pointer = 0
         super(KeyboardThreadSsh, self).__init__(name=name)
         self.start()
 
 
     def text_split(self):
         '''
         operates on global_key and cursor, returns 3 parts
@@ -340,15 +347,15 @@
         #print("D...", f"'{key}' pressed")
         #print("D...", f"{global_key} , cu=={self.cursor} :", self.text_split() )
 
 
         # the tricks: space up down
         if key=="space":
             key=" "
-            self.cursor+=1
+            #self.cursor+=1 # not here ...
         elif key=="delete":
             if self.cursor<=len(global_key):
                 global_key =  global_key[:self.cursor]+global_key[self.cursor+1:]
             key=""
         elif key=="backspace":
             global_key =  global_key[:self.cursor-1]+global_key[self.cursor:]
             self.cursor-=1
@@ -363,19 +370,36 @@
             self.cursor-=1
             key=""
         elif key=="right":
             self.cursor+=1
             key=""
         elif key=="enter":
             key="\\n"
-            self.cursor=len(global_key)
+            self.cursor=len(global_key) # there is a reason
+            n = len(self.history)
+            self.history[n] = global_key
+            self.history_pointer = n+1
+            print(self.history, self.history_pointer)
         elif key=="up":
             key=""
+            if self.history_pointer>0:
+                self.history_pointer-=1
+                global_key = self.history[self.history_pointer]
+                self.cursor=len(global_key)
         elif key=="down":
             key=""
+            if self.history_pointer<len(self.history)-1:
+                self.history_pointer+=1
+                global_key = self.history[self.history_pointer]
+                self.cursor=len(global_key)
+            elif self.history_pointer==len(self.history)-1:
+                #print("D... EDGE")
+                self.history_pointer+=1 # empty
+                global_key = ""
+                self.cursor=0
         elif key=="tab":
             key=""
         #else:
         #    self.cursor+=1
 
         # print("D...  ..........",self.cursor, "after press /    limit",len(global_key)+1)
 
@@ -452,15 +476,17 @@
 """
 
     unit = "key_enter"
     print(f"i...    creating  {unit}", end="")
     NAME = f"{unit}.py"
     UNIT1 = proj + "/" + NAME
     with open(UNIT1, "w") as f:
-        f.write(result)
+        f.write(result1)
+        f.write("\n")
+        f.write(result2)
     os.chmod(UNIT1, 0o775)
     with cd(proj):
         with cd(proj):
             os.symlink("../"+NAME, NAME)
     # --- link to test_unit.py
     with cd(proj):
         os.symlink(NAME, "test_"+NAME)
```

### Comparing `codeframe-0.2.3/codeframe/config.py` & `codeframe-0.2.5/codeframe/config.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.3/codeframe/prj_utils.py` & `codeframe-0.2.5/codeframe/prj_utils.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.2.3/codeframe.egg-info/PKG-INFO` & `codeframe-0.2.5/codeframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.2.3
+Version: 0.2.5
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
```

### Comparing `codeframe-0.2.3/setup.py` & `codeframe-0.2.5/setup.py`

 * *Files identical despite different names*

