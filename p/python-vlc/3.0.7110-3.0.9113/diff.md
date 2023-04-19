# Comparing `tmp/python-vlc-3.0.7110.tar.gz` & `tmp/python-vlc-3.0.9113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-vlc-3.0.7110.tar", last modified: Sat Aug  3 18:19:10 2019, max compression
+gzip compressed data, was "dist/python-vlc-3.0.9113.tar", last modified: Wed Apr 29 11:16:27 2020, max compression
```

## Comparing `python-vlc-3.0.7110.tar` & `python-vlc-3.0.9113.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)    26530 2019-08-03 18:18:29.000000 python-vlc-3.0.7110/COPYING
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)      131 2019-08-03 18:18:29.000000 python-vlc-3.0.7110/MANIFEST.in
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1419 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/PKG-INFO
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     2312 2019-08-03 18:18:29.000000 python-vlc-3.0.7110/README.module
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)    17484 2019-08-03 18:18:29.000000 python-vlc-3.0.7110/distribute_setup.py
-drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/examples/
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    21844 2019-02-24 15:16:27.000000 python-vlc-3.0.7110/examples/cocoavlc.py
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     5337 2015-03-07 17:40:51.000000 python-vlc-3.0.7110/examples/gtk2vlc.py
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     6052 2017-04-10 10:16:43.000000 python-vlc-3.0.7110/examples/gtkvlc.py
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     7016 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/pyqt5vlc.py
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     7466 2018-07-13 08:56:14.000000 python-vlc-3.0.7110/examples/qtvlc.py
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    21299 2019-08-03 17:03:50.000000 python-vlc-3.0.7110/examples/tkvlc.py
-drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/examples/video_sync/
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1365 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/video_sync/README.md
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)   118904 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/video_sync/figure.png
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)    14704 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/video_sync/main.py
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     5448 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/video_sync/mini_player.py
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     5489 2019-01-30 22:28:49.000000 python-vlc-3.0.7110/examples/video_sync/network.py
--rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    11187 2019-08-03 17:08:16.000000 python-vlc-3.0.7110/examples/wxvlc.py
-drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/python_vlc.egg-info/
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1419 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/python_vlc.egg-info/PKG-INFO
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)      495 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/python_vlc.egg-info/SOURCES.txt
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)        1 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/python_vlc.egg-info/dependency_links.txt
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)        4 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/python_vlc.egg-info/top_level.txt
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)       38 2019-08-03 18:19:10.000000 python-vlc-3.0.7110/setup.cfg
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1597 2019-08-03 18:18:29.000000 python-vlc-3.0.7110/setup.py
--rw-r--r--   0 oaubert   (1002) oaubert   (1002)   367971 2019-08-03 18:13:06.000000 python-vlc-3.0.7110/vlc.py
+drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)    26530 2020-04-29 11:14:12.000000 python-vlc-3.0.9113/COPYING
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)      131 2020-04-29 11:14:12.000000 python-vlc-3.0.9113/MANIFEST.in
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1419 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/PKG-INFO
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     2312 2020-04-29 11:14:12.000000 python-vlc-3.0.9113/README.module
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)    17484 2020-04-29 11:14:12.000000 python-vlc-3.0.9113/distribute_setup.py
+drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/examples/
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    21844 2019-10-31 23:25:50.000000 python-vlc-3.0.9113/examples/cocoavlc.py
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     4232 2020-03-03 15:36:14.000000 python-vlc-3.0.9113/examples/glsurface.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     3717 2020-03-03 15:30:47.000000 python-vlc-3.0.9113/examples/glsurface.py~
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     5337 2015-03-07 17:40:51.000000 python-vlc-3.0.9113/examples/gtk2vlc.py
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     7062 2019-10-31 23:21:02.000000 python-vlc-3.0.9113/examples/gtkvlc.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)    15821 2019-10-27 19:13:08.000000 python-vlc-3.0.9113/examples/pyobjcvlc.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     7810 2020-04-29 11:11:50.000000 python-vlc-3.0.9113/examples/pyqt5vlc.py
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)     7466 2018-07-13 08:56:14.000000 python-vlc-3.0.9113/examples/qtvlc.py
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    21299 2019-08-03 17:03:50.000000 python-vlc-3.0.9113/examples/tkvlc.py
+drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/examples/video_sync/
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1353 2020-04-29 11:11:50.000000 python-vlc-3.0.9113/examples/video_sync/README.md
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)    28647 2020-04-29 11:11:50.000000 python-vlc-3.0.9113/examples/video_sync/figure.png
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)    14704 2019-01-30 22:28:49.000000 python-vlc-3.0.9113/examples/video_sync/main.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     5448 2019-01-30 22:28:49.000000 python-vlc-3.0.9113/examples/video_sync/mini_player.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     6128 2020-04-29 11:11:50.000000 python-vlc-3.0.9113/examples/video_sync/network.py
+-rwxr-xr-x   0 oaubert   (1002) oaubert   (1002)    11187 2019-08-03 17:08:16.000000 python-vlc-3.0.9113/examples/wxvlc.py
+drwxr-xr-x   0 oaubert   (1002) oaubert   (1002)        0 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/python_vlc.egg-info/
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1419 2020-04-29 11:16:27.000000 python-vlc-3.0.9113/python_vlc.egg-info/PKG-INFO
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)      562 2020-04-29 11:16:27.000000 python-vlc-3.0.9113/python_vlc.egg-info/SOURCES.txt
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)        1 2020-04-29 11:16:27.000000 python-vlc-3.0.9113/python_vlc.egg-info/dependency_links.txt
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)        4 2020-04-29 11:16:27.000000 python-vlc-3.0.9113/python_vlc.egg-info/top_level.txt
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)       38 2020-04-29 11:16:27.890426 python-vlc-3.0.9113/setup.cfg
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)     1597 2020-04-29 11:14:12.000000 python-vlc-3.0.9113/setup.py
+-rw-r--r--   0 oaubert   (1002) oaubert   (1002)   369392 2020-04-29 11:13:52.000000 python-vlc-3.0.9113/vlc.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-vlc-3.0.7110/COPYING` & `python-vlc-3.0.9113/COPYING`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/PKG-INFO` & `python-vlc-3.0.9113/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.2
 Name: python-vlc
-Version: 3.0.7110
+Version: 3.0.9113
 Summary: VLC bindings for python.
 Home-page: http://wiki.videolan.org/PythonBinding
 Author: Olivier Aubert
 Author-email: contact@olivieraubert.net
 Maintainer: Olivier Aubert
 Maintainer-email: contact@olivieraubert.net
 License: LGPL-2.1+
 Description: This module provides ctypes-based bindings (see
               http://wiki.videolan.org/PythonBinding) for the native libvlc
               API (see http://wiki.videolan.org/LibVLC) of the VLC video
               player. Note that it relies on an already present install of VLC.
         
               It has been automatically generated from the include files of
-              vlc 3.0.7, using generator 1.10.
+              vlc 3.0.9, using generator 1.13.
               
 Keywords: vlc,video
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `python-vlc-3.0.7110/README.module` & `python-vlc-3.0.9113/README.module`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/distribute_setup.py` & `python-vlc-3.0.9113/distribute_setup.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/cocoavlc.py` & `python-vlc-3.0.9113/examples/cocoavlc.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,22 +63,22 @@
 from time import strftime, strptime
 try:
     from urllib import unquote as mrl_unquote  # Python 2
 except ImportError:
     from urllib.parse import unquote as mrl_unquote  # Python 3+
 
 __all__  = ('AppVLC',)
-__version__ = '19.01.31'
+__version__ = '19.08.26'
 
 _Adjust  = vlc.VideoAdjustOption  # Enum
 # <http://Wiki.VideoLan.org/Documentation:Modules/adjust>
 _Adjust3 = {_Adjust.Brightness: (0, 1, 2),
             _Adjust.Contrast:   (0, 1, 2),
             _Adjust.Gamma:   (0.01, 1, 10),
-            _Adjust.Hue:        (0, 0, 360),
+            _Adjust.Hue:     (-180, 0, 180),
             _Adjust.Saturation: (0, 1, 3)}
 _Argv0   = os.path.splitext(os.path.basename(__file__))[0]
 _macOS   = platform.mac_ver()[0:3:2]  # PYCHOK false
 _Movies  = '.m4v', '.mov', '.mp4'  # lower-case file types for movies, videos
 _Python  = sys.version.split()[0], platform.architecture()[0]  # PYCHOK false
 _Select  = 'Select a video file from the panel'
 _VLC_3_  = vlc.__version__.split('.')[0] > '2' and \
```

