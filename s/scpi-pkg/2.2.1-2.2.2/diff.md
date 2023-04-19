# Comparing `tmp/scpi_pkg-2.2.1.tar.gz` & `tmp/scpi_pkg-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpi_pkg-2.2.1.tar", last modified: Tue Mar 14 19:15:20 2023, max compression
+gzip compressed data, was "scpi_pkg-2.2.2.tar", last modified: Wed Apr 19 17:17:01 2023, max compression
```

## Comparing `scpi_pkg-2.2.1.tar` & `scpi_pkg-2.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-03-14 19:15:20.294388 scpi_pkg-2.2.1/
--rw-r--r--   0 fpalomba   (501) staff       (20)     1091 2021-11-18 19:45:12.000000 scpi_pkg-2.2.1/LICENSE
--rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-03-14 19:15:20.294442 scpi_pkg-2.2.1/PKG-INFO
--rw-r--r--   0 fpalomba   (501) staff       (20)     1887 2022-09-08 01:12:37.000000 scpi_pkg-2.2.1/README.md
--rw-r--r--   0 fpalomba   (501) staff       (20)      112 2022-03-01 16:03:56.000000 scpi_pkg-2.2.1/pyproject.toml
--rw-r--r--   0 fpalomba   (501) staff       (20)      964 2023-03-14 19:15:20.294703 scpi_pkg-2.2.1/setup.cfg
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-03-14 19:15:20.286816 scpi_pkg-2.2.1/src/
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-03-14 19:15:20.293717 scpi_pkg-2.2.1/src/scpi_pkg/
--rw-r--r--   0 fpalomba   (501) staff       (20)        0 2021-11-18 15:59:04.000000 scpi_pkg-2.2.1/src/scpi_pkg/__init__.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    53038 2023-03-14 18:53:53.000000 scpi_pkg-2.2.1/src/scpi_pkg/funs.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    33356 2023-01-25 05:32:28.000000 scpi_pkg-2.2.1/src/scpi_pkg/scdata.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    35558 2023-01-25 05:37:18.000000 scpi_pkg-2.2.1/src/scpi_pkg/scdataMulti.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    32014 2023-03-13 23:34:41.000000 scpi_pkg-2.2.1/src/scpi_pkg/scest.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    79417 2023-03-14 19:15:00.000000 scpi_pkg-2.2.1/src/scpi_pkg/scpi.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    12752 2022-11-20 15:18:05.000000 scpi_pkg-2.2.1/src/scpi_pkg/scplot.py
--rw-r--r--   0 fpalomba   (501) staff       (20)    29802 2023-01-25 21:32:03.000000 scpi_pkg-2.2.1/src/scpi_pkg/scplotMulti.py
--rw-r--r--   0 fpalomba   (501) staff       (20)       23 2023-01-24 16:16:13.000000 scpi_pkg-2.2.1/src/scpi_pkg/version.py
-drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-03-14 19:15:20.294292 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/
--rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-03-14 19:15:20.000000 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/PKG-INFO
--rw-r--r--   0 fpalomba   (501) staff       (20)      436 2023-03-14 19:15:20.000000 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)        1 2023-03-14 19:15:20.000000 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)      155 2023-03-14 19:15:20.000000 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/requires.txt
--rw-r--r--   0 fpalomba   (501) staff       (20)        9 2023-03-14 19:15:20.000000 scpi_pkg-2.2.1/src/scpi_pkg.egg-info/top_level.txt
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090963 scpi_pkg-2.2.2/
+-rw-r--r--   0 fpalomba   (501) staff       (20)     1091 2021-11-18 19:45:12.000000 scpi_pkg-2.2.2/LICENSE
+-rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-04-19 17:17:01.091024 scpi_pkg-2.2.2/PKG-INFO
+-rw-r--r--   0 fpalomba   (501) staff       (20)     1887 2022-09-08 01:12:37.000000 scpi_pkg-2.2.2/README.md
+-rw-r--r--   0 fpalomba   (501) staff       (20)      112 2022-03-01 16:03:56.000000 scpi_pkg-2.2.2/pyproject.toml
+-rw-r--r--   0 fpalomba   (501) staff       (20)      964 2023-04-19 17:17:01.091293 scpi_pkg-2.2.2/setup.cfg
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.085061 scpi_pkg-2.2.2/src/
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090233 scpi_pkg-2.2.2/src/scpi_pkg/
+-rw-r--r--   0 fpalomba   (501) staff       (20)        0 2021-11-18 15:59:04.000000 scpi_pkg-2.2.2/src/scpi_pkg/__init__.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    53510 2023-04-19 16:23:42.000000 scpi_pkg-2.2.2/src/scpi_pkg/funs.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    33356 2023-01-25 05:32:28.000000 scpi_pkg-2.2.2/src/scpi_pkg/scdata.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    35558 2023-01-25 05:37:18.000000 scpi_pkg-2.2.2/src/scpi_pkg/scdataMulti.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    32014 2023-03-13 23:34:41.000000 scpi_pkg-2.2.2/src/scpi_pkg/scest.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    79417 2023-03-14 19:15:00.000000 scpi_pkg-2.2.2/src/scpi_pkg/scpi.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    12752 2022-11-20 15:18:05.000000 scpi_pkg-2.2.2/src/scpi_pkg/scplot.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)    29802 2023-01-25 21:32:03.000000 scpi_pkg-2.2.2/src/scpi_pkg/scplotMulti.py
+-rw-r--r--   0 fpalomba   (501) staff       (20)       23 2023-03-14 19:25:03.000000 scpi_pkg-2.2.2/src/scpi_pkg/version.py
+drwxr-xr-x   0 fpalomba   (501) staff       (20)        0 2023-04-19 17:17:01.090854 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/
+-rw-r--r--   0 fpalomba   (501) staff       (20)     2425 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 fpalomba   (501) staff       (20)      436 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)        1 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)      155 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/requires.txt
+-rw-r--r--   0 fpalomba   (501) staff       (20)        9 2023-04-19 17:17:01.000000 scpi_pkg-2.2.2/src/scpi_pkg.egg-info/top_level.txt
```

### Comparing `scpi_pkg-2.2.1/LICENSE` & `scpi_pkg-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/PKG-INFO` & `scpi_pkg-2.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scpi_pkg
-Version: 2.2.1
+Version: 2.2.2
 Summary: The package computes point estimates and prediction intervals for Synthetic Control methods as proposed in Cattaneo, Feng, and Titiunik (2021).
 Home-page: https://nppackages.github.io/scpi/
 Author: Filippo Palomba
 Author-email: fpalomba@princeton.edu
 Project-URL: Bug Tracker, https://nppackages.github.io/scpi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCPI_PKG
 
 The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
