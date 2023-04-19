# Comparing `tmp/fold_core-0.0.5.tar.gz` & `tmp/fold_core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "fold_core-0.0.6.tar", max compression
```

## Comparing `fold_core-0.0.5.tar` & `fold_core-0.0.6.tar`

### file list

```diff
@@ -1,55 +1,53 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fold_core-0.0.5/.flake8
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/py.typed
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/splitters.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/__init__.py
--rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/columns.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/common.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/concat.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/residual.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/sample.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/select.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/target.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backtesting.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/checks.py
--rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/common.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/convenience.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/encase.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/memory.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/training.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/types.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/__init__.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/base.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/baseline.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/dummy.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/random.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/sklearn.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/__init__.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/columns.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/date.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/dev.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/difference.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/function.py
--rw-r--r--   0        0        0     6393 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/lags.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/math.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/update.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/window.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/checks.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/dataset.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/list.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/tests.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/trim.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 fold_core-0.0.5/.gitignore
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 fold_core-0.0.5/LICENSE
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 fold_core-0.0.5/README.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fold_core-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fold_core-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-19 12:58:38.109536 fold_core-0.0.6/LICENSE
+-rw-r--r--   0        0        0    10163 2023-04-19 12:58:38.109536 fold_core-0.0.6/README.md
+-rw-r--r--   0        0        0     3601 2023-04-19 12:58:38.141536 fold_core-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      298 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/__init__.py
+-rw-r--r--   0        0        0     5097 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/base.py
+-rw-r--r--   0        0        0      353 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10085 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1401 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6096 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2050 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6183 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4584 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3085 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     1888 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4369 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/target.py
+-rw-r--r--   0        0        0      169 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2232 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1755 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3022 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      414 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9746 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/common.py
+-rw-r--r--   0        0        0     1933 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     6962 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2817 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     5559 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1669 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/types.py
+-rw-r--r--   0        0        0      205 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3036 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/base.py
+-rw-r--r--   0        0        0     1751 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4173 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2011 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/random.py
+-rw-r--r--   0        0        0     4134 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/py.typed
+-rw-r--r--   0        0        0     6548 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/splitters.py
+-rw-r--r--   0        0        0      752 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     5858 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8417 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4088 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2730 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      622 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6393 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5499 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7397 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3558 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      711 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4238 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     1995 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     2064 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1415 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2779 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1540 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12781 1970-01-01 00:00:00.000000 fold_core-0.0.6/PKG-INFO
```

### Comparing `fold_core-0.0.5/fold/base.py` & `fold_core-0.0.6/src/fold/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/splitters.py` & `fold_core-0.0.6/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/columns.py` & `fold_core-0.0.6/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/common.py` & `fold_core-0.0.6/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/concat.py` & `fold_core-0.0.6/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/ensemble.py` & `fold_core-0.0.6/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/metalabeling.py` & `fold_core-0.0.6/src/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/residual.py` & `fold_core-0.0.6/src/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/sample.py` & `fold_core-0.0.6/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/select.py` & `fold_core-0.0.6/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/composites/target.py` & `fold_core-0.0.6/src/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/backtesting.py` & `fold_core-0.0.6/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/common.py` & `fold_core-0.0.6/src/fold/loop/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/convenience.py` & `fold_core-0.0.6/src/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/encase.py` & `fold_core-0.0.6/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/memory.py` & `fold_core-0.0.6/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/training.py` & `fold_core-0.0.6/src/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/types.py` & `fold_core-0.0.6/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/backend/__init__.py` & `fold_core-0.0.6/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/backend/ray.py` & `fold_core-0.0.6/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/loop/backend/sequential.py` & `fold_core-0.0.6/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/models/base.py` & `fold_core-0.0.6/src/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/models/baseline.py` & `fold_core-0.0.6/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/models/dummy.py` & `fold_core-0.0.6/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/models/random.py` & `fold_core-0.0.6/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/models/sklearn.py` & `fold_core-0.0.6/src/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/__init__.py` & `fold_core-0.0.6/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/columns.py` & `fold_core-0.0.6/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/date.py` & `fold_core-0.0.6/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/dev.py` & `fold_core-0.0.6/src/fold/transformations/dev.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/difference.py` & `fold_core-0.0.6/src/fold/transformations/difference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/function.py` & `fold_core-0.0.6/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/holidays.py` & `fold_core-0.0.6/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/lags.py` & `fold_core-0.0.6/src/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/math.py` & `fold_core-0.0.6/src/fold/transformations/math.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/sklearn.py` & `fold_core-0.0.6/src/fold/transformations/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/update.py` & `fold_core-0.0.6/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/transformations/window.py` & `fold_core-0.0.6/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/utils/checks.py` & `fold_core-0.0.6/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/utils/dataset.py` & `fold_core-0.0.6/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/utils/list.py` & `fold_core-0.0.6/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/utils/tests.py` & `fold_core-0.0.6/src/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/fold/utils/trim.py` & `fold_core-0.0.6/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/LICENSE` & `fold_core-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/README.md` & `fold_core-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.5/PKG-INFO` & `fold_core-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
-Project-URL: Documentation, https://dream-faster.github.io/fold
-Project-URL: Issues, https://github.com/dream-faster/fold/issues
-Project-URL: Source, https://github.com/dream-faster/fold
-Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
-License-File: LICENSE
+License: Proprietary
+Author: Mark Aron Szulyovszky
+Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: iteration-utilities
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
-Requires-Dist: tqdm
 Provides-Extra: docs
