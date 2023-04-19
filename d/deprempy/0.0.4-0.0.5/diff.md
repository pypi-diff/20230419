# Comparing `tmp/deprempy-0.0.4.tar.gz` & `tmp/deprempy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprempy-0.0.4.tar", last modified: Wed Apr 19 13:15:14 2023, max compression
+gzip compressed data, was "deprempy-0.0.5.tar", last modified: Wed Apr 19 14:40:53 2023, max compression
```

## Comparing `deprempy-0.0.4.tar` & `deprempy-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:15:14.759965 deprempy-0.0.4/
--rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3158 2023-04-19 13:15:14.758950 deprempy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2534 2023-04-19 13:15:00.000000 deprempy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:15:14.741471 deprempy-0.0.4/deprempy/
--rw-rw-rw-   0        0        0     3110 2023-04-19 12:36:52.000000 deprempy-0.0.4/deprempy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:15:14.755223 deprempy-0.0.4/deprempy.egg-info/
--rw-rw-rw-   0        0        0     3158 2023-04-19 13:15:14.000000 deprempy-0.0.4/deprempy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-19 13:15:14.000000 deprempy-0.0.4/deprempy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:15:14.000000 deprempy-0.0.4/deprempy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 13:15:14.000000 deprempy-0.0.4/deprempy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 13:15:14.759965 deprempy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-04-19 13:13:09.000000 deprempy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.859206 deprempy-0.0.5/
+-rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 deprempy-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3169 2023-04-19 14:40:53.858202 deprempy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2534 2023-04-19 13:15:00.000000 deprempy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.844455 deprempy-0.0.5/deprempy/
+-rw-rw-rw-   0        0        0     3110 2023-04-19 12:36:52.000000 deprempy-0.0.5/deprempy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:40:53.855902 deprempy-0.0.5/deprempy.egg-info/
+-rw-rw-rw-   0        0        0     3169 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 14:40:53.000000 deprempy-0.0.5/deprempy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:40:53.860522 deprempy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-04-19 14:40:01.000000 deprempy-0.0.5/setup.py
```

### Comparing `deprempy-0.0.4/LICENSE` & `deprempy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.4/PKG-INFO` & `deprempy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.4
+Version: 0.0.5
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
-Requires: bs4
+Requires: beautifulsoup4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [deprempy](https://pypi.org/project/deprempy/)
 
 Kandilli Rasathanesi araciligi ile elde edilen deprem sinyallerini kullanarak depremleri gosteren bir Python kutuphanesidir.
```

### Comparing `deprempy-0.0.4/README.md` & `deprempy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.4/deprempy/__init__.py` & `deprempy-0.0.5/deprempy/__init__.py`

 * *Files identical despite different names*

### Comparing `deprempy-0.0.4/deprempy.egg-info/PKG-INFO` & `deprempy-0.0.5/deprempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: deprempy
-Version: 0.0.4
+Version: 0.0.5
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
-Requires: bs4
+Requires: beautifulsoup4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [deprempy](https://pypi.org/project/deprempy/)
 
 Kandilli Rasathanesi araciligi ile elde edilen deprem sinyallerini kullanarak depremleri gosteren bir Python kutuphanesidir.
```

### Comparing `deprempy-0.0.4/setup.py` & `deprempy-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deprempy",
-    version="0.0.4",
+    version="0.0.5",
     description="Kandilli Rasathanesi aracılığı ile elde edilen deprem sinyallerini kullanarak depremleri gösteren bir Python kütüphanesidir.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://gihtub.com/Meinos10/deprempy",
     author="Emre",
     author_email="E.tmen2023@gmail.com",
     license="MIT",
     classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ],
     keywords=["deprempy","deprempython", "deprem", "deprem-python", "deprem-py"],
     packages=find_packages(),
-    requires=["requests", "bs4"]
+    requires=["requests", "beautifulsoup4"]
 )
```

