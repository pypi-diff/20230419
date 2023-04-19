# Comparing `tmp/mlms-0.6.0.tar.gz` & `tmp/mlms-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlms-0.6.0.tar", max compression
+gzip compressed data, was "mlms-0.7.0.tar", max compression
```

## Comparing `mlms-0.6.0.tar` & `mlms-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2859 2023-03-25 23:08:14.311742 mlms-0.6.0/README.md
--rw-r--r--   0        0        0     6587 2023-03-21 22:45:52.726991 mlms-0.6.0/mlms/.ipynb_checkpoints/ModelSelection-checkpoint.py
--rw-r--r--   0        0        0     9348 2023-03-25 20:49:54.947825 mlms-0.6.0/mlms/ModelSelection.py
--rw-r--r--   0        0        0        0 2023-03-21 21:29:03.911558 mlms-0.6.0/mlms/__init__.py
--rw-r--r--   0        0        0     2151 2023-03-25 23:02:05.893647 mlms-0.6.0/mlms/plot_roc_curve.py
--rw-r--r--   0        0        0      563 2023-03-25 23:19:19.028005 mlms-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 mlms-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2933 2023-03-25 23:51:08.294959 mlms-0.7.0/README.md
+-rw-r--r--   0        0        0     6587 2023-03-21 22:45:52.726991 mlms-0.7.0/mlms/.ipynb_checkpoints/ModelSelection-checkpoint.py
+-rw-r--r--   0        0        0     2151 2023-03-25 23:02:05.893647 mlms-0.7.0/mlms/.ipynb_checkpoints/plot_roc_curve-checkpoint.py
+-rw-r--r--   0        0        0     9485 2023-04-19 21:15:26.419951 mlms-0.7.0/mlms/ModelSelection.py
+-rw-r--r--   0        0        0        0 2023-03-21 21:29:03.911558 mlms-0.7.0/mlms/__init__.py
+-rw-r--r--   0        0        0     2151 2023-03-25 23:02:05.893647 mlms-0.7.0/mlms/plot_roc_curve.py
+-rw-r--r--   0        0        0      563 2023-04-19 21:15:36.784722 mlms-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 mlms-0.7.0/PKG-INFO
```

### Comparing `mlms-0.6.0/README.md` & `mlms-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 - `('RFR', RandomForestRegressor())`,
 - `('ETR', ExtraTreesRegressor())`
 
 ![1679487197758](image/README/1679487197758.png)
 
 Additonally, this package also alow users to plot ROC_Curve
 
+`from mlms.plot_roc_curve import Multiclass_ROC_Curve, Binary_ROC_Curve`
+
 `Multiclass_ROC_Curve(X_test, y_test, fitted_model, chart_title:str)`
 
 ![1679785680784](image/README/1679785680784.png)
 
 `Binary_ROC_Curve(y_true, y_pred,chart_name:str)`
 
 [GitHub](https://github.com/HigherHoopern/ML_ModelSelection)
```

### Comparing `mlms-0.6.0/mlms/.ipynb_checkpoints/ModelSelection-checkpoint.py` & `mlms-0.7.0/mlms/.ipynb_checkpoints/ModelSelection-checkpoint.py`

 * *Files identical despite different names*

### Comparing `mlms-0.6.0/mlms/ModelSelection.py` & `mlms-0.7.0/mlms/ModelSelection.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             df_results['kfold_std'] = df_results['kfold_results'].apply(lambda x: x.std())     
         # IPython.display.clear_output()
 
         return df_results.set_index('names'), models
 
 
 
-def Select_Regressor(scoring, K_folds,X_train, X_test, y_train, y_test):
+def Select_Regressor(scoring, K_folds,time_series,X_train, X_test, y_train, y_test):
 
     models = []
 
     models.append(('KNN', KNeighborsRegressor()))
     models.append(('CART', DecisionTreeRegressor()))
     models.append(('SVR', SVR()))
     #Neural Network
@@ -198,15 +198,18 @@
     df_results = pd.DataFrame(columns=['names','train_results','test_results','time_secs','kfold_results'])
 
     for name, model in tqdm(models):
 
         start = time()
         names.append(name)     
         ## K Fold analysis:  
-        kfold = KFold(n_splits=K_folds, random_state=42,shuffle=True)
+        if time_series == True:
+            kfold = KFold(n_splits=K_folds, random_state=42,shuffle=False)
+        else:
+            kfold = KFold(n_splits=K_folds, random_state=42,shuffle=True)
 
         if scoring == 'neg_mean_squared_error':
             # converted mean square error to positive. The lower the beter
             cv_results = -1* cross_val_score(model, X_train, y_train, cv=kfold, scoring=scoring)
         else:
             cv_results = cross_val_score(model, X_train, y_train, cv=kfold, scoring=scoring)
```

### Comparing `mlms-0.6.0/mlms/plot_roc_curve.py` & `mlms-0.7.0/mlms/.ipynb_checkpoints/plot_roc_curve-checkpoint.py`

 * *Files identical despite different names*

### Comparing `mlms-0.6.0/pyproject.toml` & `mlms-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlms"
-version = "0.6.0"
+version = "0.7.0"
 license = "MIT"
 description = "This package is to facilitate model selection in Machine Learning."
 authors = ["Jason Lu <luzhenxian@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/HigherHoopern/ML_ModelSelection"
 keywords = ["Machine Learning", "Model Selection"]
 packages = [{include = "mlms"}]
```

### Comparing `mlms-0.6.0/PKG-INFO` & `mlms-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlms
-Version: 0.6.0
+Version: 0.7.0
 Summary: This package is to facilitate model selection in Machine Learning.
 Home-page: https://github.com/HigherHoopern/ML_ModelSelection
 License: MIT
 Keywords: Machine Learning,Model Selection
 Author: Jason Lu
 Author-email: luzhenxian@hotmail.com
 Requires-Python: >=3.7,<4.0
@@ -81,14 +81,16 @@
 - `('RFR', RandomForestRegressor())`,
 - `('ETR', ExtraTreesRegressor())`
 
 ![1679487197758](image/README/1679487197758.png)
 
 Additonally, this package also alow users to plot ROC_Curve
 
+`from mlms.plot_roc_curve import Multiclass_ROC_Curve, Binary_ROC_Curve`
+
 `Multiclass_ROC_Curve(X_test, y_test, fitted_model, chart_title:str)`
 
 ![1679785680784](image/README/1679785680784.png)
 
 `Binary_ROC_Curve(y_true, y_pred,chart_name:str)`
 
 [GitHub](https://github.com/HigherHoopern/ML_ModelSelection)
```

