# Comparing `tmp/fkeycapture-1.2.1.tar.gz` & `tmp/fkeycapture-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fkeycapture-1.2.1.tar", last modified: Wed Apr 19 01:55:28 2023, max compression
+gzip compressed data, was "fkeycapture-1.2.2.tar", last modified: Wed Apr 19 15:37:16 2023, max compression
```

## Comparing `fkeycapture-1.2.1.tar` & `fkeycapture-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:55:28.390071 fkeycapture-1.2.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1574 2023-04-19 01:55:28.390071 fkeycapture-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      674 2023-04-19 01:55:07.000000 fkeycapture-1.2.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      832 2023-04-19 01:55:28.390071 fkeycapture-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:55:28.386071 fkeycapture-1.2.1/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:55:28.390071 fkeycapture-1.2.1/src/fkeycapture/
--rw-r--r--   0 runner    (1000) runner    (1000)     3409 2023-04-19 01:41:31.000000 fkeycapture-1.2.1/src/fkeycapture/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 01:55:28.390071 fkeycapture-1.2.1/src/fkeycapture.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1574 2023-04-19 01:55:28.000000 fkeycapture-1.2.1/src/fkeycapture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 01:55:28.000000 fkeycapture-1.2.1/src/fkeycapture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 01:55:28.000000 fkeycapture-1.2.1/src/fkeycapture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 01:55:28.000000 fkeycapture-1.2.1/src/fkeycapture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 fkeycapture-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2607 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1496 2023-04-19 15:32:07.000000 fkeycapture-1.2.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2021-11-16 19:33:09.000000 fkeycapture-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      827 2023-04-19 15:37:16.317670 fkeycapture-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.301670 fkeycapture-1.2.2/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.305670 fkeycapture-1.2.2/src/fkeycapture/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3538 2023-04-19 15:04:10.000000 fkeycapture-1.2.2/src/fkeycapture/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 15:37:16.313670 fkeycapture-1.2.2/src/fkeycapture.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2607 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      226 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-19 15:37:16.000000 fkeycapture-1.2.2/src/fkeycapture.egg-info/top_level.txt
```

### Comparing `fkeycapture-1.2.1/LICENSE` & `fkeycapture-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fkeycapture-1.2.1/PKG-INFO` & `fkeycapture-1.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,62 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.1
+Version: 1.2.2
 Summary: A way to capture keystrokes
 Home-page: https://github.com/Alexander-Maples/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
-Project-URL: replit, https://replit.com/@ALEXANDERMAPLES/fkeycapture
+Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
         2. Recive key as bytes (get only)
         3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
-        2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])
-        3. Use getnum like this: getnum([number of numbers to capture], [if you want int output, make this `True`])
+        2. Use get like this: `get(keycount = any int, bytes = True or False)`
+        3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
+        4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
+        #### Change log:
+        ###### v.1.2.2:
+        Internal improvements, Changelog improved
         ###### v.1.2.1:
+        Changelog issue fixed, removed the help command from 1.0.10
+        ###### v.1.2.0
         Type hinting, docstrings, and int support for getnum!
