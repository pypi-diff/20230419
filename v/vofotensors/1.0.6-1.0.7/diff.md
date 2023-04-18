# Comparing `tmp/vofotensors-1.0.6.tar.gz` & `tmp/vofotensors-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vofotensors-1.0.6.tar", last modified: Sun Mar  5 17:16:21 2023, max compression
+gzip compressed data, was "vofotensors-1.0.7.tar", last modified: Tue Apr 18 23:37:35 2023, max compression
```

## Comparing `vofotensors-1.0.6.tar` & `vofotensors-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-05 17:16:21.240358 vofotensors-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-05 17:16:18.000000 vofotensors-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-03-05 17:16:21.240358 vofotensors-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-03-05 17:16:18.000000 vofotensors-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-05 17:16:21.240358 vofotensors-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-03-05 17:16:18.000000 vofotensors-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-05 17:16:21.232358 vofotensors-1.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-03-05 17:16:18.000000 vofotensors-1.0.6/test/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-05 17:16:21.236358 vofotensors-1.0.6/vofotensors/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/abc.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/basic_tensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/deviators_2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/deviators_4.py
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/fabric_tensors.py
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/notation.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/substitutions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-03-05 17:16:18.000000 vofotensors-1.0.6/vofotensors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-05 17:16:21.236358 vofotensors-1.0.6/vofotensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-03-05 17:16:21.000000 vofotensors-1.0.6/vofotensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-03-05 17:16:21.000000 vofotensors-1.0.6/vofotensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-05 17:16:21.000000 vofotensors-1.0.6/vofotensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-05 17:16:21.000000 vofotensors-1.0.6/vofotensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-05 17:16:21.000000 vofotensors-1.0.6/vofotensors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 23:37:35.365788 vofotensors-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-18 23:37:29.000000 vofotensors-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-04-18 23:37:35.365788 vofotensors-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-04-18 23:37:29.000000 vofotensors-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 23:37:35.365788 vofotensors-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-04-18 23:37:29.000000 vofotensors-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 23:37:35.365788 vofotensors-1.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-04-18 23:37:29.000000 vofotensors-1.0.7/test/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 23:37:35.365788 vofotensors-1.0.7/vofotensors/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/abc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/basic_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/deviators_2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/deviators_4.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/fabric_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/notation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-18 23:37:29.000000 vofotensors-1.0.7/vofotensors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 23:37:35.365788 vofotensors-1.0.7/vofotensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-04-18 23:37:35.000000 vofotensors-1.0.7/vofotensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-04-18 23:37:35.000000 vofotensors-1.0.7/vofotensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 23:37:35.000000 vofotensors-1.0.7/vofotensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-18 23:37:35.000000 vofotensors-1.0.7/vofotensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-18 23:37:35.000000 vofotensors-1.0.7/vofotensors.egg-info/top_level.txt
```

### Comparing `vofotensors-1.0.6/LICENSE` & `vofotensors-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/PKG-INFO` & `vofotensors-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vofotensors
-Version: 1.0.6
+Version: 1.0.7
 Summary: V(ariety)O(f)F(iber)O(rientation)TENSORS contains selected contributions of Bauer JK, Böhlke T. Variety of fiber orientation tensors. Mathematics and Mechanics of Solids. 2022. doi:10.1177/10812865211057602
 Home-page: https://github.com/JulianKarlBauer/vofotensors
 Author: Julian Karl Bauer
 Author-email: juliankarlbauer@gmx.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vofotensors Version: 1.0.6 Summary: V(ariety)O(f)F
+Metadata-Version: 2.1 Name: vofotensors Version: 1.0.7 Summary: V(ariety)O(f)F
 (iber)O(rientation)TENSORS contains selected contributions of Bauer JK, BÃ¶hlke
 T. Variety of fiber orientation tensors. Mathematics and Mechanics of Solids.
 2022. doi:10.1177/10812865211057602 Home-page: https://github.com/
 JulianKarlBauer/vofotensors Author: Julian Karl Bauer Author-email:
 juliankarlbauer@gmx.de Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE [![PyPI version](https://badge.fury.io/py/
```

### Comparing `vofotensors-1.0.6/README.md` & `vofotensors-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/setup.py` & `vofotensors-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vofotensors",
-    version="1.0.6",
+    version="1.0.7",
     author="Julian Karl Bauer",
     author_email="juliankarlbauer@gmx.de",
     description="V(ariety)O(f)F(iber)O(rientation)TENSORS "
     "contains selected contributions of "
     "Bauer JK, Böhlke T. Variety of fiber orientation tensors. "
     "Mathematics and Mechanics of Solids. 2022. "
     "doi:10.1177/10812865211057602",
```

### Comparing `vofotensors-1.0.6/test/test_scripts.py` & `vofotensors-1.0.7/test/test_scripts.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors/deviators_2.py` & `vofotensors-1.0.7/vofotensors/deviators_2.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors/deviators_4.py` & `vofotensors-1.0.7/vofotensors/deviators_4.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors/fabric_tensors.py` & `vofotensors-1.0.7/vofotensors/fabric_tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,18 @@
         },
     },
     "triclinic": {
         "la1_la2_d1_d2_d3_d4_d5_d6_d7_d8_d9": {
             "D2": dev2s.dev2_by_la1_la2(),
             "D4": dev4s.dev4_triclinic_by_d(),
         },
+        "alpha1_alpha3_d1_d2_d3_d4_d5_d6_d7_d8_d9": {
+            "D2": dev2s.dev2_by_alpha1_alpha3(),
+            "D4": dev4s.dev4_triclinic_by_d(),
+        },
     },
 }
 
 N4s_parametric = {
     key: {
         key_sub: vofotensors.utils.combine_to_N4(**val_sub)
         for key_sub, val_sub in val.items()
```

### Comparing `vofotensors-1.0.6/vofotensors/notation.py` & `vofotensors-1.0.7/vofotensors/notation.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors/substitutions.py` & `vofotensors-1.0.7/vofotensors/substitutions.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors/utils.py` & `vofotensors-1.0.7/vofotensors/utils.py`

 * *Files identical despite different names*

### Comparing `vofotensors-1.0.6/vofotensors.egg-info/PKG-INFO` & `vofotensors-1.0.7/vofotensors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vofotensors
-Version: 1.0.6
+Version: 1.0.7
 Summary: V(ariety)O(f)F(iber)O(rientation)TENSORS contains selected contributions of Bauer JK, Böhlke T. Variety of fiber orientation tensors. Mathematics and Mechanics of Solids. 2022. doi:10.1177/10812865211057602
 Home-page: https://github.com/JulianKarlBauer/vofotensors
 Author: Julian Karl Bauer
 Author-email: juliankarlbauer@gmx.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vofotensors Version: 1.0.6 Summary: V(ariety)O(f)F
+Metadata-Version: 2.1 Name: vofotensors Version: 1.0.7 Summary: V(ariety)O(f)F
 (iber)O(rientation)TENSORS contains selected contributions of Bauer JK, BÃ¶hlke
 T. Variety of fiber orientation tensors. Mathematics and Mechanics of Solids.
 2022. doi:10.1177/10812865211057602 Home-page: https://github.com/
 JulianKarlBauer/vofotensors Author: Julian Karl Bauer Author-email:
 juliankarlbauer@gmx.de Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE [![PyPI version](https://badge.fury.io/py/
```

