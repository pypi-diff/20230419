# Comparing `tmp/ascii-cli-0.0.5.tar.gz` & `tmp/ascii-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.5.tar", last modified: Wed Apr 19 12:47:35 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.6.tar", last modified: Wed Apr 19 12:52:16 2023, max compression
```

## Comparing `ascii-cli-0.0.5.tar` & `ascii-cli-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:47:35.139051 ascii-cli-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 12:47:35.139051 ascii-cli-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:47:35.126902 ascii-cli-0.0.5/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:47:34.000000 ascii-cli-0.0.5/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 12:47:35.145308 ascii-cli-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-04-19 12:46:46.000000 ascii-cli-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:52:16.707888 ascii-cli-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:52:16.705889 ascii-cli-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:52:16.701889 ascii-cli-0.0.6/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:52:16.000000 ascii-cli-0.0.6/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:52:16.708890 ascii-cli-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-19 12:51:40.000000 ascii-cli-0.0.6/setup.py
```

### Comparing `ascii-cli-0.0.5/LICENSE` & `ascii-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.5/PKG-INFO` & `ascii-cli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.5/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.6/ascii_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.5/setup.py` & `ascii-cli-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
-            "ascii-cli = ascii:main",
+            "ascii-cli = ascii",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

