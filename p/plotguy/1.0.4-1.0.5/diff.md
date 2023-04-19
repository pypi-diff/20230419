# Comparing `tmp/plotguy-1.0.4.tar.gz` & `tmp/plotguy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.4.tar", last modified: Tue Apr 18 03:36:32 2023, max compression
+gzip compressed data, was "plotguy-1.0.5.tar", last modified: Wed Apr 19 08:47:57 2023, max compression
```

## Comparing `plotguy-1.0.4.tar` & `plotguy-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.909128 plotguy-1.0.4/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-18 03:36:32.908974 plotguy-1.0.4/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.4/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.908011 plotguy-1.0.4/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25562 2023-04-18 03:28:10.000000 plotguy-1.0.4/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.4/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.4/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.4/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.4/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.908776 plotguy-1.0.4/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-18 03:36:32.909177 plotguy-1.0.4/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-18 03:34:27.000000 plotguy-1.0.4/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.602859 plotguy-1.0.5/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-19 08:47:57.602313 plotguy-1.0.5/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.5/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.600389 plotguy-1.0.5/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25758 2023-04-19 08:44:51.000000 plotguy-1.0.5/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.5/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.5/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.5/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.5/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.601734 plotguy-1.0.5/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-19 08:47:57.603075 plotguy-1.0.5/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-19 08:45:56.000000 plotguy-1.0.5/setup.py
```

### Comparing `plotguy-1.0.4/plotguy/__init__.py` & `plotguy-1.0.5/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,20 +144,26 @@
 
     app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath, signal_settings)
 
     return app
 
 
 def plot(mode, all_para_combination={},  subchart_settings={}, number_of_curves=20, risk_free_rate='geometric_mean'):
+
+    if subchart_settings == {}: # subchart default setting
+        subchart_settings = {
+            'histogram_period': [1, 3, 5, 10, 20],
+            'subchart_1': ['volume', 'line']
+        }
+
     if mode == 'equity_curves':
         result_df = pd.read_csv('backtest_result.csv', index_col=0)
         app = equity_curves.Plot(all_para_combination, result_df, subchart_settings, number_of_curves)
 
     if mode == 'aggregate':
-
         app = aggregate.Aggregate(risk_free_rate)
 
 
     return app
 
 
 def get_latest_fed_fund_rate():
```

### Comparing `plotguy-1.0.4/plotguy/aggregate.py` & `plotguy-1.0.5/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.4/plotguy/components.py` & `plotguy-1.0.5/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.4/plotguy/equity_curves.py` & `plotguy-1.0.5/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.4/plotguy/signals.py` & `plotguy-1.0.5/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.4/setup.py` & `plotguy-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.4",
+    version="1.0.5",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

