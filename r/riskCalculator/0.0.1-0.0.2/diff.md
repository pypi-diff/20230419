# Comparing `tmp/riskCalculator-0.0.1.tar.gz` & `tmp/riskCalculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riskCalculator-0.0.1.tar", last modified: Wed Apr 19 04:39:48 2023, max compression
+gzip compressed data, was "riskCalculator-0.0.2.tar", last modified: Wed Apr 19 04:46:15 2023, max compression
```

## Comparing `riskCalculator-0.0.1.tar` & `riskCalculator-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:39:48.608777 riskCalculator-0.0.1/
--rw-r--r--   0 angusleck   (501) staff       (20)    34523 2023-04-17 22:36:31.000000 riskCalculator-0.0.1/LICENSE
--rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-19 04:39:48.608656 riskCalculator-0.0.1/PKG-INFO
--rw-r--r--   0 angusleck   (501) staff       (20)      900 2023-04-19 04:36:20.000000 riskCalculator-0.0.1/README.md
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:39:48.608044 riskCalculator-0.0.1/riskCalculator/
--rw-r--r--   0 angusleck   (501) staff       (20)       37 2023-04-19 04:39:42.000000 riskCalculator-0.0.1/riskCalculator/__init__.py
--rw-r--r--   0 angusleck   (501) staff       (20)      363 2023-04-19 04:33:42.000000 riskCalculator-0.0.1/riskCalculator/expectedSurvivors.py
--rw-r--r--   0 angusleck   (501) staff       (20)      380 2023-04-19 04:33:42.000000 riskCalculator-0.0.1/riskCalculator/likelihoodOfVictory.py
--rw-r--r--   0 angusleck   (501) staff       (20)      793 2023-04-18 04:42:03.000000 riskCalculator-0.0.1/riskCalculator/parseArguments.py
--rw-r--r--   0 angusleck   (501) staff       (20)      718 2023-04-18 00:54:01.000000 riskCalculator-0.0.1/riskCalculator/probabilityOfLosses.py
--rw-r--r--   0 angusleck   (501) staff       (20)      871 2023-04-18 03:27:18.000000 riskCalculator-0.0.1/riskCalculator/readWriteData.py
--rw-r--r--   0 angusleck   (501) staff       (20)      937 2023-04-19 04:33:42.000000 riskCalculator-0.0.1/riskCalculator/recursiveMarkovChain.py
--rw-r--r--   0 angusleck   (501) staff       (20)     1396 2023-04-19 04:39:03.000000 riskCalculator-0.0.1/riskCalculator/risk.py
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:39:48.608478 riskCalculator-0.0.1/riskCalculator.egg-info/
--rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-19 04:39:48.000000 riskCalculator-0.0.1/riskCalculator.egg-info/PKG-INFO
--rw-r--r--   0 angusleck   (501) staff       (20)      444 2023-04-19 04:39:48.000000 riskCalculator-0.0.1/riskCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 angusleck   (501) staff       (20)        1 2023-04-19 04:39:48.000000 riskCalculator-0.0.1/riskCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 angusleck   (501) staff       (20)       15 2023-04-19 04:39:48.000000 riskCalculator-0.0.1/riskCalculator.egg-info/top_level.txt
--rw-r--r--   0 angusleck   (501) staff       (20)       38 2023-04-19 04:39:48.608823 riskCalculator-0.0.1/setup.cfg
--rw-r--r--   0 angusleck   (501) staff       (20)      947 2023-04-19 04:34:41.000000 riskCalculator-0.0.1/setup.py
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:46:15.574031 riskCalculator-0.0.2/
+-rw-r--r--   0 angusleck   (501) staff       (20)    34523 2023-04-17 22:36:31.000000 riskCalculator-0.0.2/LICENSE
+-rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-19 04:46:15.573892 riskCalculator-0.0.2/PKG-INFO
+-rw-r--r--   0 angusleck   (501) staff       (20)      900 2023-04-19 04:36:20.000000 riskCalculator-0.0.2/README.md
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:46:15.573127 riskCalculator-0.0.2/riskCalculator/
+-rw-r--r--   0 angusleck   (501) staff       (20)       37 2023-04-19 04:39:42.000000 riskCalculator-0.0.2/riskCalculator/__init__.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      363 2023-04-19 04:33:42.000000 riskCalculator-0.0.2/riskCalculator/expectedSurvivors.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      380 2023-04-19 04:33:42.000000 riskCalculator-0.0.2/riskCalculator/likelihoodOfVictory.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      955 2023-04-19 04:44:17.000000 riskCalculator-0.0.2/riskCalculator/parseArguments.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      718 2023-04-18 00:54:01.000000 riskCalculator-0.0.2/riskCalculator/probabilityOfLosses.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      871 2023-04-18 03:27:18.000000 riskCalculator-0.0.2/riskCalculator/readWriteData.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      937 2023-04-19 04:33:42.000000 riskCalculator-0.0.2/riskCalculator/recursiveMarkovChain.py
+-rw-r--r--   0 angusleck   (501) staff       (20)     1468 2023-04-19 04:44:12.000000 riskCalculator-0.0.2/riskCalculator/risk.py
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-19 04:46:15.573702 riskCalculator-0.0.2/riskCalculator.egg-info/
+-rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-19 04:46:15.000000 riskCalculator-0.0.2/riskCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 angusleck   (501) staff       (20)      444 2023-04-19 04:46:15.000000 riskCalculator-0.0.2/riskCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)        1 2023-04-19 04:46:15.000000 riskCalculator-0.0.2/riskCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)       15 2023-04-19 04:46:15.000000 riskCalculator-0.0.2/riskCalculator.egg-info/top_level.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)       38 2023-04-19 04:46:15.574080 riskCalculator-0.0.2/setup.cfg
+-rw-r--r--   0 angusleck   (501) staff       (20)      947 2023-04-19 04:44:41.000000 riskCalculator-0.0.2/setup.py
```

### Comparing `riskCalculator-0.0.1/LICENSE` & `riskCalculator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.1/PKG-INFO` & `riskCalculator-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskCalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python package for calculating expected outcome of a risk battle
 Author: Angus Leck
 Author-email: aleck42@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `riskCalculator-0.0.1/README.md` & `riskCalculator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.1/riskCalculator/parseArguments.py` & `riskCalculator-0.0.2/riskCalculator/parseArguments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from argparse import *
 
 
-def parseArguments():
+def parseArguments(defaultAttackers, defaultDefenders):
     parser = ArgumentParser(description="arguments for risk calculation")
-    parser.add_argument('attackers', type=int, help='number of attackers')
-    parser.add_argument('defenders', type=int, help='number of defenders')
+    parser.add_argument(
+        'attackers',
+        type=int,
+        help='number of attackers',
+        default=defaultAttackers
+    )
+    parser.add_argument(
+        'defenders',
+        type=int,
+        help='number of defenders',
+        default=defaultDefenders
+    )
     parser.add_argument(
         '--read',
         action=BooleanOptionalAction,
         dest="read",
         help="should use saved results"
     )
     parser.add_argument(
```