-Requires-Dist: image; extra == 'docs'
-Requires-Dist: mkdocs-autorefs; extra == 'docs'
-Requires-Dist: mkdocs-gallery; extra == 'docs'
-Requires-Dist: mkdocs-glightbox; extra == 'docs'
-Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
-Requires-Dist: mkdocs-jupyter; extra == 'docs'
-Requires-Dist: mkdocs-material; extra == 'docs'
-Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: extras
-Requires-Dist: holidays; extra == 'extras'
-Requires-Dist: krisi~=0.0.8; extra == 'extras'
-Requires-Dist: ray; extra == 'extras'
 Provides-Extra: quality
-Requires-Dist: black~=22.12.0; extra == 'quality'
-Requires-Dist: flake8~=4.0.1; extra == 'quality'
-Requires-Dist: isort~=5.10.1; extra == 'quality'
-Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Provides-Extra: ray
-Requires-Dist: ray; extra == 'ray'
 Provides-Extra: tests
-Requires-Dist: holidays; extra == 'tests'
-Requires-Dist: imbalanced-learn; extra == 'tests'
-Requires-Dist: pytest-cov>=4.0; extra == 'tests'
-Requires-Dist: pytest~=7.1.2; extra == 'tests'
+Requires-Dist: black (>=22.12.0,<22.13.0) ; extra == "quality"
+Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
+Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
+Requires-Dist: image (>=1.5.33) ; extra == "docs"
+Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests"
+Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
+Requires-Dist: iteration_utilities (>=0.11)
+Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "extras"
+Requires-Dist: mkdocs-autorefs (>=0.4.0) ; extra == "docs"
+Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra == "docs"
+Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs"
+Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
+Requires-Dist: mkdocs-jupyter (>=0.24.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=9.0.0) ; extra == "docs"
+Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
+Requires-Dist: numpy (>=1.16)
+Requires-Dist: pandas (>=1.2)
+Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality"
+Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests"
+Requires-Dist: pytest-cov (>=4.0) ; extra == "tests"
+Requires-Dist: ray (>=1.4.0) ; extra == "ray" or extra == "extras"
+Requires-Dist: scikit-learn (>=0.22)
+Requires-Dist: tqdm (>=4.0)
 Description-Content-Type: text/markdown
 
 <!-- # Fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://dream-faster.github.io/fold/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/fold/docs.yaml?logo=readthedocs"></a>
   <a style="margin:2px" href="https://codecov.io/gh/dream-faster/fold" ><img src="https://codecov.io/gh/dream-faster/fold/branch/main/graph/badge.svg?token=Z7I2XSF188"/></a>