-        
-        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ Help discontinued.
-        
+        ###### v.1.0.10
+        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
+        ###### v.1.0.9
+        Fixed README issues in 1.0.8
+        ###### v.1.0.8
+        Added getchars method
+        ###### v.1.0.7
+        Added the getnum method
+        ###### v.1.0.6
+        Finally made the package usable.
+        ###### v.1.0.5
+        Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
+        ###### v.1.0.4
+        Repaired an issue in 1.0.3 which caused the module to be unusable.
+        ###### v.1.0.3
+        Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
+        ###### v.1.0.2 (Missing)
+        Unknown
+        ###### v.1.0.1
+        Corrected incorrect text in certain files
+        ###### v.0.0.6 (v.1.0.0 on PyPI)
+        Removed unnecessary code
+        ###### v.0.0.5
+        Replit support?
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `fkeycapture-1.2.1/setup.cfg` & `fkeycapture-1.2.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [metadata]
 name = fkeycapture
-version = 1.2.1
+version = 1.2.2
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = A way to capture keystrokes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Alexander-Maples/fkeycapture
 project_urls = 
 	Bug Tracker = https://github.com/Alexander-Maples/fkeycapture/issues
-	replit = https://replit.com/@ALEXANDERMAPLES/fkeycapture
+	replit = https://replit.com/@Firepup650/fkeycapture
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Natural Language :: English
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fkeycapture-1.2.1/src/fkeycapture/__init__.py` & `fkeycapture-1.2.2/src/fkeycapture/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Firepup650's fkeycapture module"""
 import termios, fcntl, sys
 global fd,flags_save,attrs_save
 fd = sys.stdin.fileno()
 flags_save = fcntl.fcntl(fd, fcntl.F_GETFL)
 attrs_save = termios.tcgetattr(fd)
 def __getp1():
-    """Internal Method"""
+    """Internal Method - Modify terminal settings"""
     import termios, fcntl, sys, os
     fd = sys.stdin.fileno()
     # save old state
     flags_save = fcntl.fcntl(fd, fcntl.F_GETFL)
     attrs_save = termios.tcgetattr(fd)
     # make raw - the way to do this comes from the termios(3) man page.
     attrs = list(attrs_save) # copy the stored version to update
@@ -25,15 +25,15 @@
     # lflag
     attrs[3] &= ~(termios.ECHONL | termios.ECHO | termios.ICANON
                   | termios.ISIG | termios.IEXTEN)
     termios.tcsetattr(fd, termios.TCSANOW, attrs)
     # turn off non-blocking
     fcntl.fcntl(fd, fcntl.F_SETFL, flags_save & ~os.O_NONBLOCK)
 def __getp2():
-    """Internal Method"""
+    """Internal Method - Reset terminal settings"""
     termios.tcsetattr(fd, termios.TCSAFLUSH, attrs_save)
     fcntl.fcntl(fd, fcntl.F_SETFL, flags_save)
 def get(keycount: int = 1, bytes: bool = False) -> str or bytes:
   """# Function: get
 
 # Inputs:
   keycount: int - Number of keys, defualts to 1
@@ -43,17 +43,18 @@
   str or bytes
 
 # Raises:
   None"""
   __getp1()
   key = sys.stdin.read(keycount)
   __getp2()
-  if bytes == True:
-    key = key.encode()
-  return key
+  if bytes:
+    return key.encode()
+  else:
+    return key
 def getnum(keycount: int = 1, ints: bool = False) -> str or int:
   """# Function: getnum
 
 # Inputs:
   keycount: int - Number of keys, defualts to 1
   ints: bool    - Wether to return the keys as ints, defaults to False
 
@@ -62,28 +63,29 @@
 
 # Raises:
   None"""
   internalcounter=0
   keys = []
   while internalcounter != keycount:
     key = get()
-    if key == "0" or key == "1" or key == "2" or key == "3" or key == "4" or key == "5" or key == "6" or key == "7" or key == "8" or key == "9":
+    if key in ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]:
       keys.append(key)
       internalcounter += 1
   key = "".join(keys)
   if not ints:
     return key
   else:
     return int(key)
-def getchars(keycount: int = 1, chars: list = ["1", "2"]) -> str:
+def getchars(keycount: int = 1, chars: list = ["1", "2"], bytes: bool = False) -> str:
   """# Function: getchars
 
 # Inputs:
   keycount: int - Number of keys, defualts to 1
   chars: list   - List of allowed keys, defaults to ["1", "2"]
+  bytes: bool   - Wether or not to return the key(s) as bytes, defaults to False
 
 # Returns:
   str
 
 # Raises:
   None"""
   internalcounter=0
@@ -91,15 +93,18 @@
   while internalcounter != keycount:
     key = get()
     for char in chars:
       if key == char:
         keys.append(key)
         internalcounter += 1
   key = "".join(keys)
-  return key
+  if not bytes:
+    return key
+  else:
+    return key.encode()
 # def help():
 #   """# Function: help
 
 # # Inputs:
 #   None
 
 # # Returns:
```

### Comparing `fkeycapture-1.2.1/src/fkeycapture.egg-info/PKG-INFO` & `fkeycapture-1.2.2/src/fkeycapture.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,62 @@
 Metadata-Version: 2.1
 Name: fkeycapture
-Version: 1.2.1
+Version: 1.2.2
 Summary: A way to capture keystrokes
 Home-page: https://github.com/Alexander-Maples/fkeycapture
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Alexander-Maples/fkeycapture/issues
-Project-URL: replit, https://replit.com/@ALEXANDERMAPLES/fkeycapture
+Project-URL: replit, https://replit.com/@Firepup650/fkeycapture
 Description: # fkeycapture
         This is a simple and easy to use package that allows you to capture individual keystrokes from the user.
         #### Forms:
         1. (Default) Recive key as a string
         2. Recive key as bytes (get only)
         3. Recive key as ints  (getnum only)
         #### How to Use:
         1. from fkeycapture import get, getnum, getchars
-        2. Use get like this: get([number of keys to capture],[if you want bytes output, make this 'True'])
-        3. Use getnum like this: getnum([number of numbers to capture], [if you want int output, make this `True`])
+        2. Use get like this: `get(keycount = any int, bytes = True or False)`
+        3. Use getnum like this: `getnum(keycount = any int, ints = True or False)`
+        4. Use getchars like this: `getchars(keycount = any int, chars = list of chars, bytes = True or False)`
+        #### Change log:
+        ###### v.1.2.2:
+        Internal improvements, Changelog improved
         ###### v.1.2.1:
+        Changelog issue fixed, removed the help command from 1.0.10
+        ###### v.1.2.0
         Type hinting, docstrings, and int support for getnum!
-        
-        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ Help discontinued.
-        
+        ###### v.1.0.10
+        ~~Now includes a help command! Use fkeycapture.help() to recive help.~~ See v.1.2.1
+        ###### v.1.0.9
+        Fixed README issues in 1.0.8
+        ###### v.1.0.8
+        Added getchars method
+        ###### v.1.0.7
+        Added the getnum method
+        ###### v.1.0.6
+        Finally made the package usable.
+        ###### v.1.0.5
+        Repaired an issue in 1.0.4 which caused the module to cause a recusion error.
+        ###### v.1.0.4
+        Repaired an issue in 1.0.3 which caused the module to be unusable.
+        ###### v.1.0.3
+        Repaired an issue in 1.0.0, 1.0.1, and 1.0.2 which caused the module to be unusable.
+        ###### v.1.0.2 (Missing)
+        Unknown
+        ###### v.1.0.1
+        Corrected incorrect text in certain files
+        ###### v.0.0.6 (v.1.0.0 on PyPI)
+        Removed unnecessary code
+        ###### v.0.0.5
+        Replit support?
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