### Comparing `riskCalculator-0.0.1/riskCalculator/probabilityOfLosses.py` & `riskCalculator-0.0.2/riskCalculator/probabilityOfLosses.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.1/riskCalculator/readWriteData.py` & `riskCalculator-0.0.2/riskCalculator/readWriteData.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.1/riskCalculator/recursiveMarkovChain.py` & `riskCalculator-0.0.2/riskCalculator/recursiveMarkovChain.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.1/riskCalculator/risk.py` & `riskCalculator-0.0.2/riskCalculator/risk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 from riskCalculator.parseArguments import *
 from riskCalculator.readWriteData import *
 from riskCalculator.likelihoodOfVictory import *
 from riskCalculator.expectedSurvivors import *
 
 
-def risk():
-    args = parseArguments()
+def risk(defaultAttackers=0, defaultDefenders=0):
+    args = parseArguments(defaultAttackers, defaultDefenders)
     attackers = args.attackers
     defenders = args.defenders
 
     # initialise variables
     maxDice = max(attackers, defenders, 200 if args.write else 1)
     expectedSurvivorsArray = [[None]*maxDice for x in range(maxDice)]
     likelihoodOfVictoryArray = [[None]*maxDice for x in range(maxDice)]
```

### Comparing `riskCalculator-0.0.1/riskCalculator.egg-info/PKG-INFO` & `riskCalculator-0.0.2/riskCalculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskCalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple python package for calculating expected outcome of a risk battle
 Author: Angus Leck
 Author-email: aleck42@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `riskCalculator-0.0.1/setup.py` & `riskCalculator-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Simple python package for calculating expected outcome of a risk battle'
 LONG_DESCRIPTION = 'Simple python package for calculating expected outcome of a risk battle'
 
 # Setting up
 setup(
     name="riskCalculator",
     version=VERSION,
```

