# Comparing `tmp/Ayra-0.0.1.tar.gz` & `tmp/Ayra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ayra-0.0.1.tar", last modified: Wed Apr 19 16:11:14 2023, max compression
+gzip compressed data, was "Ayra-0.0.2.tar", last modified: Wed Apr 19 16:20:41 2023, max compression
```

## Comparing `Ayra-0.0.1.tar` & `Ayra-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:11:14.067636 Ayra-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:11:14.067636 Ayra-0.0.1/Ayra/
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-19 16:09:09.000000 Ayra-0.0.1/Ayra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:11:14.067636 Ayra-0.0.1/Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-19 16:11:14.000000 Ayra-0.0.1/Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-19 16:11:14.000000 Ayra-0.0.1/Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:11:14.000000 Ayra-0.0.1/Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 16:11:14.000000 Ayra-0.0.1/Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-19 16:11:14.000000 Ayra-0.0.1/Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-19 16:11:14.067636 Ayra-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-19 16:09:09.000000 Ayra-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 16:11:14.067636 Ayra-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      953 2023-04-19 16:09:09.000000 Ayra-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:41.750196 Ayra-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:41.750196 Ayra-0.0.2/Ayra/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-19 16:19:38.000000 Ayra-0.0.2/Ayra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:41.750196 Ayra-0.0.2/Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-19 16:20:41.000000 Ayra-0.0.2/Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-19 16:20:41.000000 Ayra-0.0.2/Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:20:41.000000 Ayra-0.0.2/Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 16:20:41.000000 Ayra-0.0.2/Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-19 16:20:41.000000 Ayra-0.0.2/Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-19 16:20:41.750196 Ayra-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-19 16:19:38.000000 Ayra-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 16:20:41.754197 Ayra-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-19 16:19:38.000000 Ayra-0.0.2/setup.py
```

### Comparing `Ayra-0.0.1/Ayra.egg-info/PKG-INFO` & `Ayra-0.0.2/Ayra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Ayra
-Version: 0.0.1
-Summary: A Secure and Powerful Python-Telethon Based Library For Ultroid Userbot.
+Version: 0.0.2
+Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/ayra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Ayra-0.0.1/PKG-INFO` & `Ayra-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Ayra
-Version: 0.0.1
-Summary: A Secure and Powerful Python-Telethon Based Library For Ultroid Userbot.
+Version: 0.0.2
+Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/ayra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Ayra-0.0.1/setup.py` & `Ayra-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 name = "Ayra"
-version = "0.0.1"
+version = "0.0.2"
 author = "naya1503"
 author_email = "cosmospanas70@gmail.com"
-description = "A Secure and Powerful Python-Telethon Based Library For Ultroid Userbot."
+description = "A Secure and Powerful Python-Telethon Based Library For Ayra Userbot."
 license = "GNU AFFERO GENERAL PUBLIC LICENSE (v3)"
 url = "https://github.com/naya1503/ayra"
 
 setuptools.setup(
     name=name,
     version=version,
     author=author,
```

