# Comparing `tmp/lovematch-1.7.0.tar.gz` & `tmp/lovematch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lovematch-1.7.0.tar", last modified: Wed Apr 19 12:39:37 2023, max compression
+gzip compressed data, was "dist\lovematch-1.8.0.tar", last modified: Wed Apr 19 12:41:45 2023, max compression
```

## Comparing `lovematch-1.7.0.tar` & `lovematch-1.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:39:37.000000 lovematch-1.7.0/
--rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     1648 2023-04-19 12:39:37.000000 lovematch-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-04-19 12:31:26.000000 lovematch-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 12:39:37.000000 lovematch-1.7.0/lovematch/
--rw-rw-rw-   0        0        0      198 2023-04-19 12:15:32.000000 lovematch-1.7.0/lovematch/__init__.py
--rw-rw-rw-   0        0        0     1560 2023-04-19 12:15:38.000000 lovematch-1.7.0/lovematch/friendship.py
--rw-rw-rw-   0        0        0     3072 2023-04-19 12:15:33.000000 lovematch-1.7.0/lovematch/love.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:39:37.000000 lovematch-1.7.0/lovematch.egg-info/
--rw-rw-rw-   0        0        0     1648 2023-04-19 12:39:36.000000 lovematch-1.7.0/lovematch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-19 12:39:37.000000 lovematch-1.7.0/lovematch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:39:36.000000 lovematch-1.7.0/lovematch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 12:39:36.000000 lovematch-1.7.0/lovematch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 12:39:37.000000 lovematch-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1960 2023-04-19 12:36:19.000000 lovematch-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:41:45.000000 lovematch-1.8.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     1663 2023-04-19 12:41:45.000000 lovematch-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-04-19 12:31:26.000000 lovematch-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch/
+-rw-rw-rw-   0        0        0      198 2023-04-19 12:15:32.000000 lovematch-1.8.0/lovematch/__init__.py
+-rw-rw-rw-   0        0        0     1560 2023-04-19 12:15:38.000000 lovematch-1.8.0/lovematch/friendship.py
+-rw-rw-rw-   0        0        0     3072 2023-04-19 12:15:33.000000 lovematch-1.8.0/lovematch/love.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch.egg-info/
+-rw-rw-rw-   0        0        0     1663 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 12:41:45.000000 lovematch-1.8.0/lovematch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:41:45.000000 lovematch-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1975 2023-04-19 12:41:21.000000 lovematch-1.8.0/setup.py
```

### Comparing `lovematch-1.7.0/LICENSE` & `lovematch-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lovematch-1.7.0/PKG-INFO` & `lovematch-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.7.0
+Version: 1.8.0
 Summary: Realtion match percentage calculator
 Home-page: https://github.com/Devparihar5/lovematch
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: python,love,match,percentage,calculator,lovematch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -23,19 +23,22 @@
 
 ## Installation
 
 You can install `lovematch` using pip, the Python package manager:
 
 ```bash
 pip install lovematch
+```
+
 
 ## Usage
 ### You can use lovematch in your Python code as follows:
 
-```
+
+```python
 from lovematch.friendship import calculate_frindship_match_percentage
 from lovematch.love import calculate_love_match_percentage
 
 # Calculate friendship match percentage
 your_name = "Alice"
 friend_name = "Bob"
 friendship_percentage = calculate_frindship_match_percentage(your_name, friend_name)
```

### Comparing `lovematch-1.7.0/README.md` & `lovematch-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lovematch-1.7.0/lovematch/friendship.py` & `lovematch-1.8.0/lovematch/friendship.py`

 * *Files identical despite different names*

### Comparing `lovematch-1.7.0/lovematch/love.py` & `lovematch-1.8.0/lovematch/love.py`

 * *Files identical despite different names*

### Comparing `lovematch-1.7.0/lovematch.egg-info/PKG-INFO` & `lovematch-1.8.0/lovematch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lovematch
-Version: 1.7.0
+Version: 1.8.0
 Summary: Realtion match percentage calculator
 Home-page: https://github.com/Devparihar5/lovematch
 Author: Devendra Parihar
 Author-email: devendraparihar340@gmail.com
 Keywords: python,love,match,percentage,calculator,lovematch
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -23,19 +23,22 @@
 
 ## Installation
 
 You can install `lovematch` using pip, the Python package manager:
 
 ```bash
 pip install lovematch
+```
+
 
 ## Usage
 ### You can use lovematch in your Python code as follows:
 
-```
+
+```python
 from lovematch.friendship import calculate_frindship_match_percentage
 from lovematch.love import calculate_love_match_percentage
 
 # Calculate friendship match percentage
 your_name = "Alice"
 friend_name = "Bob"
 friendship_percentage = calculate_frindship_match_percentage(your_name, friend_name)
```

### Comparing `lovematch-1.7.0/setup.py` & `lovematch-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.7.0'
+VERSION = '1.8.0'
 DESCRIPTION = 'Realtion match percentage calculator'
 LONG_DESCRIPTION = '''
 
 # lovematch
 
 The `lovematch` library is a Python package that allows you to calculate friendship and love match percentages between given names.
 
 ## Installation
 
 You can install `lovematch` using pip, the Python package manager:
 
 ```bash
 pip install lovematch
+```
+
 
 ## Usage
 ### You can use lovematch in your Python code as follows:
 
-```
+
+```python
 from lovematch.friendship import calculate_frindship_match_percentage
 from lovematch.love import calculate_love_match_percentage
 
 # Calculate friendship match percentage
 your_name = "Alice"
 friend_name = "Bob"
 friendship_percentage = calculate_frindship_match_percentage(your_name, friend_name)
```

