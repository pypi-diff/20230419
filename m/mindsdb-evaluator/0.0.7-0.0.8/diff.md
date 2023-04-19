# Comparing `tmp/mindsdb_evaluator-0.0.7.tar.gz` & `tmp/mindsdb_evaluator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsdb_evaluator-0.0.7.tar", max compression
+gzip compressed data, was "mindsdb_evaluator-0.0.8.tar", max compression
```

## Comparing `mindsdb_evaluator-0.0.7.tar` & `mindsdb_evaluator-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35103 2023-04-17 03:01:27.093942 mindsdb_evaluator-0.0.7/LICENSE
--rw-r--r--   0        0        0       69 2023-04-17 03:01:27.093942 mindsdb_evaluator-0.0.7/README.md
--rw-r--r--   0        0        0      186 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/__init__.py
--rw-r--r--   0        0        0      769 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/__init__.py
--rw-r--r--   0        0        0      714 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/classification.py
--rw-r--r--   0        0        0     3512 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/forecasting.py
--rw-r--r--   0        0        0     3928 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/general.py
--rw-r--r--   0        0        0      763 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/regression.py
--rw-r--r--   0        0        0       69 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/calibration/__init__.py
--rw-r--r--   0        0        0      126 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/calibration/ece.py
--rw-r--r--   0        0        0      492 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35103 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/LICENSE
+-rw-r--r--   0        0        0       69 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/README.md
+-rw-r--r--   0        0        0      186 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/__init__.py
+-rw-r--r--   0        0        0      714 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/classification.py
+-rw-r--r--   0        0        0     3512 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/forecasting.py
+-rw-r--r--   0        0        0     4210 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/general.py
+-rw-r--r--   0        0        0      763 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/regression.py
+-rw-r--r--   0        0        0       69 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/calibration/__init__.py
+-rw-r--r--   0        0        0      126 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/calibration/ece.py
+-rw-r--r--   0        0        0      492 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.8/PKG-INFO
```

### Comparing `mindsdb_evaluator-0.0.7/LICENSE` & `mindsdb_evaluator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/__init__.py` & `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/classification.py` & `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/classification.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/forecasting.py` & `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/forecasting.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/general.py` & `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,22 @@
         y_pred = list(predictions)
         if hasattr(importlib.import_module('mindsdb_evaluator.accuracy'), accuracy_function):
             accuracy_function = getattr(importlib.import_module('mindsdb_evaluator.accuracy'),
                                         accuracy_function)
         else:
             accuracy_function = getattr(importlib.import_module('sklearn.metrics'), accuracy_function)
 
-        score = accuracy_function(y_true, y_pred)
+        try:
+            score = accuracy_function(y_true, y_pred)
+        except ValueError as e:
+            if 'mix of label input' in str(e).lower():
+                score = accuracy_function([str(y) for y in y_true],
+                                          [str(y) for y in y_pred])
+            else:
+                raise e
 
     return round(score, n_decimals)
 
 
 def evaluate_accuracies(data: pd.DataFrame,
                         predictions: pd.Series,
                         target: str,
```

### Comparing `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/regression.py` & `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/regression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.7/PKG-INFO` & `mindsdb_evaluator-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb-evaluator
-Version: 0.0.7
+Version: 0.0.8
 Summary: Model evaluation for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