@@ -266,7 +267,8 @@
 
 [Read more](https://dream-faster.github.io/fold/product/license/)
 
 ## Limitations
 
 - No intermittent time series support, very limited support for missing values.
 - No hierarchical time series support.
+
```

#### html2text {}

```diff
@@ -1,40 +1,42 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.0.5 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.0.6 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
-rigour. Project-URL: Documentation, https://dream-faster.github.io/fold
-Project-URL: Issues, https://github.com/dream-faster/fold/issues Project-URL:
-Source, https://github.com/dream-faster/fold Author-email: Mark Aron
-Szulyovszky
-dreamfaster.ai>, Daniel Szemerey
-dreamfaster.ai> License-File: LICENSE Classifier: Development Status :: 5 -
-Production/Stable Classifier: License :: Other/Proprietary License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
+rigour. License: Proprietary Author: Mark Aron Szulyovszky Requires-Python:
+>=3.7 Classifier: Development Status :: 5 - Production/Stable Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Requires-Python: >=3.7 Requires-Dist: iteration-
-utilities Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: scikit-
-learn Requires-Dist: tqdm Provides-Extra: docs Requires-Dist: image; extra ==
-'docs' Requires-Dist: mkdocs-autorefs; extra == 'docs' Requires-Dist: mkdocs-
-gallery; extra == 'docs' Requires-Dist: mkdocs-glightbox; extra == 'docs'
-Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs' Requires-Dist:
-mkdocs-jupyter; extra == 'docs' Requires-Dist: mkdocs-material; extra == 'docs'
-Requires-Dist: mkdocstrings-python; extra == 'docs' Provides-Extra: extras
-Requires-Dist: holidays; extra == 'extras' Requires-Dist: krisi~=0.0.8; extra
-== 'extras' Requires-Dist: ray; extra == 'extras' Provides-Extra: quality
-Requires-Dist: black~=22.12.0; extra == 'quality' Requires-Dist: flake8~=4.0.1;
-extra == 'quality' Requires-Dist: isort~=5.10.1; extra == 'quality' Requires-
-Dist: pre-commit~=2.20.0; extra == 'quality' Provides-Extra: ray Requires-Dist:
-ray; extra == 'ray' Provides-Extra: tests Requires-Dist: holidays; extra ==
-'tests' Requires-Dist: imbalanced-learn; extra == 'tests' Requires-Dist:
-pytest-cov>=4.0; extra == 'tests' Requires-Dist: pytest~=7.1.2; extra ==
-'tests' Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy Provides-
+Extra: docs Provides-Extra: extras Provides-Extra: quality Provides-Extra: ray
+Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ; extra ==
+"quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality" Requires-
+Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras" Requires-Dist:
+image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-learn (>=0.7.0) ;
+extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
+Requires-Dist: iteration_utilities (>=0.11) Requires-Dist: krisi
+(>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs-autorefs (>=0.4.0) ;
+extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra == "docs"
+Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs" Requires-Dist:
+mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist: mkdocs-
+jupyter (>=0.24.0) ; extra == "docs" Requires-Dist: mkdocs-material (>=9.0.0) ;
+extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
+Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2) Requires-Dist: pre-
+commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-Dist: pytest
+(>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov (>=4.0) ; extra
+== "tests" Requires-Dist: ray (>=1.4.0) ; extra == "ray" or extra == "extras"
+Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm (>=4.0) Description-
+Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                  (/fold/) ****
   A Time_Series_Continuous_Validation library that lets you build, deploy and
```

