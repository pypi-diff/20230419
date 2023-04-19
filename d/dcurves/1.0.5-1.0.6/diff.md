# Comparing `tmp/dcurves-1.0.5.tar.gz` & `tmp/dcurves-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcurves-1.0.5.tar", max compression
+gzip compressed data, was "dcurves-1.0.6.tar", max compression
```

## Comparing `dcurves-1.0.5.tar` & `dcurves-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0    11357 2021-08-15 21:03:33.309705 dcurves-1.0.5/LICENSE
--rw-r--r--   0        0        0     6148 2023-01-17 08:12:45.096584 dcurves-1.0.5/dcurves/.DS_Store
--rw-r--r--   0        0        0      144 2023-02-06 20:45:46.884334 dcurves-1.0.5/dcurves/__init__.py
--rw-r--r--   0        0        0     6871 2023-02-06 20:42:17.006154 dcurves-1.0.5/dcurves/_validate.py
--rw-r--r--   0        0        0    37679 2023-01-17 08:12:45.107152 dcurves-1.0.5/dcurves/data/df_binary.csv
--rw-r--r--   0        0        0    33284 2023-01-17 08:12:45.109518 dcurves-1.0.5/dcurves/data/df_case_control.csv
--rw-r--r--   0        0        0    50894 2023-01-17 08:12:45.110219 dcurves-1.0.5/dcurves/data/df_surv.csv
--rw-r--r--   0        0        0    19130 2023-02-07 00:05:51.694752 dcurves-1.0.5/dcurves/dca.py
--rw-r--r--   0        0        0     1068 2023-02-06 20:42:17.009911 dcurves-1.0.5/dcurves/load_test_data.py
--rw-r--r--   0        0        0     4778 2023-02-06 23:59:28.127541 dcurves-1.0.5/dcurves/plot_graphs.py
--rw-r--r--   0        0        0     1918 2023-02-06 23:55:45.804049 dcurves-1.0.5/dcurves/prevalence.py
--rw-r--r--   0        0        0     4927 2023-02-06 23:56:46.288922 dcurves-1.0.5/dcurves/risks.py
--rwxr-xr-x   0        0        0     2839 2023-02-05 21:19:31.021821 dcurves-1.0.5/docs/README.md
--rw-r--r--   0        0        0      779 2023-02-07 14:59:34.489165 dcurves-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 dcurves-1.0.5/setup.py
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 dcurves-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2023-04-12 20:17:58.498376 dcurves-1.0.6/LICENSE
+-rw-r--r--   0        0        0     6148 2023-04-12 20:17:58.498484 dcurves-1.0.6/dcurves/.DS_Store
+-rw-r--r--   0        0        0      237 2023-04-12 20:17:58.498546 dcurves-1.0.6/dcurves/__init__.py
+-rw-r--r--   0        0        0     6871 2023-04-12 20:17:58.498643 dcurves-1.0.6/dcurves/_validate.py
+-rw-r--r--   0        0        0    37679 2023-04-12 20:17:58.498907 dcurves-1.0.6/dcurves/data/df_binary.csv
+-rw-r--r--   0        0        0    33284 2023-04-12 20:17:58.499080 dcurves-1.0.6/dcurves/data/df_case_control.csv
+-rw-r--r--   0        0        0    50894 2023-04-12 20:17:58.499298 dcurves-1.0.6/dcurves/data/df_surv.csv
+-rw-r--r--   0        0        0    19201 2023-04-12 20:17:58.499401 dcurves-1.0.6/dcurves/dca.py
+-rw-r--r--   0        0        0     1068 2023-04-12 20:17:58.499508 dcurves-1.0.6/dcurves/load_test_data.py
+-rw-r--r--   0        0        0     4780 2023-04-12 20:17:58.499580 dcurves-1.0.6/dcurves/plot_graphs.py
+-rw-r--r--   0        0        0     1918 2023-04-12 20:17:58.499652 dcurves-1.0.6/dcurves/prevalence.py
+-rw-r--r--   0        0        0     4927 2023-04-12 20:17:58.499738 dcurves-1.0.6/dcurves/risks.py
+-rwxr-xr-x   0        0        0     1879 2023-04-12 20:17:58.499843 dcurves-1.0.6/docs/README.md
+-rw-r--r--   0        0        0      941 2023-04-19 15:47:18.525439 dcurves-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 dcurves-1.0.6/PKG-INFO
```

### Comparing `dcurves-1.0.5/LICENSE` & `dcurves-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/.DS_Store` & `dcurves-1.0.6/dcurves/.DS_Store`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/_validate.py` & `dcurves-1.0.6/dcurves/_validate.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/data/df_binary.csv` & `dcurves-1.0.6/dcurves/data/df_binary.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/data/df_case_control.csv` & `dcurves-1.0.6/dcurves/data/df_case_control.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/data/df_surv.csv` & `dcurves-1.0.6/dcurves/data/df_surv.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/dca.py` & `dcurves-1.0.6/dcurves/dca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
-This module houses most of the functions used in performing decision curve analysis,
-along with the main user-facing dca() functions used for binary and survival outcomes.
+This module houses most of the functions used in performing decision curve 
+analysis, along with the main user-facing dca() functions used for binary
+and survival outcomes.
 """
+
 from typing import Optional, Union, Iterable
 import pandas as pd
 import lifelines
 
 from .risks import _create_risks_df, _rectify_model_risk_boundaries
 from .prevalence import _calc_prevalence
 
@@ -20,16 +22,16 @@
     """
     Create initial dataframe that will form the outputted table containing
     net benefit/interventions avoided values for plotting.
 
     Parameters
     ----------
     thresholds : Iterable
-        Threshold values (x values) at which net benefit and net interventions avoided will be
-        calculated
+        Threshold values (x values) at which net benefit and net
+        interventions avoided will be calculated
     modelnames : list[str]
         Column names from risks_df that contain model risk scores
     input_df_rownum : int
         Number of rows in original input dataframe
     prevalence_value : int or float
         Calculated prevalence value
     harm : dict[float]
@@ -39,15 +41,17 @@
     -------
     pd.DataFrame
         DataFrame set with initial parameters
     """
 
     modelnames = modelnames + ["all", "none"]
     rows = len(thresholds) * len(modelnames)
-    model_column = pd.Series([x for y in modelnames for x in [y] * len(thresholds)])
+    model_column = pd.Series(
+        [x for y in modelnames
+         for x in [y] * len(thresholds)])
     threshold_column = pd.Series(list(thresholds) * len(modelnames))
     n_column = pd.Series([input_df_rownum] * rows)
     prevalence_column = pd.Series([prevalence_value] * rows)
     harm_column = pd.Series([0] * rows)
 
     if harm is not None:
         for model in harm.keys():
@@ -70,24 +74,26 @@
     return initial_df
 
 
 def _calc_test_pos_rate(
     risks_df: pd.DataFrame, thresholds: Iterable, model: str
 ) -> pd.Series:
     """
-    Calculate each test positive rate per threshold value, which will be used to calculate true
-    and false positive rates per threshold values in the survival DCA case.
+    Calculate each test positive rate per threshold value,
+    which will be used to calculate true and false positive rates 
+    per threshold values in the survival DCA case.
 
     Parameters
     ----------
     risks_df : pd.DataFrame
-        Data containing (converted if necessary) risk scores (scores ranging from 0 to 1
-        for columns of interest)
+        Data containing (converted if necessary) risk scores 
+        (scores ranging from 0 to 1 for columns of interest)
     thresholds : Iterable
-        Threshold values (x values) at which net test positive rate will be calculated
+        Threshold values (x values) at which net test positive 
+        rate will be calculated
     model : str
         Model column name in risks_df
 
     Returns
     -------
     pd.Series
         Calculated test positive rates for each threshold value for a model
@@ -99,31 +105,32 @@
         risk_above_thresh_tf_dict = dict(
             pd.Series(risks_df[model] >= threshold).value_counts()
         )
 
         if True not in risk_above_thresh_tf_dict:
             test_pos_rate.append(0 / len(risks_df.index))
         elif True in risk_above_thresh_tf_dict:
-            test_pos_rate.append(risk_above_thresh_tf_dict[True] / len(risks_df.index))
+            test_pos_rate.append(
+                risk_above_thresh_tf_dict[True] / len(risks_df.index))
 
     return pd.Series(test_pos_rate)
 
 
 def _calc_risk_rate_among_test_pos(
     risks_df: pd.DataFrame,
     outcome: str,
     model: str,
     thresholds: Iterable,
     time: Union[float, int],
     time_to_outcome_col: str,
 ) -> pd.Series:
     """
     Calculate the risk rate among test positive cases for each threshold value
-    , which will be used to calculate true and false positive rates per threshold
-    values in the survival DCA case.
+    , which will be used to calculate true and false positive rates per 
+    threshold values in the survival DCA case.
 
     Parameters
     ----------
     risks_df : pd.DataFrame
         Data containing (converted if necessary) risk scores (scores ranging
         from 0 to 1 for columns of interest)
     outcome : str
@@ -228,15 +235,16 @@
 
         tp_rate = []
         for threshold in thresholds:
             true_tf_above_thresh_count = (
                 (true_outcome[model] >= threshold).value_counts().get(True, 0)
             )
             tp_rate.append(
-                true_tf_above_thresh_count / num_true_outcomes * prevalence_value
+                (true_tf_above_thresh_count /
+                 num_true_outcomes) * prevalence_value
             )
 
     return pd.Series(tp_rate)
 
 
 def _calc_fp_rate(
     risks_df: pd.DataFrame,
@@ -451,29 +459,29 @@
     modelnames: list,
     thresholds: Iterable = [i / 100 for i in range(0, 100)],
     harm: Optional[dict] = None,
     models_to_prob: Optional[list] = None,
     prevalence: Optional[Union[float, int]] = None,
     time: Optional[Union[float, int]] = None,
     time_to_outcome_col: Optional[str] = None,
-    nper: Optional[int] = 1,
+    nper: Optional[int] = 1
 ) -> pd.DataFrame:
     """
     Decision curve analysis is a method for evaluating and comparing prediction
     models that incorporates clinical consequences, requiring only the data set
-    on which the models are tested, and can be applied to models that have
-    either continuous or dichotomous results. The dca function performs decision
+    on which the models are tested, and can be applied to models that have eit-
+    her continuous or dichotomous results. The dca function performs decision
     curve analysis for binary and survival outcomes.
 
     Parameters
     ----------
-    data : pd.DataFrame
+    data: pd.DataFrame
         Initial raw data ideally containing risk scores (scores ranging from 0
         to 1), or else predictor/model values, and outcome of interest
-    outcome : str
+    outcome: str
         Column name of outcome of interest in risks_df
     modelnames : list[str]
         Column names from data that contain model risk scores or values
     thresholds : Iterable
         Threshold values (x values) at which net benefit and net interventions
         avoided will be calculated
     harm : dict[float]
@@ -494,15 +502,15 @@
     Returns
     -------
     pd.DataFrame
         Data containing net benefit and interventions avoided scores to be plotted
         against threshold values
 
     Examples
-    ________
+    --------
     from dcurves import dca, plot_graphs, load_test_data
 
     import numpy as np
 
     |
 
     dca_results = \
```

