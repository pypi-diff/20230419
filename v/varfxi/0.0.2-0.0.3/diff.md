# Comparing `tmp/varfxi-0.0.2.tar.gz` & `tmp/varfxi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varfxi-0.0.2.tar", max compression
+gzip compressed data, was "varfxi-0.0.3.tar", max compression
```

## Comparing `varfxi-0.0.2.tar` & `varfxi-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.2/LICENSE
--rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.2/README.md
--rw-r--r--   0        0        0     1148 2023-04-15 10:09:04.303637 varfxi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    99899 2023-04-15 09:29:45.646044 varfxi-0.0.2/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
--rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/__init__.py
--rw-r--r--   0        0        0    99899 2023-04-15 09:39:45.792298 varfxi-0.0.2/varfxi/distGARCH.py
--rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/joyplot2.py
--rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/quantileproj.py
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 varfxi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.3/README.md
+-rw-r--r--   0        0        0     1168 2023-04-19 09:56:52.340421 varfxi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    99792 2023-04-19 09:53:31.728969 varfxi-0.0.3/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
+-rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/__init__.py
+-rw-r--r--   0        0        0    99792 2023-04-19 09:53:31.728969 varfxi-0.0.3/varfxi/distGARCH.py
+-rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/joyplot2.py
+-rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.3/varfxi/quantileproj.py
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 varfxi-0.0.3/PKG-INFO
```

### Comparing `varfxi-0.0.2/LICENSE` & `varfxi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.2/README.md` & `varfxi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.2/pyproject.toml` & `varfxi-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "varfxi"
-version = "0.0.2"
+version = "0.0.3"
 description = "Volatility based estimation for FX interventions"
 authors = ["romainlafarguette <romain.lafarguette@gmail.com>", "amineraboun <amineraboun@gmail.com>"]
 repository ="https://github.com/romainlafarguette/varfxi"
 homepage  ="https://github.com/romainlafarguette/varfxi"
 
 readme = "README.md"
 keywords = ["var", "garch"]
@@ -21,14 +21,15 @@
 numpy = "^1.24.2"
 arch = "^5.3.1"
 matplotlib = "^3.7.1"
 
 # Dev dependencies
 seaborn = "^0.12.2"
 tqdm = "^4.65.0"
+openpyxl = "^3.1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `varfxi-0.0.2/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py` & `varfxi-0.0.3/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,14 @@
                 self.params = params
                 
             # Attributes
             self.depvar = depvar_str
             self.level = level_str
             self.exog_l = exog_l
             
-            #import pdb; pdb.set_trace()
             if isinstance(lags_l, int):
                 if lags_l==0:
                     self.lags_l = None
                 else:
                     self.lags_l = np.arange(1, lags_l+1)
             elif isinstance(lags_l, list):
                 if 0 in lags_l:
@@ -1169,17 +1168,18 @@
                                   lags_l= lags_l, 
                                   vol_model= fv,
                                   dist_family=Normal()
                                  )
         mean_fit = mean_mod.fit(disp='off', verbose=verbose)
         if isinstance(lags_l, list):
             n= max(lags_l)
+            n = max(0, n-1)
         else:
