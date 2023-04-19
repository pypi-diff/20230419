# Comparing `tmp/currensees-1.0.5.tar.gz` & `tmp/currensees-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.0.5.tar", last modified: Sun Apr 16 20:57:14 2023, max compression
+gzip compressed data, was "dist/currensees-1.0.6.tar", last modified: Wed Apr 19 18:12:16 2023, max compression
```

## Comparing `currensees-1.0.5.tar` & `currensees-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 20:57:14.585621 currensees-1.0.5/
--rw-r--r--   0 finn       (501) staff       (20)     5851 2023-04-16 20:57:14.585830 currensees-1.0.5/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2810 2023-04-16 20:55:06.000000 currensees-1.0.5/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 20:57:14.581761 currensees-1.0.5/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      163 2023-04-05 11:07:01.000000 currensees-1.0.5/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      584 2023-04-16 20:45:41.000000 currensees-1.0.5/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      781 2023-04-05 16:54:46.000000 currensees-1.0.5/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      671 2023-04-05 16:57:18.000000 currensees-1.0.5/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)      940 2023-04-16 20:46:25.000000 currensees-1.0.5/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      440 2023-04-16 20:49:54.000000 currensees-1.0.5/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1030 2023-04-05 17:02:43.000000 currensees-1.0.5/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 20:56:37.000000 currensees-1.0.5/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      518 2023-04-16 20:51:55.000000 currensees-1.0.5/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 20:57:14.585302 currensees-1.0.5/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5851 2023-04-16 20:57:14.000000 currensees-1.0.5/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      449 2023-04-16 20:57:14.000000 currensees-1.0.5/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 20:57:14.000000 currensees-1.0.5/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 20:57:00.000000 currensees-1.0.5/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 20:57:14.000000 currensees-1.0.5/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-16 20:57:14.000000 currensees-1.0.5/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 20:57:14.586452 currensees-1.0.5/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-16 20:56:37.000000 currensees-1.0.5/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.756792 currensees-1.0.6/
+-rw-r--r--   0 finn       (501) staff       (20)     6309 2023-04-19 18:12:16.757166 currensees-1.0.6/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3148 2023-04-19 18:03:57.000000 currensees-1.0.6/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.749677 currensees-1.0.6/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      163 2023-04-05 11:07:01.000000 currensees-1.0.6/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      584 2023-04-16 20:45:41.000000 currensees-1.0.6/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      781 2023-04-05 16:54:46.000000 currensees-1.0.6/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      671 2023-04-05 16:57:18.000000 currensees-1.0.6/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)      940 2023-04-19 17:49:11.000000 currensees-1.0.6/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      440 2023-04-19 18:04:01.000000 currensees-1.0.6/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1030 2023-04-05 17:02:43.000000 currensees-1.0.6/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1060 2023-04-19 18:04:05.000000 currensees-1.0.6/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-19 18:10:17.000000 currensees-1.0.6/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      518 2023-04-19 17:59:07.000000 currensees-1.0.6/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-19 18:12:16.755990 currensees-1.0.6/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     6309 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-19 18:12:00.000000 currensees-1.0.6/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-19 18:12:16.000000 currensees-1.0.6/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-19 18:12:16.758298 currensees-1.0.6/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-19 18:10:17.000000 currensees-1.0.6/setup.py
```

### Comparing `currensees-1.0.5/PKG-INFO` & `currensees-1.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -45,21 +45,15 @@
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            from currensees.auth import *
-            from currensees.convert import *
-            from currensees.convert_all import *
-            from currensees.currencies import *
-            from currensees.historical import *
-            from currensees.daily_average import *
-            from currensees.weekly_average import *
+            import currensees
         
             # Authenticate and log in
             username = '<username>'
             password = '<password>'
             auth = CurrenseesAuth(username, password)
             login_response = auth.login()
         
@@ -94,14 +88,31 @@
         
             # Retrieve weekly average of all the currencies
             date_from = "2023_04_03"
             date_to = "2023_04_07"
             weekly_average = WeeklyAverage(date_from, date_to)
             print(weekly_average.fetch_weekly_average())
         
