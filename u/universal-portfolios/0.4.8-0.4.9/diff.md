# Comparing `tmp/universal-portfolios-0.4.8.tar.gz` & `tmp/universal-portfolios-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal-portfolios-0.4.8.tar", max compression
+gzip compressed data, was "universal-portfolios-0.4.9.tar", max compression
```

## Comparing `universal-portfolios-0.4.8.tar` & `universal-portfolios-0.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1162 2020-09-01 07:13:59.863893 universal-portfolios-0.4.8/LICENSE
--rw-r--r--   0        0        0     7817 2021-09-09 10:19:25.328399 universal-portfolios-0.4.8/README.md
--rw-r--r--   0        0        0      902 2022-07-04 20:02:34.287232 universal-portfolios-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       24 2021-08-18 20:48:46.919705 universal-portfolios-0.4.8/universal/__init__.py
--rw-r--r--   0        0        0    11482 2021-09-09 09:07:59.866133 universal-portfolios-0.4.8/universal/algo.py
--rw-r--r--   0        0        0      527 2021-09-09 10:23:27.407453 universal-portfolios-0.4.8/universal/algos/__init__.py
--rw-r--r--   0        0        0     1728 2021-08-18 20:48:46.920679 universal-portfolios-0.4.8/universal/algos/_up_deprecated.py
--rw-r--r--   0        0        0     4853 2021-08-30 12:16:19.300827 universal-portfolios-0.4.8/universal/algos/anticor.py
--rw-r--r--   0        0        0      902 2021-08-18 20:48:46.921563 universal-portfolios-0.4.8/universal/algos/bah.py
--rw-r--r--   0        0        0      791 2021-09-29 10:38:32.687285 universal-portfolios-0.4.8/universal/algos/bcrp.py
--rw-r--r--   0        0        0     1250 2021-09-29 10:48:26.544681 universal-portfolios-0.4.8/universal/algos/best_markowitz.py
--rw-r--r--   0        0        0     1154 2021-09-29 10:49:11.075005 universal-portfolios-0.4.8/universal/algos/best_so_far.py
--rw-r--r--   0        0        0     1762 2021-08-30 12:16:38.354403 universal-portfolios-0.4.8/universal/algos/bnn.py
--rw-r--r--   0        0        0     3809 2021-08-30 12:13:20.217489 universal-portfolios-0.4.8/universal/algos/corn.py
--rw-r--r--   0        0        0     2962 2021-08-18 20:48:46.924030 universal-portfolios-0.4.8/universal/algos/crp.py
--rw-r--r--   0        0        0     4450 2021-08-30 12:16:43.225819 universal-portfolios-0.4.8/universal/algos/cwmr.py
--rw-r--r--   0        0        0      985 2021-08-30 12:16:47.257846 universal-portfolios-0.4.8/universal/algos/dynamic_crp.py
--rw-r--r--   0        0        0      901 2021-08-30 12:16:51.801265 universal-portfolios-0.4.8/universal/algos/eg.py
--rw-r--r--   0        0        0    26623 2022-01-11 13:17:53.513539 universal-portfolios-0.4.8/universal/algos/estimators.py
--rw-r--r--   0        0        0     4074 2021-08-30 12:16:58.257631 universal-portfolios-0.4.8/universal/algos/kelly.py
--rw-r--r--   0        0        0    16271 2021-08-18 20:48:46.926640 universal-portfolios-0.4.8/universal/algos/mpt.py
--rw-r--r--   0        0        0     1945 2021-09-09 10:23:27.149667 universal-portfolios-0.4.8/universal/algos/olmar.py
--rw-r--r--   0        0        0     1836 2021-08-30 12:17:08.488998 universal-portfolios-0.4.8/universal/algos/ons.py
--rw-r--r--   0        0        0     2502 2021-08-30 12:17:12.553434 universal-portfolios-0.4.8/universal/algos/pamr.py
--rw-r--r--   0        0        0     1547 2021-08-30 12:17:16.993512 universal-portfolios-0.4.8/universal/algos/rmr.py
--rw-r--r--   0        0        0     2691 2021-08-18 20:48:46.928559 universal-portfolios-0.4.8/universal/algos/rprt.py
--rw-r--r--   0        0        0     2745 2021-08-18 20:48:46.928963 universal-portfolios-0.4.8/universal/algos/single_index_covariance_estimator.py
--rw-r--r--   0        0        0     2671 2021-09-09 10:23:27.178766 universal-portfolios-0.4.8/universal/algos/tco.py
--rw-r--r--   0        0        0       23 2021-08-18 20:48:46.929334 universal-portfolios-0.4.8/universal/algos/ternary/__init__.py
--rw-r--r--   0        0        0     5170 2021-08-18 20:48:46.929795 universal-portfolios-0.4.8/universal/algos/ternary/plotting.py
--rw-r--r--   0        0        0     2516 2021-08-30 12:17:22.267823 universal-portfolios-0.4.8/universal/algos/up.py
--rw-r--r--   0        0        0     1163 2021-08-30 12:17:26.958808 universal-portfolios-0.4.8/universal/algos/wmamr.py
--rw-r--r--   0        0        0     2569 2021-08-18 20:48:46.931074 universal-portfolios-0.4.8/universal/asset_filters.py
--rw-r--r--   0        0        0   286928 2020-09-01 07:16:39.677995 universal-portfolios-0.4.8/universal/data/djia.csv
--rw-r--r--   0        0        0   207540 2020-11-11 16:10:11.950669 universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-eur-2021.xlsx
--rw-r--r--   0        0        0   535651 2020-11-11 16:08:24.998576 universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2018.xlsx
--rw-r--r--   0        0        0   266509 2020-11-11 16:08:25.020368 universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2019.xlsx
--rw-r--r--   0        0        0   184470 2020-11-11 16:08:25.034282 universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2020.xlsx
--rw-r--r--   0        0        0   225647 2020-11-11 16:10:02.083013 universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2021.xlsx
--rw-r--r--   0        0        0   471465 2020-09-01 07:16:39.681854 universal-portfolios-0.4.8/universal/data/msci.csv
--rw-r--r--   0        0        0  2735914 2021-03-03 07:59:41.899912 universal-portfolios-0.4.8/universal/data/nyse_n.csv
--rw-r--r--   0        0        0  3760958 2021-03-03 07:59:41.918239 universal-portfolios-0.4.8/universal/data/nyse_o.csv
--rw-r--r--   0        0        0   597132 2020-09-01 07:16:39.733245 universal-portfolios-0.4.8/universal/data/sp500.csv
--rw-r--r--   0        0        0  2079522 2020-09-01 07:16:39.747054 universal-portfolios-0.4.8/universal/data/tse.csv
--rw-r--r--   0        0        0    17816 2022-03-31 13:05:36.484690 universal-portfolios-0.4.8/universal/result.py
--rw-r--r--   0        0        0    21183 2022-01-05 12:34:47.088662 universal-portfolios-0.4.8/universal/tools.py
--rw-r--r--   0        0        0    10291 2022-07-04 20:03:14.578120 universal-portfolios-0.4.8/setup.py
--rw-r--r--   0        0        0     9029 2022-07-04 20:03:14.578683 universal-portfolios-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1162 2020-09-01 07:13:59.863893 universal-portfolios-0.4.9/LICENSE
+-rw-r--r--   0        0        0     7817 2021-09-09 10:19:25.328399 universal-portfolios-0.4.9/README.md
+-rw-r--r--   0        0        0      909 2022-07-05 06:31:45.560689 universal-portfolios-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       24 2021-08-18 20:48:46.919705 universal-portfolios-0.4.9/universal/__init__.py
+-rw-r--r--   0        0        0    11482 2021-09-09 09:07:59.866133 universal-portfolios-0.4.9/universal/algo.py
+-rw-r--r--   0        0        0      527 2021-09-09 10:23:27.407453 universal-portfolios-0.4.9/universal/algos/__init__.py
+-rw-r--r--   0        0        0     1728 2021-08-18 20:48:46.920679 universal-portfolios-0.4.9/universal/algos/_up_deprecated.py
+-rw-r--r--   0        0        0     4853 2021-08-30 12:16:19.300827 universal-portfolios-0.4.9/universal/algos/anticor.py
+-rw-r--r--   0        0        0      902 2021-08-18 20:48:46.921563 universal-portfolios-0.4.9/universal/algos/bah.py
+-rw-r--r--   0        0        0      791 2021-09-29 10:38:32.687285 universal-portfolios-0.4.9/universal/algos/bcrp.py
+-rw-r--r--   0        0        0     1250 2021-09-29 10:48:26.544681 universal-portfolios-0.4.9/universal/algos/best_markowitz.py
+-rw-r--r--   0        0        0     1154 2021-09-29 10:49:11.075005 universal-portfolios-0.4.9/universal/algos/best_so_far.py
+-rw-r--r--   0        0        0     1762 2021-08-30 12:16:38.354403 universal-portfolios-0.4.9/universal/algos/bnn.py
+-rw-r--r--   0        0        0     3809 2021-08-30 12:13:20.217489 universal-portfolios-0.4.9/universal/algos/corn.py
+-rw-r--r--   0        0        0     2962 2021-08-18 20:48:46.924030 universal-portfolios-0.4.9/universal/algos/crp.py
+-rw-r--r--   0        0        0     4450 2021-08-30 12:16:43.225819 universal-portfolios-0.4.9/universal/algos/cwmr.py
+-rw-r--r--   0        0        0      985 2021-08-30 12:16:47.257846 universal-portfolios-0.4.9/universal/algos/dynamic_crp.py
+-rw-r--r--   0        0        0      901 2021-08-30 12:16:51.801265 universal-portfolios-0.4.9/universal/algos/eg.py
+-rw-r--r--   0        0        0    26623 2022-07-05 06:15:52.991998 universal-portfolios-0.4.9/universal/algos/estimators.py
+-rw-r--r--   0        0        0     4074 2021-08-30 12:16:58.257631 universal-portfolios-0.4.9/universal/algos/kelly.py
+-rw-r--r--   0        0        0    16271 2021-08-18 20:48:46.926640 universal-portfolios-0.4.9/universal/algos/mpt.py
+-rw-r--r--   0        0        0     1945 2021-09-09 10:23:27.149667 universal-portfolios-0.4.9/universal/algos/olmar.py
+-rw-r--r--   0        0        0     1836 2021-08-30 12:17:08.488998 universal-portfolios-0.4.9/universal/algos/ons.py
+-rw-r--r--   0        0        0     2502 2021-08-30 12:17:12.553434 universal-portfolios-0.4.9/universal/algos/pamr.py
+-rw-r--r--   0        0        0     1547 2021-08-30 12:17:16.993512 universal-portfolios-0.4.9/universal/algos/rmr.py
+-rw-r--r--   0        0        0     2691 2021-08-18 20:48:46.928559 universal-portfolios-0.4.9/universal/algos/rprt.py
+-rw-r--r--   0        0        0     2745 2021-08-18 20:48:46.928963 universal-portfolios-0.4.9/universal/algos/single_index_covariance_estimator.py
+-rw-r--r--   0        0        0     2671 2021-09-09 10:23:27.178766 universal-portfolios-0.4.9/universal/algos/tco.py
+-rw-r--r--   0        0        0       23 2021-08-18 20:48:46.929334 universal-portfolios-0.4.9/universal/algos/ternary/__init__.py
+-rw-r--r--   0        0        0     5170 2021-08-18 20:48:46.929795 universal-portfolios-0.4.9/universal/algos/ternary/plotting.py
+-rw-r--r--   0        0        0     2516 2021-08-30 12:17:22.267823 universal-portfolios-0.4.9/universal/algos/up.py
+-rw-r--r--   0        0        0     1163 2021-08-30 12:17:26.958808 universal-portfolios-0.4.9/universal/algos/wmamr.py
+-rw-r--r--   0        0        0     2569 2021-08-18 20:48:46.931074 universal-portfolios-0.4.9/universal/asset_filters.py
+-rw-r--r--   0        0        0   286928 2020-09-01 07:16:39.677995 universal-portfolios-0.4.9/universal/data/djia.csv
+-rw-r--r--   0        0        0   207540 2020-11-11 16:10:11.950669 universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-eur-2021.xlsx
+-rw-r--r--   0        0        0   535651 2020-11-11 16:08:24.998576 universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2018.xlsx
+-rw-r--r--   0        0        0   266509 2020-11-11 16:08:25.020368 universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2019.xlsx
+-rw-r--r--   0        0        0   184470 2020-11-11 16:08:25.034282 universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2020.xlsx
+-rw-r--r--   0        0        0   225647 2020-11-11 16:10:02.083013 universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2021.xlsx
+-rw-r--r--   0        0        0   471465 2020-09-01 07:16:39.681854 universal-portfolios-0.4.9/universal/data/msci.csv
+-rw-r--r--   0        0        0  2735914 2021-03-03 07:59:41.899912 universal-portfolios-0.4.9/universal/data/nyse_n.csv
+-rw-r--r--   0        0        0  3760958 2021-03-03 07:59:41.918239 universal-portfolios-0.4.9/universal/data/nyse_o.csv
+-rw-r--r--   0        0        0   597132 2020-09-01 07:16:39.733245 universal-portfolios-0.4.9/universal/data/sp500.csv
+-rw-r--r--   0        0        0  2079522 2020-09-01 07:16:39.747054 universal-portfolios-0.4.9/universal/data/tse.csv
+-rw-r--r--   0        0        0    17831 2022-07-05 06:27:33.813288 universal-portfolios-0.4.9/universal/result.py
+-rw-r--r--   0        0        0    21227 2022-07-05 06:34:22.848534 universal-portfolios-0.4.9/universal/tools.py
+-rw-r--r--   0        0        0    10293 2022-07-05 06:35:29.903125 universal-portfolios-0.4.9/setup.py
+-rw-r--r--   0        0        0     9031 2022-07-05 06:35:29.903921 universal-portfolios-0.4.9/PKG-INFO
```

### Comparing `universal-portfolios-0.4.8/LICENSE` & `universal-portfolios-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/README.md` & `universal-portfolios-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/pyproject.toml` & `universal-portfolios-0.4.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "universal-portfolios"
-version = "0.4.8"
+version = "0.4.9"
 description = "Collection of algorithms for online portfolio selection"
 readme = "README.md"
 repository = "https://github.com/Marigold/universal-portfolios"
 authors = ["Marigold <mojmir.vinkler@gmail.com>"]
 packages = [
     { include = "universal" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-scipy = "^1.5.2"
+python = ">=3.8,<3.11"
+scipy = "^1.8.1"
 matplotlib = "^3.3.1"
 pandas-datareader = "^0.10.0"
 statsmodels = "^0.13.2"
 scikit-learn = "^1.1.1"
 seaborn = "^0.10.1"
 requests = "^2.24.0"
 plotly = "^4.9.0"
 pandas = "^1.1.1"
 cvxopt = "1.2.5"
 tqdm = "^4.56.2"
 typing-extensions = "^3.10.0"
 urllib3 = "^1.26.6"
-Pillow = "^8.3.2"
+Pillow = "^9.2.0"
 lxml = "^4.6.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 ipdb = "^0.13.3"
 line-profiler = "^3.0.2"
 ipykernel = "^5.3.4"
```

### Comparing `universal-portfolios-0.4.8/universal/algo.py` & `universal-portfolios-0.4.9/universal/algo.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/__init__.py` & `universal-portfolios-0.4.9/universal/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/_up_deprecated.py` & `universal-portfolios-0.4.9/universal/algos/_up_deprecated.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/anticor.py` & `universal-portfolios-0.4.9/universal/algos/anticor.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/bah.py` & `universal-portfolios-0.4.9/universal/algos/bah.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/bcrp.py` & `universal-portfolios-0.4.9/universal/algos/bcrp.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/best_markowitz.py` & `universal-portfolios-0.4.9/universal/algos/best_markowitz.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/best_so_far.py` & `universal-portfolios-0.4.9/universal/algos/best_so_far.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/bnn.py` & `universal-portfolios-0.4.9/universal/algos/bnn.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/corn.py` & `universal-portfolios-0.4.9/universal/algos/corn.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/crp.py` & `universal-portfolios-0.4.9/universal/algos/crp.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/cwmr.py` & `universal-portfolios-0.4.9/universal/algos/cwmr.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/dynamic_crp.py` & `universal-portfolios-0.4.9/universal/algos/dynamic_crp.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/eg.py` & `universal-portfolios-0.4.9/universal/algos/eg.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/estimators.py` & `universal-portfolios-0.4.9/universal/algos/estimators.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/kelly.py` & `universal-portfolios-0.4.9/universal/algos/kelly.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/mpt.py` & `universal-portfolios-0.4.9/universal/algos/mpt.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/olmar.py` & `universal-portfolios-0.4.9/universal/algos/olmar.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/ons.py` & `universal-portfolios-0.4.9/universal/algos/ons.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/pamr.py` & `universal-portfolios-0.4.9/universal/algos/pamr.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/rmr.py` & `universal-portfolios-0.4.9/universal/algos/rmr.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/rprt.py` & `universal-portfolios-0.4.9/universal/algos/rprt.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/single_index_covariance_estimator.py` & `universal-portfolios-0.4.9/universal/algos/single_index_covariance_estimator.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/tco.py` & `universal-portfolios-0.4.9/universal/algos/tco.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/ternary/plotting.py` & `universal-portfolios-0.4.9/universal/algos/ternary/plotting.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/up.py` & `universal-portfolios-0.4.9/universal/algos/up.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/algos/wmamr.py` & `universal-portfolios-0.4.9/universal/algos/wmamr.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/asset_filters.py` & `universal-portfolios-0.4.9/universal/asset_filters.py`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/djia.csv` & `universal-portfolios-0.4.9/universal/data/djia.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-eur-2021.xlsx` & `universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-eur-2021.xlsx`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2018.xlsx` & `universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2018.xlsx`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2019.xlsx` & `universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2019.xlsx`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2020.xlsx` & `universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2020.xlsx`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/jpm_assumptions/jpm-matrix-usd-2021.xlsx` & `universal-portfolios-0.4.9/universal/data/jpm_assumptions/jpm-matrix-usd-2021.xlsx`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/msci.csv` & `universal-portfolios-0.4.9/universal/data/msci.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/nyse_n.csv` & `universal-portfolios-0.4.9/universal/data/nyse_n.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/nyse_o.csv` & `universal-portfolios-0.4.9/universal/data/nyse_o.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/sp500.csv` & `universal-portfolios-0.4.9/universal/data/sp500.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/data/tse.csv` & `universal-portfolios-0.4.9/universal/data/tse.csv`

 * *Files identical despite different names*

### Comparing `universal-portfolios-0.4.8/universal/result.py` & `universal-portfolios-0.4.9/universal/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,15 @@
             return [ax1]
         else:
             if show_only_important:
                 ix = self.B.abs().sum().nlargest(n=20).index
                 B = self.B.loc[:, ix].copy()
                 assets = B.columns if assets else False
                 if B.shape[1] > 20:
-                    B["_others"] = self.B.drop(ix, 1).sum(1)
+                    B["_others"] = self.B.drop(ix, axis=1).sum(1)
             else:
                 B = self.B.copy()
 
             figsize = plt.rcParams["figure.figsize"]
             plt.figure(1, figsize=(figsize[0] * 2, figsize[1] * 1.5))
             ax1 = plt.subplot2grid((3, 1), (0, 0), rowspan=2)
             res.plot(assets=assets, ax=ax1, color=color, **kwargs)
@@ -415,24 +415,24 @@
             if color is None:
                 color = _colors_hash(B.columns)
             else:
                 # remove first color used for portfolio
                 color = color[1:]
 
             # plot weights as lines
-            if B.drop(["CASH"], 1, errors="ignore").values.min() < -0.01:
+            if B.drop(["CASH"], axis=1, errors="ignore").values.min() < -0.01:
                 B.plot(
                     ax=ax2,
                     ylim=(min(0.0, B.values.min()), max(1.0, B.values.max())),
                     legend=False,
                     color=_colors_hash(B.columns),
                 )
             # plot weights as area chart
             else:
-                B = B.drop("CASH", 1, errors="ignore")
+                B = B.drop("CASH", axis=1, errors="ignore")
                 # fix rounding errors near zero
                 if B.values.min() < 0:
                     pB = B - B.values.min()
                 else:
                     pB = B
                 pB.plot(
                     ax=ax2,
```

### Comparing `universal-portfolios-0.4.8/universal/tools.py` & `universal-portfolios-0.4.9/universal/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,19 +735,20 @@
         "KBE",
         "USDU",
         "UUP",
         "TYD",
     ]
 
 
-def same_vol(S, target=None):
+def same_vol(S, target=None, target_vol=None):
     R = S.pct_change().drop("RFR", axis=1)
     rfr = S["RFR"]
     vol = R.std()
-    target_vol = vol[target] if target else vol.mean()
+    if not target_vol:
+        target_vol = vol[target] if target else vol.mean()
     leverage = target_vol / vol
     R = (leverage * (R.sub(rfr / 252, axis=0))).add(rfr / 252, axis=0)
     S = (1 + R.fillna(0)).cumprod()
     S["RFR"] = rfr
     return S
```

### Comparing `universal-portfolios-0.4.8/setup.py` & `universal-portfolios-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,41 +41,41 @@
                'data/tse.csv',
                'data/tse.csv',
                'data/tse.csv',
                'data/tse.csv',
                'data/tse.csv']}
 
 install_requires = \