### Comparing `python-vlc-3.0.7110/examples/gtk2vlc.py` & `python-vlc-3.0.9113/examples/gtk2vlc.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/gtkvlc.py` & `python-vlc-3.0.9113/examples/gtkvlc.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,39 +36,59 @@
 gi.require_version('Gtk', '3.0')
 from gi.repository import Gdk
 from gi.repository import Gtk
 
 Gdk.threads_init ()
 
 import sys
+import ctypes
 import vlc
 
 from gettext import gettext as _
 
 # Create a single vlc.Instance() to be shared by (possible) multiple players.
 if 'linux' in sys.platform:
     # Inform libvlc that Xlib is not initialized for threads
     instance = vlc.Instance("--no-xlib")
 else:
     instance = vlc.Instance()
 
+
+def get_window_pointer(window):
+    """ Use the window.__gpointer__ PyCapsule to get the C void* pointer to the window
+    """
+    # get the c gpointer of the gdk window
+    ctypes.pythonapi.PyCapsule_GetPointer.restype = ctypes.c_void_p
+    ctypes.pythonapi.PyCapsule_GetPointer.argtypes = [ctypes.py_object]
+    return ctypes.pythonapi.PyCapsule_GetPointer(window.__gpointer__, None)
+
+
 class VLCWidget(Gtk.DrawingArea):
     """Simple VLC widget.
 
     Its player can be controlled through the 'player' attribute, which
     is a vlc.MediaPlayer() instance.
     """
     __gtype_name__ = 'VLCWidget'
 
     def __init__(self, *p):
         Gtk.DrawingArea.__init__(self)
         self.player = instance.media_player_new()
         def handle_embed(*args):
             if sys.platform == 'win32':
