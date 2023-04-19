# Comparing `tmp/deprempy-0.0.2.tar.gz` & `tmp/deprempy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprempy-0.0.2.tar", last modified: Wed Apr 19 13:10:38 2023, max compression
+gzip compressed data, was "deprempy-0.0.3.tar", last modified: Wed Apr 19 13:11:50 2023, max compression
```

## Comparing `deprempy-0.0.2.tar` & `deprempy-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:10:38.840330 deprempy-0.0.2/
--rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-04-19 13:10:38.839256 deprempy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-04-19 13:10:17.000000 deprempy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:10:38.824790 deprempy-0.0.2/deprempy/
--rw-rw-rw-   0        0        0     3110 2023-04-19 12:36:52.000000 deprempy-0.0.2/deprempy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:10:38.837049 deprempy-0.0.2/deprempy.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-04-19 13:10:38.000000 deprempy-0.0.2/deprempy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-19 13:10:38.000000 deprempy-0.0.2/deprempy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:10:38.000000 deprempy-0.0.2/deprempy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 13:10:38.000000 deprempy-0.0.2/deprempy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 13:10:38.840330 deprempy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-04-19 13:10:32.000000 deprempy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:11:50.248933 deprempy-0.0.3/
+-rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-04-19 13:11:50.247920 deprempy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2540 2023-04-19 13:11:35.000000 deprempy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 13:11:50.234316 deprempy-0.0.3/deprempy/
+-rw-rw-rw-   0        0        0     3110 2023-04-19 12:36:52.000000 deprempy-0.0.3/deprempy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:11:50.245896 deprempy-0.0.3/deprempy.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-04-19 13:11:50.000000 deprempy-0.0.3/deprempy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-19 13:11:50.000000 deprempy-0.0.3/deprempy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:11:50.000000 deprempy-0.0.3/deprempy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 13:11:50.000000 deprempy-0.0.3/deprempy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:11:50.248933 deprempy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-04-19 13:11:45.000000 deprempy-0.0.3/setup.py
```

### Comparing `deprempy-0.0.2/LICENSE` & `deprempy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.2/PKG-INFO` & `deprempy-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.
 Home-page: https://gihtub.com/Meinos10/deprempy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: deprempy,deprempython,deprem,deprem-python,deprem-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: requests
 Requires: bs4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [sozlukpy](https://pypi.org/project/deprempy/)
+# [deprempy](https://pypi.org/project/deprempy/)
 
-Kandilli Rasathanesi aracÄ±lÄ±ÄŸÄ± ile elde edilen deprem sinyallerini kullanarak depremleri gÃ¶steren bir Python kÃ¼tÃ¼phanesidir.
+Kandilli Rasathanesi aracÄ±lÄ±ÄŸÄ± ile elde edilen deprem sinyallerini kullanarak depremleri gosteren bir Python kutuphanesidir.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install -U deprempy
```

### Comparing `deprempy-0.0.2/README.md` & `deprempy-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# [sozlukpy](https://pypi.org/project/deprempy/)
+# [deprempy](https://pypi.org/project/deprempy/)
 
-Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.
+Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gosteren bir Python kutuphanesidir.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install -U deprempy
```

### Comparing `deprempy-0.0.2/deprempy/__init__.py` & `deprempy-0.0.3/deprempy/__init__.py`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.2/deprempy.egg-info/PKG-INFO` & `deprempy-0.0.3/deprempy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.
 Home-page: https://gihtub.com/Meinos10/deprempy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: deprempy,deprempython,deprem,deprem-python,deprem-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: requests
 Requires: bs4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [sozlukpy](https://pypi.org/project/deprempy/)
+# [deprempy](https://pypi.org/project/deprempy/)
 
-Kandilli Rasathanesi aracÄ±lÄ±ÄŸÄ± ile elde edilen deprem sinyallerini kullanarak depremleri gÃ¶steren bir Python kÃ¼tÃ¼phanesidir.
+Kandilli Rasathanesi aracÄ±lÄ±ÄŸÄ± ile elde edilen deprem sinyallerini kullanarak depremleri gosteren bir Python kutuphanesidir.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install -U deprempy
```

### Comparing `deprempy-0.0.2/setup.py` & `deprempy-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deprempy",
-    version="0.0.2",
+    version="0.0.3",
     description="Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://gihtub.com/Meinos10/deprempy",
     author="Emre",
     author_email="E.tmen2023@gmail.com",
     license="MIT",
```

