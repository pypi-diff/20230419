# Comparing `tmp/pypots-0.0.8.tar.gz` & `tmp/pypots-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.0.8.tar", last modified: Tue Sep 13 10:28:36 2022, max compression
+gzip compressed data, was "pypots-0.0.9.tar", last modified: Tue Dec 20 14:04:38 2022, max compression
```

## Comparing `pypots-0.0.8.tar` & `pypots-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.434891 pypots-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-09-13 10:28:25.000000 pypots-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8669 2022-09-13 10:28:36.434891 pypots-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8168 2022-09-13 10:28:25.000000 pypots-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.426890 pypots-0.0.8/pypots/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7040 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/classification/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/classification/brits.py
--rw-r--r--   0 runner    (1001) docker     (121)     7563 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/classification/grud.py
--rw-r--r--   0 runner    (1001) docker     (121)    25705 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/classification/raindrop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4978 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/clustering/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    18923 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/clustering/crli.py
--rw-r--r--   0 runner    (1001) docker     (121)    18770 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/clustering/vader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/dataset_for_brits.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/dataset_for_grud.py
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/dataset_for_mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6567 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/data/load_specific_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/forecasting/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    15885 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/forecasting/bttf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    18436 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/brits.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/locf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9413 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/saits.py
--rw-r--r--   0 runner    (1001) docker     (121)    11996 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/imputation/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5110 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/test_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/test_imputation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/tests/unified_data_for_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11747 2022-09-13 10:28:25.000000 pypots-0.0.8/pypots/utils/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 10:28:36.430890 pypots-0.0.8/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8669 2022-09-13 10:28:36.000000 pypots-0.0.8/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-09-13 10:28:36.000000 pypots-0.0.8/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 10:28:36.000000 pypots-0.0.8/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-13 10:28:36.000000 pypots-0.0.8/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-13 10:28:36.000000 pypots-0.0.8/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-13 10:28:36.434891 pypots-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-09-13 10:28:25.000000 pypots-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.568948 pypots-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-20 14:04:24.000000 pypots-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2022-12-20 14:04:38.568948 pypots-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2022-12-20 14:04:24.000000 pypots-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.560948 pypots-0.0.9/pypots/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.564948 pypots-0.0.9/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/classification/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/classification/brits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/classification/grud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/classification/raindrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.564948 pypots-0.0.9/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/clustering/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18923 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/clustering/crli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18770 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/clustering/vader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.564948 pypots-0.0.9/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/dataset_for_brits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/dataset_for_grud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/dataset_for_mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/data/load_specific_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.568948 pypots-0.0.9/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/forecasting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/forecasting/bttf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.568948 pypots-0.0.9/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/brits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/locf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/saits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/imputation/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.568948 pypots-0.0.9/pypots/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/test_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/test_imputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/tests/unified_data_for_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.568948 pypots-0.0.9/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2022-12-20 14:04:24.000000 pypots-0.0.9/pypots/utils/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:04:38.560948 pypots-0.0.9/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2022-12-20 14:04:38.000000 pypots-0.0.9/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-20 14:04:38.000000 pypots-0.0.9/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:04:38.000000 pypots-0.0.9/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-20 14:04:38.000000 pypots-0.0.9/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-20 14:04:38.000000 pypots-0.0.9/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 14:04:38.568948 pypots-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-12-20 14:04:24.000000 pypots-0.0.9/setup.py
```

### Comparing `pypots-0.0.8/LICENSE` & `pypots-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/PKG-INFO` & `pypots-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
 Home-page: https://github.com/WenjieDu/PyPOTS
 Download-URL: https://github.com/WenjieDu/PyPOTS/archive/master.zip
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,partially observed,time series,missing data,missing values
+Keywords: data mining,neural networks,machine learning,deep learning,time-series analysis,partially observed,irregular sampled,incomplete time series,missing data,missing values
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/figs/PyPOTS%20logo.svg?sanitize=true' width='200' align='right' /></a>
 
 ## <p align='center'>Welcome to PyPOTS</p>
 **<p align='center'>A Python Toolbox for Data Mining on Partially-Observed Time Series</p>**
@@ -31,58 +31,86 @@
     </a>
     <!-- GitHub Testing -->
     <a alt='GitHub Testing' href='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml'> 
         <img src='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg'>
     </a>
     <!-- Coveralls report -->
     <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/PyPOTS'> 
-        <img src='https://coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg'>
+        <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyPOTS?branch=main&logo=coveralls&labelColor=3F5767'>
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pepy.tech/project/pypots'>
-        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total Downloads'>
+        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads'>
     </a>
-    <!-- Visit number -->
-    <img src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false'>
     <!-- Zenodo DOI -->
     <a alt='Zenodo DOI' href='https://zenodo.org/badge/latestdoi/475477908'>
         <img src='https://zenodo.org/badge/475477908.svg'>
     </a>
     <!-- Code of Conduct -->
     <a alt='CODE_OF_CONDUCT' href='CODE_OF_CONDUCT.md'> 
         <img src='https://img.shields.io/badge/Contributor%20Covenant-v2.1-4baaaa.svg'>
     </a>
