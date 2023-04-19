# Comparing `tmp/codigofacilito_jorgef-0.0.1.tar.gz` & `tmp/codigofacilito_jorgef-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codigofacilito_jorgef-0.0.1.tar", last modified: Wed Apr 19 11:16:06 2023, max compression
+gzip compressed data, was "codigofacilito_jorgef-0.0.2.tar", last modified: Wed Apr 19 11:25:37 2023, max compression
```

## Comparing `codigofacilito_jorgef-0.0.1.tar` & `codigofacilito_jorgef-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:16:06.425611 codigofacilito_jorgef-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-04-18 15:56:29.000000 codigofacilito_jorgef-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      910 2023-04-19 11:16:06.425110 codigofacilito_jorgef-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-19 11:10:16.000000 codigofacilito_jorgef-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:16:06.412007 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef/
--rw-rw-rw-   0        0        0       56 2023-04-19 11:08:02.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef/__init__.py
--rw-rw-rw-   0        0        0      373 2023-04-19 11:08:02.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef/__main__.py
--rw-rw-rw-   0        0        0       14 2023-04-18 16:57:51.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef/config.py
--rw-rw-rw-   0        0        0      279 2023-04-18 17:05:56.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef/workshops.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:16:06.423154 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/
--rw-rw-rw-   0        0        0      910 2023-04-19 11:16:06.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-04-19 11:16:06.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:16:06.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 11:16:06.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-19 11:16:06.000000 codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 11:16:06.426317 codigofacilito_jorgef-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-04-19 11:08:02.000000 codigofacilito_jorgef-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:25:37.610028 codigofacilito_jorgef-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 15:56:29.000000 codigofacilito_jorgef-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1052 2023-04-19 11:25:37.610028 codigofacilito_jorgef-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-19 11:24:20.000000 codigofacilito_jorgef-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:25:37.597030 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef/
+-rw-rw-rw-   0        0        0       56 2023-04-19 11:08:02.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef/__init__.py
+-rw-rw-rw-   0        0        0      373 2023-04-19 11:08:02.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef/__main__.py
+-rw-rw-rw-   0        0        0       14 2023-04-18 16:57:51.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef/config.py
+-rw-rw-rw-   0        0        0      279 2023-04-18 17:05:56.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef/workshops.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:25:37.608029 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-04-19 11:25:37.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-04-19 11:25:37.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:25:37.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 11:25:37.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-19 11:25:37.000000 codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:25:37.611029 codigofacilito_jorgef-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-04-19 11:25:30.000000 codigofacilito_jorgef-0.0.2/setup.py
```

### Comparing `codigofacilito_jorgef-0.0.1/LICENSE.txt` & `codigofacilito_jorgef-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codigofacilito_jorgef-0.0.1/PKG-INFO` & `codigofacilito_jorgef-0.0.2/codigofacilito_jorgef.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: codigofacilito_jorgef
-Version: 0.0.1
+Name: codigofacilito-jorgef
+Version: 0.0.2
 Summary: este paquete de prueba, permite consumir el api de codigo facilito
 Home-page: https://github.com/JorgeFigueroa/codigofacilito_package
 Author: Jorge figueroa
 Author-email: atientas0412@gmail.com
 License: MIT
 Keywords: codigofacilito_jorgef
 Platform: UNKNOWN
@@ -12,24 +12,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+
 python -m venv .venv
 venv\Scripts\activate
 
 pip install requests
 pip freeze > requirements.txt
 
 ## provando un paquete
 python -m nome_paquete
 
 python setup.py sdist
-pip install pip --upgrade
+##pip install pip --upgrade  DA ERRORE
 pip install twine
 twine upload dist/*
 
 
+##TEST 
+pip install codigofacilito-jorgef==0.0.1
+python
+>>> from codigofacilito_jorgef import unreleased
+>>> unreleased()
```

### Comparing `codigofacilito_jorgef-0.0.1/codigofacilito_jorgef.egg-info/PKG-INFO` & `codigofacilito_jorgef-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: codigofacilito-jorgef
-Version: 0.0.1
+Name: codigofacilito_jorgef
+Version: 0.0.2
 Summary: este paquete de prueba, permite consumir el api de codigo facilito
 Home-page: https://github.com/JorgeFigueroa/codigofacilito_package
 Author: Jorge figueroa
 Author-email: atientas0412@gmail.com
 License: MIT
 Keywords: codigofacilito_jorgef
 Platform: UNKNOWN
@@ -12,24 +12,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+
 python -m venv .venv
 venv\Scripts\activate
 
 pip install requests
 pip freeze > requirements.txt
 
 ## provando un paquete
 python -m nome_paquete
 
 python setup.py sdist
-pip install pip --upgrade
+##pip install pip --upgrade  DA ERRORE
 pip install twine
 twine upload dist/*
 
 
+##TEST 
+pip install codigofacilito-jorgef==0.0.1
+python
+>>> from codigofacilito_jorgef import unreleased
+>>> unreleased()
```

### Comparing `codigofacilito_jorgef-0.0.1/setup.py` & `codigofacilito_jorgef-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path  # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'este paquete de prueba, permite consumir el api de codigo facilito'
 PACKAGE_NAME = 'codigofacilito_jorgef'
 AUTHOR = 'Jorge figueroa'
 EMAIL = 'atientas0412@gmail.com'
 GITHUB_URL = 'https://github.com/JorgeFigueroa/codigofacilito_package'
 
 setup(
```

