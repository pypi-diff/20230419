# Comparing `tmp/ascii-cli-0.0.3.tar.gz` & `tmp/ascii-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.3.tar", last modified: Wed Apr 19 12:35:24 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.4.tar", last modified: Wed Apr 19 12:39:58 2023, max compression
```

## Comparing `ascii-cli-0.0.3.tar` & `ascii-cli-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:35:24.809886 ascii-cli-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 12:35:24.807881 ascii-cli-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:35:24.804882 ascii-cli-0.0.3/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 12:35:24.809886 ascii-cli-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-04-19 12:34:59.000000 ascii-cli-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:39:58.453477 ascii-cli-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:39:58.452512 ascii-cli-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:39:58.446476 ascii-cli-0.0.4/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:39:58.000000 ascii-cli-0.0.4/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:39:58.454480 ascii-cli-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-04-19 12:39:36.000000 ascii-cli-0.0.4/setup.py
```

### Comparing `ascii-cli-0.0.3/LICENSE` & `ascii-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.3/PKG-INFO` & `ascii-cli-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.3/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.4/ascii_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.3/setup.py` & `ascii-cli-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
             "ascii-cli = src.ascii:main",
         ],
     },
```

