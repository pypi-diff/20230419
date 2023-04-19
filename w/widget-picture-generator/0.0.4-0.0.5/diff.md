# Comparing `tmp/widget-picture-generator-0.0.4.tar.gz` & `tmp/widget-picture-generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widget-picture-generator-0.0.4.tar", last modified: Wed Apr 19 13:31:50 2023, max compression
+gzip compressed data, was "widget-picture-generator-0.0.5.tar", last modified: Wed Apr 19 13:40:51 2023, max compression
```

## Comparing `widget-picture-generator-0.0.4.tar` & `widget-picture-generator-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.146733 widget-picture-generator-0.0.4/
--rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.4/LICENSE
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:31:50.146611 widget-picture-generator-0.0.4/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      912 2023-04-19 12:49:31.000000 widget-picture-generator-0.0.4/README.md
--rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:31:50.146778 widget-picture-generator-0.0.4/setup.cfg
--rw-r--r--   0 maxmoffa   (502) staff       (20)      797 2023-04-19 13:29:48.000000 widget-picture-generator-0.0.4/setup.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.145586 widget-picture-generator-0.0.4/widget_picture_generator/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     3316 2023-04-19 13:15:43.000000 widget-picture-generator-0.0.4/widget_picture_generator/__init__.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:31:50.146435 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      302 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/SOURCES.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/dependency_links.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        9 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/requires.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)       25 2023-04-19 13:31:50.000000 widget-picture-generator-0.0.4/widget_picture_generator.egg-info/top_level.txt
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.025050 widget-picture-generator-0.0.5/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.5/LICENSE
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:40:51.024934 widget-picture-generator-0.0.5/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      912 2023-04-19 12:49:31.000000 widget-picture-generator-0.0.5/README.md
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:40:51.025098 widget-picture-generator-0.0.5/setup.cfg
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      826 2023-04-19 13:40:33.000000 widget-picture-generator-0.0.5/setup.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.023981 widget-picture-generator-0.0.5/widget_picture_generator/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     3500 2023-04-19 13:38:53.000000 widget-picture-generator-0.0.5/widget_picture_generator/__init__.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.024765 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      302 2023-04-19 13:40:51.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       27 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/requires.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       25 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/top_level.txt
```

### Comparing `widget-picture-generator-0.0.4/LICENSE` & `widget-picture-generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.4/PKG-INFO` & `widget-picture-generator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widget-picture-generator-0.0.4/README.md` & `widget-picture-generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.4/setup.py` & `widget-picture-generator-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="widget-picture-generator",
-    version="0.0.4",
+    version="0.0.5",
     author="Massimo Moffa",
     author_email="massimo.moffa@sensesquare.eu",
     description="This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sense-Square/widget-picture-generator",
     packages=setuptools.find_packages(),
     install_requires=[
-        'selenium'
+        'selenium',
+        'webdriver-manager'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `widget-picture-generator-0.0.4/widget_picture_generator/__init__.py` & `widget-picture-generator-0.0.5/widget_picture_generator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.chrome.service import Service as ChromeService
+from webdriver_manager.chrome import ChromeDriverManager
 from time import sleep
 import json
 
 #
 #   Widget Picture Generator
 #   - This library use the square dashboard to generate widget picture
 # 
 
 # This is the url used to load the widget export
 SQUARE_EXPORT_URL = "https://square.sensesquare.eu/export/widget/"
 
-class WidgetPictureGenerator:
+class widget_picture_generator:
         
     # Constructor
     def __init__(self, apikey, width=1280, height=720):
 
         # Prepare options for headless browser
         options = webdriver.ChromeOptions()
         options.add_argument("--headless")
 
         # Set apikey
         self._apikey = apikey
 
         # Setup driver
-        self._driver = webdriver.Chrome(options=options)
+        self._driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install(), options=options))
 
         # Set resolution
         self._driver.set_window_size(width, height)
 
     # Load widget and wait
     def _load_widget(self, id, state, theme="light", timeout=2):         
 
@@ -95,15 +97,15 @@
 
 
 
 # Main example
 if __name__ == "__main__": 
 
     # Init the generator (the constructor accept width and height)
-    wpg = WidgetPictureGenerator("U1OA1O4KL0B4")
+    wpg = widget_picture_generator("<APIKEY>")
 
     # Generate an example picture
     wpg.get_widget_picture_file("test.png", "widget_data_chart", {
         "device": {
             "key": 'ITCAMBAT134567',
             "value": 'ITCAMBAT134567'
         },
```

### Comparing `widget-picture-generator-0.0.4/widget_picture_generator.egg-info/PKG-INFO` & `widget-picture-generator-0.0.5/widget_picture_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

