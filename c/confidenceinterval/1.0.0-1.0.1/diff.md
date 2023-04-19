# Comparing `tmp/confidenceinterval-1.0.0.tar.gz` & `tmp/confidenceinterval-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidenceinterval-1.0.0.tar", last modified: Sat Mar 11 17:08:47 2023, max compression
+gzip compressed data, was "confidenceinterval-1.0.1.tar", last modified: Wed Apr 19 15:58:56 2023, max compression
```

## Comparing `confidenceinterval-1.0.0.tar` & `confidenceinterval-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-03-11 17:08:47.852393 confidenceinterval-1.0.0/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.0/LICENSE
--rw-r--r--   0 gildenbj   (501) staff       (20)     5043 2023-03-11 17:08:47.852562 confidenceinterval-1.0.0/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)     4504 2023-03-11 17:04:32.000000 confidenceinterval-1.0.0/README.md
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-03-11 17:08:47.849625 confidenceinterval-1.0.0/confidenceinterval/
--rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-03-11 16:11:08.000000 confidenceinterval-1.0.0/confidenceinterval/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1662 2023-03-11 16:44:57.000000 confidenceinterval-1.0.0/confidenceinterval/auc.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    14158 2023-03-11 16:34:15.000000 confidenceinterval-1.0.0/confidenceinterval/binary_metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1211 2023-03-11 16:29:23.000000 confidenceinterval-1.0.0/confidenceinterval/bootstrap.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.0/confidenceinterval/delong.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    21277 2023-03-11 15:07:46.000000 confidenceinterval-1.0.0/confidenceinterval/metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7428 2023-03-11 16:41:28.000000 confidenceinterval-1.0.0/confidenceinterval/takahashi_methods.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.0/confidenceinterval/utils.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-03-11 17:08:47.852086 confidenceinterval-1.0.0/confidenceinterval.egg-info/
--rw-r--r--   0 gildenbj   (501) staff       (20)     5043 2023-03-11 17:08:47.000000 confidenceinterval-1.0.0/confidenceinterval.egg-info/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)      498 2023-03-11 17:08:47.000000 confidenceinterval-1.0.0/confidenceinterval.egg-info/SOURCES.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-03-11 17:08:47.000000 confidenceinterval-1.0.0/confidenceinterval.egg-info/dependency_links.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       37 2023-03-11 17:08:47.000000 confidenceinterval-1.0.0/confidenceinterval.egg-info/requires.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-03-11 17:08:47.000000 confidenceinterval-1.0.0/confidenceinterval.egg-info/top_level.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-03-11 17:08:47.853312 confidenceinterval-1.0.0/setup.cfg
--rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-03-11 17:07:40.000000 confidenceinterval-1.0.0/setup.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.531017 confidenceinterval-1.0.1/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.1/LICENSE
+-rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.1/MANIFEST.in
+-rw-r--r--   0 gildenbj   (501) staff       (20)     6371 2023-04-19 15:58:56.531139 confidenceinterval-1.0.1/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)     5832 2023-03-12 11:17:32.000000 confidenceinterval-1.0.1/README.md
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.529255 confidenceinterval-1.0.1/confidenceinterval/
+-rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-03-11 16:11:08.000000 confidenceinterval-1.0.1/confidenceinterval/__init__.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1662 2023-03-11 16:44:57.000000 confidenceinterval-1.0.1/confidenceinterval/auc.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    14158 2023-03-11 16:34:15.000000 confidenceinterval-1.0.1/confidenceinterval/binary_metrics.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1211 2023-03-11 16:29:23.000000 confidenceinterval-1.0.1/confidenceinterval/bootstrap.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.1/confidenceinterval/delong.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    21277 2023-03-11 15:07:46.000000 confidenceinterval-1.0.1/confidenceinterval/metrics.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7428 2023-03-11 16:41:28.000000 confidenceinterval-1.0.1/confidenceinterval/takahashi_methods.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.1/confidenceinterval/utils.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-04-19 15:58:56.530771 confidenceinterval-1.0.1/confidenceinterval.egg-info/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     6371 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)      527 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/SOURCES.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/dependency_links.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       37 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/requires.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-04-19 15:58:56.000000 confidenceinterval-1.0.1/confidenceinterval.egg-info/top_level.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       36 2023-03-11 10:51:04.000000 confidenceinterval-1.0.1/requirements.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-04-19 15:58:56.531683 confidenceinterval-1.0.1/setup.cfg
+-rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-04-19 15:58:43.000000 confidenceinterval-1.0.1/setup.py
```

### Comparing `confidenceinterval-1.0.0/LICENSE` & `confidenceinterval-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/PKG-INFO` & `confidenceinterval-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,135 @@
-Metadata-Version: 2.1
-Name: confidenceinterval
-Version: 1.0.0
-Summary: Confidence Intervals in python
-Home-page: https://github.com/jacobgil/confidenceinterval
-Author: Jacob Gildenblat
-Author-email: jacob.gildenblat@gmail.com
-Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # The long missing python library for confidence intervals
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
-[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceintervals)
 
 `pip install confidenceinterval`
 
 This is a package that computes common machine learning metrics like F1, and returns their confidence intervals.
 
