# Comparing `tmp/widget-picture-generator-0.0.5.tar.gz` & `tmp/widget-picture-generator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widget-picture-generator-0.0.5.tar", last modified: Wed Apr 19 13:40:51 2023, max compression
+gzip compressed data, was "widget-picture-generator-0.0.6.tar", last modified: Wed Apr 19 13:53:03 2023, max compression
```

## Comparing `widget-picture-generator-0.0.5.tar` & `widget-picture-generator-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.025050 widget-picture-generator-0.0.5/
--rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.5/LICENSE
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:40:51.024934 widget-picture-generator-0.0.5/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      912 2023-04-19 12:49:31.000000 widget-picture-generator-0.0.5/README.md
--rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:40:51.025098 widget-picture-generator-0.0.5/setup.cfg
--rw-r--r--   0 maxmoffa   (502) staff       (20)      826 2023-04-19 13:40:33.000000 widget-picture-generator-0.0.5/setup.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.023981 widget-picture-generator-0.0.5/widget_picture_generator/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     3500 2023-04-19 13:38:53.000000 widget-picture-generator-0.0.5/widget_picture_generator/__init__.py
-drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:40:51.024765 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/
--rw-r--r--   0 maxmoffa   (502) staff       (20)     1451 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/PKG-INFO
--rw-r--r--   0 maxmoffa   (502) staff       (20)      302 2023-04-19 13:40:51.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/SOURCES.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/dependency_links.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)       27 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/requires.txt
--rw-r--r--   0 maxmoffa   (502) staff       (20)       25 2023-04-19 13:40:50.000000 widget-picture-generator-0.0.5/widget_picture_generator.egg-info/top_level.txt
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:53:03.988895 widget-picture-generator-0.0.6/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)    35149 2023-04-19 12:59:55.000000 widget-picture-generator-0.0.6/LICENSE
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1962 2023-04-19 13:53:03.988774 widget-picture-generator-0.0.6/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1423 2023-04-19 13:52:45.000000 widget-picture-generator-0.0.6/README.md
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       38 2023-04-19 13:53:03.988939 widget-picture-generator-0.0.6/setup.cfg
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      797 2023-04-19 13:50:08.000000 widget-picture-generator-0.0.6/setup.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:53:03.987774 widget-picture-generator-0.0.6/widget_picture_generator/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     3316 2023-04-19 13:49:57.000000 widget-picture-generator-0.0.6/widget_picture_generator/__init__.py
+drwxr-xr-x   0 maxmoffa   (502) staff       (20)        0 2023-04-19 13:53:03.988607 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/
+-rw-r--r--   0 maxmoffa   (502) staff       (20)     1962 2023-04-19 13:53:03.000000 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/PKG-INFO
+-rw-r--r--   0 maxmoffa   (502) staff       (20)      302 2023-04-19 13:53:03.000000 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)        1 2023-04-19 13:53:03.000000 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)        9 2023-04-19 13:53:03.000000 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/requires.txt
+-rw-r--r--   0 maxmoffa   (502) staff       (20)       25 2023-04-19 13:53:03.000000 widget-picture-generator-0.0.6/widget_picture_generator.egg-info/top_level.txt
```

### Comparing `widget-picture-generator-0.0.5/LICENSE` & `widget-picture-generator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `widget-picture-generator-0.0.5/PKG-INFO` & `widget-picture-generator-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,14 @@
 ### Introduction
 The Python library WidgetPictureGenerator has been designed to generate widget images quickly and easily. This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards.
 
 The WidgetPictureGenerator Python library supports a wide range of widgets, giving users the ability to select the desired type of widget and customize it to create an image that meets their needs. WidgetPictureGenerator is easy to use and comes with detailed documentation and numerous code examples to help users get started creating high-quality widget images.
 
 ### Based on Selenium
 The WidgetPictureGenerator library uses the web automation framework Selenium to create widget images. Selenium is a widely used framework for web script automation and allows users to simulate user interaction with a web page.
+
+### Selenium installation
+Selenium requires a driver to interface with the chosen browser. Chrome, for example, requires chromedriver, which needs to be installed before the below examples can be run. Make sure it’s in your PATH, e. g., place it in /usr/bin or /usr/local/bin.
+
+Failure to observe this step will give you an error selenium.common.exceptions.WebDriverException: Message: ‘chromedriver’ executable needs to be in PATH.
+
+Chrome Drive Interface:	https://sites.google.com/chromium.org/driver/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `widget-picture-generator-0.0.5/README.md` & `widget-picture-generator-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,8 +3,15 @@
 
 ### Introduction
 The Python library WidgetPictureGenerator has been designed to generate widget images quickly and easily. This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards.
 
 The WidgetPictureGenerator Python library supports a wide range of widgets, giving users the ability to select the desired type of widget and customize it to create an image that meets their needs. WidgetPictureGenerator is easy to use and comes with detailed documentation and numerous code examples to help users get started creating high-quality widget images.
 
 ### Based on Selenium
