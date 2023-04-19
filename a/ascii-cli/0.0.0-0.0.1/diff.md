# Comparing `tmp/ascii-cli-0.0.0.tar.gz` & `tmp/ascii-cli-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.0.tar", last modified: Wed Apr 19 10:46:51 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.1.tar", last modified: Wed Apr 19 11:41:37 2023, max compression
```

## Comparing `ascii-cli-0.0.0.tar` & `ascii-cli-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:46:51.365130 ascii-cli-0.0.0/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 10:46:51.355138 ascii-cli-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 10:46:51.366129 ascii-cli-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-04-19 10:41:28.000000 ascii-cli-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:46:51.265128 ascii-cli-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 10:46:51.348138 ascii-cli-0.0.0/src/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:46:51.000000 ascii-cli-0.0.0/src/ascii_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 11:41:37.791545 ascii-cli-0.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-19 11:41:37.789528 ascii-cli-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:41:37.791545 ascii-cli-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-04-19 11:40:53.000000 ascii-cli-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:41:37.727523 ascii-cli-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:41:37.786533 ascii-cli-0.0.1/src/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:41:37.000000 ascii-cli-0.0.1/src/ascii_cli.egg-info/top_level.txt
```

### Comparing `ascii-cli-0.0.0/LICENSE` & `ascii-cli-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.0/PKG-INFO` & `ascii-cli-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.0
+Version: 0.0.1
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.0/setup.py` & `ascii-cli-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.0",
+    version="0.0.1",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
             "ascii-cli = ascii_cli.cli:main",
         ],
```

### Comparing `ascii-cli-0.0.0/src/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.1/src/ascii_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.0
+Version: 0.0.1
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