### Comparing `dcurves-1.0.5/dcurves/load_test_data.py` & `dcurves-1.0.6/dcurves/load_test_data.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/plot_graphs.py` & `dcurves-1.0.6/dcurves/plot_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-This module houses plotting functions used in the user-facing plot_graphs() function
-to plot net-benefit scores and net interventions avoided.
+This module houses plotting functions used in the user-facing plot_graphs() 
+function to plot net-benefit scores and net interventions avoided.
 """
 from typing import Optional, Iterable
 import random
 import matplotlib.pyplot as plt
 import pandas as pd
 
 
@@ -150,7 +150,8 @@
 
     if graph_type == "net_benefit":
         _plot_net_benefit(plot_df=plot_df, y_limits=y_limits, color_names=color_names)
     elif graph_type == "net_intervention_avoided":
         _plot_net_intervention_avoided(
             plot_df=plot_df, y_limits=y_limits, color_names=color_names
         )
+
```

### Comparing `dcurves-1.0.5/dcurves/prevalence.py` & `dcurves-1.0.6/dcurves/prevalence.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/dcurves/risks.py` & `dcurves-1.0.6/dcurves/risks.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.5/docs/README.md` & `dcurves-1.0.6/docs/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,49 @@
+## Contributors
+
+- Shaun Porwal (shaun.porwal@gmail.com)
+
 # dcurves
 Diagnostic and prognostic models are typically evaluated with measures of accuracy that do not address clinical
 consequences. Decision-analytic techniques allow assessment of clinical outcomes, but often require collection of
 additional information that may be cumbersome to apply to models that yield continuous results. Decision Curve
 Analysis is a method for evaluating and comparing prediction models that incorporates clinical consequences,
 requiring only the data set on which the models are tested, and can be applied to models that have either continuous or
 dichotomous results. The dca function performs decision curve analysis for binary and survival outcomes. Review the
 DCA tutorial (towards the bottom) for a detailed walk-through of various applications. Also, see
 www.decisioncurveanalysis.org for more information.
 
-#### Installation
 
-###### Use the package manager [pip](https://pip.pypa.io/en/stable/) to install dcurves
+## Table Of Contents
+
+The documentation follows the best practice for
+project documentation as described by Daniele Procida
+in the [Diátaxis documentation framework](https://diataxis.fr/)
+and consists of four separate parts:
+
+1. [Tutorials](tutorials.md)
+2. [How-To Guides](how-to-guides.md)
+3. [Reference](reference.md)
+4. [Explanation](explanation.md)
+
+Quickly find what you're looking for depending on
+your use case by looking at the different pages.
+
+## Project Overview
+
+::: dcurves
 
-###### While this is the quick-and-dirty method to install a package such as `dcurves` into your local environment, you should use a virtual environment and make sure your dependencies are compatible while using `dcurves`
 
-```bash
-pip install dcurves
-```
-###### Import dcurves and numpy
-```python
-from dcurves import dca, plot_graphs, load_test_data
-import numpy as np
-```
-##### Usage - Binary Outcomes
-```python
-from dcurves import dca, plot_graphs, load_test_data
-import numpy as np
-
-dca_results = \
-    dca(
-        data=load_test_data.load_binary_df(),
-        outcome='cancer',
-        modelnames=['famhistory'],
-        thresholds=np.arange(0,0.46,0.01)
-    )
-
-plot_graphs(
-    plot_df=dca_results,
-    graph_type='net_benefit',
-    y_limits=[-0.05, 0.15],
-    color_names=['blue', 'red', 'green']
-)
-```
-##### Usage - Survival Outcomes
-```python
-from dcurves import dca, plot_graphs, load_test_data
-import numpy as np
-
-dca_results = \
-    dca(
-        data=load_test_data.load_survival_df(),
-        outcome='cancer',
-        modelnames=['famhistory', 'marker', 'cancerpredmarker'],
-        models_to_prob=['marker'],
-        thresholds=np.arange(0,0.46,0.01),
-        time_to_outcome_col='ttcancer',
-        time=1
-    )
-
-plot_graphs(
-    plot_df=dca_results,
-    graph_type='net_benefit',
-    y_limits=[-0.025, 0.175],
-    color_names=['blue', 'red', 'green', 'purple', 'black']
-)
-```
-#### In-depth tutorial and explanations:
+## In-depth tutorial and explanations:
 ###### https://www.danieldsjoberg.com/dca-tutorial/dca-tutorial-python.html
 
-#### Contributing
+## Contributing
 
 ###### Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change
 
 ###### Please make sure to update tests as appropriate
 
-#### License
+## License
 [Apache 2.0]([https://choosealicense.com/licenses/apache-2.0/])
 
-##### Note
+## Note
 ###### setup.py is deprecated now that dependencies are managed by `poetry` package manager
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcurves-1.0.5/pyproject.toml` & `dcurves-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "dcurves"
-version = "1.0.5"
+version = "1.0.6"
 description = "A Python package for Decision Curve Analysis to evaluate prediction models, molecular markers, and diagnostic tests. For RELEASE NOTES, check RELEASE.md here: https://github.com/MSKCC-Epi-Bio/dcurves/RELEASE.md"
-authors = ["shaunporwal <shaun.porwal@gmail.com>"]
+authors = ["shaunporwal <shaun.porwal@gmail.com>", "rohansingh <singhrohan@outlook.com>"]
 readme = "docs/README.md"
 
 [tool.poetry.dependencies]
-python = "~3.11.1"
+python = "^3.8"
 lifelines = "~0.27.4"
 matplotlib = "^3.5.2"
 pandas = "~1.5.3"
-statsmodels = "~0.13.2"
+statsmodels = "~0.13.5"
 typing = "~3.7.4.3"
+mkdocs = "^1.4.2"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+mkdocs-material = "^9.0.14"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "~7.2.1"
 jupyterlab = "~3.6.1"
+tox = "^4.4.6"
 pytest-cov = "^4.0.0"
 black = "^23.1.0"
 pylint = "^2.16.1"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [repositories]
 pypi = {url = "https://pypi.org/"}
```