-The WidgetPictureGenerator library uses the web automation framework Selenium to create widget images. Selenium is a widely used framework for web script automation and allows users to simulate user interaction with a web page.
+The WidgetPictureGenerator library uses the web automation framework Selenium to create widget images. Selenium is a widely used framework for web script automation and allows users to simulate user interaction with a web page.
+
+### Selenium installation
+Selenium requires a driver to interface with the chosen browser. Chrome, for example, requires chromedriver, which needs to be installed before the below examples can be run. Make sure it’s in your PATH, e. g., place it in /usr/bin or /usr/local/bin.
+
+Failure to observe this step will give you an error selenium.common.exceptions.WebDriverException: Message: ‘chromedriver’ executable needs to be in PATH.
+
+Chrome Drive Interface:	https://sites.google.com/chromium.org/driver/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `widget-picture-generator-0.0.5/setup.py` & `widget-picture-generator-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="widget-picture-generator",
-    version="0.0.5",
+    version="0.0.6",
     author="Massimo Moffa",
     author_email="massimo.moffa@sensesquare.eu",
     description="This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sense-Square/widget-picture-generator",
     packages=setuptools.find_packages(),
     install_requires=[
-        'selenium',
-        'webdriver-manager'
+        'selenium'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `widget-picture-generator-0.0.5/widget_picture_generator/__init__.py` & `widget-picture-generator-0.0.6/widget_picture_generator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.chrome.service import Service as ChromeService
-from webdriver_manager.chrome import ChromeDriverManager
 from time import sleep
 import json
 
 #
 #   Widget Picture Generator
 #   - This library use the square dashboard to generate widget picture
 # 
@@ -25,15 +23,15 @@
         options = webdriver.ChromeOptions()
         options.add_argument("--headless")
 
         # Set apikey
         self._apikey = apikey
 
         # Setup driver
-        self._driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install(), options=options))
+        self._driver = webdriver.Chrome(options=options)
 
         # Set resolution
         self._driver.set_window_size(width, height)
 
     # Load widget and wait
     def _load_widget(self, id, state, theme="light", timeout=2):
```

### Comparing `widget-picture-generator-0.0.5/widget_picture_generator.egg-info/PKG-INFO` & `widget-picture-generator-0.0.6/widget_picture_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widget-picture-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards
 Home-page: https://github.com/Sense-Square/widget-picture-generator
 Author: Massimo Moffa
 Author-email: massimo.moffa@sensesquare.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,14 @@
 ### Introduction
 The Python library WidgetPictureGenerator has been designed to generate widget images quickly and easily. This library can be used to generate high-quality images of any type of widget, such as charts, maps, and leaderboards.
 
 The WidgetPictureGenerator Python library supports a wide range of widgets, giving users the ability to select the desired type of widget and customize it to create an image that meets their needs. WidgetPictureGenerator is easy to use and comes with detailed documentation and numerous code examples to help users get started creating high-quality widget images.
 
 ### Based on Selenium
 The WidgetPictureGenerator library uses the web automation framework Selenium to create widget images. Selenium is a widely used framework for web script automation and allows users to simulate user interaction with a web page.
+
+### Selenium installation
+Selenium requires a driver to interface with the chosen browser. Chrome, for example, requires chromedriver, which needs to be installed before the below examples can be run. Make sure it’s in your PATH, e. g., place it in /usr/bin or /usr/local/bin.
+
+Failure to observe this step will give you an error selenium.common.exceptions.WebDriverException: Message: ‘chromedriver’ executable needs to be in PATH.
+
+Chrome Drive Interface:	https://sites.google.com/chromium.org/driver/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

