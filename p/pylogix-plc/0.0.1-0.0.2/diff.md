# Comparing `tmp/pylogix_plc-0.0.1.tar.gz` & `tmp/pylogix_plc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogix_plc-0.0.1.tar", last modified: Wed Apr 19 00:19:11 2023, max compression
+gzip compressed data, was "pylogix_plc-0.0.2.tar", last modified: Wed Apr 19 00:21:47 2023, max compression
```

## Comparing `pylogix_plc-0.0.1.tar` & `pylogix_plc-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 00:19:11.277465 pylogix_plc-0.0.1/
--rw-rw-rw-   0        0        0     3776 2023-04-19 00:19:11.272461 pylogix_plc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-04-18 21:07:42.000000 pylogix_plc-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 00:19:11.207468 pylogix_plc-0.0.1/guesser_game/
--rw-rw-rw-   0        0        0      320 2023-03-07 06:02:06.000000 pylogix_plc-0.0.1/guesser_game/GuesserGame.py
--rw-rw-rw-   0        0        0       45 2023-03-07 06:02:06.000000 pylogix_plc-0.0.1/guesser_game/__init__.py
--rw-rw-rw-   0        0        0     2373 2023-03-07 06:02:06.000000 pylogix_plc-0.0.1/guesser_game/numberGuesserGame.py
--rw-rw-rw-   0        0        0     1055 2023-03-07 06:02:06.000000 pylogix_plc-0.0.1/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 00:19:11.267464 pylogix_plc-0.0.1/pylogix_plc.egg-info/
--rw-rw-rw-   0        0        0     3776 2023-04-19 00:19:10.000000 pylogix_plc-0.0.1/pylogix_plc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-19 00:19:10.000000 pylogix_plc-0.0.1/pylogix_plc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 00:19:10.000000 pylogix_plc-0.0.1/pylogix_plc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 00:19:10.000000 pylogix_plc-0.0.1/pylogix_plc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 00:19:11.277465 pylogix_plc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3900 2023-04-19 00:18:41.000000 pylogix_plc-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:21:47.016730 pylogix_plc-0.0.2/
+-rw-rw-rw-   0        0        0     3776 2023-04-19 00:21:47.016730 pylogix_plc-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-04-18 21:07:42.000000 pylogix_plc-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 00:21:46.976911 pylogix_plc-0.0.2/guesser_game/
+-rw-rw-rw-   0        0        0      320 2023-03-07 06:02:06.000000 pylogix_plc-0.0.2/guesser_game/GuesserGame.py
+-rw-rw-rw-   0        0        0       45 2023-03-07 06:02:06.000000 pylogix_plc-0.0.2/guesser_game/__init__.py
+-rw-rw-rw-   0        0        0     2373 2023-03-07 06:02:06.000000 pylogix_plc-0.0.2/guesser_game/numberGuesserGame.py
+-rw-rw-rw-   0        0        0     1055 2023-03-07 06:02:06.000000 pylogix_plc-0.0.2/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 00:21:47.011734 pylogix_plc-0.0.2/pylogix_plc.egg-info/
+-rw-rw-rw-   0        0        0     3776 2023-04-19 00:21:46.000000 pylogix_plc-0.0.2/pylogix_plc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-19 00:21:46.000000 pylogix_plc-0.0.2/pylogix_plc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 00:21:46.000000 pylogix_plc-0.0.2/pylogix_plc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 00:21:46.000000 pylogix_plc-0.0.2/pylogix_plc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 00:21:47.016730 pylogix_plc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3900 2023-04-19 00:21:32.000000 pylogix_plc-0.0.2/setup.py
```

### Comparing `pylogix_plc-0.0.1/PKG-INFO` & `pylogix_plc-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogix_plc
-Version: 0.0.1
+Version: 0.0.2
 Summary: The new Python package, called https://pylogix.com/ provides a communication driver that simplifies the process of reading and writing tag values from Rockwell Automation ControlLogix.
 Home-page: https://github.com/PYLOGiX-DEV/pylogix_
 Author: https://pylogix.com/
 Author-email: dev@pylogix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylogix_plc-0.0.1/README.md` & `pylogix_plc-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pylogix_plc-0.0.1/guesser_game/numberGuesserGame.py` & `pylogix_plc-0.0.2/guesser_game/numberGuesserGame.py`

 * *Files identical despite different names*

### Comparing `pylogix_plc-0.0.1/license.txt` & `pylogix_plc-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `pylogix_plc-0.0.1/pylogix_plc.egg-info/PKG-INFO` & `pylogix_plc-0.0.2/pylogix_plc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogix-plc
-Version: 0.0.1
+Version: 0.0.2
 Summary: The new Python package, called https://pylogix.com/ provides a communication driver that simplifies the process of reading and writing tag values from Rockwell Automation ControlLogix.
 Home-page: https://github.com/PYLOGiX-DEV/pylogix_
 Author: https://pylogix.com/
 Author-email: dev@pylogix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylogix_plc-0.0.1/setup.py` & `pylogix_plc-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setup(
     name="pylogix_plc",
-    version="0.0.1",
+    version="0.0.2",
     author="https://pylogix.com/",
     author_email="dev@pylogix.com",
     description="The new Python package, called https://pylogix.com/ provides a communication driver that simplifies the process of reading and writing tag values from Rockwell Automation ControlLogix.",
     long_description="""
 # pylogix - A Python Package for Rockwell Automation ControlLogix, CompactLogix and Micro8xx PLC's
 
 Pylogix is a Python package developed by  [Pylogix](https://pylogix.com/) ,  -  [https://pylogix.com/](https://pylogix.com/), which is a software company that allows you to easily read/write values from tags in Rockwell Automation ControlLogix, CompactLogix, and Micro8xx PLC's over Ethernet I/P.
```