-['Pillow>=8.3.2,<9.0.0',
+['Pillow>=9.2.0,<10.0.0',
  'cvxopt==1.2.5',
  'lxml>=4.6.3,<5.0.0',
  'matplotlib>=3.3.1,<4.0.0',
  'pandas-datareader>=0.10.0,<0.11.0',
  'pandas>=1.1.1,<2.0.0',
  'plotly>=4.9.0,<5.0.0',
  'requests>=2.24.0,<3.0.0',
  'scikit-learn>=1.1.1,<2.0.0',
- 'scipy>=1.5.2,<2.0.0',
+ 'scipy>=1.8.1,<2.0.0',
  'seaborn>=0.10.1,<0.11.0',
  'statsmodels>=0.13.2,<0.14.0',
  'tqdm>=4.56.2,<5.0.0',
  'typing-extensions>=3.10.0,<4.0.0',
  'urllib3>=1.26.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'universal-portfolios',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Collection of algorithms for online portfolio selection',
     'long_description': '# Universal Portfolios\n\n![PyPi Version](https://img.shields.io/pypi/v/universal-portfolios?style=flat-square)\n![PyPi License](https://img.shields.io/pypi/l/universal-portfolios?style=flat-square)\n![PyPi Downloads](https://img.shields.io/pypi/dm/universal-portfolios?style=flat-square)\n\n![Open PRs](https://img.shields.io/github/issues-pr-raw/Marigold/universal-portfolios?style=flat-square)\n![Contributors](https://img.shields.io/badge/contributors-9-orange.svg?style=flat-square)\n![Repo size](https://img.shields.io/github/repo-size/Marigold/universal-portfolios?style=flat-square)\n\n\nThe purpose of this Python package is to put together different Online Portfolio Selection (OLPS) algorithms and provide unified tools for their analysis.\n\n\nIn short, the purpose of OLPS is to _choose portfolio weights in every period to maximize its final wealth_. Examples of such portfolios could be the [Markowitz portfolio](http://en.wikipedia.org/wiki/Modern_portfolio_theory) or the [Universal portfolio](http://en.wikipedia.org/wiki/Universal_portfolio_algorithm). There is currently an active research in the area of online portfolios and even though the results are mostly theoretical, algorithms for practical use start to appear.\n\nSeveral state-of-the-art algorithms are implemented, based on my understanding of the available literature. Contributions or corrections are more than welcomed.\n\n## Outline of this package\n\n* `examples` contains two Python Notebooks:\n   - [Online Portfolios](http://nbviewer.ipython.org/github/Marigold/universal-portfolios/blob/master/On-line%20portfolios.ipynb) : explains the basic use of the library. Script sequence, various options, method arguments, and a strategy template to get you started.\n   - [Modern Portfolio Theory](http://nbviewer.ipython.org/github/Marigold/universal-portfolios/blob/master/modern-portfolio-theory.ipynb) : goes deeper into the OLPS principle and the tools developped in this library to approach it.\n\n* `universal.data` contains various datasets to help you in your journey\n\n* `universal.algos` hosts the implementations of various OLPS algorithms from the litterature :\n\n<div align="center">\n\n| Benchmarks | Follow the winner | Follow the loser | Pattern matching | Other |\n|---|---|---|---|---|\n| __[BAH](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/bah.py)__ | __[Universal Portfolios](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/up.py)__ | __[Anticorr](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/anticor.py)__ | __[BNN](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/bnn.py)__ | __[Markovitz](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/best_markowitz.py)__ |\n| __[CRP](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/crp.py)__ | __[Exponential Gradient](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/eg.py)__ | __[PAMR](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/pamr.py)__ | __[CORN](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/corn.py)__ | __[Kelly](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/kelly.py)__ |\n| __[BCRP](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/bcrp.py)__ || __[OLMAR](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/olmar.py)__ || __[Best so far](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/best_so_far.py)__ |\n| __[DCRP](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/dynamic_crp.py)__ || __[RMR](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/rmr.py)__ || __[ONS](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/ons.py)__ |\n||| __[CWMR](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/cwmr.py)__ || __[MPT](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/mpt.py)__ |\n||| __[WMAMR](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/wmamr.py)__ |||\n||| __[RPRT](https://github.com/Marigold/universal-portfolios/blob/master/universal/algos/rprt.py)__ |||\n\n</div>\n\n\n* `universal.algo` provides a general class inherited by all the individual algos\' subclasses. Algo computes the weights at every timestep.\n\n* `universal.result` computes the portfolio wealth from the weights and various metrics on the strategy\'s performance.\n\n\n## Quick Start\n\n```python\nfrom universal import tools\nfrom universal.algos import CRP\n\nif __name__ == \'__main__\':\n  # Run CRP on a computed-generated portfolio of 3 stocks and plot the results\n  tools.quickrun(CRP())\n\n```\n\n\n## Additional Resources\n\nIf you do not know what online portfolio is, look at [Ernest Chan blog](http://epchan.blogspot.cz/2007/01/universal-portfolios.html), [CASTrader](http://www.castrader.com/2006/11/universal_portf.html) or a recent [survey by Bin Li and Steven C. H. Hoi](http://arxiv.org/abs/1212.2129).\n\nPaul Perry followed up on this and made a [comparison of all algorithms](http://nbviewer.ipython.org/github/paulperry/quant/blob/master/OLPS_Comparison.ipynb) on more recent ETF datasets. The original authors of some of the algorithms recently published their own implementation on GitHub - [Online Portfolio Selection Toolbox](https://github.com/OLPS/OLPS) in MATLAB.\n\nIf you are more into R or just looking for a good resource about Universal Portfolios, check out blog and package [logopt](http://optimallog.blogspot.cz/) by Marc Delvaux.\n\nNote : If you don\'t want to install the package locally, you can run both notebooks with Binder - [modern-portfolio-theory.ipynb ![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Marigold/universal-portfolios/master?filepath=modern-portfolio-theory.ipynb) or [On-line portfolios.ipynb ![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Marigold/universal-portfolios/master?filepath=On-line%20portfolios.ipynb)\n\n## Installation\n\nOnly Python 3 is supported\n\n```\npip install universal-portfolios\n```\n\n## Development\n\n[poetry](https://python-poetry.org/) is used to manage the dependencies. Run `poetry install` to install a virtual environment and then `poetry shell` to launch it.\n\nExporting dependencies to the `requirements.txt` file is needed for mybinder.org. It is done via\n\n```\npoetry export --without-hashes -f requirements.txt > requirements.txt\n```\n\n### Formatting\n\nWe use pre-commit hook to automatically format code and check for linting errors before each commit. If the checks fail you need to resolve the errors and amend the change set.\n\nTo setup the pre-commit hooks you need to [install it first](https://pre-commit.com/#installation) and then enter the project root directory and invoke the command (only once!):\n\n```\npre-commit install\n```\n\n\n## Running Tests\n\n```\npoetry run python -m pytest --capture=no --ff -x tests/\n```\n\n## Contributors\n\nCreator : [Marigold](https://github.com/Marigold)\n\n_Thank you for your contributions!_\n\n[Alexander Myltsev](https://github.com/alexander-myltsev) | [angonyfox](https://github.com/angonyfox) | [booxter](https://github.com/booxter) | [dexhunter](https://github.com/dexhunter) | [DrPaprikaa](https://github.com/DrPaprikaa) | [paulorodriguesxv](https://github.com/paulorodriguesxv) | [stergnator](https://github.com/stergnator) | [Xander Dunn](https://github.com/xanderdunn)\n\n## Disclaimer\n\nThis software is for educational purposes only and is far from any production environment. Do not risk money which you are afraid to lose.\nUse the software at your own risk. The authors assume no responsibility for your trading results.\n',
     'author': 'Marigold',
     'author_email': 'mojmir.vinkler@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Marigold/universal-portfolios',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `universal-portfolios-0.4.8/PKG-INFO` & `universal-portfolios-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: universal-portfolios
-Version: 0.4.8
+Version: 0.4.9
 Summary: Collection of algorithms for online portfolio selection
 Home-page: https://github.com/Marigold/universal-portfolios
 Author: Marigold
 Author-email: mojmir.vinkler@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pillow (>=8.3.2,<9.0.0)
+Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: cvxopt (==1.2.5)
 Requires-Dist: lxml (>=4.6.3,<5.0.0)
 Requires-Dist: matplotlib (>=3.3.1,<4.0.0)
 Requires-Dist: pandas (>=1.1.1,<2.0.0)
 Requires-Dist: pandas-datareader (>=0.10.0,<0.11.0)
 Requires-Dist: plotly (>=4.9.0,<5.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: scipy (>=1.5.2,<2.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: seaborn (>=0.10.1,<0.11.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tqdm (>=4.56.2,<5.0.0)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Project-URL: Repository, https://github.com/Marigold/universal-portfolios
 Description-Content-Type: text/markdown
```

