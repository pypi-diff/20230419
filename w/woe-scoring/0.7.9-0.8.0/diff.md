# Comparing `tmp/woe_scoring-0.7.9.tar.gz` & `tmp/woe_scoring-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woe_scoring-0.7.9.tar", max compression
+gzip compressed data, was "woe_scoring-0.8.0.tar", max compression
```

## Comparing `woe_scoring-0.7.9.tar` & `woe_scoring-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2022-10-19 05:26:04.023549 woe_scoring-0.7.9/LICENSE
--rw-r--r--   0        0        0      533 2022-10-19 07:27:48.791953 woe_scoring-0.7.9/pyproject.toml
--rw-r--r--   0        0        0       80 2022-10-19 07:27:55.878684 woe_scoring-0.7.9/woe_scoring/__init__.py
--rw-r--r--   0        0        0       62 2022-10-19 05:26:04.024413 woe_scoring-0.7.9/woe_scoring/core/__init__.py
--rw-r--r--   0        0        0       94 2022-10-19 05:26:04.024664 woe_scoring-0.7.9/woe_scoring/core/binning/__init__.py
--rw-r--r--   0        0        0    15886 2022-10-19 05:26:04.024865 woe_scoring-0.7.9/woe_scoring/core/binning/functions.py
--rw-r--r--   0        0        0    10788 2022-10-19 07:28:39.481580 woe_scoring-0.7.9/woe_scoring/core/main.py
--rw-r--r--   0        0        0      150 2022-10-19 05:26:04.025257 woe_scoring-0.7.9/woe_scoring/core/model/__init__.py
--rw-r--r--   0        0        0    20930 2022-10-19 05:43:39.895766 woe_scoring-0.7.9/woe_scoring/core/model/functions.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 woe_scoring-0.7.9/setup.py
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 woe_scoring-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-10-19 05:26:04.023549 woe_scoring-0.8.0/LICENSE
+-rw-r--r--   0        0        0      533 2023-04-19 09:06:21.886073 woe_scoring-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-19 09:06:21.886220 woe_scoring-0.8.0/woe_scoring/__init__.py
+-rw-r--r--   0        0        0       62 2022-10-19 05:26:04.024413 woe_scoring-0.8.0/woe_scoring/core/__init__.py
+-rw-r--r--   0        0        0       94 2022-10-19 05:26:04.024664 woe_scoring-0.8.0/woe_scoring/core/binning/__init__.py
+-rw-r--r--   0        0        0    21992 2023-04-19 09:06:21.886869 woe_scoring-0.8.0/woe_scoring/core/binning/functions.py
+-rw-r--r--   0        0        0    10932 2022-10-19 09:46:50.410755 woe_scoring-0.8.0/woe_scoring/core/main.py
+-rw-r--r--   0        0        0      150 2022-10-19 05:26:04.025257 woe_scoring-0.8.0/woe_scoring/core/model/__init__.py
+-rw-r--r--   0        0        0    27095 2023-04-19 09:06:21.887225 woe_scoring-0.8.0/woe_scoring/core/model/functions.py
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 woe_scoring-0.8.0/setup.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 woe_scoring-0.8.0/PKG-INFO
```

### Comparing `woe_scoring-0.7.9/LICENSE` & `woe_scoring-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woe_scoring-0.7.9/pyproject.toml` & `woe_scoring-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woe_scoring"
-version = "0.7.9"
+version = "0.8.0"
 description = "Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API"
 authors = ["Stroganov Kirill <kiraplenkin@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = ">=1.19.5"
```

### Comparing `woe_scoring-0.7.9/woe_scoring/core/main.py` & `woe_scoring-0.8.0/woe_scoring/core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,17 @@
         self.coef_: List[float] = []
         self.intercept_: float = 0.0
         self.model = None
 
     def fit(self, x: pd.DataFrame, y: Union[pd.Series, np.ndarray]):
         x, self.feature_names_ = prepare_data(x, special_cols=self.special_cols)
 
+        if self.unused_cols:
+            self.feature_names_ = [feature for feature in self.feature_names_ if feature not in self.unused_cols]
+
         if self.C is None:
             self.C = 1.0e4 / x.shape[0]
 
         if self.max_vars is not None and self.max_vars < 1:
             self.max_vars = int(len(self.feature_names_) * self.max_vars)
 
         if self.selection_method == 'iv':
```

### Comparing `woe_scoring-0.7.9/woe_scoring/core/model/functions.py` & `woe_scoring-0.8.0/woe_scoring/core/model/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,38 @@
 from joblib import Parallel, delayed
 from sklearn.feature_selection import SequentialFeatureSelector
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import cross_val_score
 
 
 def _calc_score(
-        x: [pd.DataFrame, np.ndarray],
+        x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         var: str,
         random_state: int = None,
         class_weight: str = None,
         cv: int = 3,
-        c: float = None,
+        c: float = 1.0,
         scoring: str = "roc_auc",
-        n_jobs: int = None,
+        n_jobs: int = 1,
 ) -> float:
+    """Calculate the score of a feature.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        var: Name of the feature.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        scoring: Scoring method.
+        n_jobs: Number of jobs.
+    Returns:
+        Score of the feature."""
+
     model = LogisticRegression(
         random_state=random_state,
         class_weight=class_weight,
         n_jobs=n_jobs,
         C=c,
     )
     scores = cross_val_score(
@@ -37,25 +51,40 @@
         scoring=scoring,
         n_jobs=n_jobs,
     )
     return (np.mean(scores) * 2 - 1) * 100
 
 
 def _check_features_gini_threshold(
-        x: [pd.DataFrame, np.ndarray],
+        x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
         gini_threshold: float,
         random_state: int = None,
         class_weight: str = None,
         cv: int = 3,
         c: float = None,
         scoring: str = "roc_auc",
         n_jobs: int = None
 ) -> List[str]:
+    """Check if a feature has a Gini score below a threshold.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+        gini_threshold: Gini threshold.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        scoring: Scoring method.
+        n_jobs: Number of jobs.
+    Returns:
+        List of features with a Gini score below a threshold."""
+
     to_drop = [
         feature_name
         for feature_name in feature_names
         if _calc_score(
             x,
             y,
             feature_name,
@@ -68,29 +97,45 @@
         )
            < gini_threshold
     ]
     return [var for var in feature_names if var not in to_drop]
 
 
 def _check_correlation_threshold(
-        x: [pd.DataFrame, np.ndarray],
+        x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
         corr_threshold: float,
         random_state: int,
         class_weight: str,
         cv: int,
         c: float,
         scoring: str,
         n_jobs: int
 ) -> List[str]:
-    iter = product(feature_names, feature_names)
-    for var_a, var_b in iter:
+    """Check if a feature has a correlation score below a threshold.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+        corr_threshold: Correlation threshold.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        scoring: Scoring method.
+        n_jobs: Number of jobs.
+    Returns:
+        List of features with a correlation score below a threshold."""
+
+    iterator = product(feature_names, feature_names)
+    correlation = x[feature_names].corr()
+    for var_a, var_b in iterator:
         if (var_a != var_b) and (var_a in feature_names) and (var_b in feature_names) and abs(
-                x[feature_names].corr()[var_a][var_b]
+                correlation[var_a][var_b]
         ) >= corr_threshold:
             if _calc_score(
                     x,
                     y,
                     var_a,
                     random_state,
                     class_weight,
@@ -112,37 +157,62 @@
                 feature_names.remove(var_b)
             else:
                 feature_names.remove(var_a)
     return feature_names
 
 
 def _check_min_pct_group(
-        x: [pd.DataFrame, np.ndarray],
+        x: Union[pd.DataFrame, np.ndarray],
         feature_names: List[str],
         min_pct_group: float,
 ) -> List[str]:
+    """Check if a feature has a minimum percentage of values below a threshold.
+    Args:
+        x: DataFrame or numpy array.
+        feature_names: List of features.
+        min_pct_group: Minimum percentage of values below a threshold.
+    Returns:
+        List of features with a minimum percentage of values below a threshold."""
+
     to_drop = [
-        feature_name for feature_name in feature_names if x[feature_name].value_counts().min() < min_pct_group
+        feature_name for feature_name in feature_names if
+        x[feature_name].value_counts(normalize=True).min() < min_pct_group
     ]
     return [var for var in feature_names if var not in to_drop]
 
 
 def _feature_selector(
-        x: [pd.DataFrame, np.ndarray],
+        x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
         random_state: int,
         class_weight: str,
         cv: int,
         c: float,
         n_jobs: int,
         max_vars: Union[int, float],
         direction: str,
         scoring: str,
 ) -> List[str]:
+    """Feature selector.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        n_jobs: Number of jobs.
+        max_vars: Maximum number of features.
+        direction: Direction of selection.
+        scoring: Scoring method.
+    Returns:
+        List of features."""
+
     sfs = SequentialFeatureSelector(
         LogisticRegression(
             random_state=random_state,
             class_weight=class_weight,
             n_jobs=n_jobs,
             C=c,
         ),
@@ -153,29 +223,46 @@
         scoring=scoring,
     )
     sfs.fit(x[feature_names], y)
     return list(np.array(feature_names)[list(sfs.get_support())])
 
 
 def sequential_feature_select(
-        x: [pd.DataFrame],
+        x: pd.DataFrame,
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
         gini_threshold: float,
         corr_threshold: float,
         min_pct_group: float,
         random_state: int,
         class_weight: str,
         max_vars: Union[int, float],
         direction: str,
         cv: int,
         c: float,
         scoring: str,
         n_jobs: int,
 ) -> List[str]:
+    """Sequential feature selector.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+        gini_threshold: Gini threshold.
+        corr_threshold: Correlation threshold.
+        min_pct_group: Minimum percentage of values below a threshold.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        scoring: Scoring method.
+        n_jobs: Number of jobs.
+    Returns:
+        List of features."""
+
     feature_names = _check_min_pct_group(
         x,
         feature_names=feature_names,
         min_pct_group=min_pct_group,
     )
 
     feature_names = _check_features_gini_threshold(
@@ -214,14 +301,22 @@
         scoring=scoring,
         n_jobs=n_jobs
     )
     return feature_names
 
 
 def _calc_iv_dict(x: pd.DataFrame, y: np.ndarray, feature: str) -> Dict:
+    """Calculate IV for a feature.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature: Feature name.
+    Returns:
+        Dictionary with feature name as key and IV as value."""
+
     _iv = 0
     for value in x[feature].sort_values().unique():
         bad = y[x[feature] == value].sum()
         good = len(y[x[feature] == value]) - bad
         all_bad = y.sum()
         all_good = len(y) - all_bad
         _iv += ((good / all_good) - (bad / all_bad)) * value
@@ -239,20 +334,38 @@
         min_pct_group: float,
         random_state: int,
         class_weight: str,
         cv: int,
         c: float,
         scoring: str,
 ) -> List[str]:
+    """Information value feature selector.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+        iv_threshold: Information value threshold.
+        max_vars: Maximum number of features.
+        n_jobs: Number of jobs.
+        corr_threshold: Correlation threshold.
+        min_pct_group: Minimum percentage of values below a threshold.
+        random_state: Random state.
+        class_weight: Class weight.
+        cv: Number of folds.
+        c: Regularization parameter.
+        scoring: Scoring method.
+    Returns:
+        List of features."""
+
     temp_res_dict = Parallel(n_jobs=n_jobs)(
         delayed(_calc_iv_dict)(x, y, feature) for feature in feature_names
     )
     res_dict = {}
     for d in temp_res_dict:
-        res_dict.update(d)
+        res_dict |= d
 
     feature_names = [feature for feature in dict(sorted(res_dict.items(), key=itemgetter(1), reverse=True)) if
                      res_dict[feature] >= iv_threshold][:max_vars]
 
     feature_names = _check_min_pct_group(
         x,
         feature_names=feature_names,
@@ -269,42 +382,68 @@
         c=c,
         scoring=scoring,
         n_jobs=n_jobs
     )
     return feature_names
 
 
-def _check_pvalue(model: sm.Logit) -> List[int]:
+def _check_pvalue_and_sign(model: sm.Logit) -> List[int]:
+    """Check p-value.
+    Args:
+        model: Model.
+    Returns:
+        List of variables with p-values > 0.05 or positive sign."""
+
+    # return [
+    #     model.wald_test_terms().table.index[i]
+    #     for i, pvalue in enumerate(model.wald_test_terms().table["pvalue"])
+    #     if pvalue > 0.05
+    # ]
+
     return [
-        model.wald_test_terms().table.index[i]
-        for i, pvalue in enumerate(model.wald_test_terms().table["pvalue"])
-        if pvalue > 0.05
+        model.summary().tables[1].data[i][0]
+        for i in range(2, len(model.summary().tables[1].data))
+        if float(model.summary().tables[1].data[i][1]) > 0
+        or float(model.summary().tables[1].data[i][4]) > 0.05
     ]
 
 
 def create_model(
         x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
 ) -> sm.Logit:
+    """Create Logistic Regression model.
+    Args:
+        x: DataFrame or numpy array.
+        y: Series or numpy array.
+        feature_names: List of features.
+    Returns:
+        Model."""
+
     model = sm.Logit(y, sm.add_constant(x[feature_names])).fit()
 
-    to_drop = _check_pvalue(model)
+    to_drop = _check_pvalue_and_sign(model)
     while len(to_drop) > 0:
         feature_names = [feature for feature in feature_names if feature not in to_drop]
         model = sm.Logit(y, sm.add_constant(x[feature_names])).fit()
-        to_drop = _check_pvalue(model)
+        to_drop = _check_pvalue_and_sign(model)
 
     return model
 
 
 def save_reports(
         model: sm.Logit,
         path: str = os.getcwd()
 ) -> None:
+    """Save model reports.
+    Args:
+        model: Model.
+        path: Path to save reports."""
+
     try:
         with open(
                 os.path.join(path, "model_summary.txt"), "w"
         ) as outfile:
             outfile.write(model.summary().as_text())
 
         with open(
@@ -312,14 +451,21 @@
         ) as outfile:
             model.wald_test_terms().summary_frame().to_string(outfile)
     except Exception as e:
         print(f"Problem with saving: {e}")
 
 
 def predict_proba(x: Union[pd.DataFrame, np.ndarray], model: sm.Logit):
+    """Predict probabilities.
+    Args:
+        x: DataFrame or numpy array.
+        model: Model.
+    Returns:
+        Probabilities."""
+
     return model.predict(sm.add_constant(x))
 
 
 def generate_sql(
         feature_names: List[str],
         encoder,
         model_results,
@@ -390,28 +536,49 @@
         for idx in range(1, model_results.shape[0])
     )
     sql.extend(("))), ',', '.') as PD", " FROM a) ", "SELECT * FROM b"))
     return "".join(sql)
 
 
 def _calc_score_points(woe, coef, intercept, factor, offset: float, n_features: int) -> int:
-    b = offset - factor * intercept
-    s = -factor * coef * woe
-    return int(round(s + b / n_features))
+    """Calculate score points.
+    Args:
+        woe: WOE.
+        coef: Coefficient.
+        intercept: Intercept.
+        factor: Factor.
+        offset: Offset.
+        n_features: Number of features.
+    Returns:
+        Score points."""
+
+    return -(woe * coef + intercept / n_features) * factor + offset / n_features
 
 
 def _calc_stats_for_feature(
         idx,
         feature,
         feature_names: List[str],
         encoder,
         model_results,
         factor: float,
         offset: float,
 ) -> pd.DataFrame:
+    """Calculate stats for feature.
+    Args:
+        idx: Index.
+        feature: Feature.
+        feature_names: Feature names.
+        encoder: Encoder.
+        model_results: Model results.
+        factor: Factor.
+        offset: Offset.
+    Returns:
+        Stats for feature."""
+
     result_dict = {
         "feature": [],
         "coef": [],
         "pvalue": [],
         "bin": [],
         "WOE": [],
         "IV": [],
@@ -419,27 +586,27 @@
         "total": [],
         "event_cnt": [],
         "non_event_cnt": [],
         "event_rate": [],
         "score_ball": [],
     }
     if idx < 1:
-        result_dict["feature"].append(feature.replace("WOE_", ""))
-        result_dict["coef"].append(model_results.loc[idx, "coef"])
-        result_dict["pvalue"].append(model_results.loc[idx, "P>|z|"])
-        for key in result_dict:
+        _update_result_dict(
+            result_dict, feature, model_results, idx
+        )
+        for key, value in result_dict.items():
             if key not in ["feature", "coef", "pvalue"]:
-                result_dict[key].append("-")
+                value.append("-")
     else:
         for i, _ in enumerate(encoder.woe_iv_dict):
             if list(encoder.woe_iv_dict[i])[0] == feature.replace("WOE_", ""):
                 for _bin in encoder.woe_iv_dict[i][feature.replace("WOE_", "")]:
-                    result_dict["feature"].append(feature.replace("WOE_", ""))
-                    result_dict["coef"].append(model_results.loc[idx, "coef"])
-                    result_dict["pvalue"].append(model_results.loc[idx, "P>|z|"])
+                    _update_result_dict(
+                        result_dict, feature, model_results, idx
+                    )
                     result_dict["bin"].append(
                         [val if val != -1 else str(val).replace("-1", "missing") for val in _bin["bin"]]
                     )
                     result_dict["WOE"].append(_bin["woe"])
                     result_dict["IV"].append(_bin["iv"])
                     result_dict["percent_of_population"].append(_bin["pct"])
                     result_dict["total"].append(_bin["total"])
@@ -450,26 +617,52 @@
                         _calc_score_points(
                             woe=result_dict["WOE"][-1],
                             coef=result_dict["coef"][-1],
                             intercept=model_results.iloc[0, 1],
                             factor=factor,
                             offset=offset,
                             n_features=len(feature_names),
+
                         )
                     )
     return pd.DataFrame.from_dict(result_dict)
 
 
