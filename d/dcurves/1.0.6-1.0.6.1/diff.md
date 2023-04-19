# Comparing `tmp/dcurves-1.0.6.tar.gz` & `tmp/dcurves-1.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcurves-1.0.6.tar", max compression
+gzip compressed data, was "dcurves-1.0.6.1.tar", max compression
```

## Comparing `dcurves-1.0.6.tar` & `dcurves-1.0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0    11357 2023-04-12 20:17:58.498376 dcurves-1.0.6/LICENSE
--rw-r--r--   0        0        0     6148 2023-04-12 20:17:58.498484 dcurves-1.0.6/dcurves/.DS_Store
--rw-r--r--   0        0        0      237 2023-04-12 20:17:58.498546 dcurves-1.0.6/dcurves/__init__.py
--rw-r--r--   0        0        0     6871 2023-04-12 20:17:58.498643 dcurves-1.0.6/dcurves/_validate.py
--rw-r--r--   0        0        0    37679 2023-04-12 20:17:58.498907 dcurves-1.0.6/dcurves/data/df_binary.csv
--rw-r--r--   0        0        0    33284 2023-04-12 20:17:58.499080 dcurves-1.0.6/dcurves/data/df_case_control.csv
--rw-r--r--   0        0        0    50894 2023-04-12 20:17:58.499298 dcurves-1.0.6/dcurves/data/df_surv.csv
--rw-r--r--   0        0        0    19201 2023-04-12 20:17:58.499401 dcurves-1.0.6/dcurves/dca.py
--rw-r--r--   0        0        0     1068 2023-04-12 20:17:58.499508 dcurves-1.0.6/dcurves/load_test_data.py
--rw-r--r--   0        0        0     4780 2023-04-12 20:17:58.499580 dcurves-1.0.6/dcurves/plot_graphs.py
--rw-r--r--   0        0        0     1918 2023-04-12 20:17:58.499652 dcurves-1.0.6/dcurves/prevalence.py
--rw-r--r--   0        0        0     4927 2023-04-12 20:17:58.499738 dcurves-1.0.6/dcurves/risks.py
--rwxr-xr-x   0        0        0     1879 2023-04-12 20:17:58.499843 dcurves-1.0.6/docs/README.md
--rw-r--r--   0        0        0      941 2023-04-19 15:47:18.525439 dcurves-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 dcurves-1.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2023-04-12 20:17:58.498376 dcurves-1.0.6.1/LICENSE
+-rw-r--r--   0        0        0     6148 2023-04-12 20:17:58.498484 dcurves-1.0.6.1/dcurves/.DS_Store
+-rw-r--r--   0        0        0      237 2023-04-12 20:17:58.498546 dcurves-1.0.6.1/dcurves/__init__.py
+-rw-r--r--   0        0        0     6871 2023-04-12 20:17:58.498643 dcurves-1.0.6.1/dcurves/_validate.py
+-rw-r--r--   0        0        0    37679 2023-04-12 20:17:58.498907 dcurves-1.0.6.1/dcurves/data/df_binary.csv
+-rw-r--r--   0        0        0    33284 2023-04-12 20:17:58.499080 dcurves-1.0.6.1/dcurves/data/df_case_control.csv
+-rw-r--r--   0        0        0    50894 2023-04-12 20:17:58.499298 dcurves-1.0.6.1/dcurves/data/df_surv.csv
+-rw-r--r--   0        0        0    19201 2023-04-12 20:17:58.499401 dcurves-1.0.6.1/dcurves/dca.py
+-rw-r--r--   0        0        0     1068 2023-04-12 20:17:58.499508 dcurves-1.0.6.1/dcurves/load_test_data.py
+-rw-r--r--   0        0        0     4792 2023-04-19 18:26:36.630912 dcurves-1.0.6.1/dcurves/plot_graphs.py
+-rw-r--r--   0        0        0     1918 2023-04-12 20:17:58.499652 dcurves-1.0.6.1/dcurves/prevalence.py
+-rw-r--r--   0        0        0     4927 2023-04-12 20:17:58.499738 dcurves-1.0.6.1/dcurves/risks.py
+-rwxr-xr-x   0        0        0     1879 2023-04-12 20:17:58.499843 dcurves-1.0.6.1/docs/README.md
+-rw-r--r--   0        0        0     1134 2023-04-19 18:27:43.569816 dcurves-1.0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 dcurves-1.0.6.1/PKG-INFO
```

### Comparing `dcurves-1.0.6/LICENSE` & `dcurves-1.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/.DS_Store` & `dcurves-1.0.6.1/dcurves/.DS_Store`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/_validate.py` & `dcurves-1.0.6.1/dcurves/_validate.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/data/df_binary.csv` & `dcurves-1.0.6.1/dcurves/data/df_binary.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/data/df_case_control.csv` & `dcurves-1.0.6.1/dcurves/data/df_case_control.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/data/df_surv.csv` & `dcurves-1.0.6.1/dcurves/data/df_surv.csv`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/dca.py` & `dcurves-1.0.6.1/dcurves/dca.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/load_test_data.py` & `dcurves-1.0.6.1/dcurves/load_test_data.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/plot_graphs.py` & `dcurves-1.0.6.1/dcurves/plot_graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         plt.plot(
             single_model_df["threshold"],
             single_model_df["net_benefit"],
             color=color_name,
         )
         plt.ylim(y_limits)
         plt.legend(modelnames)
