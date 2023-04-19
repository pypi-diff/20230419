# Comparing `tmp/netlink-client-0.2.4.tar.gz` & `tmp/netlink-client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-client-0.2.4.tar", last modified: Wed Apr 19 16:05:12 2023, max compression
+gzip compressed data, was "netlink-client-0.2.5.tar", last modified: Wed Apr 19 16:08:41 2023, max compression
```

## Comparing `netlink-client-0.2.4.tar` & `netlink-client-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:05:12.673559 netlink-client-0.2.4/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)       34 2023-04-19 15:30:06.000000 netlink-client-0.2.4/MANIFEST.in
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      979 2023-04-19 16:05:12.673559 netlink-client-0.2.4/PKG-INFO
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      683 2023-04-19 15:51:57.000000 netlink-client-0.2.4/README.md
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      504 2023-04-19 16:05:12.673559 netlink-client-0.2.4/setup.cfg
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      425 2023-04-19 15:27:10.000000 netlink-client-0.2.4/setup.py
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:05:12.669559 netlink-client-0.2.4/src/
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:05:12.669559 netlink-client-0.2.4/src/netlink_Boaz_Tene/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     2459 2023-04-19 14:57:29.000000 netlink-client-0.2.4/src/netlink_Boaz_Tene/main.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     3439 2023-04-19 14:57:29.000000 netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     1237 2023-04-19 14:57:29.000000 netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink.h
--rw-rw-r--   0 boaz      (1000) boaz      (1000)     5381 2023-04-19 14:57:29.000000 netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink_class.c
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      962 2023-04-19 14:57:29.000000 netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink_class.h
-drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:05:12.673559 netlink-client-0.2.4/src/netlink_client.egg-info/
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      979 2023-04-19 16:05:12.000000 netlink-client-0.2.4/src/netlink_client.egg-info/PKG-INFO
--rw-rw-r--   0 boaz      (1000) boaz      (1000)      377 2023-04-19 16:05:12.000000 netlink-client-0.2.4/src/netlink_client.egg-info/SOURCES.txt
--rw-rw-r--   0 boaz      (1000) boaz      (1000)        1 2023-04-19 16:05:12.000000 netlink-client-0.2.4/src/netlink_client.egg-info/dependency_links.txt
--rw-rw-r--   0 boaz      (1000) boaz      (1000)        8 2023-04-19 16:05:12.000000 netlink-client-0.2.4/src/netlink_client.egg-info/top_level.txt
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)       34 2023-04-19 15:30:06.000000 netlink-client-0.2.5/MANIFEST.in
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      986 2023-04-19 16:08:41.676225 netlink-client-0.2.5/PKG-INFO
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      690 2023-04-19 16:08:20.000000 netlink-client-0.2.5/README.md
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      504 2023-04-19 16:08:41.676225 netlink-client-0.2.5/setup.cfg
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      425 2023-04-19 15:27:10.000000 netlink-client-0.2.5/setup.py
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.672225 netlink-client-0.2.5/src/
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/src/netlink_Boaz_Tene/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     2459 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/main.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     3439 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     1237 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.h
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)     5381 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.c
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      962 2023-04-19 14:57:29.000000 netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.h
+drwxrwxr-x   0 boaz      (1000) boaz      (1000)        0 2023-04-19 16:08:41.676225 netlink-client-0.2.5/src/netlink_client.egg-info/
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      986 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/PKG-INFO
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)      377 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)        1 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 boaz      (1000) boaz      (1000)        8 2023-04-19 16:08:41.000000 netlink-client-0.2.5/src/netlink_client.egg-info/top_level.txt
```

### Comparing `netlink-client-0.2.4/PKG-INFO` & `netlink-client-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Netlink client for linux
 Home-page: https://github.com/BoazTene/netlink
 Author: Boaz Tene
 Author-email: boaztene2005@gmail.com
 License: GNU General Public License
 Platform: = Linux
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 A simple python module for the kernel netlink interface.
 
 
 ## Installition
 
 #### Installition via pip
 `
-pip install netlink
+pip install netlink-client
 `
 
 #### Installition from source
 To install from source:
 
 ```
 git clone https://github.com/BoazTene/netlink
```

### Comparing `netlink-client-0.2.4/README.md` & `netlink-client-0.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A simple python module for the kernel netlink interface.
 
 
 ## Installition
 
 #### Installition via pip
 `
-pip install netlink
+pip install netlink-client
 `
 
 #### Installition from source
 To install from source:
 
 ```
 git clone https://github.com/BoazTene/netlink
```

### Comparing `netlink-client-0.2.4/src/netlink_Boaz_Tene/main.c` & `netlink-client-0.2.5/src/netlink_Boaz_Tene/main.c`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink.c` & `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.c`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink.h` & `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink.h`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink_class.c` & `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.c`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.4/src/netlink_Boaz_Tene/netlink_class.h` & `netlink-client-0.2.5/src/netlink_Boaz_Tene/netlink_class.h`

 * *Files identical despite different names*

### Comparing `netlink-client-0.2.4/src/netlink_client.egg-info/PKG-INFO` & `netlink-client-0.2.5/src/netlink_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Netlink client for linux
 Home-page: https://github.com/BoazTene/netlink
 Author: Boaz Tene
 Author-email: boaztene2005@gmail.com
 License: GNU General Public License
 Platform: = Linux
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 A simple python module for the kernel netlink interface.
 
 
 ## Installition
 
 #### Installition via pip
 `
-pip install netlink
+pip install netlink-client
 `
 
 #### Installition from source
 To install from source:
 
 ```
 git clone https://github.com/BoazTene/netlink
```

