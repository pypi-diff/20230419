# Comparing `tmp/vtmmpy-1.0.2.tar.gz` & `tmp/vtmmpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.2.tar", last modified: Wed Apr 19 13:12:14 2023, max compression
+gzip compressed data, was "vtmmpy-1.0.3.tar", last modified: Wed Apr 19 13:22:49 2023, max compression
```

## Comparing `vtmmpy-1.0.2.tar` & `vtmmpy-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/
--rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.2/LICENSE
--rw-rw-r--   0 tony      (1000) tony      (1000)     3933 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     3458 2023-04-18 14:37:28.000000 vtmmpy-1.0.2/README.md
--rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.2/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/setup.cfg
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.446843 vtmmpy-1.0.2/src/
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/src/vtmmpy/
--rw-r--r--   0 tony      (1000) tony      (1000)     8279 2023-04-18 14:04:08.000000 vtmmpy-1.0.2/src/vtmmpy/__init__.py
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:12:14.450843 vtmmpy-1.0.2/src/vtmmpy.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3933 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-19 13:12:14.000000 vtmmpy-1.0.2/src/vtmmpy.egg-info/top_level.txt
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/
+-rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.3/LICENSE
+-rw-rw-r--   0 tony      (1000) tony      (1000)     3693 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     3218 2023-04-19 13:22:05.000000 vtmmpy-1.0.3/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.3/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/setup.cfg
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/vtmmpy/
+-rw-r--r--   0 tony      (1000) tony      (1000)     8279 2023-04-18 14:04:08.000000 vtmmpy-1.0.3/src/vtmmpy/__init__.py
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-19 13:22:49.339610 vtmmpy-1.0.3/src/vtmmpy.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3693 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-19 13:22:49.000000 vtmmpy-1.0.3/src/vtmmpy.egg-info/top_level.txt
```

### Comparing `vtmmpy-1.0.2/LICENSE` & `vtmmpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.2/PKG-INFO` & `vtmmpy-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **Vectorized Transfer Matrix Method Python** 
 The transfer matrix method (TMM) is an analytic approach for obtaining the reflection and transmission coefficients in stratified media. vtmmpy is a vectorised implementation of the TMM written in Python. It has a focus on speed and ease of use. 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/MTM.png) 
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/MTM.png?raw=true) 
 
 ### **Installation**
 
 ---
 
 ```
 pip install vtmmpy 
@@ -64,17 +64,15 @@
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
-Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown in refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
-
-Under cirtain circumstances, it may also be necessary to change the "shelf" (see [refractiveindex.info](https://refractiveindex.info/) for details). By default the "main" shelf is used. This attribute can be changed as follows: ```tmm.shelf = <shelf>```.
+Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown on refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
 
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
@@ -95,8 +93,8 @@
 
 ### **Examples**
 
 --- 
 
 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/2dplots.png)
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/2dplots.png?raw=true)
```

### Comparing `vtmmpy-1.0.2/README.md` & `vtmmpy-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # **Vectorized Transfer Matrix Method Python** 
 The transfer matrix method (TMM) is an analytic approach for obtaining the reflection and transmission coefficients in stratified media. vtmmpy is a vectorised implementation of the TMM written in Python. It has a focus on speed and ease of use. 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/MTM.png) 
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/MTM.png?raw=true) 
 
 ### **Installation**
 
 ---
 
 ```
 pip install vtmmpy 
@@ -50,17 +50,15 @@
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
-Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown in refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
-
-Under cirtain circumstances, it may also be necessary to change the "shelf" (see [refractiveindex.info](https://refractiveindex.info/) for details). By default the "main" shelf is used. This attribute can be changed as follows: ```tmm.shelf = <shelf>```.
+Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown on refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
 
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
@@ -81,8 +79,8 @@
 
 ### **Examples**
 
 --- 
 
 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/2dplots.png)
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/2dplots.png?raw=true)
```

### Comparing `vtmmpy-1.0.2/setup.cfg` & `vtmmpy-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtmmpy
-version = 1.0.2
+version = 1.0.3
 author = Tony
 author_email = tk_87@hotmail.com
 description = A vectorized implementation of the transfer matrix method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AI-Tony/vtmmpy/tree/main
 project_urls =
```

### Comparing `vtmmpy-1.0.2/src/vtmmpy/__init__.py` & `vtmmpy-1.0.3/src/vtmmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.2/src/vtmmpy.egg-info/PKG-INFO` & `vtmmpy-1.0.3/src/vtmmpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **Vectorized Transfer Matrix Method Python** 
 The transfer matrix method (TMM) is an analytic approach for obtaining the reflection and transmission coefficients in stratified media. vtmmpy is a vectorised implementation of the TMM written in Python. It has a focus on speed and ease of use. 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/MTM.png) 
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/MTM.png?raw=true) 
 
 ### **Installation**
 
 ---
 
 ```
 pip install vtmmpy 
@@ -64,17 +64,15 @@
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
-Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown in refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
-
-Under cirtain circumstances, it may also be necessary to change the "shelf" (see [refractiveindex.info](https://refractiveindex.info/) for details). By default the "main" shelf is used. This attribute can be changed as follows: ```tmm.shelf = <shelf>```.
+Internally, vtmmpy uses the [regidx](https://gitlab.com/benvial/refidx) Python package to download refractive index data from [refractiveindex.info](https://refractiveindex.info/) for your choosen materials and spectral range. At this point, you will be presented with a few options corresponding to the data source ("Page" dropdown on refractiveindex.info). Study these carefully and refer to [refractiveindex.info](https://refractiveindex.info/) for more detailed information about how the data were obtained. Your choice here could greatly impact the accuracy of your results.
 
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
@@ -95,8 +93,8 @@
 
 ### **Examples**
 
 --- 
 
 
 
-![](https://github.com/AI-Tony/vtmmpy/raw/master/images/2dplots.png)
+![](https://github.com/AI-Tony/vtmmpy/blob/main/images/2dplots.png?raw=true)
```

