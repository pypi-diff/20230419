# Comparing `tmp/aplr-2.2.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-2.3.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 280687 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   307712 b- defN 23-Apr-04 15:19 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   320512 b- defN 23-Apr-04 15:23 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-04 15:14 aplr/__init__.py
--rw-rw-rw-  2.0 fat     5969 b- defN 23-Apr-04 15:14 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-Apr-04 15:23 aplr-2.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      626 b- defN 23-Apr-04 15:23 aplr-2.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-04 15:23 aplr-2.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-04 15:23 aplr-2.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      690 b- defN 23-Apr-04 15:23 aplr-2.2.0.dist-info/RECORD
-9 files, 636783 bytes uncompressed, 279515 bytes compressed:  56.1%
+Zip file size: 290643 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   319488 b- defN 23-Apr-19 16:18 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   330752 b- defN 23-Apr-19 16:23 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-19 16:13 aplr/__init__.py
+-rw-rw-rw-  2.0 fat     6009 b- defN 23-Apr-19 16:13 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-Apr-19 16:23 aplr-2.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      626 b- defN 23-Apr-19 16:23 aplr-2.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-19 16:23 aplr-2.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-19 16:23 aplr-2.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      690 b- defN 23-Apr-19 16:23 aplr-2.3.0.dist-info/RECORD
+9 files, 658839 bytes uncompressed, 289471 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-2.2.0.dist-info/LICENSE
+Filename: aplr-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-2.2.0.dist-info/METADATA
+Filename: aplr-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-2.2.0.dist-info/WHEEL
+Filename: aplr-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-2.2.0.dist-info/top_level.txt
+Filename: aplr-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-2.2.0.dist-info/RECORD
+Filename: aplr-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -44,17 +44,17 @@
         self.APLRRegressor.min_observations_in_split=self.min_observations_in_split
         self.APLRRegressor.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
         self.APLRRegressor.max_eligible_terms=self.max_eligible_terms
         self.APLRRegressor.verbosity=self.verbosity
         self.APLRRegressor.tweedie_power=self.tweedie_power
         self.APLRRegressor.validation_tuning_metric=self.validation_tuning_metric
 
-    def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[]):
+    def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[],group:npt.ArrayLike = np.empty(0)):
         self.__set_params_cpp()
-        self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints)
+        self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group)
 
     def predict(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=True)->npt.ArrayLike:
         return self.APLRRegressor.predict(X, cap_predictions_to_minmax_in_training)
 
     def set_term_names(self, X_names:List[str]):
         self.APLRRegressor.set_term_names(X_names)
```

## Comparing `aplr-2.2.0.dist-info/LICENSE` & `aplr-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-2.2.0.dist-info/METADATA` & `aplr-2.3.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 2.2.0
+Version: 2.3.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

## Comparing `aplr-2.2.0.dist-info/RECORD` & `aplr-2.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-aplr_cpp.cp39-win_amd64.pyd,sha256=BzLI6rBc7pzCMPvcWETvzWEdj_XitFW5edFMtpTAM5s,307712
-aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=hFg4quKrn5oHB6h7FVkqCpGcc7hLZCk_WVifUar3bJA,320512
+aplr_cpp.cp39-win_amd64.pyd,sha256=B_UBy_OiEMQRaOujrM-lY2FDOZHpiF_1rTeDLRPyHwg,319488
+aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=67WMNOpCjLdIJoIabE7mpU9s1Zzd-4OeYyUFyfblgn4,330752
 aplr/__init__.py,sha256=jLHRAp1zq22wmHqFIghBqfVSnMBnd27LjffHgzI07Hw,19
-aplr/aplr.py,sha256=UmZ_0fCLgcl8RT9T9MrlUemGDyfBtqnC-b_Wa945beA,5969
-aplr-2.2.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
-aplr-2.2.0.dist-info/METADATA,sha256=SNWlrsfgUAbQXlsQeYllD3mQLB7Sk6X9TuqcQ6ekW7s,626
-aplr-2.2.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-aplr-2.2.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
-aplr-2.2.0.dist-info/RECORD,,
+aplr/aplr.py,sha256=5AWYY5QUOhlvlMAdTgyFwGvCqqQ3ff8QZYudxh2IHl4,6009
+aplr-2.3.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
+aplr-2.3.0.dist-info/METADATA,sha256=2vty0HaGwjH2snFrMihNiA5rOFtjKCxplJDWbR1r3_o,626
+aplr-2.3.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+aplr-2.3.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
+aplr-2.3.0.dist-info/RECORD,,
```