-⭐ Very easy to use, with the standard scikit-learn naming convention and interface:
 
-e.g roc_auc_score(y_true, y_pred).
+⭐ Very easy to use, with the standard scikit-learn naming convention and interface.
 
 ⭐ Support for many metrics, with modern confidence interval methods.
 
-⭐ Support for both analytical computation of the confidence intervals, and bootstrapping.
+⭐ Support for both analytical computation of the confidence intervals, and bootstrapping methods.
+
+⭐ Easy to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
+
+## The motivation
+
+A confidence interval gives you a lower and upper bound on your metric. It's affected by the sample size, and by how sensitive the metric is to changes in the data.
+
+When making decisions based on metrics, you should prefer narrow intervals. If the interval is wide, you can't be confident that your high performing metric is not just by luck.
+
+While confidence intervals are commonly used by statisticans, with many great R language implementations,
+they are astonishingly rarely used by python users, although python took over the data science world !
+
+Part of this is because there were no simple to use python packages for this.
 
-⭐ East to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
 
 ## Getting started
 
 ```python
 from confidenceinterval import roc_auc_score
 auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95)
 auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
+auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_percentile', n_resamples=5000)
 ```
 
+## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
-For a bootstrap computation of the CI, for any of the methods belonw, you can just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 
-## Supported methods
+For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
+These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
 
-### Get a confidence interval for any external metric
-With the bootstrap_ci method, you can get the CI for a an external metric method.
-As an example, lets get the CI for the balanced accuracy metric. It's not implemented yet in this package,
-but we can easily get the CI for it:
+You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
+
+```python
+random_state = np.random.default_rng()
+n_resamples=9999
+```
+
+## Get a confidence interval for any external metric with Bootstrapping
+With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
+
+As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
 
 ```python
 from confidenceinterval.bootstrap import bootstrap_ci
 # You can specify a random generator for reproducability, or pass None
 random_generator = np.random.default_rng()
 bootstrap_ci(y_true=y_true,
              y_pred=y_pred,
              metric=sklearn.metrics.balanced_accuracy_score,
              confidence_level=0.95,
              n_resamples=9999,
              method='bootstrap_bca',
              random_state=random_generator)
 ```
 
-### F1, Precision, Recall (with Macro and Micro averaging)
+## F1, Precision, Recall (with Macro and Micro averaging)
 ```python
 from confidence interval import precision_score, recall_score, f1_score
 ```
 
 These methods also accept average='micro' or average='macro'.
 
 The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below). 
 
 
-### ROC AUC
+## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
 
 
-### Binary metrics
+## Binary metrics
 ```python
-from confidence interval import accuracy_score, ppv_score, npv_score,
-                                tpr_score, fpr_score, tnr_score
+from confidence interval import accuracy_score,
+                                ppv_score,
+                                npv_score,
+                                tpr_score,
+                                fpr_score,
+                                tnr_score
+# Wilson is used by default:
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95)
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='jeffreys')
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='agresti_coull')
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
+
 ```
 
 For these methods, the confidence interval is estimated by treating the ratio as a binomial proportion,
 see the [wiki page](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval).
 
 By default method='wilson', the wilson interval, which behaves better for smaller samples.
 
 method can be one of ['wilson', 'normal', 'agresti_coull', 'beta', 'jeffreys', 'binom_test'], or one of the boostrap methods.
 
 ----------
 
-### References
+## References
 
 The binomial confidence interval computation uses the statsmodels package:
 https://www.statsmodels.org/dev/generated/statsmodels.stats.proportion.proportion_confint.html
 
-Yandex data schhol implementation of the fast delong method:
+Yandex data school implementation of the fast delong method:
 https://github.com/yandexdataschool/roc_comparison
 
 https://ieeexplore.ieee.org/document/6851192
 X. Sun and W. Xu, "Fast Implementation of DeLong’s Algorithm for Comparing the Areas Under Correlated Receiver Operating Characteristic Curves," in IEEE Signal Processing Letters, vol. 21, no. 11, pp. 1389-1393, Nov. 2014, doi: 10.1109/LSP.2014.2337313.
 
 https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8936911/#APP2
