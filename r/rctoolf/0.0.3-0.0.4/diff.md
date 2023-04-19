# Comparing `tmp/rctoolf-0.0.3.tar.gz` & `tmp/rctoolf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rctoolf-0.0.3.tar", last modified: Wed Apr 19 08:29:32 2023, max compression
+gzip compressed data, was "rctoolf-0.0.4.tar", last modified: Wed Apr 19 08:59:17 2023, max compression
```

## Comparing `rctoolf-0.0.3.tar` & `rctoolf-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.870358 rctoolf-0.0.3/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.3/LICENSE
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.3/MANIFEST.in
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:29:32.869980 rctoolf-0.0.3/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        9 2023-04-14 09:14:57.000000 rctoolf-0.0.3/README.md
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      572 2023-04-19 08:28:51.000000 rctoolf-0.0.3/pyproject.toml
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-19 08:29:32.870480 rctoolf-0.0.3/setup.cfg
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.866205 rctoolf-0.0.3/src/
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.868125 rctoolf-0.0.3/src/rctoolf/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-19 08:28:58.000000 rctoolf-0.0.3/src/rctoolf/__init__.py
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1336 2023-04-14 00:35:51.000000 rctoolf-0.0.3/src/rctoolf/webhook.py
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.869410 rctoolf-0.0.3/src/rctoolf.egg-info/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      231 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/SOURCES.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/dependency_links.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/top_level.txt
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:59:17.592279 rctoolf-0.0.4/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.4/LICENSE
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.4/MANIFEST.in
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:59:17.591928 rctoolf-0.0.4/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        9 2023-04-14 09:14:57.000000 rctoolf-0.0.4/README.md
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      572 2023-04-19 08:59:02.000000 rctoolf-0.0.4/pyproject.toml
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-19 08:59:17.592368 rctoolf-0.0.4/setup.cfg
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:59:17.587904 rctoolf-0.0.4/src/
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:59:17.589858 rctoolf-0.0.4/src/rctoolf/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-19 08:58:06.000000 rctoolf-0.0.4/src/rctoolf/__init__.py
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1197 2023-04-19 08:58:44.000000 rctoolf-0.0.4/src/rctoolf/webhook.py
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:59:17.591487 rctoolf-0.0.4/src/rctoolf.egg-info/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:59:17.000000 rctoolf-0.0.4/src/rctoolf.egg-info/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      231 2023-04-19 08:59:17.000000 rctoolf-0.0.4/src/rctoolf.egg-info/SOURCES.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-19 08:59:17.000000 rctoolf-0.0.4/src/rctoolf.egg-info/dependency_links.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-19 08:59:17.000000 rctoolf-0.0.4/src/rctoolf.egg-info/top_level.txt
```

### Comparing `rctoolf-0.0.3/LICENSE` & `rctoolf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rctoolf-0.0.3/PKG-INFO` & `rctoolf-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rctoolf-0.0.3/pyproject.toml` & `rctoolf-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rctoolf"
-version = "0.0.3"
+version = "0.0.4"
 description = "Tools for RC"
 readme = "README.md"
 authors = [{ name = "Glorin Li", email = "ligr1991@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rctoolf-0.0.3/src/rctoolf/webhook.py` & `rctoolf-0.0.4/src/rctoolf/webhook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 #!/usr/bin/env python
 # encoding: utf-8
 from urllib import request
 import json
 
 
 class Webhook:
-    def __init__(self, url, author_name, author_icon, author_link):
+    def __init__(self, url):
         self._url = url
-        self._author_name = author_name
-        self._author_icon = author_icon
-        self._author_link = author_link
-
     def _send(self, payload):
         json_data = json.dumps(payload)
         # print('Json data')
         print(json_data)
 
         req = request.Request(self._url, data=json_data.encode())
         req.add_header('Content-Type', 'application/json')
 
         res_data = request.urlopen(req)
         res = res_data.read()
         print("Result:")
         print(res)
 
-    def send_card(self, title, message, fields):
+    def send_card(self, title, message, fields, author_name, author_icon, author_link):
         payload = {
             "attachments": [
                 {
                     "type": "Card",
                     "fallback": "Something bad happened",
                     "color": "#00ff2a",
                     "title": title,
                     "text": message,
-                    "author_name": self._author_name,
-                    "author_icon": self._author_icon,
-                    "author_link": self._author_link,
+                    "author_name": author_name,
+                    "author_icon": author_icon,
+                    "author_link": author_link,
                     "fields": fields
                 }
             ]
         }
 
         self._send(payload)
```

### Comparing `rctoolf-0.0.3/src/rctoolf.egg-info/PKG-INFO` & `rctoolf-0.0.4/src/rctoolf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

