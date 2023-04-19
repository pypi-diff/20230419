# Comparing `tmp/ascii-cli-0.0.4.tar.gz` & `tmp/ascii-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.4.tar", last modified: Wed Apr 19 12:39:58 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.5.tar", last modified: Wed Apr 19 12:47:35 2023, max compression
```

## Comparing `ascii-cli-0.0.4.tar` & `ascii-cli-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:39:58.453477 ascii-cli-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 12:39:58.452512 ascii-cli-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:39:58.446476 ascii-cli-0.0.4/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 12:39:58.454480 ascii-cli-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-04-19 12:39:36.000000 ascii-cli-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:47:35.139051 ascii-cli-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:47:35.139051 ascii-cli-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:47:35.126902 ascii-cli-0.0.5/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:47:35.145308 ascii-cli-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-04-19 12:46:46.000000 ascii-cli-0.0.5/setup.py
```

### Comparing `ascii-cli-0.0.4/LICENSE` & `ascii-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.4/PKG-INFO` & `ascii-cli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.4/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.5/ascii_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.4/setup.py` & `ascii-cli-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
-            "ascii-cli = src.ascii:main",
+            "ascii-cli = ascii:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