-                self.player.set_hwnd(self.get_window().get_handle())
+                # get the win32 handle
+                gdkdll = ctypes.CDLL('libgdk-3-0.dll')
+                handle = gdkdll.gdk_win32_window_get_handle(get_window_pointer(self.get_window()))
+                self.player.set_hwnd(handle)
+            elif sys.platform == 'darwin':
+                # get the nsview pointer. NB need to manually specify function signature
+                gdkdll = ctypes.CDLL('libgdk-3.0.dll')
+                get_nsview = gdkdll.gdk_quaerz_window_get_nsview
+                get_nsview.restype, get_nsview.argtypes = [ctypes.c_void_p],  ctypes.c_void_p
+                self.player.set_nsobject(get_nsview(get_window_pointer(self.get_window())))
             else:
                 self.player.set_xwindow(self.get_window().get_xid())
             return True
         self.connect("realize", handle_embed)
         self.set_size_request(320, 200)
 
 class DecoratedVLCWidget(Gtk.VBox):
```

### Comparing `python-vlc-3.0.7110/examples/pyqt5vlc.py` & `python-vlc-3.0.9113/examples/pyqt5vlc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+#
+# PyQt5 example for VLC Python bindings
+# Copyright (C) 2009-2010 the VideoLAN team
+#
+# This program is free software; you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation; either version 2 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston MA 02110-1301, USA.
+#
 """
 A simple example for VLC python bindings using PyQt5.
 
 Author: Saveliy Yusufov, Columbia University, sy2685@columbia.edu
 Date: 25 December 2018
 """
```

### Comparing `python-vlc-3.0.7110/examples/qtvlc.py` & `python-vlc-3.0.9113/examples/qtvlc.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/tkvlc.py` & `python-vlc-3.0.9113/examples/tkvlc.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/video_sync/README.md` & `python-vlc-3.0.9113/examples/video_sync/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## Video Synchronization with python-vlc
 
-<img src="figure.png" width="500" align="right">
+<img src="figure.png" width="600" align="center">
 
 Each video player is launched as a separate process. `main.py` is the entry point into the program. It creates the "main" video player with all of its respective controls. The main video player is started alongside a multithreaded server that "broadcasts" signals (e.g. play, pause, stop, and etc.) and the current time of the video player, to all client/slave videos. Specifically, this is accomplished by putting the current time or the signal of the main video player into a `queue` (FIFO). The multithreaded server gets the value from the queue and sends the value to each connected client.
 
 In a somewhat similar fashion, each "slave" video player is launched as a separate process, along with a client. The client has a `data_receiver` thread that continuously listens for data, receives data, parses the data, and puts the data into a `queue` that is specific to that "slave" video player. The "slave" video player gets the value from the queue and updates itself in accordance with that value.
 
 In order to facilitate interprocess communication, UNIX domain sockets are used to send and receive data. For the time being, Windows users have to use TCP/IP sockets.
 
