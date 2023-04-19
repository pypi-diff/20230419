# Comparing `tmp/pyfomo-0.0.8.tar.gz` & `tmp/pyfomo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfomo-0.0.8.tar", last modified: Tue Feb 28 21:51:35 2023, max compression
+gzip compressed data, was "pyfomo-0.0.9.tar", last modified: Tue Feb 28 21:55:39 2023, max compression
```

## Comparing `pyfomo-0.0.8.tar` & `pyfomo-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:51:35.627829 pyfomo-0.0.8/
--rw-r--r--   0 bill      (1000) bill      (1000)    35119 2023-02-28 14:23:36.000000 pyfomo-0.0.8/LICENSE
--rw-r--r--   0 bill      (1000) bill      (1000)     3472 2023-02-28 21:51:35.627829 pyfomo-0.0.8/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)     2981 2023-02-28 20:36:15.000000 pyfomo-0.0.8/README.md
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:51:35.627829 pyfomo-0.0.8/fomo/
--rw-r--r--   0 bill      (1000) bill      (1000)       67 2023-02-27 20:36:32.000000 pyfomo-0.0.8/fomo/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)    23172 2023-02-28 18:25:18.000000 pyfomo-0.0.8/fomo/estimator.py
--rw-r--r--   0 bill      (1000) bill      (1000)    10377 2023-02-28 18:42:17.000000 pyfomo-0.0.8/fomo/metrics.py
--rw-r--r--   0 bill      (1000) bill      (1000)     5685 2023-02-28 14:24:34.000000 pyfomo-0.0.8/fomo/problem.py
--rw-r--r--   0 bill      (1000) bill      (1000)     4941 2023-02-28 14:24:38.000000 pyfomo-0.0.8/fomo/surrogate_models.py
--rw-r--r--   0 bill      (1000) bill      (1000)     3413 2023-02-28 14:24:43.000000 pyfomo-0.0.8/fomo/surrogate_problem.py
--rw-r--r--   0 bill      (1000) bill      (1000)     3190 2023-02-28 15:09:06.000000 pyfomo-0.0.8/fomo/utils.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:51:35.627829 pyfomo-0.0.8/pyfomo.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     3472 2023-02-28 21:51:35.000000 pyfomo-0.0.8/pyfomo.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)      356 2023-02-28 21:51:35.000000 pyfomo-0.0.8/pyfomo.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        1 2023-02-28 21:51:35.000000 pyfomo-0.0.8/pyfomo.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) bill      (1000)      181 2023-02-28 21:51:35.000000 pyfomo-0.0.8/pyfomo.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        5 2023-02-28 21:51:35.000000 pyfomo-0.0.8/pyfomo.egg-info/top_level.txt
--rw-r--r--   0 bill      (1000) bill      (1000)       80 2023-02-28 20:51:34.000000 pyfomo-0.0.8/pyproject.toml
--rw-r--r--   0 bill      (1000) bill      (1000)      802 2023-02-28 21:51:35.627829 pyfomo-0.0.8/setup.cfg
--rw-r--r--   0 bill      (1000) bill      (1000)      780 2023-02-28 21:38:48.000000 pyfomo-0.0.8/setup.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:51:35.627829 pyfomo-0.0.8/tests/
--rw-r--r--   0 bill      (1000) bill      (1000)     2870 2023-02-28 14:25:16.000000 pyfomo-0.0.8/tests/test_estimator.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:55:39.307826 pyfomo-0.0.9/
+-rw-r--r--   0 bill      (1000) bill      (1000)    35119 2023-02-28 14:23:36.000000 pyfomo-0.0.9/LICENSE
+-rw-r--r--   0 bill      (1000) bill      (1000)     3508 2023-02-28 21:55:39.307826 pyfomo-0.0.9/PKG-INFO
+-rw-r--r--   0 bill      (1000) bill      (1000)     2981 2023-02-28 20:36:15.000000 pyfomo-0.0.9/README.md
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:55:39.307826 pyfomo-0.0.9/fomo/
+-rw-r--r--   0 bill      (1000) bill      (1000)       67 2023-02-27 20:36:32.000000 pyfomo-0.0.9/fomo/__init__.py
+-rw-r--r--   0 bill      (1000) bill      (1000)    23172 2023-02-28 18:25:18.000000 pyfomo-0.0.9/fomo/estimator.py
+-rw-r--r--   0 bill      (1000) bill      (1000)    10377 2023-02-28 18:42:17.000000 pyfomo-0.0.9/fomo/metrics.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     5685 2023-02-28 14:24:34.000000 pyfomo-0.0.9/fomo/problem.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     4941 2023-02-28 14:24:38.000000 pyfomo-0.0.9/fomo/surrogate_models.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     3413 2023-02-28 14:24:43.000000 pyfomo-0.0.9/fomo/surrogate_problem.py
+-rw-r--r--   0 bill      (1000) bill      (1000)     3190 2023-02-28 15:09:06.000000 pyfomo-0.0.9/fomo/utils.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:55:39.307826 pyfomo-0.0.9/pyfomo.egg-info/
+-rw-r--r--   0 bill      (1000) bill      (1000)     3508 2023-02-28 21:55:39.000000 pyfomo-0.0.9/pyfomo.egg-info/PKG-INFO
+-rw-r--r--   0 bill      (1000) bill      (1000)      356 2023-02-28 21:55:39.000000 pyfomo-0.0.9/pyfomo.egg-info/SOURCES.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)        1 2023-02-28 21:55:39.000000 pyfomo-0.0.9/pyfomo.egg-info/dependency_links.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)      165 2023-02-28 21:55:39.000000 pyfomo-0.0.9/pyfomo.egg-info/requires.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)        5 2023-02-28 21:55:39.000000 pyfomo-0.0.9/pyfomo.egg-info/top_level.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)       85 2023-02-28 21:54:53.000000 pyfomo-0.0.9/pyproject.toml
+-rw-r--r--   0 bill      (1000) bill      (1000)      780 2023-02-28 21:55:39.307826 pyfomo-0.0.9/setup.cfg
+-rw-r--r--   0 bill      (1000) bill      (1000)      750 2023-02-28 21:54:39.000000 pyfomo-0.0.9/setup.py
+drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2023-02-28 21:55:39.307826 pyfomo-0.0.9/tests/
+-rw-r--r--   0 bill      (1000) bill      (1000)     2870 2023-02-28 14:25:16.000000 pyfomo-0.0.9/tests/test_estimator.py
```

### Comparing `pyfomo-0.0.8/LICENSE` & `pyfomo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/PKG-INFO` & `pyfomo-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfomo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fairness oriented Multi-objective Optimization
 Home-page: https://github.com/cavalab/fomo
 Author: William La Cava
 Author-email: williamlacava@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