-            n = lags_l
-            
+            n = max(0, lags_l-1)
+
         mean_forecast = mean_fit.forecast(start_date= self.df.index[n])
         performance = pd.Series({
                  'R2': mean_fit.res.rsquared, 
                 'R2_adj': mean_fit.res.rsquared_adj,
                 'AIC': mean_fit.res.aic, 
                 'BIC': mean_fit.res.bic,                
                 'RMSE': mean_forecast.rmse(), 
@@ -1312,15 +1312,15 @@
                             data=residuals,
                             vol_model= volatility_model,
                             dist_family= distribution_family, 
                             init_type = 'ZEROMEAN'
                            )
         vol_fit = vol_mod.fit(verbose=False)
 
-        vol_forecast = vol_fit.forecast(start_date= self.epsilon.dropna().index[0])
+        vol_forecast = vol_fit.forecast(start_date= residuals.dropna().index[0])
             
         KS_normalized_innovations, KS_normalized_innovations_pvalues, _  = vol_forecast.KS_normalized_innovations(threshold=threshold, verbose=False)
         KS_PIT_test, KS_PIT_test_pvalues, _ = vol_forecast.KS_PIT_test(threshold=threshold, verbose=False)
         log_score = vol_forecast.log_score(aggr_func='EWMA')    
         
         performance = {
             'KS_normalized_innovations': KS_normalized_innovations,
@@ -1369,16 +1369,18 @@
         """
         Search for the best Out-of-Sample Volatility and Distribution
             Test 2-by-2 combinations of 
                 Volatility Models: 'Constant', 'ARCH', 'EGARCH', 'GARCH', 'GJR-GARCH', 'EWMA', 'RiskMetric'
                 Distribution Families: 'Normal', 'StudentT', 'SkewStudent', 'GeneralizedError'
                 
             Choose among the well specified model, i.e, those passing the pis and kolmogorov test, 
-                the model with the best performance on the complete distribution based on the log_score and on the tails based on the tailed_log_score
-                if no combination is well specified, return the combination with best performance regardless if specified or not
+                the model with the best performance based on the tailed_log_score on the tails specified (by default both tails) is chosen 
+                    If there is more than 1 take the model with the best performance on the complete distribution using the log_score
+                    
+            If no combination is well specified, return the combination with best performance regardless if specified or not
 
         Output:
         -------
             performance: pd.DataFrame
                 Summary Table on the out-of-sample performance of all possible combinations of GARCH type volatility models and Distributions 
             
         """
@@ -1499,20 +1501,22 @@
                 cond_var = vol_fit.res.conditional_volatility**2
                 variance = pd.Series(index=self.df.index, dtype='float64')                
                 variance.loc[cond_var.index] = cond_var
                 variance = variance.bfill()
                 fv = FixedVariance(variance, unit_scale=True)
 
             # Re-train the main model with the previous Conditional Variance
-            performance, mean_mod, mean_fit, mean_forecast = self.extract_mean(exog_l= self.best_combination,
-                                                                               lags_l=self.best_lag, 
-                                                                               fv= fv)
-            performance, vol_mod, vol_fit, vol_forecast = self.assess_vol_dist_model(residuals = mean_fit.res.resid.dropna(),
-                                                                                     volatility_model= self.best_vol_mod,
-                                                                                     distribution_family = self.best_distrib)
+            performance, mean_mod, mean_fit, mean_forecast = self.extract_mean(
+                exog_l= self.best_combination,
+                lags_l=self.best_lag, 
+                fv= fv)
+            performance, vol_mod, vol_fit, vol_forecast = self.assess_vol_dist_model(
+                residuals = mean_fit.res.resid.dropna(),
+                volatility_model= self.best_vol_mod, 
+                distribution_family = self.best_distrib)
 
             mean_params = mean_fit.res.params.drop('sigma2') if (i==0) else mean_fit.res.params
             mean_pvalues = mean_fit.res.pvalues.drop('sigma2') if (i==0) else mean_fit.res.pvalues            
             
             iter_params[f"iteration_{i}"] = pd.concat([
                 pd.concat([mean_params, vol_fit.res.params]),
                 pd.concat([mean_pvalues, vol_fit.res.pvalues])
```

### Comparing `varfxi-0.0.2/varfxi/distGARCH.py` & `varfxi-0.0.3/varfxi/distGARCH.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,14 @@
                 self.params = params
                 
             # Attributes
             self.depvar = depvar_str
             self.level = level_str
             self.exog_l = exog_l
             
-            #import pdb; pdb.set_trace()
             if isinstance(lags_l, int):
                 if lags_l==0:
                     self.lags_l = None
                 else:
                     self.lags_l = np.arange(1, lags_l+1)
             elif isinstance(lags_l, list):
                 if 0 in lags_l:
@@ -1169,17 +1168,18 @@
                                   lags_l= lags_l, 
                                   vol_model= fv,
                                   dist_family=Normal()
                                  )
         mean_fit = mean_mod.fit(disp='off', verbose=verbose)
         if isinstance(lags_l, list):
             n= max(lags_l)
+            n = max(0, n-1)
         else:
-            n = lags_l
-            
+            n = max(0, lags_l-1)
+
         mean_forecast = mean_fit.forecast(start_date= self.df.index[n])
         performance = pd.Series({
                  'R2': mean_fit.res.rsquared, 
                 'R2_adj': mean_fit.res.rsquared_adj,
                 'AIC': mean_fit.res.aic, 
                 'BIC': mean_fit.res.bic,                
                 'RMSE': mean_forecast.rmse(), 
@@ -1312,15 +1312,15 @@
                             data=residuals,
                             vol_model= volatility_model,
                             dist_family= distribution_family, 
                             init_type = 'ZEROMEAN'
                            )
         vol_fit = vol_mod.fit(verbose=False)
 
-        vol_forecast = vol_fit.forecast(start_date= self.epsilon.dropna().index[0])
+        vol_forecast = vol_fit.forecast(start_date= residuals.dropna().index[0])
             
         KS_normalized_innovations, KS_normalized_innovations_pvalues, _  = vol_forecast.KS_normalized_innovations(threshold=threshold, verbose=False)
         KS_PIT_test, KS_PIT_test_pvalues, _ = vol_forecast.KS_PIT_test(threshold=threshold, verbose=False)
         log_score = vol_forecast.log_score(aggr_func='EWMA')    
         
         performance = {
             'KS_normalized_innovations': KS_normalized_innovations,
@@ -1369,16 +1369,18 @@
         """
         Search for the best Out-of-Sample Volatility and Distribution
             Test 2-by-2 combinations of 
                 Volatility Models: 'Constant', 'ARCH', 'EGARCH', 'GARCH', 'GJR-GARCH', 'EWMA', 'RiskMetric'
                 Distribution Families: 'Normal', 'StudentT', 'SkewStudent', 'GeneralizedError'
                 
             Choose among the well specified model, i.e, those passing the pis and kolmogorov test, 
-                the model with the best performance on the complete distribution based on the log_score and on the tails based on the tailed_log_score
-                if no combination is well specified, return the combination with best performance regardless if specified or not
+                the model with the best performance based on the tailed_log_score on the tails specified (by default both tails) is chosen 
+                    If there is more than 1 take the model with the best performance on the complete distribution using the log_score
+                    
+            If no combination is well specified, return the combination with best performance regardless if specified or not
 
         Output:
         -------
             performance: pd.DataFrame
                 Summary Table on the out-of-sample performance of all possible combinations of GARCH type volatility models and Distributions 
             
         """
@@ -1499,20 +1501,22 @@
                 cond_var = vol_fit.res.conditional_volatility**2
                 variance = pd.Series(index=self.df.index, dtype='float64')                
                 variance.loc[cond_var.index] = cond_var
                 variance = variance.bfill()
                 fv = FixedVariance(variance, unit_scale=True)
 
             # Re-train the main model with the previous Conditional Variance
-            performance, mean_mod, mean_fit, mean_forecast = self.extract_mean(exog_l= self.best_combination,
-                                                                               lags_l=self.best_lag, 
-                                                                               fv= fv)
-            performance, vol_mod, vol_fit, vol_forecast = self.assess_vol_dist_model(residuals = mean_fit.res.resid.dropna(),
-                                                                                     volatility_model= self.best_vol_mod,
-                                                                                     distribution_family = self.best_distrib)
+            performance, mean_mod, mean_fit, mean_forecast = self.extract_mean(
+                exog_l= self.best_combination,
+                lags_l=self.best_lag, 
+                fv= fv)
+            performance, vol_mod, vol_fit, vol_forecast = self.assess_vol_dist_model(
+                residuals = mean_fit.res.resid.dropna(),
+                volatility_model= self.best_vol_mod, 
+                distribution_family = self.best_distrib)
 
             mean_params = mean_fit.res.params.drop('sigma2') if (i==0) else mean_fit.res.params
             mean_pvalues = mean_fit.res.pvalues.drop('sigma2') if (i==0) else mean_fit.res.pvalues            
             
             iter_params[f"iteration_{i}"] = pd.concat([
                 pd.concat([mean_params, vol_fit.res.params]),
                 pd.concat([mean_pvalues, vol_fit.res.pvalues])
```

### Comparing `varfxi-0.0.2/varfxi/joyplot2.py` & `varfxi-0.0.3/varfxi/joyplot2.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.2/varfxi/quantileproj.py` & `varfxi-0.0.3/varfxi/quantileproj.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.2/PKG-INFO` & `varfxi-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfxi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Volatility based estimation for FX interventions
 Home-page: https://github.com/romainlafarguette/varfxi
 Keywords: var,garch
 Author: romainlafarguette
 Author-email: romain.lafarguette@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: arch (>=5.3.1,<6.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/romainlafarguette/varfxi
 Description-Content-Type: text/markdown
 
 VaR-Rule for FX Interventions
```