```

### Comparing `scpi_pkg-2.2.1/README.md` & `scpi_pkg-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/setup.cfg` & `scpi_pkg-2.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.7
 install_requires = 
 	cvxpy >= 1.1.18
 	dask >= 2021.04.0
 	ecos >= 2.0.7
 	luddite >= 1.0.2
 	numpy >= 1.20.1
-	pandas >= 1.2.4
+	pandas >= 1.5.0
 	plotnine >= 0.8.0
 	scikit-learn >= 0.24.1
 	scipy >= 1.7.1
 	statsmodels >= 0.12.2
 
 [options.packages.find]
 where = src
```

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/funs.py` & `scpi_pkg-2.2.2/src/scpi_pkg/funs.py`

 * *Files 1% similar despite different names*

```diff
@@ -979,32 +979,32 @@
 
         if e_method == 'gaussian':
             x_more = numpy.vstack((preds, x))
             fit = cond_pred(y=y, x=x, xpreds=x_more, method='lm')
             e_mean = fit[:len(preds)]
             if effect == "time":
                 e_mean = pandas.DataFrame(data=e_mean, index=idx)
-                e_mean = e_mean.mean(level='Time').values[:, 0]
+                e_mean = e_mean.groupby(level='Time').mean().values[:, 0]
 
             y_fit = fit[len(preds):]
             y_var = numpy.log((y - y_fit)**2)
             var_pred = cond_pred(y=y_var, x=x, xpreds=x_more, method='lm')
             if effect == "time":
                 var_pred = pandas.DataFrame(data=var_pred[:len(preds)], index=idx)
-                var_pred = var_pred.mean(level='Time').values[:, 0]
+                var_pred = var_pred.groupby(level='Time').mean().values[:, 0]
             else:
                 var_pred = var_pred[:len(preds)]
             e_sig2 = numpy.exp(var_pred)
 
             q_pred = cond_pred(y=y - y_fit, x=x, xpreds=x_more, method='qreg', tau=[0.25, 0.75])
             if effect == "time":
                 q3_pred = pandas.DataFrame(data=q_pred[:len(preds), 1], index=idx)
                 q1_pred = pandas.DataFrame(data=q_pred[:len(preds), 0], index=idx)
-                q3_pred = q3_pred.mean(level='Time').values[:, 0]
-                q1_pred = q1_pred.mean(level='Time').values[:, 0]
+                q3_pred = q3_pred.groupby(level='Time').mean().values[:, 0]
+                q1_pred = q1_pred.groupby(level='Time').mean().values[:, 0]
             else:
                 q3_pred = q_pred[:len(preds), 1]
                 q1_pred = q_pred[:len(preds), 0]
             IQ_pred = q3_pred - q1_pred
             IQ_pred = numpy.absolute(IQ_pred)
             e_sig = numpy.c_[numpy.sqrt(e_sig2), IQ_pred / 1.34].min(axis=1)
 
@@ -1021,32 +1021,32 @@
 
         elif e_method == 'ls':
             x_more = numpy.vstack((preds, x))
             fit = cond_pred(y=y, x=x, xpreds=x_more, method='lm')
             e_mean = fit[:len(preds)]
             if effect == "time":
                 e_mean = pandas.DataFrame(data=e_mean, index=idx)
-                e_mean = e_mean.mean(level='Time').values[:, 0]
+                e_mean = e_mean.groupby(level='Time').mean().values[:, 0]
 
             y_fit = fit[len(preds):]
             y_var = numpy.log((y - y_fit)**2)
             var_pred = cond_pred(y=y_var, x=x, xpreds=x_more, method='lm')
             res_var = var_pred[len(preds):]
             if effect == "time":
                 var_pred = pandas.DataFrame(data=var_pred[:len(preds)], index=idx)
-                var_pred = var_pred.mean(level='Time').values[:, 0]
+                var_pred = var_pred.groupby(level='Time').mean().values[:, 0]
             else:
                 var_pred = var_pred[:len(preds)]
 
             q_pred = cond_pred(y=y - y_fit, x=x, xpreds=x_more, method='qreg', tau=[0.25, 0.75])
             if effect == "time":
                 q3_pred = pandas.DataFrame(data=q_pred[:len(preds), 1], index=idx)
                 q1_pred = pandas.DataFrame(data=q_pred[:len(preds), 0], index=idx)
-                q3_pred = q3_pred.mean(level='Time').values[:, 0]
-                q1_pred = q1_pred.mean(level='Time').values[:, 0]
+                q3_pred = q3_pred.groupby(level='Time').mean().values[:, 0]
+                q1_pred = q1_pred.groupby(level='Time').mean().values[:, 0]
             else:
                 q3_pred = q_pred[:len(preds), 1]
                 q1_pred = q_pred[:len(preds), 0]
             IQ_pred = q3_pred - q1_pred
             IQ_pred = numpy.absolute(IQ_pred)
             e_sig = numpy.sqrt(numpy.exp(var_pred[:len(preds)]))
             e_sig = numpy.c_[e_sig, IQ_pred / 1.34].min(axis=1)
@@ -1063,16 +1063,16 @@
 
         elif e_method == 'qreg':
             e_pred = cond_pred(y=y, x=x, xpreds=preds,
                                method='qreg', tau=[alpha, 1 - alpha])
             if effect == "time":
                 e_pred_lb = pandas.DataFrame(data=e_pred[:, 0], index=idx)
                 e_pred_ub = pandas.DataFrame(data=e_pred[:, 1], index=idx)
-                e_pred_lb = e_pred_lb.mean(level='Time').values[:, 0]
-                e_pred_ub = e_pred_ub.mean(level='Time').values[:, 0]
+                e_pred_lb = e_pred_lb.groupby(level='Time').mean().values[:, 0]
+                e_pred_ub = e_pred_ub.groupby(level='Time').mean().values[:, 0]
             else:
                 e_pred_lb = e_pred[:, [0]]
                 e_pred_ub = e_pred[:, [1]]
 
             lb = e_pred_lb
             ub = e_pred_ub
 
@@ -1356,18 +1356,23 @@
         cols = False
 
     if cols is True:
         for tr in tr_units:
             X_r = X.loc[pandas.IndexSlice[tr, :, :]]
             csel = [c.split("_")[0] == tr for c in X_r.columns.tolist()]
             X_rc = X_r.loc[:, numpy.array(csel)]
+            # to ensure backward compatibility with Python 3.7 (IndexSlice did not remove the column automatically)
+            if 'ID' in X_rc.index.names:
+                X_rc = X_rc.reset_index(level=0, drop=True)
             matdict[tr] = X_rc
     else:
         for tr in tr_units:
             X_r = X.loc[pandas.IndexSlice[tr, :, :]]
+            if 'ID' in X_r.index.names:  # to ensure backward compatibility with Python 3.7
+                X_r = X_r.reset_index(level=0, drop=True)
             matdict[tr] = X_r
 
     return matdict
 
 def CIrename(ci, citype):
     CI = deepcopy(ci)
     CI.columns = [c + "_" + citype for c in ci.columns]
```

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scdata.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scdata.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scdataMulti.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scdataMulti.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scest.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scest.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scpi.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scpi.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scplot.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scplot.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg/scplotMulti.py` & `scpi_pkg-2.2.2/src/scpi_pkg/scplotMulti.py`

 * *Files identical despite different names*

### Comparing `scpi_pkg-2.2.1/src/scpi_pkg.egg-info/PKG-INFO` & `scpi_pkg-2.2.2/src/scpi_pkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scpi-pkg
-Version: 2.2.1
+Version: 2.2.2
 Summary: The package computes point estimates and prediction intervals for Synthetic Control methods as proposed in Cattaneo, Feng, and Titiunik (2021).
 Home-page: https://nppackages.github.io/scpi/
 Author: Filippo Palomba
 Author-email: fpalomba@princeton.edu
 Project-URL: Bug Tracker, https://nppackages.github.io/scpi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCPI_PKG
 
 The `scpi_pkg` package provides Python implementations of estimation and inference procedures for Synthetic Control methods.
```