+    <!-- Slack Workspace -->
+    <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'> 
+        <img src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'>
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error, and unexpected malfunction, missing values are common to see in time series from the real-world environment. This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced data analysis. Although this problem is important, the area of data mining on POTS still lacks a dedicated toolkit. PyPOTS is created to fill in this blank.
 
 ⦿ `Mission`: PyPOTS is born to become a handy toolbox that is going to make data mining on POTS easy rather than tedious, to help engineers and researchers focus more on the core problems in their hands rather than on how to deal with the missing parts in their data. PyPOTS will keep integrating classical and the latest state-of-the-art data mining algorithms for partially-observed multivariate time series. For sure, besides various algorithms, PyPOTS is going to have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='180'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='190'/></a>
 To make various open-source time-series datasets readily available to our users, PyPOTS gets supported by project [TSDB (Time-Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading time-series datasets super easy! 
 
 Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠! It now supports a total of 119 open-source datasets.
 <br clear='left'>
 
 ## ❖ Installation
 Install the latest release from PyPI:
 > pip install pypots
 
+<details open>
+<summary><b>Below is an example applying SAITS in PyPOTS to impute missing values in the dataset PhysioNet2012:</b></summary>
+
+``` python
+import numpy as np
+from sklearn.preprocessing import StandardScaler
+from pypots.data import load_specific_dataset, mcar, masked_fill
+from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae
+# Data preprocessing. Tedious, but PyPOTS can help. 🤓
+data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
+X = data['X']
+num_samples = len(X['RecordID'].unique())
+X = X.drop('RecordID', axis = 1)
+X = StandardScaler().fit_transform(X.to_numpy())
+X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth
+X = masked_fill(X, 1 - missing_mask, np.nan)
+# Model training. This is PyPOTS showtime. 💪
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits.fit(X)  # train the model. Here I use the whole dataset as the training set, because ground truth is not visible to the model.
+imputation = saits.impute(X)  # impute the originally-missing values and artificially-missing values
+mae = cal_mae(imputation, X_intact, indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+```
+</details>
+
 ## ❖ Available Algorithms
-| Task                          | Type           | Algorithm                                                                 | Year | Reference |        
-|-------------------------------|----------------|---------------------------------------------------------------------------|------|-----------|
-| Imputation                    | Neural Network | SAITS: Self-Attention-based Imputation for Time Series                    | 2022 | [^1]      |
-| Imputation                    | Neural Network | Transformer                                                               | 2017 | [^2] [^1] |
-| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)                | 2018 | [^3]      |
-| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                   | -    | -         |
-| Classification                | Neural Network | GRU-D                                                                     | 2018 | [^4]      |
-| Classification                | Neural Network | Raindrop                                                                  | 2022 | [^5]      |
-| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data)  | 2021 | [^6]      |
-| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                        | 2019 | [^7]      |
-| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                             | 2021 | [^8]      |
+| Task                          | Type           | Algorithm                                                                | Year | Reference |        
+|-------------------------------|----------------|--------------------------------------------------------------------------|------|-----------|
+| Imputation                    | Neural Network | SAITS (Self-Attention-based Imputation for Time Series)                  | 2022 | [^1]      |
+| Imputation                    | Neural Network | Transformer                                                              | 2017 | [^2] [^1] |
+| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)               | 2018 | [^3]      |
+| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                  | -    | -         |
+| Classification                | Neural Network | GRU-D                                                                    | 2018 | [^4]      |
+| Classification                | Neural Network | Raindrop                                                                 | 2022 | [^5]      |
+| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data) | 2021 | [^6]      |
+| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                       | 2019 | [^7]      |
+| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                            | 2021 | [^8]      |
 
 ## ❖ Reference
 If you find PyPOTS is helpful to your research, please cite it as below and ⭐️star this repository to make others notice this work. 🤗
 
 ```bibtex
 @misc{du2022PyPOTS,
 author = {Wenjie Du},
@@ -93,20 +121,29 @@
 }
 ```
 
 or
 
 `Wenjie Du. (2022). PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/10.5281/zenodo.6823222`
 