-Note: for the sake of clarity, the figure on the right only shows the case of 3 client/slave videos.
+Note: for the sake of clarity, the figure only shows the case of 3 client/slave videos.
```

### Comparing `python-vlc-3.0.7110/examples/video_sync/main.py` & `python-vlc-3.0.9113/examples/video_sync/main.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/video_sync/mini_player.py` & `python-vlc-3.0.9113/examples/video_sync/mini_player.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/examples/video_sync/network.py` & `python-vlc-3.0.9113/examples/video_sync/network.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 Author: Saveliy Yusufov, Columbia University, sy2685@columbia.edu
 Date: 25 January 2019
 """
 
 import os
 import platform
 import socket
-import threading
 import sys
+import struct
+import threading
 import logging
 from concurrent import futures
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 logger.setLevel(logging.DEBUG)
@@ -100,19 +101,21 @@
         while True:
             client, _ = self.sock.accept()
             logger.info("Accepted Connection from: %s", client)
             self.clients.add(client)
 
     def data_sender(self):
         while True:
-            data = "{},".format(self.data_queue.get())
+            data = self.data_queue.get()
+            data = str(data).encode()
+            msg = struct.pack(">I", len(data)) + data
 
             with futures.ThreadPoolExecutor(max_workers=5) as ex:
                 for client in self.clients:
-                    ex.submit(self.sendall, client, data.encode())
+                    ex.submit(self.sendall, client, msg)
 
     def sendall(self, client, data):
         """Wraps socket module's `sendall` function"""
         try:
             client.sendall(data)
         except socket.error:
             logger.exception("Connection to client: %s was broken!", client)
@@ -149,27 +152,47 @@
                 logger.exception()
                 sys.exit(1)
 
         thread = threading.Thread(target=self.data_receiver, args=())
         thread.daemon = True
         thread.start()
 
+    def recv_all(self, size):
+        """Helper function to recv `size` number of bytes, or return False"""
+        data = bytearray()
+
+        while (len(data) < size):
+            packet = self.sock.recv(size - len(data))
+            if not packet:
+                return False
+
+            data.extend(packet)
+
+        return data
+
+    def recv_msg(self):
+        """Receive the message size, n, and receive n bytes into a buffer"""
+        raw_msg_size = self.recv_all(4)
+        if not raw_msg_size:
+            return False
+
+        msg_size = struct.unpack(">I", raw_msg_size)[0]
+        return self.recv_all(msg_size)
+
     def data_receiver(self):
         """Handles receiving, parsing, and queueing data"""
         logger.info("New data receiver thread started.")
 
         try:
             while True:
-                data = self.sock.recv(4096)
-                if data:
-                    data = data.decode()
-
-                    for char in data.split(','):
-                        if char:
-                            if char == 'd':
-                                self.data_queue.queue.clear()
-                            else:
-                                self.data_queue.put(char)
+                raw_data = self.recv_msg()
+                if raw_data:
+                    data = raw_data.decode()
+                    if 'd' in set(data):
+                        self.data_queue.queue.clear()
+                        continue
+                    else:
+                        self.data_queue.put(data)
         except:
             logger.exception("Closing socket: %s", self.sock)
             self.sock.close()
             return
```

### Comparing `python-vlc-3.0.7110/examples/wxvlc.py` & `python-vlc-3.0.9113/examples/wxvlc.py`

 * *Files identical despite different names*

### Comparing `python-vlc-3.0.7110/python_vlc.egg-info/PKG-INFO` & `python-vlc-3.0.9113/python_vlc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.2
 Name: python-vlc
