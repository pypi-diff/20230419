# Comparing `tmp/fold_core-0.0.4.tar.gz` & `tmp/fold_core-0.0.5.tar.gz`

## Comparing `fold_core-0.0.4.tar` & `fold_core-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,55 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fold_core-0.0.4/.flake8
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fold_core-0.0.4/codecov.yml
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fold_core-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/py.typed
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/splitters.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/common.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/sample.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/select.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/composites/target.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/common.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/training.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/types.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/base.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/random.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/models/sklearn.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6393 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/transformations/window.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/utils/list.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 fold_core-0.0.4/src/fold/utils/trim.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 fold_core-0.0.4/.gitignore
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 fold_core-0.0.4/LICENSE
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 fold_core-0.0.4/README.md
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 fold_core-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    12448 2020-02-02 00:00:00.000000 fold_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fold_core-0.0.5/.flake8
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/__init__.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/py.typed
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/splitters.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/columns.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/common.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/concat.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/residual.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/sample.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/select.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/composites/target.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/checks.py
+-rw-r--r--   0        0        0     9746 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/common.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/convenience.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/encase.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/memory.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/training.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/types.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/__init__.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/base.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/baseline.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/dummy.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/random.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/models/sklearn.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/date.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/difference.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/function.py
+-rw-r--r--   0        0        0     6393 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/math.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/update.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/transformations/window.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/checks.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/list.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/tests.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 fold_core-0.0.5/fold/utils/trim.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 fold_core-0.0.5/.gitignore
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 fold_core-0.0.5/LICENSE
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 fold_core-0.0.5/README.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fold_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fold_core-0.0.5/PKG-INFO
```

### Comparing `fold_core-0.0.4/src/fold/base.py` & `fold_core-0.0.5/fold/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/splitters.py` & `fold_core-0.0.5/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/columns.py` & `fold_core-0.0.5/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/common.py` & `fold_core-0.0.5/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/concat.py` & `fold_core-0.0.5/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/ensemble.py` & `fold_core-0.0.5/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/metalabeling.py` & `fold_core-0.0.5/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/residual.py` & `fold_core-0.0.5/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/sample.py` & `fold_core-0.0.5/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/select.py` & `fold_core-0.0.5/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/composites/target.py` & `fold_core-0.0.5/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/backtesting.py` & `fold_core-0.0.5/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/common.py` & `fold_core-0.0.5/fold/loop/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/convenience.py` & `fold_core-0.0.5/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/encase.py` & `fold_core-0.0.5/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/memory.py` & `fold_core-0.0.5/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/training.py` & `fold_core-0.0.5/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/types.py` & `fold_core-0.0.5/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/backend/__init__.py` & `fold_core-0.0.5/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/backend/ray.py` & `fold_core-0.0.5/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/loop/backend/sequential.py` & `fold_core-0.0.5/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/models/base.py` & `fold_core-0.0.5/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/models/baseline.py` & `fold_core-0.0.5/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/models/dummy.py` & `fold_core-0.0.5/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/models/random.py` & `fold_core-0.0.5/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/models/sklearn.py` & `fold_core-0.0.5/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/__init__.py` & `fold_core-0.0.5/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/columns.py` & `fold_core-0.0.5/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/date.py` & `fold_core-0.0.5/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/dev.py` & `fold_core-0.0.5/fold/transformations/dev.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/difference.py` & `fold_core-0.0.5/fold/transformations/difference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/function.py` & `fold_core-0.0.5/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/holidays.py` & `fold_core-0.0.5/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/lags.py` & `fold_core-0.0.5/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/math.py` & `fold_core-0.0.5/fold/transformations/math.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/sklearn.py` & `fold_core-0.0.5/fold/transformations/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/update.py` & `fold_core-0.0.5/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/transformations/window.py` & `fold_core-0.0.5/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/utils/checks.py` & `fold_core-0.0.5/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/utils/dataset.py` & `fold_core-0.0.5/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/utils/list.py` & `fold_core-0.0.5/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/utils/tests.py` & `fold_core-0.0.5/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/src/fold/utils/trim.py` & `fold_core-0.0.5/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/.gitignore` & `fold_core-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/LICENSE` & `fold_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/README.md` & `fold_core-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.4/pyproject.toml` & `fold_core-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "fold-core"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -25,17 +25,17 @@
 dependencies = [
   "numpy",
   "pandas",
   "tqdm",
   "scikit-learn",
   "iteration_utilities",
 ]
-description = "Timeseries modelling on a rolling/expanding window basis."
+description = "A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour."
 keywords = []
-license = "MIT"
+license-files = { paths = ["LICENSE"] }
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold"
 Issues = "https://github.com/dream-faster/fold/issues"
 Source = "https://github.com/dream-faster/fold"
@@ -68,15 +68,15 @@
   "ray",
   "holidays",
   "krisi~=0.0.8",
 ]
 
 [tool.hatch.envs.quality]
 dependencies = [
-  "fold[quality]"
+  ".[quality]"
 ]
 detached = true
 
 [tool.hatch.envs.quality.scripts]
 check = [
   "flake8 src tests",
   "black --check --diff --preview src tests",
@@ -85,15 +85,15 @@
 format = [
   "isort src tests",
   "black --preview src tests",
   "check",
 ]
 
 [tool.hatch.envs.test]
-dependencies = ["fold[tests]"]
+dependencies = [".[tests]"]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest tests/ --durations 0 -s"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310"]
 
