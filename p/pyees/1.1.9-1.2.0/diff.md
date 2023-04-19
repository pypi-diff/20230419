# Comparing `tmp/pyees-1.1.9.tar.gz` & `tmp/pyees-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.1.9.tar", last modified: Wed Apr 19 08:52:34 2023, max compression
+gzip compressed data, was "pyees-1.2.0.tar", last modified: Wed Apr 19 08:54:08 2023, max compression
```

## Comparing `pyees-1.1.9.tar` & `pyees-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 08:52:34.315971 pyees-1.1.9/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-04-19 08:52:34.321955 pyees-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 08:52:34.156312 pyees-1.1.9/pyees/
--rw-rw-rw-   0        0        0      641 2023-04-18 11:09:16.000000 pyees-1.1.9/pyees/__init__.py
--rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.9/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.9/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.9/pyees/prop.py
--rw-rw-rw-   0        0        0    14902 2023-04-19 08:51:38.000000 pyees-1.1.9/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.9/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.9/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.9/pyees/testFit.py
--rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.9/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-16 08:44:33.000000 pyees-1.1.9/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15043 2023-04-19 08:45:19.000000 pyees-1.1.9/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.9/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.1.9/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.9/pyees/testVariable.py
--rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.1.9/pyees/unit.py
--rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.9/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:52:34.297021 pyees-1.1.9/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-04-19 08:52:33.000000 pyees-1.1.9/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-19 08:52:33.000000 pyees-1.1.9/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 08:52:33.000000 pyees-1.1.9/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-19 08:52:33.000000 pyees-1.1.9/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 08:52:33.000000 pyees-1.1.9/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 08:52:34.346888 pyees-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-19 08:52:24.000000 pyees-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:54:08.715070 pyees-1.2.0/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-04-19 08:54:08.719038 pyees-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 08:54:08.579368 pyees-1.2.0/pyees/
+-rw-rw-rw-   0        0        0      641 2023-04-19 08:53:52.000000 pyees-1.2.0/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.2.0/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.0/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.2.0/pyees/prop.py
+-rw-rw-rw-   0        0        0    14902 2023-04-19 08:53:57.000000 pyees-1.2.0/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.2.0/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.0/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.2.0/pyees/testFit.py
+-rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.2.0/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-16 08:44:33.000000 pyees-1.2.0/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15043 2023-04-19 08:45:19.000000 pyees-1.2.0/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.0/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.0/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.2.0/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.0/pyees/unit.py
+-rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.2.0/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:54:08.698095 pyees-1.2.0/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-04-19 08:54:07.000000 pyees-1.2.0/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-19 08:54:08.000000 pyees-1.2.0/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 08:54:07.000000 pyees-1.2.0/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-19 08:54:07.000000 pyees-1.2.0/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 08:54:07.000000 pyees-1.2.0/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 08:54:08.742975 pyees-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-04-19 08:54:03.000000 pyees-1.2.0/setup.py
```

### Comparing `pyees-1.1.9/LICENSE.txt` & `pyees-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/PKG-INFO` & `pyees-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.9
+Version: 1.2.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.9/README.md` & `pyees-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/__init__.py` & `pyees-1.2.0/pyees/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # import the necessary modules
 from pyees.variable import variable
 from pyees.fit import dummy_fit, pol_fit, lin_fit, exp_fit, pow_fit, logistic_fit, logistic_100_fit
-from pyees.readData import SheetsFromFile, FileFromSheets
+from pyees.readData import sheetsFromFile, fileFromSheets
 from pyees.prop import prop
 from pyees.solve import solve
 from pyees.unit import addNewUnit
 
 
 ## TODO undersøg om man kan bruge evalueringer af funktioner til at bestemme uncertanty propagation - selv med produktreglen
 ## TODO fit - få det til at virke som i bogen
```

### Comparing `pyees-1.1.9/pyees/fit.py` & `pyees-1.2.0/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/profilePyees.py` & `pyees-1.2.0/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/prop.py` & `pyees-1.2.0/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/readData.py` & `pyees-1.2.0/pyees/readData.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import string
 try:
     from variable import variable
 except ImportError:
     from pyees.variable import variable
 
-def FileFromSheets(Sheets):
+def fileFromSheets(Sheets):
     ## TODO save Sheet as xlFile
     raise NotImplementedError()
 
 def sheetsFromFile(xlFile, dataRange: str | list[str], uncertRange: str | list[str] = None, sheets: int | list[int] = None):
     dat = _SheetsFromFile(xlFile, dataRange, uncertRange, sheets)
     if len(dat.dat) == 1:
         return dat.dat[0]
```

### Comparing `pyees-1.1.9/pyees/solve.py` & `pyees-1.2.0/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/stackOverflowODR.py` & `pyees-1.2.0/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testFit.py` & `pyees-1.2.0/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testProp.py` & `pyees-1.2.0/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testPyees.py` & `pyees-1.2.0/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testReadData.py` & `pyees-1.2.0/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testSolve.py` & `pyees-1.2.0/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testUnit.py` & `pyees-1.2.0/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/testVariable.py` & `pyees-1.2.0/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/unit.py` & `pyees-1.2.0/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees/variable.py` & `pyees-1.2.0/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.9/pyees.egg-info/PKG-INFO` & `pyees-1.2.0/pyees.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.9
+Version: 1.2.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.9/setup.py` & `pyees-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.1.9',
+    version='1.2.0',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