-Version: 3.0.7110
+Version: 3.0.9113
 Summary: VLC bindings for python.
 Home-page: http://wiki.videolan.org/PythonBinding
 Author: Olivier Aubert
 Author-email: contact@olivieraubert.net
 Maintainer: Olivier Aubert
 Maintainer-email: contact@olivieraubert.net
 License: LGPL-2.1+
 Description: This module provides ctypes-based bindings (see
               http://wiki.videolan.org/PythonBinding) for the native libvlc
               API (see http://wiki.videolan.org/LibVLC) of the VLC video
               player. Note that it relies on an already present install of VLC.
         
               It has been automatically generated from the include files of
-              vlc 3.0.7, using generator 1.10.
+              vlc 3.0.9, using generator 1.13.
               
 Keywords: vlc,video
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `python-vlc-3.0.7110/setup.py` & `python-vlc-3.0.9113/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distribute_setup import use_setuptools
 use_setuptools()
 
 from setuptools import setup
 
 setup(name='python-vlc',
-      version = '3.0.7110',
+      version = '3.0.9113',
       author='Olivier Aubert',
       author_email='contact@olivieraubert.net',
       maintainer='Olivier Aubert',
       maintainer_email='contact@olivieraubert.net',
       url='http://wiki.videolan.org/PythonBinding',
       py_modules=['vlc'],
       keywords = [ 'vlc', 'video' ],
@@ -31,9 +31,9 @@
       description = "VLC bindings for python.",
       long_description = """This module provides ctypes-based bindings (see
       http://wiki.videolan.org/PythonBinding) for the native libvlc
       API (see http://wiki.videolan.org/LibVLC) of the VLC video
       player. Note that it relies on an already present install of VLC.
 
       It has been automatically generated from the include files of
-      vlc 3.0.7, using generator 1.10.
+      vlc 3.0.9, using generator 1.13.
       """)
```

### Comparing `python-vlc-3.0.7110/vlc.py` & `python-vlc-3.0.9113/vlc.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 
 # Used by EventManager in override.py
 from inspect import getargspec
 
 import logging
 logger = logging.getLogger(__name__)
 
-__version__ = "3.0.7110"
-__libvlc_version__ = "3.0.7"
-__generator_version__ = "1.10"
-build_date  = "Sat Aug  3 20:13:06 2019 3.0.7"
+__version__ = "3.0.9113"
+__libvlc_version__ = "3.0.9"
+__generator_version__ = "1.13"
+build_date  = "Wed Apr 29 13:13:52 2020 3.0.9"
 
 # The libvlc doc states that filenames are expected to be in UTF8, do
 # not rely on sys.getfilesystemencoding() which will be confused,
 # esp. on windows.
 DEFAULT_ENCODING = 'utf-8'
 
 if sys.version_info[0] > 2:
@@ -153,14 +153,17 @@
                     p = p.format(homedir = homedir,
                                  programfiles = programfiles,
                                  libname = '\\VLC\\' + libname)
                     if os.path.exists(p):
                         plugin_path = os.path.dirname(p)
                         break
             if plugin_path is not None:  # try loading
+                 # PyInstaller Windows fix
+                if 'PyInstallerCDLL' in ctypes.CDLL.__name__:
+                    ctypes.windll.kernel32.SetDllDirectoryW(None)
                 p = os.getcwd()
                 os.chdir(plugin_path)
                  # if chdir failed, this will raise an exception
                 dll = ctypes.CDLL(libname)
                  # restore cwd after dll has been loaded
                 os.chdir(p)
             else:  # may fail
@@ -254,14 +257,23 @@
     """Return the default VLC.Instance.
     """
     global _default_instance
     if _default_instance is None:
         _default_instance = Instance()
     return _default_instance
 
+def try_fspath(path):
+    """Try calling os.fspath
+    os.fspath is only available from py3.6
+    """
+    try:
+        return os.fspath(path)
+    except (AttributeError, TypeError):
+        return path
+
 _Cfunctions = {}  # from LibVLC __version__
 _Globals = globals()  # sys.modules[__name__].__dict__
 
 def _Cfunction(name, flags, errcheck, *types):
     """(INTERNAL) New ctypes function binding.
     """
     if hasattr(dll, name) and name in _Globals:
@@ -1342,14 +1354,39 @@
         ('WhitePoint', ctypes.c_uint16 * 2),
         ('MaxMasteringLuminance', ctypes.c_uint),
         ('MinMasteringLuminance', ctypes.c_uint),
         ('MaxContentLightLevel', ctypes.c_uint16),
         ('MaxFrameAverageLightLevel', ctypes.c_uint16),
         ]
 
+class VideoSetupDeviceCfg(_Cstruct):
+    _fields_ = [
+        ('hardware_decoding', ctypes.c_bool),
+    ]
+
+class VideoSetupDeviceInfo(_Cstruct):
+    # FIXME: this is normally a union for D3D11/D3D9. We only define
+    # the mapping for d3d11 here
+    _fields_ = [
+        ('device_context', ctypes.c_void_p),
+    ]
+
+class VideoRenderCfg(_Cstruct):
+    _fields_ = [
+        ('width', ctypes.c_uint),
+        ('height', ctypes.c_uint),
+        ('bitdepth', ctypes.c_uint),
+        ('full_range', ctypes.c_bool),
+        # FIXME: should be references to enums
+        ('colorspace', ctypes.c_uint),
+        ('primaries', ctypes.c_uint),
+        ('transfer', ctypes.c_uint),
+        ('device', ctypes.c_void_p),
+        ]
+
 # Generated callback definitions #
 class Callback(ctypes.c_void_p):
     """Callback function notification.
     @param p_event: the event triggering the callback.
     """
     pass
 class LogCb(ctypes.c_void_p):
@@ -1526,41 +1563,41 @@
     LogCb.__doc__ = '''Callback prototype for LibVLC log message handler.
         @param data: data pointer as given to L{libvlc_log_set}().
         @param level: message level (@ref L{LogLevel}).
         @param ctx: message context (meta-information about the message).
         @param fmt: printf() format string (as defined by ISO C11).
         @param args: variable argument list for the format @note Log message handlers B{must} be thread-safe. @warning The message context pointer, the format string parameters and the variable arguments are only valid until the callback returns.
     '''
-    MediaOpenCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p), ctypes.POINTER(ctypes.c_uint64))
+    MediaOpenCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_int), ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p), ctypes.POINTER(ctypes.c_uint64))
     MediaOpenCb.__doc__ = '''Callback prototype to open a custom bitstream input media.
         The same media item can be opened multiple times. Each time, this callback
         is invoked. It should allocate and initialize any instance-specific
         resources, then store them in *datap. The instance resources can be freed
         in the @ref libvlc_media_close_cb callback.
         @param opaque: private pointer as passed to L{libvlc_media_new_callbacks}().
         @return: datap storage space for a private data pointer, sizep byte length of the bitstream or UINT64_MAX if unknown.
     '''