+
 Confidence interval for micro-averaged F1 and macro-averaged F1 scores
 `Kanae Takahashi,1,2 Kouji Yamamoto,3 Aya Kuchiba,4,5 and Tatsuki Koyama6`
 
 B. Efron and R. J. Tibshirani, An Introduction to the Bootstrap, Chapman & Hall/CRC, Boca Raton, FL, USA (1993)
 
-Nathaniel E. Helwig, “Bootstrap Confidence Intervals”, http://users.stat.umn.edu/~helwig/notes/bootci-Notes.pdf
+http://users.stat.umn.edu/~helwig/notes/bootci-Notes.pdf
+`Nathaniel E. Helwig, “Bootstrap Confidence Intervals”`
+
 
-Bootstrapping (statistics), Wikipedia, https://en.wikipedia.org/wiki/Bootstrapping_%28statistics%29
+Bootstrapping (statistics), Wikipedia, https://en.wikipedia.org/wiki/Bootstrapping_%28statistics%29
```

### Comparing `confidenceinterval-1.0.0/confidenceinterval/auc.py` & `confidenceinterval-1.0.1/confidenceinterval/auc.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/binary_metrics.py` & `confidenceinterval-1.0.1/confidenceinterval/binary_metrics.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/bootstrap.py` & `confidenceinterval-1.0.1/confidenceinterval/bootstrap.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/delong.py` & `confidenceinterval-1.0.1/confidenceinterval/delong.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/metrics.py` & `confidenceinterval-1.0.1/confidenceinterval/metrics.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/takahashi_methods.py` & `confidenceinterval-1.0.1/confidenceinterval/takahashi_methods.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval/utils.py` & `confidenceinterval-1.0.1/confidenceinterval/utils.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.0/confidenceinterval.egg-info/PKG-INFO` & `confidenceinterval-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.0
+Version: 1.0.1
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,106 +13,138 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The long missing python library for confidence intervals
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/jacobgil/confidenceinterval/workflows/Tests/badge.svg)
-[![Downloads](https://static.pepy.tech/personalized-badge/confidenceinterval?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=Monthly%20Downloads)](https://pepy.tech/project/confidenceintervals)
 
 `pip install confidenceinterval`
 
 This is a package that computes common machine learning metrics like F1, and returns their confidence intervals.
 
-⭐ Very easy to use, with the standard scikit-learn naming convention and interface:
 
-e.g roc_auc_score(y_true, y_pred).
+⭐ Very easy to use, with the standard scikit-learn naming convention and interface.
 
 ⭐ Support for many metrics, with modern confidence interval methods.
 
-⭐ Support for both analytical computation of the confidence intervals, and bootstrapping.
+⭐ Support for both analytical computation of the confidence intervals, and bootstrapping methods.
+
+⭐ Easy to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
+
+## The motivation
+
+A confidence interval gives you a lower and upper bound on your metric. It's affected by the sample size, and by how sensitive the metric is to changes in the data.
+
+When making decisions based on metrics, you should prefer narrow intervals. If the interval is wide, you can't be confident that your high performing metric is not just by luck.
+
+While confidence intervals are commonly used by statisticans, with many great R language implementations,
+they are astonishingly rarely used by python users, although python took over the data science world !
+
+Part of this is because there were no simple to use python packages for this.
 
-⭐ East to use interface to compute confidence intervals on new metrics that don't appear here, with bootstrapping.
 
 ## Getting started
 
 ```python
 from confidenceinterval import roc_auc_score
 auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95)
 auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
+auc, ci = roc_auc_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_percentile', n_resamples=5000)
 ```
 
+## All methods do an analytical computation by default, but can do bootsrapping instead
 By default all the methods return an analytical computation of the confidence interval (CI).
-For a bootstrap computation of the CI, for any of the methods belonw, you can just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
 
-## Supported methods
+For a bootstrap computation of the CI for any of the methods belonw, just specify method='bootstrap_bca', or method='bootstrap_percentile' or method='bootstrap_basic'.
+These are different ways of doing the bootstrapping, but method='bootstrap_bca' is the generalibly reccomended method.
+
+You can also pass the number of bootstrap resamples (n_resamples), and a random generator for controling the reproducability:
 
-### Get a confidence interval for any external metric
-With the bootstrap_ci method, you can get the CI for a an external metric method.
-As an example, lets get the CI for the balanced accuracy metric. It's not implemented yet in this package,
-but we can easily get the CI for it:
+```python
+random_state = np.random.default_rng()
+n_resamples=9999
+```
+
+## Get a confidence interval for any external metric with Bootstrapping
+With the bootstrap_ci method, you can get the CI for any metric function that gets y_true and y_pred as arguments.
+
+As an example, lets get the CI for the balanced accuracy metric from scikit-learn.
 
 ```python
 from confidenceinterval.bootstrap import bootstrap_ci
 # You can specify a random generator for reproducability, or pass None
 random_generator = np.random.default_rng()
 bootstrap_ci(y_true=y_true,
              y_pred=y_pred,
              metric=sklearn.metrics.balanced_accuracy_score,
              confidence_level=0.95,
              n_resamples=9999,
              method='bootstrap_bca',
              random_state=random_generator)
 ```
 
-### F1, Precision, Recall (with Macro and Micro averaging)
+## F1, Precision, Recall (with Macro and Micro averaging)
 ```python
 from confidence interval import precision_score, recall_score, f1_score
 ```
 
 These methods also accept average='micro' or average='macro'.
 
 The analytical computation here is using the (amazing) 2022 paper of Takahashi et al (reference below). 
 
 
-### ROC AUC
+## ROC AUC
 ```python
 from confidence interval import roc_auc_score
 ```
 The analytical computation here is a fast implementation of the DeLong method.
 
 
-### Binary metrics
+## Binary metrics
 ```python
-from confidence interval import accuracy_score, ppv_score, npv_score,
-                                tpr_score, fpr_score, tnr_score
+from confidence interval import accuracy_score,
+                                ppv_score,
+                                npv_score,
+                                tpr_score,
+                                fpr_score,
+                                tnr_score
+# Wilson is used by default:
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95)
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='jeffreys')
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='agresti_coull')
+ppv, ci = ppv_score(y_true, y_pred, confidence_level=0.95, method='bootstrap_bca')
+
 ```
 
 For these methods, the confidence interval is estimated by treating the ratio as a binomial proportion,
 see the [wiki page](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval).
 
 By default method='wilson', the wilson interval, which behaves better for smaller samples.
 
 method can be one of ['wilson', 'normal', 'agresti_coull', 'beta', 'jeffreys', 'binom_test'], or one of the boostrap methods.
 
 ----------
 
-### References
+## References
 
 The binomial confidence interval computation uses the statsmodels package:
 https://www.statsmodels.org/dev/generated/statsmodels.stats.proportion.proportion_confint.html
 
-Yandex data schhol implementation of the fast delong method:
+Yandex data school implementation of the fast delong method:
 https://github.com/yandexdataschool/roc_comparison
 
 https://ieeexplore.ieee.org/document/6851192
 X. Sun and W. Xu, "Fast Implementation of DeLong’s Algorithm for Comparing the Areas Under Correlated Receiver Operating Characteristic Curves," in IEEE Signal Processing Letters, vol. 21, no. 11, pp. 1389-1393, Nov. 2014, doi: 10.1109/LSP.2014.2337313.
 
 https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8936911/#APP2
+
 Confidence interval for micro-averaged F1 and macro-averaged F1 scores
 `Kanae Takahashi,1,2 Kouji Yamamoto,3 Aya Kuchiba,4,5 and Tatsuki Koyama6`
 
 B. Efron and R. J. Tibshirani, An Introduction to the Bootstrap, Chapman & Hall/CRC, Boca Raton, FL, USA (1993)
 
-Nathaniel E. Helwig, “Bootstrap Confidence Intervals”, http://users.stat.umn.edu/~helwig/notes/bootci-Notes.pdf
+http://users.stat.umn.edu/~helwig/notes/bootci-Notes.pdf
+`Nathaniel E. Helwig, “Bootstrap Confidence Intervals”`
+
 
 Bootstrapping (statistics), Wikipedia, https://en.wikipedia.org/wiki/Bootstrapping_%28statistics%29
```

### Comparing `confidenceinterval-1.0.0/setup.cfg` & `confidenceinterval-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confidenceinterval
-version = 1.0.0
+version = 1.0.1
 author = Jacob Gildenblat
 author_email = jacob.gildenblat@gmail.com
 description = Confidence Intervals in python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jacobgil/confidenceinterval
 project_urls =
```

### Comparing `confidenceinterval-1.0.0/setup.py` & `confidenceinterval-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='confidenceinterval',
-    version='1.0.0',
+    version='1.0.1',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Confidence Intervals in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/confidenceinterval',
     project_urls={
```

