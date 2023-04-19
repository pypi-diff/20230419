# Comparing `tmp/widget-picture-generator-0.0.3.tar.gz` & `tmp/widget-picture-generator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widget-picture-generator-0.0.3.tar", last modified: Wed Apr 19 13:26:48 2023, max compression
+gzip compressed data, was "widget-picture-generator-0.0.4.tar", last modified: Wed Apr 19 13:31:50 2023, max compression
```

## Comparing `widget-picture-generator-0.0.3.tar` & `widget-picture-generator-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:26:48.642558 widget-picture-generator-0.0.3/
--rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.3/LICENSE
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:26:48.642433 widget-picture-generator-0.0.3/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      912 2023-04-19 12:49:31.000000 widget-picture-generator-0.0.3/README.md
--rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:26:48.642609 widget-picture-generator-0.0.3/setup.cfg
--rw-r--r--   0 maxmoffa   (502) staff       (20)      778 2023-04-19 13:26:19.000000 widget-picture-generator-0.0.3/setup.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:26:48.641636 widget-picture-generator-0.0.3/src/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     3316 2023-04-19 13:15:43.000000 widget-picture-generator-0.0.3/src/WidgetPictureGenerator.py
--rw-r--r--   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:01:02.000000 widget-picture-generator-0.0.3/src/__init__.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:26:48.642257 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:26:48.000000 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      311 2023-04-19 13:26:48.000000 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/SOURCES.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:26:48.000000 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/dependency_links.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        9 2023-04-19 13:26:48.000000 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/requires.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        4 2023-04-19 13:26:48.000000 widget-picture-generator-0.0.3/widget_picture_generator.egg-info/top_level.txt
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.146733 widget-picture-generator-0.0.4/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.4/LICENSE
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:31:50.146611 widget-picture-generator-0.0.4/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      912 2023-04-19 12:49:31.000000 widget-picture-generator-0.0.4/README.md
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:31:50.146778 widget-picture-generator-0.0.4/setup.cfg
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      797 2023-04-19 13:29:48.000000 widget-picture-generator-0.0.4/setup.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.145586 widget-picture-generator-0.0.4/widget_picture_generator/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     3316 2023-04-19 13:15:43.000000 widget-picture-generator-0.0.4/widget_picture_generator/__init__.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.146435 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      302 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)        9 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/requires.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       25 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/top_level.txt
```

### Comparing `widget-picture-generator-0.0.3/LICENSE` & `widget-picture-generator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.3/PKG-INFO` & `widget-picture-generator-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widget-picture-generator-0.0.3/README.md` & `widget-picture-generator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.3/setup.py` & `widget-picture-generator-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="widget-picture-generator",
-    version="0.0.3",
+    version="0.0.4",
     author="Massimo Moffa",
     author_email="massimo.moffa@sensesquare.eu",
     description="This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sense-Square/widget-picture-generator",
-    packages=['src'],
+    packages=setuptools.find_packages(),
     install_requires=[
         'selenium'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `widget-picture-generator-0.0.3/src/WidgetPictureGenerator.py` & `widget-picture-generator-0.0.4/widget_picture_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.3/widget_picture_generator.egg-info/PKG-INFO` & `widget-picture-generator-0.0.4/widget_picture_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

