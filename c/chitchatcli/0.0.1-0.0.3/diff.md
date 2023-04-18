# Comparing `tmp/chitchatcli-0.0.1.tar.gz` & `tmp/chitchatcli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chitchatcli-0.0.1.tar", last modified: Tue Apr 18 21:24:42 2023, max compression
+gzip compressed data, was "chitchatcli-0.0.3.tar", last modified: Tue Apr 18 22:58:54 2023, max compression
```

## Comparing `chitchatcli-0.0.1.tar` & `chitchatcli-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:24:42.373365 chitchatcli-0.0.1/
--rw-r--r--   0 ben        (501) staff       (20)     1064 2023-04-18 20:24:23.000000 chitchatcli-0.0.1/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:24:42.372569 chitchatcli-0.0.1/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1501 2023-04-18 20:58:00.000000 chitchatcli-0.0.1/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:24:42.350186 chitchatcli-0.0.1/chitchatcli/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 21:15:52.000000 chitchatcli-0.0.1/chitchatcli/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6639 2023-04-18 21:16:48.000000 chitchatcli-0.0.1/chitchatcli/__main__.py
--rw-r--r--   0 ben        (501) staff       (20)      836 2023-04-18 21:14:56.000000 chitchatcli-0.0.1/chitchatcli/globalvaribles.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:24:42.371444 chitchatcli-0.0.1/chitchatcli/utilis/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 20:59:05.000000 chitchatcli-0.0.1/chitchatcli/utilis/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     7824 2023-04-18 21:19:33.000000 chitchatcli-0.0.1/chitchatcli/utilis/apicalls.py
--rw-r--r--   0 ben        (501) staff       (20)     1017 2023-04-18 21:16:48.000000 chitchatcli-0.0.1/chitchatcli/utilis/event.py
--rw-r--r--   0 ben        (501) staff       (20)     3457 2023-04-18 21:16:48.000000 chitchatcli-0.0.1/chitchatcli/utilis/helper_functions.py
--rw-r--r--   0 ben        (501) staff       (20)     2786 2023-04-18 21:16:48.000000 chitchatcli-0.0.1/chitchatcli/utilis/process.py
--rw-r--r--   0 ben        (501) staff       (20)    18393 2023-04-18 21:16:48.000000 chitchatcli-0.0.1/chitchatcli/utilis/screen_functions.py
--rw-r--r--   0 ben        (501) staff       (20)     1068 2023-04-18 18:42:12.000000 chitchatcli-0.0.1/chitchatcli/utilis/storage.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 21:24:42.356010 chitchatcli-0.0.1/chitchatcli.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 21:24:42.000000 chitchatcli-0.0.1/chitchatcli.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      510 2023-04-18 21:24:42.000000 chitchatcli-0.0.1/chitchatcli.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-18 21:24:42.000000 chitchatcli-0.0.1/chitchatcli.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       74 2023-04-18 21:24:42.000000 chitchatcli-0.0.1/chitchatcli.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-04-18 21:24:42.000000 chitchatcli-0.0.1/chitchatcli.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-04-18 21:24:42.373529 chitchatcli-0.0.1/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      888 2023-04-18 21:22:37.000000 chitchatcli-0.0.1/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 22:58:54.220447 chitchatcli-0.0.3/
+-rw-r--r--   0 ben        (501) staff       (20)     1064 2023-04-18 20:24:23.000000 chitchatcli-0.0.3/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 22:58:54.219779 chitchatcli-0.0.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1501 2023-04-18 20:58:00.000000 chitchatcli-0.0.3/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 22:58:54.191519 chitchatcli-0.0.3/chitchatcli/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 21:15:52.000000 chitchatcli-0.0.3/chitchatcli/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6623 2023-04-18 22:15:49.000000 chitchatcli-0.0.3/chitchatcli/__main__.py
+-rw-r--r--   0 ben        (501) staff       (20)      836 2023-04-18 21:14:56.000000 chitchatcli-0.0.3/chitchatcli/globalvaribles.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 22:58:54.217513 chitchatcli-0.0.3/chitchatcli/utilis/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-18 20:59:05.000000 chitchatcli-0.0.3/chitchatcli/utilis/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     7824 2023-04-18 21:19:33.000000 chitchatcli-0.0.3/chitchatcli/utilis/apicalls.py
+-rw-r--r--   0 ben        (501) staff       (20)      910 2023-04-18 22:34:45.000000 chitchatcli-0.0.3/chitchatcli/utilis/event.py
+-rw-r--r--   0 ben        (501) staff       (20)     3457 2023-04-18 22:46:46.000000 chitchatcli-0.0.3/chitchatcli/utilis/helper_functions.py
+-rw-r--r--   0 ben        (501) staff       (20)     2906 2023-04-18 22:48:05.000000 chitchatcli-0.0.3/chitchatcli/utilis/process.py
+-rw-r--r--   0 ben        (501) staff       (20)    18393 2023-04-18 21:16:48.000000 chitchatcli-0.0.3/chitchatcli/utilis/screen_functions.py
+-rw-r--r--   0 ben        (501) staff       (20)     1068 2023-04-18 18:42:12.000000 chitchatcli-0.0.3/chitchatcli/utilis/storage.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-18 22:58:54.199640 chitchatcli-0.0.3/chitchatcli.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     1935 2023-04-18 22:58:54.000000 chitchatcli-0.0.3/chitchatcli.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      510 2023-04-18 22:58:54.000000 chitchatcli-0.0.3/chitchatcli.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-18 22:58:54.000000 chitchatcli-0.0.3/chitchatcli.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       74 2023-04-18 22:58:54.000000 chitchatcli-0.0.3/chitchatcli.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-04-18 22:58:54.000000 chitchatcli-0.0.3/chitchatcli.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-04-18 22:58:54.221157 chitchatcli-0.0.3/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      888 2023-04-18 22:58:41.000000 chitchatcli-0.0.3/setup.py
```

### Comparing `chitchatcli-0.0.1/LICENSE.txt` & `chitchatcli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/PKG-INFO` & `chitchatcli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitchatcli
-Version: 0.0.1
+Version: 0.0.3
 Summary: A command line chatting software designed for developers to communicate with each other.
 Author: Benjamin Eruvieru
 Author-email: benjamineruvieru@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `chitchatcli-0.0.1/README.md` & `chitchatcli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli/__main__.py` & `chitchatcli-0.0.3/chitchatcli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import curses
 from curses import wrapper
 from chitchatcli.utilis.process import process_commands
 from chitchatcli.globalvaribles import globalstate
-from chitchatcli.utilis.helper_functions import homepage, log, showError
+from chitchatcli.utilis.helper_functions import homepage
 
 
 def main(stdscr):
     stdscr = curses.initscr()
     stdscr.clear()
     height, width = stdscr.getmaxyx()
     curses.curs_set(2)
```