-        plt.grid(b=True, which="both", axis="both")
+        plt.grid(visible=True, which="both", axis="both")
         plt.xlabel("Threshold Values")
         plt.ylabel("Calculated Net Benefit")
     plt.show()
 
 
 def _plot_net_intervention_avoided(
     plot_df: pd.DataFrame,
@@ -95,15 +95,15 @@
             single_model_df["threshold"],
             single_model_df["net_intervention_avoided"],
             color=color_name,
         )
 
         plt.ylim(y_limits)
         plt.legend(modelnames)
-        plt.grid(b=True, which="both", axis="both")
+        plt.grid(visible=True, which="both", axis="both")
         plt.xlabel("Threshold Values")
         plt.ylabel("Calculated Net Reduction of Interventions")
     plt.show()
 
 
 def plot_graphs(
     plot_df: pd.DataFrame,
```

### Comparing `dcurves-1.0.6/dcurves/prevalence.py` & `dcurves-1.0.6.1/dcurves/prevalence.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/dcurves/risks.py` & `dcurves-1.0.6.1/dcurves/risks.py`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/docs/README.md` & `dcurves-1.0.6.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `dcurves-1.0.6/pyproject.toml` & `dcurves-1.0.6.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcurves"
-version = "1.0.6"
+version = "1.0.6.1"
 description = "A Python package for Decision Curve Analysis to evaluate prediction models, molecular markers, and diagnostic tests. For RELEASE NOTES, check RELEASE.md here: https://github.com/MSKCC-Epi-Bio/dcurves/RELEASE.md"
 authors = ["shaunporwal <shaun.porwal@gmail.com>", "rohansingh <singhrohan@outlook.com>"]
 readme = "docs/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 lifelines = "~0.27.4"
@@ -19,14 +19,23 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "~7.2.1"
 jupyterlab = "~3.6.1"
 tox = "^4.4.6"
 pytest-cov = "^4.0.0"
 black = "^23.1.0"
 pylint = "^2.16.1"
+towncrier = "^22.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [repositories]
 pypi = {url = "https://pypi.org/"}
+
+[tool.towncrier]
+package = "dcurves"
+package_dir = "dcurves"
+filename = "CHANGELOG.md"
+directory = "newsfragments"
+underlines = ["^", "~"]
+issue_format = "GH-{issue}"
```

### Comparing `dcurves-1.0.6/PKG-INFO` & `dcurves-1.0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcurves
-Version: 1.0.6
+Version: 1.0.6.1
 Summary: A Python package for Decision Curve Analysis to evaluate prediction models, molecular markers, and diagnostic tests. For RELEASE NOTES, check RELEASE.md here: https://github.com/MSKCC-Epi-Bio/dcurves/RELEASE.md
 Author: shaunporwal
 Author-email: shaun.porwal@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