-    MediaReadCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.c_char_p, ctypes.c_size_t)
+    MediaReadCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_ssize_t), ctypes.c_void_p, ctypes.POINTER(ctypes.c_char), ctypes.c_size_t)
     MediaReadCb.__doc__ = '''Callback prototype to read data from a custom bitstream input media.
         @param opaque: private pointer as set by the @ref libvlc_media_open_cb callback.
         @param buf: start address of the buffer to read data into.
         @param len: bytes length of the buffer.
         @return: strictly positive number of bytes read, 0 on end-of-stream, or -1 on non-recoverable error @note If no data is immediately available, then the callback should sleep. @warning The application is responsible for avoiding deadlock situations. In particular, the callback should return an error if playback is stopped; if it does not return, then L{libvlc_media_player_stop}() will never return.
     '''
-    MediaSeekCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.c_uint64)
+    MediaSeekCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_int), ctypes.c_void_p, ctypes.c_uint64)
     MediaSeekCb.__doc__ = '''Callback prototype to seek a custom bitstream input media.
         @param opaque: private pointer as set by the @ref libvlc_media_open_cb callback.
         @param offset: absolute byte offset to seek to.
         @return: 0 on success, -1 on error.
     '''
     MediaCloseCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p)
     MediaCloseCb.__doc__ = '''Callback prototype to close a custom bitstream input media.
         @param opaque: private pointer as set by the @ref libvlc_media_open_cb callback.
     '''
-    VideoLockCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_void_p), ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p))
+    VideoLockCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p))
     VideoLockCb.__doc__ = '''Callback prototype to allocate and lock a picture buffer.
         Whenever a new video frame needs to be decoded, the lock callback is
         invoked. Depending on the video chroma, one or three pixel planes of
         adequate dimensions must be returned via the second parameter. Those
         planes must be aligned on 32-bytes boundaries.
         @param opaque: private pointer as passed to L{libvlc_video_set_callbacks}() [IN].
         @param planes: start address of the pixel planes (LibVLC allocates the array of void pointers, this callback must initialize the array) [OUT].
@@ -1580,15 +1617,15 @@
     VideoDisplayCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p)
     VideoDisplayCb.__doc__ = '''Callback prototype to display a picture.
         When the video frame needs to be shown, as determined by the media playback
         clock, the display callback is invoked.
         @param opaque: private pointer as passed to L{libvlc_video_set_callbacks}() [IN].
         @param picture: private pointer returned from the @ref libvlc_video_lock_cb callback [IN].
     '''
-    VideoFormatCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p), ctypes.c_char_p, ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint))
+    VideoFormatCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_void_p), ctypes.c_char_p, ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint))
     VideoFormatCb.__doc__ = '''Callback prototype to configure picture buffers format.
         This callback gets the format of the video as output by the video decoder
         and the chain of video filters (if any). It can opt to change any parameter
         as it needs. In that case, LibVLC will attempt to convert the video format
         (rescaling and chroma conversion) but these operations can be CPU intensive.
         @param opaque: pointer to the private pointer passed to L{libvlc_video_set_callbacks}() [IN/OUT].
         @param chroma: pointer to the 4 bytes video format identifier [IN/OUT].