### Comparing `chitchatcli-0.0.1/chitchatcli/globalvaribles.py` & `chitchatcli-0.0.3/chitchatcli/globalvaribles.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/apicalls.py` & `chitchatcli-0.0.3/chitchatcli/utilis/apicalls.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/event.py` & `chitchatcli-0.0.3/chitchatcli/utilis/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 #!/usr/bin/python3
 
 """This module defines all the socket functions"""
 
 import socketio
 from chitchatcli.globalvaribles import globalstate
-from chitchatcli.utilis.helper_functions import renderMessage, showError
+from chitchatcli.utilis.helper_functions import renderMessage
 from datetime import datetime
 
 sio = socketio.Client()
 
 
 @sio.event
-def connect():
-    pass
-
-
-@sio.event
-def disconnect():
-    showError('Disconnected from server', message_win=globalstate.message_win)
-
-
-@sio.event
 def message(data):
     renderMessage(message_win=globalstate.message_win, message=data)
 
 
 def connectToSocket():
     sio.connect(globalstate.BASEURL, headers={'X-Token': globalstate.TOKEN})
 
 
+def disconnectFromSocket():
+    sio.disconnect()
+
+
 def sendMessage(message_win, message):
     msgdata = {"createdAt": int(datetime.now().timestamp() * 1000),
                "senderusername": globalstate.USERNAME,
                "message": message
                }
     renderMessage(message_win, message=msgdata)
     sio.emit('message', {"message": message,
```

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/helper_functions.py` & `chitchatcli-0.0.3/chitchatcli/utilis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/process.py` & `chitchatcli-0.0.3/chitchatcli/utilis/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from chitchatcli.utilis import screen_functions
 from chitchatcli.globalvaribles import globalstate
 from chitchatcli.utilis.helper_functions import homepage, showError
 from chitchatcli.utilis.event import sendMessage
 from chitchatcli.utilis.apicalls import logout
+from chitchatcli.utilis.event import disconnectFromSocket
 
 
 def process_commands(text, message_win, input_win):
     if text.lower().strip() == 'help':
         screen_functions.runhelp(message_win)
     elif text.lower().strip() == 'quit':
+        disconnectFromSocket()
         globalstate.RUNNING = False
         return
     elif text == 'back':
+        disconnectFromSocket()
         homepage(message_win)
     elif len(text) <= 0:
         return
     elif globalstate.STATUS == 'confirmotp':
         screen_functions.confirmOtp(message_win, text)
     elif globalstate.STATUS == 'command':
         text = text.lower().strip()
```

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/screen_functions.py` & `chitchatcli-0.0.3/chitchatcli/utilis/screen_functions.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli/utilis/storage.py` & `chitchatcli-0.0.3/chitchatcli/utilis/storage.py`

 * *Files identical despite different names*

### Comparing `chitchatcli-0.0.1/chitchatcli.egg-info/PKG-INFO` & `chitchatcli-0.0.3/chitchatcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitchatcli
-Version: 0.0.1
+Version: 0.0.3
 Summary: A command line chatting software designed for developers to communicate with each other.
 Author: Benjamin Eruvieru
 Author-email: benjamineruvieru@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `chitchatcli-0.0.1/setup.py` & `chitchatcli-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name="chitchatcli",
-    version="0.0.1",
+    version="0.0.3",
     author="Benjamin Eruvieru",
     author_email="benjamineruvieru@gmail.com",
     description="A command line chatting software designed for developers to communicate with each other.",
     packages=find_packages(),
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=["python-socketio[client]",
```

