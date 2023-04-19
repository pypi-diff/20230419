# Comparing `tmp/ascii-cli-0.0.2.tar.gz` & `tmp/ascii-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.0.2.tar", last modified: Wed Apr 19 12:28:14 2023, max compression
+gzip compressed data, was "ascii-cli-0.0.3.tar", last modified: Wed Apr 19 12:35:24 2023, max compression
```

## Comparing `ascii-cli-0.0.2.tar` & `ascii-cli-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:28:14.832008 ascii-cli-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      750 2023-04-19 12:28:14.830033 ascii-cli-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 12:28:14.832008 ascii-cli-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-04-19 12:28:07.000000 ascii-cli-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:28:14.772022 ascii-cli-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:28:14.827007 ascii-cli-0.0.2/src/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0      750 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:28:14.000000 ascii-cli-0.0.2/src/ascii_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:35:24.809886 ascii-cli-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:35:24.807881 ascii-cli-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-19 08:36:47.000000 ascii-cli-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:35:24.804882 ascii-cli-0.0.3/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0      750 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:35:24.000000 ascii-cli-0.0.3/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:35:24.809886 ascii-cli-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-04-19 12:34:59.000000 ascii-cli-0.0.3/setup.py
```

### Comparing `ascii-cli-0.0.2/LICENSE` & `ascii-cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.0.2/PKG-INFO` & `ascii-cli-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.0.2/setup.py` & `ascii-cli-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.0.2",
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
+    version="0.0.3",
+    packages=find_packages(),
     install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
             "ascii-cli = src.ascii:main",
         ],
     },
     classifiers=[
```

### Comparing `ascii-cli-0.0.2/src/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.0.3/ascii_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