@@ -104,16 +104,22 @@
 exclude = [
   "/.github",
   "/docs",
   "/.devcontainer",
   "/.pre-commit-config.yaml",
   "/.gitignore",
   "/tests",
+  "/.vscode",
+  "mkdocs.yml",
+  "codecov.yml",
 ]
 
+[tool.hatch.build]
+sources = ["src"]
+
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 testpaths = ["tests"]
 addopts = [
   "--doctest-modules",
@@ -121,15 +127,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.0.4/PKG-INFO` & `fold_core-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.0.4
-Summary: Timeseries modelling on a rolling/expanding window basis.
+Version: 0.0.5
+Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 Project-URL: Documentation, https://dream-faster.github.io/fold
 Project-URL: Issues, https://github.com/dream-faster/fold/issues
 Project-URL: Source, https://github.com/dream-faster/fold
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
-License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,38 +1,40 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.0.4 Summary: Timeseries
-modelling on a rolling/expanding window basis. Project-URL: Documentation,
-https://dream-faster.github.io/fold Project-URL: Issues, https://github.com/
-dream-faster/fold/issues Project-URL: Source, https://github.com/dream-faster/
-fold Author-email: Mark Aron Szulyovszky
+Metadata-Version: 2.1 Name: fold-core Version: 0.0.5 Summary: A Time Series
+Cross-Validation library that lets you build, deploy and update composite
+models easily. An order of magnitude speed-up, combined with flexibility and
+rigour. Project-URL: Documentation, https://dream-faster.github.io/fold
+Project-URL: Issues, https://github.com/dream-faster/fold/issues Project-URL:
+Source, https://github.com/dream-faster/fold Author-email: Mark Aron
+Szulyovszky
 dreamfaster.ai>, Daniel Szemerey
-dreamfaster.ai> License-Expression: MIT License-File: LICENSE Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7 Requires-
-Dist: iteration-utilities Requires-Dist: numpy Requires-Dist: pandas Requires-
-Dist: scikit-learn Requires-Dist: tqdm Provides-Extra: docs Requires-Dist:
-image; extra == 'docs' Requires-Dist: mkdocs-autorefs; extra == 'docs'
-Requires-Dist: mkdocs-gallery; extra == 'docs' Requires-Dist: mkdocs-glightbox;
-extra == 'docs' Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
-Requires-Dist: mkdocs-jupyter; extra == 'docs' Requires-Dist: mkdocs-material;
-extra == 'docs' Requires-Dist: mkdocstrings-python; extra == 'docs' Provides-
-Extra: extras Requires-Dist: holidays; extra == 'extras' Requires-Dist:
-krisi~=0.0.8; extra == 'extras' Requires-Dist: ray; extra == 'extras' Provides-
-Extra: quality Requires-Dist: black~=22.12.0; extra == 'quality' Requires-Dist:
-flake8~=4.0.1; extra == 'quality' Requires-Dist: isort~=5.10.1; extra ==
-'quality' Requires-Dist: pre-commit~=2.20.0; extra == 'quality' Provides-Extra:
-ray Requires-Dist: ray; extra == 'ray' Provides-Extra: tests Requires-Dist:
-holidays; extra == 'tests' Requires-Dist: imbalanced-learn; extra == 'tests'
-Requires-Dist: pytest-cov>=4.0; extra == 'tests' Requires-Dist: pytest~=7.1.2;
-extra == 'tests' Description-Content-Type: text/markdown
+dreamfaster.ai> License-File: LICENSE Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: Other/Proprietary License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Requires-Python: >=3.7 Requires-Dist: iteration-
+utilities Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: scikit-
+learn Requires-Dist: tqdm Provides-Extra: docs Requires-Dist: image; extra ==
+'docs' Requires-Dist: mkdocs-autorefs; extra == 'docs' Requires-Dist: mkdocs-
+gallery; extra == 'docs' Requires-Dist: mkdocs-glightbox; extra == 'docs'
+Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs' Requires-Dist:
+mkdocs-jupyter; extra == 'docs' Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: mkdocstrings-python; extra == 'docs' Provides-Extra: extras
+Requires-Dist: holidays; extra == 'extras' Requires-Dist: krisi~=0.0.8; extra
+== 'extras' Requires-Dist: ray; extra == 'extras' Provides-Extra: quality
+Requires-Dist: black~=22.12.0; extra == 'quality' Requires-Dist: flake8~=4.0.1;
+extra == 'quality' Requires-Dist: isort~=5.10.1; extra == 'quality' Requires-
+Dist: pre-commit~=2.20.0; extra == 'quality' Provides-Extra: ray Requires-Dist:
+ray; extra == 'ray' Provides-Extra: tests Requires-Dist: holidays; extra ==
+'tests' Requires-Dist: imbalanced-learn; extra == 'tests' Requires-Dist:
+pytest-cov>=4.0; extra == 'tests' Requires-Dist: pytest~=7.1.2; extra ==
+'tests' Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                  (/fold/) ****
   A Time_Series_Continuous_Validation library that lets you build, deploy and
```