@@ -1650,15 +1687,15 @@
     '''
     AudioSetVolumeCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p, ctypes.c_float, ctypes.c_bool)
     AudioSetVolumeCb.__doc__ = '''Callback prototype for audio volume change.
         @param data: data pointer as passed to L{libvlc_audio_set_callbacks}() [IN].
         @param volume: software volume (1. = nominal, 0. = mute).
         @param mute: muted flag.
     '''
-    AudioSetupCb = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.POINTER(ctypes.c_void_p), ctypes.c_char_p, ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint))
+    AudioSetupCb = ctypes.CFUNCTYPE(ctypes.POINTER(ctypes.c_int), ctypes.POINTER(ctypes.c_void_p), ctypes.c_char_p, ctypes.POINTER(ctypes.c_uint), ctypes.POINTER(ctypes.c_uint))
     AudioSetupCb.__doc__ = '''Callback prototype to setup the audio playback.
         This is called when the media player needs to create a new audio output.
         @param opaque: pointer to the data pointer passed to L{libvlc_audio_set_callbacks}() [IN/OUT].
         @param format: 4 bytes sample format [IN/OUT].
         @param rate: sample rate [IN/OUT].
         @param channels: channels count [IN/OUT].
         @return: 0 on success, anything else to skip audio playback.
@@ -1867,15 +1904,15 @@
         if PYTHON3:
             args = [ str_to_bytes(a) for a in args ]
         return libvlc_new(len(args), args)
 
     def media_player_new(self, uri=None):
         """Create a new MediaPlayer instance.
 
-        @param uri: an optional URI to play in the player.
+        @param uri: an optional URI to play in the player as a str, bytes or PathLike object.
         """
         p = libvlc_media_player_new(self)
         if uri:
             p.set_media(self.media_new(uri))
         p._instance = self
         return p
 
@@ -1899,30 +1936,41 @@
         and rather at the Instance level. For instance, the marquee
         filter must be specified when creating the vlc.Instance or
         vlc.MediaPlayer.
 
         Alternatively, options can be added to the media using the
         Media.add_options method (with the same limitation).
 
+        @param mrl: A str, bytes or PathLike object
         @param options: optional media option=value strings
         """
+        mrl = try_fspath(mrl)
         if ':' in mrl and mrl.index(':') > 1:
             # Assume it is a URL
             m = libvlc_media_new_location(self, str_to_bytes(mrl))
         else:
             # Else it should be a local path.
             m = libvlc_media_new_path(self, str_to_bytes(os.path.normpath(mrl)))
         for o in options:
             libvlc_media_add_option(m, str_to_bytes(o))
         m._instance = self
         return m
 
+    def media_new_path(self, path):
+        """Create a media for a certain file path.
+        See L{media_release}.
+        @param path: A str, byte, or PathLike object representing a local filesystem path.
+        @return: the newly created media or None on error.
+        """
+        path = try_fspath(path)
+        return libvlc_media_new_path(self, str_to_bytes(path))
+
     def media_list_new(self, mrls=None):
         """Create a new MediaList instance.