+def _update_result_dict(result_dict, feature, model_results, idx) -> None:
+    """Update result dict.
+    Args:
+        result_dict: Result dict.
+        feature: Feature.
+        model_results: Model results.
+        idx: Index.
+    Returns:
+        None."""
+
+    result_dict["feature"].append(feature.replace("WOE_", ""))
+    result_dict["coef"].append(model_results.loc[idx, "coef"])
+    result_dict["pvalue"].append(model_results.loc[idx, "P>|z|"])
+
+
 def _calc_stats(
         feature_names: List[str],
         encoder,
         model_results,
         factor: float,
         offset: float,
 ) -> List[pd.DataFrame]:
+    """Calculate stats.
+    Args:
+        feature_names: Feature names.
+        encoder: Encoder.
+        model_results: Model results.
+        factor: Factor.
+        offset: Offset.
+    Returns:
+        Stats."""
+
     feature_stats = []
     for idx, feature in enumerate(model_results.iloc[:, 0]):
         res_df = _calc_stats_for_feature(
             idx,
             feature,
             feature_names,
             encoder,
@@ -485,15 +678,26 @@
 def _build_excel_sheet_with_charts(
         feature_stats: list[pd.DataFrame],
         writer: pd.ExcelWriter,
         width: int = 640,
         height: int = 480,
         first_plot_position: str = 'A',
         second_plot_position: str = "J",
-):
+) -> None:
+    """Build excel sheet with charts.
+    Args:
+        feature_stats: Feature stats.
+        writer: Writer.
+        width: Width.
+        height: Height.
+        first_plot_position: First plot position.
+        second_plot_position: Second plot position.
+    Returns:
+        None."""
+
     # Get workbook link
     workbook = writer.book
     # Create merge format
     merge_format = workbook.add_format(
         {
             'bold': 1,
             'border': 1,
@@ -597,14 +801,26 @@
         encoder,
         model_results,
         base_scorecard_points: int,
         odds: int,
         points_to_double_odds: int,
         path: str,
 ) -> None:
+    """Save scorecard.
+    Args:
+        feature_names: Feature names.
+        encoder: Encoder.
+        model_results: Model results.
+        base_scorecard_points: Base scorecard points.
+        odds: Odds.
+        points_to_double_odds: Points to double odds.
+        path: Path.
+    Returns:
+        None."""
+
     factor = points_to_double_odds / np.log(2)
     offset = base_scorecard_points - factor * np.log(odds)
 
     feature_stats = _calc_stats(
         feature_names=feature_names,
         encoder=encoder,
         model_results=model_results,
```

### Comparing `woe_scoring-0.7.9/setup.py` & `woe_scoring-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pandas>=1.2.2',
  'scikit-learn>=0.24.1',
  'scipy>=1.6.1',
  'statsmodels>=0.12.2']
 
 setup_kwargs = {
     'name': 'woe-scoring',
-    'version': '0.7.9',
+    'version': '0.8.0',
     'description': 'Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API',
     'long_description': 'None',
     'author': 'Stroganov Kirill',
     'author_email': 'kiraplenkin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `woe_scoring-0.7.9/PKG-INFO` & `woe_scoring-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woe-scoring
-Version: 0.7.9
+Version: 0.8.0
 Summary: Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API
 License: MIT
 Author: Stroganov Kirill
 Author-email: kiraplenkin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