@@ -110,7 +112,8 @@
 
 <!-- start contact -->
 
 
 - William La Cava: william dot lacava at childrens dot harvard dot edu
 
 <!-- end contact -->
+
```

### Comparing `pyfomo-0.0.8/README.md` & `pyfomo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/estimator.py` & `pyfomo-0.0.9/fomo/estimator.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/metrics.py` & `pyfomo-0.0.9/fomo/metrics.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/problem.py` & `pyfomo-0.0.9/fomo/problem.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/surrogate_models.py` & `pyfomo-0.0.9/fomo/surrogate_models.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/surrogate_problem.py` & `pyfomo-0.0.9/fomo/surrogate_problem.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/fomo/utils.py` & `pyfomo-0.0.9/fomo/utils.py`

 * *Files identical despite different names*

### Comparing `pyfomo-0.0.8/pyfomo.egg-info/PKG-INFO` & `pyfomo-0.0.9/pyfomo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfomo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fairness oriented Multi-objective Optimization
 Home-page: https://github.com/cavalab/fomo
 Author: William La Cava
 Author-email: williamlacava@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
@@ -110,7 +112,8 @@
 
 <!-- start contact -->
 
 
 - William La Cava: william dot lacava at childrens dot harvard dot edu
 
 <!-- end contact -->
+
```

### Comparing `pyfomo-0.0.8/setup.cfg` & `pyfomo-0.0.9/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [metadata]
 name = pyfomo
-version = 0.0.8
+version = 0.0.9
 description = Fairness oriented Multi-objective Optimization
 author = William La Cava
 author_email = williamlacava@gmail.com
 url = https://github.com/cavalab/fomo
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
-packages = find:fomo
+packages = fomo
 python_requires = >=3.7
 setup_requires = 
 	numpy
 install_requires = 
-	setuptools<60.0
 	scikit-learn
 	pymoo
 
 [options.extras_require]
 docs = 
 	sphinx
 	recommonmark
```

### Comparing `pyfomo-0.0.8/tests/test_estimator.py` & `pyfomo-0.0.9/tests/test_estimator.py`

 * *Files identical despite different names*

