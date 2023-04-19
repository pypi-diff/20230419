# Comparing `tmp/netlink-client-0.2.5.tar.gz` & `tmp/netlink-client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-client-0.2.5.tar", last modified: Wed Apr 19 16:08:41 2023, max compression
+gzip compressed data, was "netlink-client-1.0.0.tar", last modified: Wed Apr 19 17:12:00 2023, max compression
```

## Comparing `netlink-client-0.2.5.tar` & `netlink-client-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)       34 2023-04-19 15:30:06.000000 netlink-client-0.2.5/MANIFEST.in
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      986 2023-04-19 16:08:41.676225 netlink-client-0.2.5/PKG-INFO
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      690 2023-04-19 16:08:20.000000 netlink-client-0.2.5/README.md
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      504 2023-04-19 16:08:41.676225 netlink-client-0.2.5/setup.cfg
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      425 2023-04-19 15:27:10.000000 netlink-client-0.2.5/setup.py
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.672225 netlink-client-0.2.5/src/
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/src/netlink_Boaz_Tene/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     2459 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/main.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     3439 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     1237 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.h
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     5381 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      962 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.h
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/src/netlink_client.egg-info/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      986 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/PKG-INFO
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      377 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/SOURCES.txt
--rw-rw-r--   0 boaz      (1000) boaz      (1000)        1 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/dependency_links.txt
--rw-rw-r--   0 boaz      (1000) boaz      (1000)        8 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/top_level.txt
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 17:12:00.521832 netlink-client-1.0.0/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)       34 2023-04-19 17:06:09.000000 netlink-client-1.0.0/MANIFEST.in
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     1016 2023-04-19 17:12:00.521832 netlink-client-1.0.0/PKG-INFO
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      720 2023-04-19 17:06:24.000000 netlink-client-1.0.0/README.md
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      504 2023-04-19 17:12:00.521832 netlink-client-1.0.0/setup.cfg
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      425 2023-04-19 17:06:09.000000 netlink-client-1.0.0/setup.py
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 17:12:00.517832 netlink-client-1.0.0/src/
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 17:12:00.521832 netlink-client-1.0.0/src/netlink_Boaz_Tene/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     2459 2023-04-19 17:06:09.000000 netlink-client-1.0.0/src/netlink_Boaz_Tene/main.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     3432 2023-04-19 17:06:15.000000 netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     1237 2023-04-19 17:06:09.000000 netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink.h
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     5410 2023-04-19 17:11:46.000000 netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink_class.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      962 2023-04-19 17:06:09.000000 netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink_class.h
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 17:12:00.521832 netlink-client-1.0.0/src/netlink_client.egg-info/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     1016 2023-04-19 17:12:00.000000 netlink-client-1.0.0/src/netlink_client.egg-info/PKG-INFO
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      391 2023-04-19 17:12:00.000000 netlink-client-1.0.0/src/netlink_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)        1 2023-04-19 17:12:00.000000 netlink-client-1.0.0/src/netlink_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)        8 2023-04-19 17:12:00.000000 netlink-client-1.0.0/src/netlink_client.egg-info/top_level.txt
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 17:12:00.521832 netlink-client-1.0.0/tests/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      139 2023-04-19 17:08:04.000000 netlink-client-1.0.0/tests/test.py
```

### Comparing `netlink-client-0.2.5/PKG-INFO` & `netlink-client-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-client
-Version: 0.2.5
+Version: 1.0.0
 Summary: Python Netlink client for linux
 Home-page: https://github.com/BoazTene/netlink
 Author: Boaz Tene
 Author-email: boaztene2005@gmail.com
 License: GNU General Public License
 Platform: = Linux
 Description-Content-Type: text/markdown
@@ -42,13 +42,13 @@
 from netlink import NetLink
 
 netlink = NetLink(31) // 31 is the magic number
 
 netlink.send(b"Hello Netlink!")
 result = netlink.recv(1024) // number of bytes
 
-print(result.decode('utf8'))
+print(result.decode('utf8')) // prints result from kernel.
 
 netlink.close() // closes the connection
 ```
 
 netlink Copyright (C) 2023 Boaz Tene
```

### Comparing `netlink-client-0.2.5/README.md` & `netlink-client-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 from netlink import NetLink
 
 netlink = NetLink(31) // 31 is the magic number
 
 netlink.send(b"Hello Netlink!")
 result = netlink.recv(1024) // number of bytes
 
-print(result.decode('utf8'))
+print(result.decode('utf8')) // prints result from kernel.
 
 netlink.close() // closes the connection
 ```
 
 netlink Copyright (C) 2023 Boaz Tene
```

### Comparing `netlink-client-0.2.5/src/netlink_Boaz_Tene/main.c` & `netlink-client-1.0.0/src/netlink_Boaz_Tene/main.c`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.c` & `netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink.c`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   struct msghdr msg;
 
   memset(nlh, 0, NLMSG_SPACE(size));
   nlh->nlmsg_len = NLMSG_SPACE(size);
   nlh->nlmsg_pid = getpid();
   nlh->nlmsg_flags = 0;
 
-  strncpy(NLMSG_DATA(nlh), message, size);
+  strcpy(NLMSG_DATA(nlh), message);
 
   iov.iov_base = (void *)nlh;
   iov.iov_len = nlh->nlmsg_len;
   memset(&msg, 0, sizeof(msg));
   msg.msg_name = (void *)&nl->dst_addr;
   msg.msg_namelen = sizeof(nl->dst_addr);
   msg.msg_iov = &iov;
```

### Comparing `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.h` & `netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink.h`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.c` & `netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink_class.c`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,29 @@
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 */
 #include <Python.h>
 #include "netlink_class.h"
 
 static PyObject *netlink_send(NetLink *self, PyObject *args) {
-  const char *message;
+  Py_buffer buffer;
 
-  if (!PyArg_ParseTuple(args, "y", &message)) {
+  if (!PyArg_ParseTuple(args, "y*", &buffer)) {
     PyErr_SetString(PyExc_TypeError, "Received invalid argument.");
     return NULL;
   }
 
-  send_nl(self->netlink, message, sizeof(message));
+  send_nl(self->netlink, (char *) buffer.buf, buffer.len);
+  PyBuffer_Release(&buffer);
 
   Py_RETURN_NONE;
 }
 
 static PyObject *netlink_recv(NetLink *self, PyObject *args) {
-  ssize_t bytes;
+  int bytes;
 
   if (!PyArg_ParseTuple(args, "i", &bytes)) {
     PyErr_SetString(PyExc_TypeError, "Received invalid argument.");
     return NULL;
   }
 
   char *buf = (char *)PyMem_Malloc(bytes);
```

### Comparing `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.h` & `netlink-client-1.0.0/src/netlink_Boaz_Tene/netlink_class.h`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.5/src/netlink_client.egg-info/PKG-INFO` & `netlink-client-1.0.0/src/netlink_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-client
-Version: 0.2.5
+Version: 1.0.0
 Summary: Python Netlink client for linux
 Home-page: https://github.com/BoazTene/netlink
 Author: Boaz Tene
 Author-email: boaztene2005@gmail.com
 License: GNU General Public License
 Platform: = Linux
 Description-Content-Type: text/markdown
@@ -42,13 +42,13 @@
 from netlink import NetLink
 
 netlink = NetLink(31) // 31 is the magic number
 
 netlink.send(b"Hello Netlink!")
 result = netlink.recv(1024) // number of bytes
 
-print(result.decode('utf8'))
+print(result.decode('utf8')) // prints result from kernel.
 
 netlink.close() // closes the connection
 ```
 
 netlink Copyright (C) 2023 Boaz Tene
```

