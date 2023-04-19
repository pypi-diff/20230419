# Comparing `tmp/maskcovid-0.0.1.tar.gz` & `tmp/maskcovid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maskcovid-0.0.1.tar", last modified: Mon Apr  3 14:27:24 2023, max compression
+gzip compressed data, was "maskcovid-0.0.2.tar", last modified: Wed Apr 19 14:20:18 2023, max compression
```

## Comparing `maskcovid-0.0.1.tar` & `maskcovid-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-03 14:27:24.272187 maskcovid-0.0.1/
--rw-rw-r--   0 inoseizuru   (501) staff       (20)     1068 2023-04-03 14:18:51.000000 maskcovid-0.0.1/LICENSE
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1739 2023-04-03 14:27:24.272043 maskcovid-0.0.1/PKG-INFO
--rw-rw-r--   0 inoseizuru   (501) staff       (20)     1090 2023-04-03 14:18:51.000000 maskcovid-0.0.1/README.md
--rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-04-03 14:27:24.272236 maskcovid-0.0.1/setup.cfg
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1069 2023-04-03 14:24:47.000000 maskcovid-0.0.1/setup.py
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-03 14:27:24.271100 maskcovid-0.0.1/src/
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-03 14:27:24.271829 maskcovid-0.0.1/src/maskcovid.egg-info/
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1739 2023-04-03 14:27:24.000000 maskcovid-0.0.1/src/maskcovid.egg-info/PKG-INFO
--rw-r--r--   0 inoseizuru   (501) staff       (20)      231 2023-04-03 14:27:24.000000 maskcovid-0.0.1/src/maskcovid.egg-info/SOURCES.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-04-03 14:27:24.000000 maskcovid-0.0.1/src/maskcovid.egg-info/dependency_links.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)       45 2023-04-03 14:27:24.000000 maskcovid-0.0.1/src/maskcovid.egg-info/entry_points.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)       10 2023-04-03 14:27:24.000000 maskcovid-0.0.1/src/maskcovid.egg-info/top_level.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)      809 2023-04-03 14:15:50.000000 maskcovid-0.0.1/src/maskcovid.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-19 14:20:18.444769 maskcovid-0.0.2/
+-rw-rw-r--   0 inoseizuru   (501) staff       (20)     1068 2023-04-03 14:18:51.000000 maskcovid-0.0.2/LICENSE
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1739 2023-04-19 14:20:18.444603 maskcovid-0.0.2/PKG-INFO
+-rw-rw-r--   0 inoseizuru   (501) staff       (20)     1090 2023-04-03 14:18:51.000000 maskcovid-0.0.2/README.md
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-04-19 14:20:18.444821 maskcovid-0.0.2/setup.cfg
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1069 2023-04-19 14:18:10.000000 maskcovid-0.0.2/setup.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-19 14:20:18.443560 maskcovid-0.0.2/src/
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-04-19 14:20:18.444385 maskcovid-0.0.2/src/maskcovid.egg-info/
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1739 2023-04-19 14:20:18.000000 maskcovid-0.0.2/src/maskcovid.egg-info/PKG-INFO
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      231 2023-04-19 14:20:18.000000 maskcovid-0.0.2/src/maskcovid.egg-info/SOURCES.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-04-19 14:20:18.000000 maskcovid-0.0.2/src/maskcovid.egg-info/dependency_links.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       45 2023-04-19 14:20:18.000000 maskcovid-0.0.2/src/maskcovid.egg-info/entry_points.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       10 2023-04-19 14:20:18.000000 maskcovid-0.0.2/src/maskcovid.egg-info/top_level.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      921 2023-04-19 14:17:00.000000 maskcovid-0.0.2/src/maskcovid.py
```

### Comparing `maskcovid-0.0.1/LICENSE` & `maskcovid-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maskcovid-0.0.1/PKG-INFO` & `maskcovid-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskcovid
-Version: 0.0.1
+Version: 0.0.2
 Summary: maskcovid is a PyPI tool that predicts the number of people infected by day and up to one month from the date Japan began its liberal mask-wearing policy in the current Covid-19 epidemic.
 Home-page: https://github.com/i-inose/maskcovid
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/maskcovid
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maskcovid-0.0.1/README.md` & `maskcovid-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `maskcovid-0.0.1/setup.py` & `maskcovid-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="maskcovid",
-    version="0.0.1",
+    version="0.0.2",
     author="Izuru Inose",
     author_email="i.inose0304@gmail.com",
     description="maskcovid is a PyPI tool that predicts the number of people infected by day and up to one month from the date Japan began its liberal mask-wearing policy in the current Covid-19 epidemic.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/i-inose/maskcovid",
     project_urls={
```

### Comparing `maskcovid-0.0.1/src/maskcovid.egg-info/PKG-INFO` & `maskcovid-0.0.2/src/maskcovid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskcovid
-Version: 0.0.1
+Version: 0.0.2
 Summary: maskcovid is a PyPI tool that predicts the number of people infected by day and up to one month from the date Japan began its liberal mask-wearing policy in the current Covid-19 epidemic.
 Home-page: https://github.com/i-inose/maskcovid
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/maskcovid
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maskcovid-0.0.1/src/maskcovid.py` & `maskcovid-0.0.2/src/maskcovid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import os
 import pandas as pd
 import subprocess as sp
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
 from datetime import datetime
 from pmdarima.arima import auto_arima
 
-sp.call("wget -nc https://covid19.mhlw.go.jp/public/opendata/newly_confirmed_cases_daily.csv", shell = True)
+if not os.path.exists("newly_confirmed_cases_daily.csv"):
+    sp.call("wget https://covid19.mhlw.go.jp/public/opendata/newly_confirmed_cases_daily.csv", shell=True)
 
 df = pd.read_csv("newly_confirmed_cases_daily.csv")
 df = df[['Date', 'ALL']]
 df['Date'] = pd.to_datetime(df['Date'])
 df = df.set_index('Date')
 df = df.iloc[1152:, :]
 
@@ -21,8 +23,10 @@
 
 plt.plot(df, label='Result')
 plt.plot(pd.date_range(start=df.index[-1], periods=30, freq='D'), pred, label='Prediction')
 plt.ylabel('Number of infected [daily]')
 plt.xlabel('Date')
 plt.grid()
 plt.legend()
-plt.show()
+plt.show()
+
+os.remove("newly_confirmed_cases_daily.csv")
```