-        @param mrls: optional list of MRL strings
+        @param mrls: optional list of MRL strings, bytes, or PathLike objects.
         """
         l = libvlc_media_list_new(self)
         # We should take the lock, but since we did not leak the
         # reference, nobody else can access it.
         if mrls:
             for m in mrls:
                 l.add_media(m)
@@ -2309,23 +2357,14 @@
         See L{media_release}.
         @param psz_mrl: the media location.
         @return: the newly created media or None on error.
         '''
         return libvlc_media_new_location(self, str_to_bytes(psz_mrl))
 
 
-    def media_new_path(self, path):
-        '''Create a media for a certain file path.
-        See L{media_release}.
-        @param path: local filesystem path.
-        @return: the newly created media or None on error.
-        '''
-        return libvlc_media_new_path(self, str_to_bytes(path))
-
-
     def media_new_fd(self, fd):
         '''Create a media for an already open file descriptor.
         The file descriptor shall be open for reading (or reading and writing).
         Regular file descriptors, pipe read descriptors and character device
         descriptors (including TTYs) are supported on all platforms.
         Block device descriptors are supported where available.
         Directory descriptors are supported on systems that provide fdopendir().
@@ -3009,14 +3048,15 @@
     def add_media(self, mrl):
         """Add media instance to media list.
 
         The L{lock} should be held upon entering this function.
         @param mrl: a media instance or a MRL.
         @return: 0 on success, -1 if the media list is read-only.
         """
+        mrl = try_fspath(mrl)
         if isinstance(mrl, basestring):
             mrl = (self.get_instance() or get_default_instance()).media_new(mrl)
         return libvlc_media_list_add_media(self, mrl)
 
 
 
     def release(self):
@@ -5829,15 +5869,15 @@
     @param i_priority: from 0 (low priority) to 4 (high priority).
     @param psz_uri: Uri of the slave (should contain a valid scheme).
     @return: 0 on success, -1 on error.
     @version: LibVLC 3.0.0 and later.
     '''
     f = _Cfunctions.get('libvlc_media_slaves_add', None) or \
         _Cfunction('libvlc_media_slaves_add', ((1,), (1,), (1,), (1,),), None,
-                    ctypes.c_int, Media, MediaSlaveType, ctypes.c_int, ctypes.c_char_p)
+                    ctypes.c_int, Media, MediaSlaveType, ctypes.c_uint, ctypes.c_char_p)
     return f(p_md, i_type, i_priority, psz_uri)
 
 def libvlc_media_slaves_clear(p_md):
     '''Clear all slaves previously added by L{libvlc_media_slaves_add}() or
     internally.
     @param p_md: media descriptor object.
     @version: LibVLC 3.0.0 and later.
@@ -5855,26 +5895,26 @@
     @param p_md: media descriptor object.
     @param ppp_slaves: address to store an allocated array of slaves (must be freed with L{libvlc_media_slaves_release}()) [OUT].
     @return: the number of slaves (zero on error).
     @version: LibVLC 3.0.0 and later. See L{libvlc_media_slaves_add}.
     '''
     f = _Cfunctions.get('libvlc_media_slaves_get', None) or \
         _Cfunction('libvlc_media_slaves_get', ((1,), (1,),), None,
-                    ctypes.c_int, Media, ctypes.POINTER(ctypes.POINTER(MediaSlave)))
+                    ctypes.c_uint, Media, ctypes.POINTER(ctypes.POINTER(MediaSlave)))
     return f(p_md, ppp_slaves)
 
 def libvlc_media_slaves_release(pp_slaves, i_count):
     '''Release a media descriptor's slave list.
     @param pp_slaves: slave array to release.
     @param i_count: number of elements in the array.
     @version: LibVLC 3.0.0 and later.
     '''
     f = _Cfunctions.get('libvlc_media_slaves_release', None) or \
         _Cfunction('libvlc_media_slaves_release', ((1,), (1,),), None,
-                    None, ctypes.POINTER(MediaSlave), ctypes.c_int)
+                    None, ctypes.POINTER(MediaSlave), ctypes.c_uint)
     return f(pp_slaves, i_count)
 
 def libvlc_renderer_item_hold(p_item):
     '''Hold a renderer item, i.e. creates a new reference
     This functions need to called from the libvlc_RendererDiscovererItemAdded
     callback if the libvlc user wants to use this item after. (for display or
     for passing it to the mediaplayer for example).
@@ -7203,15 +7243,15 @@
     @param p_mi: the media player.
     @param position: position at which to display the title, or libvlc_position_disable to prevent the title from being displayed.
     @param timeout: title display timeout in milliseconds (ignored if libvlc_position_disable).
     @version: libVLC 2.1.0 or later.
     '''
     f = _Cfunctions.get('libvlc_media_player_set_video_title_display', None) or \
         _Cfunction('libvlc_media_player_set_video_title_display', ((1,), (1,), (1,),), None,
-                    None, MediaPlayer, Position, ctypes.c_int)
+                    None, MediaPlayer, Position, ctypes.c_uint)
     return f(p_mi, position, timeout)
 
 def libvlc_media_player_add_slave(p_mi, i_type, psz_uri, b_select):
     '''Add a slave to the current media player.
     @note: If the player is playing, the slave will be added directly. This call
     will also update the slave list of the attached L{Media}.
     @param p_mi: the media player.
@@ -7612,15 +7652,15 @@
     @param psz_filepath: the path of a file or a folder to save the screenshot into.
     @param i_width: the snapshot's width.
     @param i_height: the snapshot's height.
     @return: 0 on success, -1 if the video was not found.
     '''
     f = _Cfunctions.get('libvlc_video_take_snapshot', None) or \
         _Cfunction('libvlc_video_take_snapshot', ((1,), (1,), (1,), (1,), (1,),), None,
-                    ctypes.c_int, MediaPlayer, ctypes.c_uint, ctypes.c_char_p, ctypes.c_int, ctypes.c_int)
+                    ctypes.c_int, MediaPlayer, ctypes.c_uint, ctypes.c_char_p, ctypes.c_uint, ctypes.c_uint)
     return f(p_mi, num, psz_filepath, i_width, i_height)
 
 def libvlc_video_set_deinterlace(p_mi, psz_mode):
     '''Enable or disable deinterlace filter.
     @param p_mi: libvlc media player.
     @param psz_mode: type of deinterlace filter, None to disable.
     '''
```