----
-‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and <a alt='GitHub Discussions' href='https://github.com/WenjieDu/PyPOTS/discussions'><img align='center' src='https://img.shields.io/badge/Chat-in_Discussions-green?logo=github&color=60A98D'></a>, or create an issue.
+## ❖ Attention 👀
+The documentation and tutorials are under construction. And a short paper introducing PyPOTS is on the way! 🚀 Stay tuned please!
+
+‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and chat on <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'><img align='center' src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'></a>, or create an issue. If you have any additional questions or have interests in collaboration, please take a look at [my GitHub profile](https://github.com/WenjieDu) and feel free to contact me 🤝.
 
 Thank you all for your attention! 😃
 
+
 [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516.
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural Networks for Multivariate Time Series with Missing Values. Scientific Reports, 8.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning Representations for Incomplete Time Series Clustering. AAAI 2021.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience, 8.
 [^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for Multidimensional Time Series Prediction. IEEE transactions on pattern analysis and machine intelligence, PP.
+
+<details>
+<summary>🏠 Visits</summary>
+<img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
+</details>
+
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.0.8 Summary: A Python Toolbox for
+Metadata-Version: 2.1 Name: pypots Version: 0.0.9 Summary: A Python Toolbox for
 Data Mining on Partially-Observed Time Series Home-page: https://github.com/
 WenjieDu/PyPOTS Download-URL: https://github.com/WenjieDu/PyPOTS/archive/
 master.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,partially
-observed,time series,missing data,missing values Description-Content-Type:
-text/markdown License-File: LICENSE [https://raw.githubusercontent.com/
-WenjieDu/PyPOTS/main/docs/figs/PyPOTS%20logo.svg?sanitize=true] ##
+Keywords: data mining,neural networks,machine learning,deep learning,time-
+series analysis,partially observed,irregular sampled,incomplete time
+series,missing data,missing values Description-Content-Type: text/markdown
+License-File: LICENSE [https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/
+docs/figs/PyPOTS%20logo.svg?sanitize=true] ##
                                Welcome to PyPOTS
 **
       A Python Toolbox for Data Mining on Partially-Observed Time Series
 **
  [https://img.shields.io/badge/python-v3-yellowgreen]  [https://img.shields.io/
   static/v1?label=%E2%9D%A4%EF%B8%8F&message=PyTorch&color=DC583A]  [PyPI]
  [https://img.shields.io/badge/License-GPL--v3-green?color=79C641]  [https://
 github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg]  [https://
-        coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg]  [https://
+               img.shields.io/coverallsCoverage/github/WenjieDu/
+        PyPOTS?branch=main&logo=coveralls&labelColor=3F5767]  [https://
                      static.pepy.tech/personalized-badge/
-pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total
-           Downloads]  [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false]
+pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads]
    [https://zenodo.org/badge/475477908.svg]  [https://img.shields.io/badge/
-                    Contributor%20Covenant-v2.1-4baaaa.svg]
+ Contributor%20Covenant-v2.1-4baaaa.svg]  [https://img.shields.io/badge/Slack-
+            PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of data mining on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS is born to
@@ -39,20 +40,37 @@
 TSDB%20logo.svg?sanitize=true] To make various open-source time-series datasets
 readily available to our users, PyPOTS gets supported by project [TSDB (Time-
 Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading
 time-series datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB)
 right now to know more about this handy tool ð ! It now supports a total of
 119 open-source datasets.
 ## â Installation Install the latest release from PyPI: > pip install pypots
-## â Available Algorithms | Task | Type | Algorithm | Year | Reference | |---
-----------------------------|----------------|---------------------------------
-------------------------------------------|------|-----------| | Imputation |
-Neural Network | SAITS: Self-Attention-based Imputation for Time Series | 2022
-| [^1] | | Imputation | Neural Network | Transformer | 2017 | [^2] [^1] | |
-Imputation,
+Below is an example applying SAITS in PyPOTS to impute missing values in the
+dataset PhysioNet2012: ``` python import numpy as np from sklearn.preprocessing
+import StandardScaler from pypots.data import load_specific_dataset, mcar,
+masked_fill from pypots.imputation import SAITS from pypots.utils.metrics
+import cal_mae # Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop('RecordID', axis = 1) X = StandardScaler().fit_transform(X.to_numpy()) X
+= X.reshape(num_samples, 48, -1) X_intact, X, missing_mask, indicating_mask =
+mcar(X, 0.1) # hold out 10% observed values as ground truth X = masked_fill(X,
+1 - missing_mask, np.nan) # Model training. This is PyPOTS showtime. ðª saits
+= SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(X) # train the
+model. Here I use the whole dataset as the training set, because ground truth
+is not visible to the model. imputation = saits.impute(X) # impute the
+originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms |
+Task | Type | Algorithm | Year | Reference | |-------------------------------|-
+---------------|---------------------------------------------------------------
+-----------|------|-----------| | Imputation | Neural Network | SAITS (Self-
+Attention-based Imputation for Time Series) | 2022 | [^1] | | Imputation |
+Neural Network | Transformer | 2017 | [^2] [^1] | | Imputation,
 Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for
 Time Series) | 2018 | [^3] | | Imputation | Naive | LOCF (Last Observation
 Carried Forward) | - | - | | Classification | Neural Network | GRU-D | 2018 |
 [^4] | | Classification | Neural Network | Raindrop | 2022 | [^5] | |
 Clustering | Neural Network | CRLI (Clustering Representation Learning on
 Incomplete time-series data) | 2021 | [^6] | | Clustering | Neural Network |
 VaDER (Variational Deep Embedding with Recurrence) | 2019 | [^7] | |
@@ -60,32 +78,38 @@
 2021 | [^8] | ## â Reference If you find PyPOTS is helpful to your research,
 please cite it as below and â­ï¸star this repository to make others notice
 this work. ð¤ ```bibtex @misc{du2022PyPOTS, author = {Wenjie Du}, title = {
 {PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series}},
 howpublished = {\url{https://github.com/wenjiedu/pypots}}, year = {2022}, doi =
 {10.5281/zenodo.6823222}, } ``` or `Wenjie Du. (2022). PyPOTS: A Python Toolbox
 for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/
-10.5281/zenodo.6823222` --- â¼ï¸ PyPOTS is currently under developing. If you
+10.5281/zenodo.6823222` ## â Attention ð The documentation and tutorials
+are under construction. And a short paper introducing PyPOTS is on the way!
+ð Stay tuned please! â¼ï¸ PyPOTS is currently under developing. If you
 like it and look forward to its growth, please give PyPOTS a star and watch it
 to keep you posted on its progress and to let me know that its development is
 meaningful. If you have any feedback, or want to contribute ideas/suggestions
 or share time-series related algorithms/papers, please join PyPOTS community
-and [https://img.shields.io/badge/Chat-in_Discussions-
-green?logo=github&color=60A98D], or create an issue. Thank you all for your
-attention! ð [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-
-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516. [^2]:
-Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N.,
-Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
-[^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS:
-Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018. [^4]: Che,
-Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural
-Networks for Multivariate Time Series with Missing Values. Scientific Reports,
-8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-
-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
-[^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning
-Representations for Incomplete Time Series Clustering. AAAI 2021. [^7]: Jong,
-J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman,
-H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep learning for clustering
-of multivariate clinical patient trajectories with missing values. GigaScience,
-8. [^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for
-Multidimensional Time Series Prediction. IEEE transactions on pattern analysis
-and machine intelligence, PP.
+and chat on [https://img.shields.io/badge/Slack-PyPOTS-
+grey?logo=slack&labelColor=4A154B&color=62BCE5], or create an issue. If you
+have any additional questions or have interests in collaboration, please take a
+look at [my GitHub profile](https://github.com/WenjieDu) and feel free to
+contact me ð¤. Thank you all for your attention! ð [^1]: Du, W., Cote, D.,
+& Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series.
+ArXiv, abs/2202.08516. [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit,
+J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is
+All you Need. NeurIPS 2017. [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L.,
+& Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series.
+NeurIPS 2018. [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y.
+(2018). Recurrent Neural Networks for Multivariate Time Series with Missing
+Values. Scientific Reports, 8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., &
+Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate
+Time Series. ICLR 2022. [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W.
+(2021). Learning Representations for Incomplete Time Series Clustering. AAAI
+2021. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
+Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep
+learning for clustering of multivariate clinical patient trajectories with
+missing values. GigaScience, 8. [^8]: Sun, L., & Chen, X. (2021). Bayesian
+Temporal Factorization for Multidimensional Time Series Prediction. IEEE
+transactions on pattern analysis and machine intelligence, PP.  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `pypots-0.0.8/README.md` & `pypots-0.0.9/pypots.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pypots
+Version: 0.0.9
+Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
+Home-page: https://github.com/WenjieDu/PyPOTS
+Download-URL: https://github.com/WenjieDu/PyPOTS/archive/master.zip
+Author: Wenjie Du
+Author-email: wenjay.du@gmail.com
+License: GPL-3.0
+Keywords: data mining,neural networks,machine learning,deep learning,time-series analysis,partially observed,irregular sampled,incomplete time series,missing data,missing values
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/figs/PyPOTS%20logo.svg?sanitize=true' width='200' align='right' /></a>
 
 ## <p align='center'>Welcome to PyPOTS</p>
 **<p align='center'>A Python Toolbox for Data Mining on Partially-Observed Time Series</p>**
 
 <p align='center'>
     <!-- Python version -->
@@ -18,58 +31,86 @@
     </a>
     <!-- GitHub Testing -->
     <a alt='GitHub Testing' href='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml'> 
         <img src='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg'>
     </a>
     <!-- Coveralls report -->
     <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/PyPOTS'> 
-        <img src='https://coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg'>
+        <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyPOTS?branch=main&logo=coveralls&labelColor=3F5767'>
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pepy.tech/project/pypots'>
-        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total Downloads'>
+        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads'>
     </a>
-    <!-- Visit number -->
-    <img src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false'>
     <!-- Zenodo DOI -->
     <a alt='Zenodo DOI' href='https://zenodo.org/badge/latestdoi/475477908'>
         <img src='https://zenodo.org/badge/475477908.svg'>
     </a>
     <!-- Code of Conduct -->
     <a alt='CODE_OF_CONDUCT' href='CODE_OF_CONDUCT.md'> 
         <img src='https://img.shields.io/badge/Contributor%20Covenant-v2.1-4baaaa.svg'>
     </a>
+    <!-- Slack Workspace -->
+    <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'> 
+        <img src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'>
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error, and unexpected malfunction, missing values are common to see in time series from the real-world environment. This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced data analysis. Although this problem is important, the area of data mining on POTS still lacks a dedicated toolkit. PyPOTS is created to fill in this blank.
 
 ⦿ `Mission`: PyPOTS is born to become a handy toolbox that is going to make data mining on POTS easy rather than tedious, to help engineers and researchers focus more on the core problems in their hands rather than on how to deal with the missing parts in their data. PyPOTS will keep integrating classical and the latest state-of-the-art data mining algorithms for partially-observed multivariate time series. For sure, besides various algorithms, PyPOTS is going to have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='180'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='190'/></a>
 To make various open-source time-series datasets readily available to our users, PyPOTS gets supported by project [TSDB (Time-Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading time-series datasets super easy! 
 
 Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠! It now supports a total of 119 open-source datasets.
 <br clear='left'>
 
 ## ❖ Installation
 Install the latest release from PyPI:
 > pip install pypots
 
+<details open>
+<summary><b>Below is an example applying SAITS in PyPOTS to impute missing values in the dataset PhysioNet2012:</b></summary>
+
+``` python
+import numpy as np
+from sklearn.preprocessing import StandardScaler
+from pypots.data import load_specific_dataset, mcar, masked_fill
+from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae
+# Data preprocessing. Tedious, but PyPOTS can help. 🤓
+data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
+X = data['X']
+num_samples = len(X['RecordID'].unique())
+X = X.drop('RecordID', axis = 1)
+X = StandardScaler().fit_transform(X.to_numpy())
+X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth
+X = masked_fill(X, 1 - missing_mask, np.nan)
+# Model training. This is PyPOTS showtime. 💪
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits.fit(X)  # train the model. Here I use the whole dataset as the training set, because ground truth is not visible to the model.
+imputation = saits.impute(X)  # impute the originally-missing values and artificially-missing values
+mae = cal_mae(imputation, X_intact, indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+```
+</details>
+
 ## ❖ Available Algorithms
-| Task                          | Type           | Algorithm                                                                 | Year | Reference |        
-|-------------------------------|----------------|---------------------------------------------------------------------------|------|-----------|
-| Imputation                    | Neural Network | SAITS: Self-Attention-based Imputation for Time Series                    | 2022 | [^1]      |
-| Imputation                    | Neural Network | Transformer                                                               | 2017 | [^2] [^1] |
-| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)                | 2018 | [^3]      |
-| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                   | -    | -         |
-| Classification                | Neural Network | GRU-D                                                                     | 2018 | [^4]      |
-| Classification                | Neural Network | Raindrop                                                                  | 2022 | [^5]      |
-| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data)  | 2021 | [^6]      |
-| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                        | 2019 | [^7]      |
-| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                             | 2021 | [^8]      |
+| Task                          | Type           | Algorithm                                                                | Year | Reference |        
+|-------------------------------|----------------|--------------------------------------------------------------------------|------|-----------|
+| Imputation                    | Neural Network | SAITS (Self-Attention-based Imputation for Time Series)                  | 2022 | [^1]      |
+| Imputation                    | Neural Network | Transformer                                                              | 2017 | [^2] [^1] |
+| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)               | 2018 | [^3]      |
+| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                  | -    | -         |
+| Classification                | Neural Network | GRU-D                                                                    | 2018 | [^4]      |
+| Classification                | Neural Network | Raindrop                                                                 | 2022 | [^5]      |
+| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data) | 2021 | [^6]      |
+| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                       | 2019 | [^7]      |
+| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                            | 2021 | [^8]      |
 
 ## ❖ Reference
 If you find PyPOTS is helpful to your research, please cite it as below and ⭐️star this repository to make others notice this work. 🤗
 
 ```bibtex
 @misc{du2022PyPOTS,
 author = {Wenjie Du},
@@ -80,20 +121,29 @@
 }
 ```
 
 or
 
 `Wenjie Du. (2022). PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/10.5281/zenodo.6823222`
 
----
-‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and <a alt='GitHub Discussions' href='https://github.com/WenjieDu/PyPOTS/discussions'><img align='center' src='https://img.shields.io/badge/Chat-in_Discussions-green?logo=github&color=60A98D'></a>, or create an issue.
+## ❖ Attention 👀
+The documentation and tutorials are under construction. And a short paper introducing PyPOTS is on the way! 🚀 Stay tuned please!
+
+‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and chat on <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'><img align='center' src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'></a>, or create an issue. If you have any additional questions or have interests in collaboration, please take a look at [my GitHub profile](https://github.com/WenjieDu) and feel free to contact me 🤝.
 
 Thank you all for your attention! 😃
 
+
 [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516.
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural Networks for Multivariate Time Series with Missing Values. Scientific Reports, 8.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning Representations for Incomplete Time Series Clustering. AAAI 2021.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience, 8.
-[^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for Multidimensional Time Series Prediction. IEEE transactions on pattern analysis and machine intelligence, PP.
+[^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for Multidimensional Time Series Prediction. IEEE transactions on pattern analysis and machine intelligence, PP.
+
+<details>
+<summary>🏠 Visits</summary>
+<img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
+</details>
+
```

#### html2text {}

```diff
@@ -1,24 +1,31 @@
-[https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/figs/
-PyPOTS%20logo.svg?sanitize=true] ##
+Metadata-Version: 2.1 Name: pypots Version: 0.0.9 Summary: A Python Toolbox for
+Data Mining on Partially-Observed Time Series Home-page: https://github.com/
+WenjieDu/PyPOTS Download-URL: https://github.com/WenjieDu/PyPOTS/archive/
+master.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0
+Keywords: data mining,neural networks,machine learning,deep learning,time-
+series analysis,partially observed,irregular sampled,incomplete time
+series,missing data,missing values Description-Content-Type: text/markdown
+License-File: LICENSE [https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/
+docs/figs/PyPOTS%20logo.svg?sanitize=true] ##
                                Welcome to PyPOTS
 **
       A Python Toolbox for Data Mining on Partially-Observed Time Series
 **
  [https://img.shields.io/badge/python-v3-yellowgreen]  [https://img.shields.io/
   static/v1?label=%E2%9D%A4%EF%B8%8F&message=PyTorch&color=DC583A]  [PyPI]
  [https://img.shields.io/badge/License-GPL--v3-green?color=79C641]  [https://
 github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg]  [https://
-        coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg]  [https://
+               img.shields.io/coverallsCoverage/github/WenjieDu/
+        PyPOTS?branch=main&logo=coveralls&labelColor=3F5767]  [https://
                      static.pepy.tech/personalized-badge/
-pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total
-           Downloads]  [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false]
+pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads]
    [https://zenodo.org/badge/475477908.svg]  [https://img.shields.io/badge/
-                    Contributor%20Covenant-v2.1-4baaaa.svg]
+ Contributor%20Covenant-v2.1-4baaaa.svg]  [https://img.shields.io/badge/Slack-
+            PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of data mining on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS is born to
@@ -33,20 +40,37 @@
 TSDB%20logo.svg?sanitize=true] To make various open-source time-series datasets
 readily available to our users, PyPOTS gets supported by project [TSDB (Time-
 Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading
 time-series datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB)
 right now to know more about this handy tool ð ! It now supports a total of
 119 open-source datasets.
 ## â Installation Install the latest release from PyPI: > pip install pypots
-## â Available Algorithms | Task | Type | Algorithm | Year | Reference | |---
-----------------------------|----------------|---------------------------------
-------------------------------------------|------|-----------| | Imputation |
-Neural Network | SAITS: Self-Attention-based Imputation for Time Series | 2022
-| [^1] | | Imputation | Neural Network | Transformer | 2017 | [^2] [^1] | |
-Imputation,
+Below is an example applying SAITS in PyPOTS to impute missing values in the
+dataset PhysioNet2012: ``` python import numpy as np from sklearn.preprocessing
+import StandardScaler from pypots.data import load_specific_dataset, mcar,
+masked_fill from pypots.imputation import SAITS from pypots.utils.metrics
+import cal_mae # Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop('RecordID', axis = 1) X = StandardScaler().fit_transform(X.to_numpy()) X
+= X.reshape(num_samples, 48, -1) X_intact, X, missing_mask, indicating_mask =
+mcar(X, 0.1) # hold out 10% observed values as ground truth X = masked_fill(X,
+1 - missing_mask, np.nan) # Model training. This is PyPOTS showtime. ðª saits
+= SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(X) # train the
+model. Here I use the whole dataset as the training set, because ground truth
+is not visible to the model. imputation = saits.impute(X) # impute the
+originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms |
+Task | Type | Algorithm | Year | Reference | |-------------------------------|-
+---------------|---------------------------------------------------------------
+-----------|------|-----------| | Imputation | Neural Network | SAITS (Self-
+Attention-based Imputation for Time Series) | 2022 | [^1] | | Imputation |
+Neural Network | Transformer | 2017 | [^2] [^1] | | Imputation,
 Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for
 Time Series) | 2018 | [^3] | | Imputation | Naive | LOCF (Last Observation
 Carried Forward) | - | - | | Classification | Neural Network | GRU-D | 2018 |
 [^4] | | Classification | Neural Network | Raindrop | 2022 | [^5] | |
 Clustering | Neural Network | CRLI (Clustering Representation Learning on
 Incomplete time-series data) | 2021 | [^6] | | Clustering | Neural Network |
 VaDER (Variational Deep Embedding with Recurrence) | 2019 | [^7] | |
@@ -54,32 +78,38 @@
 2021 | [^8] | ## â Reference If you find PyPOTS is helpful to your research,
 please cite it as below and â­ï¸star this repository to make others notice
 this work. ð¤ ```bibtex @misc{du2022PyPOTS, author = {Wenjie Du}, title = {
 {PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series}},
 howpublished = {\url{https://github.com/wenjiedu/pypots}}, year = {2022}, doi =
 {10.5281/zenodo.6823222}, } ``` or `Wenjie Du. (2022). PyPOTS: A Python Toolbox
 for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/
-10.5281/zenodo.6823222` --- â¼ï¸ PyPOTS is currently under developing. If you
+10.5281/zenodo.6823222` ## â Attention ð The documentation and tutorials
+are under construction. And a short paper introducing PyPOTS is on the way!
+ð Stay tuned please! â¼ï¸ PyPOTS is currently under developing. If you
 like it and look forward to its growth, please give PyPOTS a star and watch it
 to keep you posted on its progress and to let me know that its development is
 meaningful. If you have any feedback, or want to contribute ideas/suggestions
 or share time-series related algorithms/papers, please join PyPOTS community
-and [https://img.shields.io/badge/Chat-in_Discussions-
-green?logo=github&color=60A98D], or create an issue. Thank you all for your
-attention! ð [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-
-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516. [^2]:
-Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N.,
-Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
-[^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS:
-Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018. [^4]: Che,
-Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural
-Networks for Multivariate Time Series with Missing Values. Scientific Reports,
-8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-
-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
-[^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning
-Representations for Incomplete Time Series Clustering. AAAI 2021. [^7]: Jong,
-J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman,
-H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep learning for clustering
-of multivariate clinical patient trajectories with missing values. GigaScience,
-8. [^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for
-Multidimensional Time Series Prediction. IEEE transactions on pattern analysis
-and machine intelligence, PP.
+and chat on [https://img.shields.io/badge/Slack-PyPOTS-
+grey?logo=slack&labelColor=4A154B&color=62BCE5], or create an issue. If you
+have any additional questions or have interests in collaboration, please take a
+look at [my GitHub profile](https://github.com/WenjieDu) and feel free to
+contact me ð¤. Thank you all for your attention! ð [^1]: Du, W., Cote, D.,
+& Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series.
+ArXiv, abs/2202.08516. [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit,
+J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is
+All you Need. NeurIPS 2017. [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L.,
+& Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series.
+NeurIPS 2018. [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y.
+(2018). Recurrent Neural Networks for Multivariate Time Series with Missing
+Values. Scientific Reports, 8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., &
+Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate
+Time Series. ICLR 2022. [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W.
+(2021). Learning Representations for Incomplete Time Series Clustering. AAAI
+2021. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
+Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep
+learning for clustering of multivariate clinical patient trajectories with
+missing values. GigaScience, 8. [^8]: Sun, L., & Chen, X. (2021). Bayesian
+Temporal Factorization for Multidimensional Time Series Prediction. IEEE
+transactions on pattern analysis and machine intelligence, PP.  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `pypots-0.0.8/pypots/__version__.py` & `pypots-0.0.9/pypots/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 
-version = "0.0.8"
+version = "0.0.9"
```

### Comparing `pypots-0.0.8/pypots/base.py` & `pypots-0.0.9/pypots/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/classification/base.py` & `pypots-0.0.9/pypots/classification/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/classification/brits.py` & `pypots-0.0.9/pypots/classification/brits.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/classification/grud.py` & `pypots-0.0.9/pypots/classification/grud.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/classification/raindrop.py` & `pypots-0.0.9/pypots/classification/raindrop.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,28 @@
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Linear
 from torch.nn import TransformerEncoderLayer, TransformerEncoder
 from torch.nn import init
 from torch.nn.parameter import Parameter
 from torch.utils.data import DataLoader
-from torch_geometric.nn.conv import MessagePassing
-from torch_geometric.nn.inits import glorot
-from torch_geometric.typing import PairTensor, Adj, OptTensor
-from torch_geometric.utils import softmax
-from torch_scatter import scatter
-from torch_sparse import SparseTensor
+
+try:
+    from torch_geometric.nn.conv import MessagePassing
+    from torch_geometric.nn.inits import glorot
+    from torch_geometric.typing import PairTensor, Adj, OptTensor
+    from torch_geometric.utils import softmax
+    from torch_scatter import scatter
+    from torch_sparse import SparseTensor
+except ImportError as e:
+    print(
+        f"{e}\n"
+        "torch_geometric is missing, "
+        "please install it with 'pip install torch_geometric' or 'conda install -c pyg pyg'"
+    )
 
 from pypots.classification.base import BaseNNClassifier
 from pypots.data.dataset_for_grud import DatasetForGRUD
 
 
 class PositionalEncodingTF(nn.Module):
     """Generate positional encoding according to time information."""
```

### Comparing `pypots-0.0.8/pypots/clustering/base.py` & `pypots-0.0.9/pypots/clustering/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/clustering/crli.py` & `pypots-0.0.9/pypots/clustering/crli.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/clustering/vader.py` & `pypots-0.0.9/pypots/clustering/vader.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/__init__.py` & `pypots-0.0.9/pypots/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/base.py` & `pypots-0.0.9/pypots/data/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/dataset_for_brits.py` & `pypots-0.0.9/pypots/data/dataset_for_brits.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/dataset_for_grud.py` & `pypots-0.0.9/pypots/data/dataset_for_grud.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/dataset_for_mit.py` & `pypots-0.0.9/pypots/data/dataset_for_mit.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/generating.py` & `pypots-0.0.9/pypots/data/generating.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/integration.py` & `pypots-0.0.9/pypots/data/integration.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/data/load_specific_datasets.py` & `pypots-0.0.9/pypots/data/load_specific_datasets.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     """
     X = data["X"].drop(data["static_features"], axis=1)
 
     def apply_func(df_temp):  # pad and truncate to set the max length of samples as 48
         missing = list(set(range(0, 48)).difference(set(df_temp["Time"])))
         missing_part = pd.DataFrame({"Time": missing})
-        df_temp = df_temp.append(missing_part, ignore_index=False, sort=False)  # pad
+        df_temp = pd.concat([df_temp, missing_part], ignore_index=False, sort=False)  # pad
         df_temp = df_temp.set_index("Time").sort_index().reset_index()
         df_temp = df_temp.iloc[:48]  # truncate
         return df_temp
 
     X = X.groupby("RecordID").apply(apply_func)
     X = X.drop("RecordID", axis=1)  #
     X = X.reset_index()
```

### Comparing `pypots-0.0.8/pypots/forecasting/base.py` & `pypots-0.0.9/pypots/forecasting/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/forecasting/bttf.py` & `pypots-0.0.9/pypots/forecasting/bttf.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/imputation/base.py` & `pypots-0.0.9/pypots/imputation/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/imputation/brits.py` & `pypots-0.0.9/pypots/imputation/brits.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/imputation/locf.py` & `pypots-0.0.9/pypots/imputation/locf.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/imputation/saits.py` & `pypots-0.0.9/pypots/imputation/saits.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/imputation/transformer.py` & `pypots-0.0.9/pypots/imputation/transformer.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/tests/test_classification.py` & `pypots-0.0.9/pypots/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/tests/test_clustering.py` & `pypots-0.0.9/pypots/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/tests/test_forecasting.py` & `pypots-0.0.9/pypots/tests/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/tests/test_imputation.py` & `pypots-0.0.9/pypots/tests/test_imputation.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots/tests/unified_data_for_test.py` & `pypots-0.0.9/pypots/tests/unified_data_for_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Generate the unified test data.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
-import pandas as pd
 import torch
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
 
 from pypots.data import generate_random_walk_for_classification, mcar, masked_fill
 from pypots.data import load_specific_dataset
 
@@ -71,29 +70,14 @@
 
 
 def gene_physionet2012():
     """Generate PhysioNet2012."""
     # generate samples
     df = load_specific_dataset("physionet_2012")
     X = df["X"]
-    X = X.drop(df["static_features"], axis=1)
-
-    def apply_func(df_temp):
-        missing = list(set(range(0, 48)).difference(set(df_temp["Time"])))
-        missing_part = pd.DataFrame({"Time": missing})
-        df_temp = df_temp.append(missing_part, ignore_index=False, sort=False)
-        df_temp = df_temp.set_index("Time").sort_index().reset_index()
-        df_temp = df_temp.iloc[:48]
-        return df_temp
-
-    X = X.groupby("RecordID").apply(apply_func)
-    X = X.drop("RecordID", axis=1)
-    X = X.reset_index()
-    X = X.drop(["level_1", "Time"], axis=1)
-
     y = df["y"]
     all_recordID = X["RecordID"].unique()
     train_set_ids, test_set_ids = train_test_split(all_recordID, test_size=0.2)
     train_set_ids, val_set_ids = train_test_split(train_set_ids, test_size=0.2)
     train_set = X[X["RecordID"].isin(train_set_ids)]
     val_set = X[X["RecordID"].isin(val_set_ids)]
     test_set = X[X["RecordID"].isin(test_set_ids)]
```

### Comparing `pypots-0.0.8/pypots/utils/metrics.py` & `pypots-0.0.9/pypots/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/pypots.egg-info/PKG-INFO` & `pypots-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pypots
-Version: 0.0.8
-Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
-Home-page: https://github.com/WenjieDu/PyPOTS
-Download-URL: https://github.com/WenjieDu/PyPOTS/archive/master.zip
-Author: Wenjie Du
-Author-email: wenjay.du@gmail.com
-License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,partially observed,time series,missing data,missing values
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/figs/PyPOTS%20logo.svg?sanitize=true' width='200' align='right' /></a>
 
 ## <p align='center'>Welcome to PyPOTS</p>
 **<p align='center'>A Python Toolbox for Data Mining on Partially-Observed Time Series</p>**
 
 <p align='center'>
     <!-- Python version -->
@@ -31,58 +18,86 @@
     </a>
     <!-- GitHub Testing -->
     <a alt='GitHub Testing' href='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml'> 
         <img src='https://github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg'>
     </a>
     <!-- Coveralls report -->
     <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/PyPOTS'> 
-        <img src='https://coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg'>
+        <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyPOTS?branch=main&logo=coveralls&labelColor=3F5767'>
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pepy.tech/project/pypots'>
-        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total Downloads'>
+        <img src='https://static.pepy.tech/personalized-badge/pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads'>
     </a>
-    <!-- Visit number -->
-    <img src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false'>
     <!-- Zenodo DOI -->
     <a alt='Zenodo DOI' href='https://zenodo.org/badge/latestdoi/475477908'>
         <img src='https://zenodo.org/badge/475477908.svg'>
     </a>
     <!-- Code of Conduct -->
     <a alt='CODE_OF_CONDUCT' href='CODE_OF_CONDUCT.md'> 
         <img src='https://img.shields.io/badge/Contributor%20Covenant-v2.1-4baaaa.svg'>
     </a>
+    <!-- Slack Workspace -->
+    <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'> 
+        <img src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'>
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error, and unexpected malfunction, missing values are common to see in time series from the real-world environment. This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced data analysis. Although this problem is important, the area of data mining on POTS still lacks a dedicated toolkit. PyPOTS is created to fill in this blank.
 
 ⦿ `Mission`: PyPOTS is born to become a handy toolbox that is going to make data mining on POTS easy rather than tedious, to help engineers and researchers focus more on the core problems in their hands rather than on how to deal with the missing parts in their data. PyPOTS will keep integrating classical and the latest state-of-the-art data mining algorithms for partially-observed multivariate time series. For sure, besides various algorithms, PyPOTS is going to have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='180'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/figs/TSDB%20logo.svg?sanitize=true" align='left' width='190'/></a>
 To make various open-source time-series datasets readily available to our users, PyPOTS gets supported by project [TSDB (Time-Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading time-series datasets super easy! 
 
 Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠! It now supports a total of 119 open-source datasets.
 <br clear='left'>
 
 ## ❖ Installation
 Install the latest release from PyPI:
 > pip install pypots
 
+<details open>
+<summary><b>Below is an example applying SAITS in PyPOTS to impute missing values in the dataset PhysioNet2012:</b></summary>
+
+``` python
+import numpy as np
+from sklearn.preprocessing import StandardScaler
+from pypots.data import load_specific_dataset, mcar, masked_fill
+from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae
+# Data preprocessing. Tedious, but PyPOTS can help. 🤓
+data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
+X = data['X']
+num_samples = len(X['RecordID'].unique())
+X = X.drop('RecordID', axis = 1)
+X = StandardScaler().fit_transform(X.to_numpy())
+X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth
+X = masked_fill(X, 1 - missing_mask, np.nan)
+# Model training. This is PyPOTS showtime. 💪
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits.fit(X)  # train the model. Here I use the whole dataset as the training set, because ground truth is not visible to the model.
+imputation = saits.impute(X)  # impute the originally-missing values and artificially-missing values
+mae = cal_mae(imputation, X_intact, indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+```
+</details>
+
 ## ❖ Available Algorithms
-| Task                          | Type           | Algorithm                                                                 | Year | Reference |        
-|-------------------------------|----------------|---------------------------------------------------------------------------|------|-----------|
-| Imputation                    | Neural Network | SAITS: Self-Attention-based Imputation for Time Series                    | 2022 | [^1]      |
-| Imputation                    | Neural Network | Transformer                                                               | 2017 | [^2] [^1] |
-| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)                | 2018 | [^3]      |
-| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                   | -    | -         |
-| Classification                | Neural Network | GRU-D                                                                     | 2018 | [^4]      |
-| Classification                | Neural Network | Raindrop                                                                  | 2022 | [^5]      |
-| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data)  | 2021 | [^6]      |
-| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                        | 2019 | [^7]      |
-| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                             | 2021 | [^8]      |
+| Task                          | Type           | Algorithm                                                                | Year | Reference |        
+|-------------------------------|----------------|--------------------------------------------------------------------------|------|-----------|
+| Imputation                    | Neural Network | SAITS (Self-Attention-based Imputation for Time Series)                  | 2022 | [^1]      |
+| Imputation                    | Neural Network | Transformer                                                              | 2017 | [^2] [^1] |
+| Imputation,<br>Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for Time Series)               | 2018 | [^3]      |
+| Imputation                    | Naive          | LOCF (Last Observation Carried Forward)                                  | -    | -         |
+| Classification                | Neural Network | GRU-D                                                                    | 2018 | [^4]      |
+| Classification                | Neural Network | Raindrop                                                                 | 2022 | [^5]      |
+| Clustering                    | Neural Network | CRLI (Clustering Representation Learning on Incomplete time-series data) | 2021 | [^6]      |
+| Clustering                    | Neural Network | VaDER (Variational Deep Embedding with Recurrence)                       | 2019 | [^7]      |
+| Forecasting                   | Probabilistic  | BTTF (Bayesian Temporal Tensor Factorization)                            | 2021 | [^8]      |
 
 ## ❖ Reference
 If you find PyPOTS is helpful to your research, please cite it as below and ⭐️star this repository to make others notice this work. 🤗
 
 ```bibtex
 @misc{du2022PyPOTS,
 author = {Wenjie Du},
@@ -93,20 +108,29 @@
 }
 ```
 
 or
 
 `Wenjie Du. (2022). PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/10.5281/zenodo.6823222`
 
----
-‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and <a alt='GitHub Discussions' href='https://github.com/WenjieDu/PyPOTS/discussions'><img align='center' src='https://img.shields.io/badge/Chat-in_Discussions-green?logo=github&color=60A98D'></a>, or create an issue.
+## ❖ Attention 👀
+The documentation and tutorials are under construction. And a short paper introducing PyPOTS is on the way! 🚀 Stay tuned please!
+
+‼️ PyPOTS is currently under developing. If you like it and look forward to its growth, <ins>please give PyPOTS a star and watch it to keep you posted on its progress and to let me know that its development is meaningful</ins>. If you have any feedback, or want to contribute ideas/suggestions or share time-series related algorithms/papers, please join PyPOTS community and chat on <a alt='Slack Workspace' href='https://join.slack.com/t/pypots-dev/shared_invite/zt-1gq6ufwsi-p0OZdW~e9UW_IA4_f1OfxA'><img align='center' src='https://img.shields.io/badge/Slack-PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5'></a>, or create an issue. If you have any additional questions or have interests in collaboration, please take a look at [my GitHub profile](https://github.com/WenjieDu) and feel free to contact me 🤝.
 
 Thank you all for your attention! 😃
 
+
 [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516.
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural Networks for Multivariate Time Series with Missing Values. Scientific Reports, 8.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning Representations for Incomplete Time Series Clustering. AAAI 2021.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience, 8.
 [^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for Multidimensional Time Series Prediction. IEEE transactions on pattern analysis and machine intelligence, PP.
+
+<details>
+<summary>🏠 Visits</summary>
+<img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
+</details>
+
```

#### html2text {}

```diff
@@ -1,30 +1,24 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.0.8 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://github.com/
-WenjieDu/PyPOTS Download-URL: https://github.com/WenjieDu/PyPOTS/archive/
-master.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,partially
-observed,time series,missing data,missing values Description-Content-Type:
-text/markdown License-File: LICENSE [https://raw.githubusercontent.com/
-WenjieDu/PyPOTS/main/docs/figs/PyPOTS%20logo.svg?sanitize=true] ##
+[https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/figs/
+PyPOTS%20logo.svg?sanitize=true] ##
                                Welcome to PyPOTS
 **
       A Python Toolbox for Data Mining on Partially-Observed Time Series
 **
  [https://img.shields.io/badge/python-v3-yellowgreen]  [https://img.shields.io/
   static/v1?label=%E2%9D%A4%EF%B8%8F&message=PyTorch&color=DC583A]  [PyPI]
  [https://img.shields.io/badge/License-GPL--v3-green?color=79C641]  [https://
 github.com/WenjieDu/PyPOTS/actions/workflows/testing.yml/badge.svg]  [https://
-        coveralls.io/repos/github/WenjieDu/PyPOTS/badge.svg]  [https://
+               img.shields.io/coverallsCoverage/github/WenjieDu/
+        PyPOTS?branch=main&logo=coveralls&labelColor=3F5767]  [https://
                      static.pepy.tech/personalized-badge/
-pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Total
-           Downloads]  [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits&edge_flat=false]
+pypots?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads]
    [https://zenodo.org/badge/475477908.svg]  [https://img.shields.io/badge/
-                    Contributor%20Covenant-v2.1-4baaaa.svg]
+ Contributor%20Covenant-v2.1-4baaaa.svg]  [https://img.shields.io/badge/Slack-
+            PyPOTS-grey?logo=slack&labelColor=4A154B&color=62BCE5]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of data mining on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS is born to
@@ -39,20 +33,37 @@
 TSDB%20logo.svg?sanitize=true] To make various open-source time-series datasets
 readily available to our users, PyPOTS gets supported by project [TSDB (Time-
 Series DataBase)](https://github.com/WenjieDu/TSDB), a toolbox making loading
 time-series datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB)
 right now to know more about this handy tool ð ! It now supports a total of
 119 open-source datasets.
 ## â Installation Install the latest release from PyPI: > pip install pypots
-## â Available Algorithms | Task | Type | Algorithm | Year | Reference | |---
-----------------------------|----------------|---------------------------------
-------------------------------------------|------|-----------| | Imputation |
-Neural Network | SAITS: Self-Attention-based Imputation for Time Series | 2022
-| [^1] | | Imputation | Neural Network | Transformer | 2017 | [^2] [^1] | |
-Imputation,
+Below is an example applying SAITS in PyPOTS to impute missing values in the
+dataset PhysioNet2012: ``` python import numpy as np from sklearn.preprocessing
+import StandardScaler from pypots.data import load_specific_dataset, mcar,
+masked_fill from pypots.imputation import SAITS from pypots.utils.metrics
+import cal_mae # Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop('RecordID', axis = 1) X = StandardScaler().fit_transform(X.to_numpy()) X
+= X.reshape(num_samples, 48, -1) X_intact, X, missing_mask, indicating_mask =
+mcar(X, 0.1) # hold out 10% observed values as ground truth X = masked_fill(X,
+1 - missing_mask, np.nan) # Model training. This is PyPOTS showtime. ðª saits
+= SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(X) # train the
+model. Here I use the whole dataset as the training set, because ground truth
+is not visible to the model. imputation = saits.impute(X) # impute the
+originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms |
+Task | Type | Algorithm | Year | Reference | |-------------------------------|-
+---------------|---------------------------------------------------------------
+-----------|------|-----------| | Imputation | Neural Network | SAITS (Self-
+Attention-based Imputation for Time Series) | 2022 | [^1] | | Imputation |
+Neural Network | Transformer | 2017 | [^2] [^1] | | Imputation,
 Classification | Neural Network | BRITS (Bidirectional Recurrent Imputation for
 Time Series) | 2018 | [^3] | | Imputation | Naive | LOCF (Last Observation
 Carried Forward) | - | - | | Classification | Neural Network | GRU-D | 2018 |
 [^4] | | Classification | Neural Network | Raindrop | 2022 | [^5] | |
 Clustering | Neural Network | CRLI (Clustering Representation Learning on
 Incomplete time-series data) | 2021 | [^6] | | Clustering | Neural Network |
 VaDER (Variational Deep Embedding with Recurrence) | 2019 | [^7] | |
@@ -60,32 +71,38 @@
 2021 | [^8] | ## â Reference If you find PyPOTS is helpful to your research,
 please cite it as below and â­ï¸star this repository to make others notice
 this work. ð¤ ```bibtex @misc{du2022PyPOTS, author = {Wenjie Du}, title = {
 {PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series}},
 howpublished = {\url{https://github.com/wenjiedu/pypots}}, year = {2022}, doi =
 {10.5281/zenodo.6823222}, } ``` or `Wenjie Du. (2022). PyPOTS: A Python Toolbox
 for Data Mining on Partially-Observed Time Series. Zenodo. https://doi.org/
-10.5281/zenodo.6823222` --- â¼ï¸ PyPOTS is currently under developing. If you
+10.5281/zenodo.6823222` ## â Attention ð The documentation and tutorials
+are under construction. And a short paper introducing PyPOTS is on the way!
+ð Stay tuned please! â¼ï¸ PyPOTS is currently under developing. If you
 like it and look forward to its growth, please give PyPOTS a star and watch it
 to keep you posted on its progress and to let me know that its development is
 meaningful. If you have any feedback, or want to contribute ideas/suggestions
 or share time-series related algorithms/papers, please join PyPOTS community
-and [https://img.shields.io/badge/Chat-in_Discussions-
-green?logo=github&color=60A98D], or create an issue. Thank you all for your
-attention! ð [^1]: Du, W., Cote, D., & Liu, Y. (2022). SAITS: Self-
-Attention-based Imputation for Time Series. ArXiv, abs/2202.08516. [^2]:
-Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N.,
-Kaiser, L., & Polosukhin, I. (2017). Attention is All you Need. NeurIPS 2017.
-[^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). BRITS:
-Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018. [^4]: Che,
-Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). Recurrent Neural
-Networks for Multivariate Time Series with Missing Values. Scientific Reports,
-8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). Graph-
-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022.
-[^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). Learning
-Representations for Incomplete Time Series Clustering. AAAI 2021. [^7]: Jong,
-J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman,
-H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep learning for clustering
-of multivariate clinical patient trajectories with missing values. GigaScience,
-8. [^8]: Sun, L., & Chen, X. (2021). Bayesian Temporal Factorization for
-Multidimensional Time Series Prediction. IEEE transactions on pattern analysis
-and machine intelligence, PP.
+and chat on [https://img.shields.io/badge/Slack-PyPOTS-
+grey?logo=slack&labelColor=4A154B&color=62BCE5], or create an issue. If you
+have any additional questions or have interests in collaboration, please take a
+look at [my GitHub profile](https://github.com/WenjieDu) and feel free to
+contact me ð¤. Thank you all for your attention! ð [^1]: Du, W., Cote, D.,
+& Liu, Y. (2022). SAITS: Self-Attention-based Imputation for Time Series.
+ArXiv, abs/2202.08516. [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit,
+J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). Attention is
+All you Need. NeurIPS 2017. [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L.,
+& Li, Y. (2018). BRITS: Bidirectional Recurrent Imputation for Time Series.
+NeurIPS 2018. [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y.
+(2018). Recurrent Neural Networks for Multivariate Time Series with Missing
+Values. Scientific Reports, 8. [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., &
+Zitnik, M. (2022). Graph-Guided Network for Irregularly Sampled Multivariate
+Time Series. ICLR 2022. [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W.
+(2021). Learning Representations for Incomplete Time Series Clustering. AAAI
+2021. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
+Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). Deep
+learning for clustering of multivariate clinical patient trajectories with
+missing values. GigaScience, 8. [^8]: Sun, L., & Chen, X. (2021). Bayesian
+Temporal Factorization for Multidimensional Time Series Prediction. IEEE
+transactions on pattern analysis and machine intelligence, PP.  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `pypots-0.0.8/pypots.egg-info/SOURCES.txt` & `pypots-0.0.9/pypots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypots-0.0.8/setup.py` & `pypots-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,30 +17,32 @@
     url="https://github.com/WenjieDu/PyPOTS",
     download_url="https://github.com/WenjieDu/PyPOTS/archive/master.zip",
     keywords=[
         "data mining",
         "neural networks",
         "machine learning",
         "deep learning",
+        "time-series analysis",
         "partially observed",
-        "time series",
+        "irregular sampled",
+        "incomplete time series",
         "missing data",
         "missing values",
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "matplotlib",
         "numpy",
         "scikit_learn",
         "scipy",
         "torch>=1.10",  # torch_sparse v0.6.12 requires 1.9<=torch<1.10, v0.6.13 needs torch>=1.10
-        "torch_sparse==0.6.13",
-        "torch_scatter",
-        "torch_geometric",
+        # "torch_sparse==0.6.13",
+        # "torch_scatter",
+        # "torch_geometric",
         "tensorboard",
         "pandas",
         "pycorruptor",
         "tsdb",
     ],
     setup_requires=["setuptools>=38.6.0"],
 )
```