+            # Initialize the MarginsSpreads class with a username and date
+            day = 19
+            month = 4
+            year = 2023
+            margins_spreads_instance = MarginsSpreads(username, day, month, year)
+        
+            # Fetch all margins and spreads data for the given user and date
+            all_margins_spreads = margins_spreads_instance.get_margins_spreads()
+            print("All Margins and Spreads:")
+            print(all_margins_spreads)
+        
+            # Fetch margin and spread data for a specific UUID
+            uuid = "data_uuid"
+            margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
+            print(f"Margin and Spread for UUID {uuid}:")
+            print(margin_spread)
+        
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
         
         .. _user account: https://moatsystems.com/currency-api/
```

### Comparing `currensees-1.0.5/README.md` & `currensees-1.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,15 @@
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 Usage Example
 -------------
 
 ```python
-from currensees.auth import *
-from currensees.convert import *
-from currensees.convert_all import *
-from currensees.currencies import *
-from currensees.historical import *
-from currensees.daily_average import *
-from currensees.weekly_average import *
+import currensees
 
 # Authenticate and log in
 username = '<username>'
 password = '<password>'
 auth = CurrenseesAuth(username, password)
 login_response = auth.login()
 
@@ -72,14 +66,31 @@
 print(daily_average.fetch_daily_average())
 
 # Retrieve weekly average of all the currencies
 date_from = "2023_04_03"
 date_to = "2023_04_07"
 weekly_average = WeeklyAverage(date_from, date_to)
 print(weekly_average.fetch_weekly_average())
+
+# Initialize the MarginsSpreads class with a username and date
+day = 19
+month = 4
+year = 2023
+margins_spreads_instance = MarginsSpreads(username, day, month, year)
+
+# Fetch all margins and spreads data for the given user and date
+all_margins_spreads = margins_spreads_instance.get_margins_spreads()
+print("All Margins and Spreads:")
+print(all_margins_spreads)
+
+# Fetch margin and spread data for a specific UUID
+uuid = "data_uuid"
+margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
+print(f"Margin and Spread for UUID {uuid}:")
+print(margin_spread)
 ```
 
 ## Setting up Currency API Account
 
 Subscribe here for a [user account](https://moatsystems.com/currency-api/).
```

### Comparing `currensees-1.0.5/currensees/auth.py` & `currensees-1.0.6/currensees/auth.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees/convert.py` & `currensees-1.0.6/currensees/convert.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees/convert_all.py` & `currensees-1.0.6/currensees/convert_all.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees/currencies.py` & `currensees-1.0.6/currensees/currencies.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees/historical.py` & `currensees-1.0.6/currensees/historical.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees/weekly_average.py` & `currensees-1.0.6/currensees/weekly_average.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.5/currensees.egg-info/PKG-INFO` & `currensees-1.0.6/currensees.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -45,21 +45,15 @@
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            from currensees.auth import *
-            from currensees.convert import *
-            from currensees.convert_all import *
-            from currensees.currencies import *
-            from currensees.historical import *
-            from currensees.daily_average import *
-            from currensees.weekly_average import *
+            import currensees
         
             # Authenticate and log in
             username = '<username>'
             password = '<password>'
             auth = CurrenseesAuth(username, password)
             login_response = auth.login()
         
@@ -94,14 +88,31 @@
         
             # Retrieve weekly average of all the currencies
             date_from = "2023_04_03"
             date_to = "2023_04_07"
             weekly_average = WeeklyAverage(date_from, date_to)
             print(weekly_average.fetch_weekly_average())
         
+            # Initialize the MarginsSpreads class with a username and date
+            day = 19
+            month = 4
+            year = 2023
+            margins_spreads_instance = MarginsSpreads(username, day, month, year)
+        
+            # Fetch all margins and spreads data for the given user and date
+            all_margins_spreads = margins_spreads_instance.get_margins_spreads()
+            print("All Margins and Spreads:")
+            print(all_margins_spreads)
+        
+            # Fetch margin and spread data for a specific UUID
+            uuid = "data_uuid"
+            margin_spread = margins_spreads_instance.get_margin_spread_by_uuid(uuid)
+            print(f"Margin and Spread for UUID {uuid}:")
+            print(margin_spread)
+        
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
         
         .. _user account: https://moatsystems.com/currency-api/
```

### Comparing `currensees-1.0.5/setup.py` & `currensees-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

