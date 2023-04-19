# Comparing `tmp/fold_wrappers-0.0.2.tar.gz` & `tmp/fold_wrappers-0.1.0.tar.gz`

## Comparing `fold_wrappers-0.0.2.tar` & `fold_wrappers-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/.isort.cfg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/examples/statsforecast.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/convenience.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/lightgbm.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/neuralforecast.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/prophet.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/sktime.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/statsforecast.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/statsmodels.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/fold_wrappers/xgboost.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/LICENSE
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/README.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 fold_wrappers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.isort.cfg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/examples/statsforecast.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/convenience.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/lightgbm.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/neuralforecast.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/prophet.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/sktime.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/statsforecast.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/statsmodels.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/xgboost.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/LICENSE
+-rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/README.md
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/PKG-INFO
```

### Comparing `fold_wrappers-0.0.2/.vscode/settings.json` & `fold_wrappers-0.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/examples/statsforecast.py` & `fold_wrappers-0.1.0/examples/statsforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/convenience.py` & `fold_wrappers-0.1.0/fold_wrappers/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/lightgbm.py` & `fold_wrappers-0.1.0/fold_wrappers/lightgbm.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/neuralforecast.py` & `fold_wrappers-0.1.0/fold_wrappers/neuralforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/prophet.py` & `fold_wrappers-0.1.0/fold_wrappers/prophet.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/sktime.py` & `fold_wrappers-0.1.0/fold_wrappers/sktime.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/statsforecast.py` & `fold_wrappers-0.1.0/fold_wrappers/statsforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/statsmodels.py` & `fold_wrappers-0.1.0/fold_wrappers/statsmodels.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/fold_wrappers/xgboost.py` & `fold_wrappers-0.1.0/fold_wrappers/xgboost.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/.gitignore` & `fold_wrappers-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/LICENSE` & `fold_wrappers-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.0.2/README.md` & `fold_wrappers-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,36 +23,36 @@
     <a href="https://dream-faster.github.io/fold-wrappers/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 # Available models
 
-|                                                                                                                                                                                                                                             | Name                                   |                          Link                          | Supports<br />Online <br />updating | Wrapper Name<br />& Import Location                                            |
-| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:| :------------------------------------- | :----------------------------------------------------: | :---------------------------------: | ------------------------------------------------------------------------------ |
-| <img alt='StatsDorecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                                                                      | StatsForecast                          |   [GitHub](https://github.com/Nixtla/statsforecast)    |                 ❌                  | **WrapStatsForecast**<br />`from fold_wrappers import WrapStatsForecast` |
-| <img alt='NeuralForecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                                                                      | NeuralForecast (beta)                          |   [GitHub](https://github.com/Nixtla/neuralforecast)    |                 ❌                  | **WrapNeuralForecast**<br />`from fold_wrappers import WrapNeuralForecast` |
-| <img alt='XGBoost Logo' src='https://camo.githubusercontent.com/0ea6e7814dd771f740509bbb668d251d485a6e21f12e287be7cc2275e0eab1d1/68747470733a2f2f7867626f6f73742e61692f696d616765732f6c6f676f2f7867626f6f73742d6c6f676f2e737667' height=64> | XGBoost                                |       [GitHub](https://github.com/dmlc/xgboost)        |                 ✅                    | **WrapXGB**<br />`from fold_wrappers import WrapXGB`               |
-| <img alt='LightGBM Logo' src='https://lightgbm.readthedocs.io/en/latest/_images/LightGBM_logo_black_text.svg' height=64> | LightGBM                                |       [GitHub](https://github.com/Microsoft/LightGBM)        |                 ✅                    | **WrapLGBM**<br />`from fold_wrappers import WrapLGBM`               |
-| <img alt='Sktime Logo' src='https://github.com/sktime/sktime/raw/main/docs/source/images/sktime-logo.jpg?raw=true' height=64>                                                                                                               | SKTime (beta)                                 |       [GitHub](https://github.com/sktime/sktime)       |                 ✅                  | **WrapSktime**<br />`from fold_wrappers import WrapSktime`                |
-| <img alt='Statsmodels Logo' src='https://github.com/statsmodels/statsmodels/raw/main/docs/source/images/statsmodels-logo-v2-horizontal.svg' width=160>                                                                                      | Statsmodels                            |  [GitHub](https://github.com/statsmodels/statsmodels)  |                 ✅                  | **WrapStatsModels**<br />`from fold_wrappers import WrapStatsModels` |
-| <img alt='Prophet Logo' src='https://miro.medium.com/v2/resize:fit:964/0*tVCene42rgUTNv9Q.png' width=160>                                                                                                                                   | Prophet                                |     [GitHub](https://github.com/facebook/prophet)      |                 ✅                  | **WrapProphet**<br />`from fold_wrappers import WrapProphet`             |
-| <img alt='Scikit-Learn Logo' src='https://raw.githubusercontent.com/scikit-learn/scikit-learn/main/doc/logos/scikit-learn-logo.png' width=160>                                                                                              | Sklearn <br/>(natively available in `fold`) | [GitHub](https://github.com/scikit-learn/scikit-learn) |             🟡<br/>(some)              | Sklearn doesn't need to be wrapped,<br />just pass in the models.              |
+|                                                                                                                                                                                                                                             | Name                                        |                          Link                          | Supports<br />Online <br />updating | Wrapper Name<br />& Import Location                                        |
+|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------|:------------------------------------------------------:|:-----------------------------------:|----------------------------------------------------------------------------|
+|                                                   <img alt='StatsDorecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                    | StatsForecast                               |   [GitHub](https://github.com/Nixtla/statsforecast)    |                  ❌                  | **WrapStatsForecast**<br />`from fold_wrappers import WrapStatsForecast`   |
+|                                                   <img alt='NeuralForecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                   | NeuralForecast (beta)                       |   [GitHub](https://github.com/Nixtla/neuralforecast)   |                  ❌                  | **WrapNeuralForecast**<br />`from fold_wrappers import WrapNeuralForecast` |
+| <img alt='XGBoost Logo' src='https://camo.githubusercontent.com/0ea6e7814dd771f740509bbb668d251d485a6e21f12e287be7cc2275e0eab1d1/68747470733a2f2f7867626f6f73742e61692f696d616765732f6c6f676f2f7867626f6f73742d6c6f676f2e737667' height=64> | XGBoost                                     |       [GitHub](https://github.com/dmlc/xgboost)        |                  ✅                  | **WrapXGB**<br />`from fold_wrappers import WrapXGB`                       |
+|                                                          <img alt='LightGBM Logo' src='https://lightgbm.readthedocs.io/en/latest/_images/LightGBM_logo_black_text.svg' height=64>                                                           | LightGBM                                    |    [GitHub](https://github.com/Microsoft/LightGBM)     |                  ✅                  | **WrapLGBM**<br />`from fold_wrappers import WrapLGBM`                     |
+|                                                        <img alt='Sktime Logo' src='https://github.com/sktime/sktime/raw/main/docs/source/images/sktime-logo.jpg?raw=true' height=64>                                                        | SKTime (beta)                               |       [GitHub](https://github.com/sktime/sktime)       |                  ✅                  | **WrapSktime**<br />`from fold_wrappers import WrapSktime`                 |
+|                                           <img alt='Statsmodels Logo' src='https://github.com/statsmodels/statsmodels/raw/main/docs/source/images/statsmodels-logo-v2-horizontal.svg' width=160>                                            | Statsmodels                                 |  [GitHub](https://github.com/statsmodels/statsmodels)  |                  ✅                  | **WrapStatsModels**<br />`from fold_wrappers import WrapStatsModels`       |
+|                                                                  <img alt='Prophet Logo' src='https://miro.medium.com/v2/resize:fit:964/0*tVCene42rgUTNv9Q.png' width=160>                                                                  | Prophet                                     |     [GitHub](https://github.com/facebook/prophet)      |                  ✅                  | **WrapProphet**<br />`from fold_wrappers import WrapProphet`               |
+|                                               <img alt='Scikit-Learn Logo' src='https://raw.githubusercontent.com/scikit-learn/scikit-learn/main/doc/logos/scikit-learn-logo.png' width=160>                                                | Sklearn <br/>(natively available in `fold`) | [GitHub](https://github.com/scikit-learn/scikit-learn) |            🟡<br/>(some)            | Sklearn doesn't need to be wrapped,<br />just pass in the models.          |
 
 # Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold-wrappers/archive/main.zip
+  pip install fold-wrappers
   ```
 - Depending on what model you'd like to wrap, you can either install the library directly or run
    ```
-  pip install "git+https://github.com/dream-faster/fold-wrappers.git#egg=fold-wrappers[<your_library_name>]"
+  pip install "fold-wrappers[<your_library_name>]"
   ```
 
 # Quickstart
```

#### html2text {}

```diff
@@ -8,21 +8,21 @@
                              To be used with Fold.
 
                               Explore_the_docs_Â»
 
 # Available models | | Name | Link | Supports
 Online
 updating | Wrapper Name
-& Import Location | | :--------------------------------------------------------
+& Import Location | |:---------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---------------------:| :------------------------------------- | :--------------
---------------------------------------: | :---------------------------------: |
------------------------------------------------------------------------------
-- | | [StatsDorecast Logo] | StatsForecast | [GitHub](https://github.com/
+--------------------:|:--------------------------------------------|:----------
+--------------------------------------------:|:--------------------------------
+---:|--------------------------------------------------------------------------
+--| | [StatsDorecast Logo] | StatsForecast | [GitHub](https://github.com/
 Nixtla/statsforecast) | â | **WrapStatsForecast**
 `from fold_wrappers import WrapStatsForecast` | | [NeuralForecast Logo] |
 NeuralForecast (beta) | [GitHub](https://github.com/Nixtla/neuralforecast) |
 â | **WrapNeuralForecast**
 `from fold_wrappers import WrapNeuralForecast` | | [XGBoost Logo] | XGBoost |
 [GitHub](https://github.com/dmlc/xgboost) | â | **WrapXGB**
 `from fold_wrappers import WrapXGB` | | [LightGBM Logo] | LightGBM | [GitHub]
@@ -35,35 +35,34 @@
 `from fold_wrappers import WrapStatsModels` | | [Prophet Logo] | Prophet |
 [GitHub](https://github.com/facebook/prophet) | â | **WrapProphet**
 `from fold_wrappers import WrapProphet` | | [Scikit-Learn Logo] | Sklearn
 (natively available in `fold`) | [GitHub](https://github.com/scikit-learn/
 scikit-learn) | ð¡
 (some) | Sklearn doesn't need to be wrapped,
 just pass in the models. | # Installation - Prerequisites: `python >= 3.7` and
-`pip` - Install from git directly: ``` pip install https://github.com/dream-
-faster/fold-wrappers/archive/main.zip ``` - Depending on what model you'd like
-to wrap, you can either install the library directly or run ``` pip install
-"git+https://github.com/dream-faster/fold-wrappers.git#egg=fold-wrappers[]" ```
-# Quickstart You can quickly train your chosen models and get predictions by
-running: ```python from fold import ExpandingWindowSplitter, train_evaluate
-from fold.utils.dataset import get_preprocessed_dataset from
-statsforecast.models import ARIMA from fold_wrappers import WrapStatsForecast
-X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
-target_col="temperature", shorten=1000 ) model = WrapStatsForecast
-( model_class=ARIMA, # Pass in the class init_args={"order": (1, 0, 0)}, # and
-the arguments to pass in at `init()` online_mode=False, # Enable online updates
-where available ) splitter = ExpandingWindowSplitter(initial_train_window=0.2,
-step=50) scorecard, predictions, trained_pipeline = train_evaluate(model, X, y,
-splitter) ``` You can also wrap a model that you have initiate first: ```python
-wrapped_model = WrapStatsForecast.from_model( ARIMA(order=(1, 0, 0)),
-online_mode=False # Enable online updates where available ) ``` ## Our Open-
-core Time Series Toolkit [![Krisi](https://raw.githubusercontent.com/dream-
-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)]
-(https://github.com/dream-faster/krisi) [![Fold](https://
-raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+`pip` - Install from pypi: ``` pip install fold-wrappers ``` - Depending on
+what model you'd like to wrap, you can either install the library directly or
+run ``` pip install "fold-wrappers[]" ``` # Quickstart You can quickly train
+your chosen models and get predictions by running: ```python from fold import
+ExpandingWindowSplitter, train_evaluate from fold.utils.dataset import
+get_preprocessed_dataset from statsforecast.models import ARIMA from
+fold_wrappers import WrapStatsForecast X, y = get_preprocessed_dataset
+( "weather/historical_hourly_la", target_col="temperature", shorten=1000 )
+model = WrapStatsForecast( model_class=ARIMA, # Pass in the class init_args=
+{"order": (1, 0, 0)}, # and the arguments to pass in at `init()`
+online_mode=False, # Enable online updates where available ) splitter =
+ExpandingWindowSplitter(initial_train_window=0.2, step=50) scorecard,
+predictions, trained_pipeline = train_evaluate(model, X, y, splitter) ``` You
+can also wrap a model that you have initiate first: ```python wrapped_model =
+WrapStatsForecast.from_model( ARIMA(order=(1, 0, 0)), online_mode=False #
+Enable online updates where available ) ``` ## Our Open-core Time Series
+Toolkit [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/
+docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://
+github.com/dream-faster/krisi) [![Fold](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
 Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
 overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
 dream-faster/fold-models) [![Fold/Wrapper](https://raw.githubusercontent.com/
 dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
 wrappers) If you want to try them out, we'd love to hear about your use case
```

### Comparing `fold_wrappers-0.0.2/pyproject.toml` & `fold_wrappers-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
  
 [project]
 name = "fold-wrappers"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -19,18 +19,18 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: Other/Proprietary License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy",
-  "fold-core~=0.0.4",
+  "fold-core~=0.1",
 ]
 description = "3rd party model wrappers for fold."
-keywords = []
+keywords = ["time-series", "machine-learning", "forecasting", "forecast", "nowcast", "models", "time-series-regression", "time-series-classification", "financial-machine-learning"]
 license = { file="LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold-wrappers"
 Issues = "https://github.com/dream-faster/fold-wrappers/issues"
@@ -41,15 +41,15 @@
   "black~=22.10.0",
   "flake8~=4.0.1",
   "isort~=5.10.1",
   "pre-commit~=2.20.0",
 ]
 tests = [
   "pytest~=7.1.2",
-  "fold-core~=0.0.4",
+  "fold-core~=0.1",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings-python",
   "mkdocs-include-markdown-plugin",
   "mkdocs-autorefs"
 ]
@@ -128,15 +128,15 @@
 pythonpath = [
   "src"
 ]
 testpaths = ["tests"]
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_wrappers-0.0.2/PKG-INFO` & `fold_wrappers-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-wrappers
-Version: 0.0.2
+Version: 0.1.0
 Summary: 3rd party model wrappers for fold.
 Project-URL: Documentation, https://dream-faster.github.io/fold-wrappers
 Project-URL: Issues, https://github.com/dream-faster/fold-wrappers/issues
 Project-URL: Source, https://github.com/dream-faster/fold-wrappers
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -24,26 +24,27 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
+Keywords: financial-machine-learning,forecast,forecasting,machine-learning,models,nowcast,time-series,time-series-classification,time-series-regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: fold-core~=0.0.4
+Requires-Dist: fold-core~=0.1
 Requires-Dist: numpy
 Provides-Extra: docs
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: lightgbm
@@ -62,15 +63,15 @@
 Requires-Dist: pmdarima>=2.0.0; extra == 'sktime'
 Requires-Dist: sktime>=0.16.0; extra == 'sktime'
 Provides-Extra: statsforecast
 Requires-Dist: statsforecast>=1.5; extra == 'statsforecast'
 Provides-Extra: statsmodels
 Requires-Dist: statsmodels>=0.12.0; extra == 'statsmodels'
 Provides-Extra: tests
-Requires-Dist: fold-core~=0.0.4; extra == 'tests'
+Requires-Dist: fold-core~=0.1; extra == 'tests'
 Requires-Dist: pytest~=7.1.2; extra == 'tests'
 Provides-Extra: xgboost
 Requires-Dist: xgboost; extra == 'xgboost'
 Description-Content-Type: text/markdown
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml"><img alt="Statsforecast Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml/badge.svg"/></a>
@@ -97,36 +98,36 @@
     <a href="https://dream-faster.github.io/fold-wrappers/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 # Available models
 
-|                                                                                                                                                                                                                                             | Name                                   |                          Link                          | Supports<br />Online <br />updating | Wrapper Name<br />& Import Location                                            |
-| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:| :------------------------------------- | :----------------------------------------------------: | :---------------------------------: | ------------------------------------------------------------------------------ |
-| <img alt='StatsDorecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                                                                      | StatsForecast                          |   [GitHub](https://github.com/Nixtla/statsforecast)    |                 ❌                  | **WrapStatsForecast**<br />`from fold_wrappers import WrapStatsForecast` |
-| <img alt='NeuralForecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                                                                      | NeuralForecast (beta)                          |   [GitHub](https://github.com/Nixtla/neuralforecast)    |                 ❌                  | **WrapNeuralForecast**<br />`from fold_wrappers import WrapNeuralForecast` |
-| <img alt='XGBoost Logo' src='https://camo.githubusercontent.com/0ea6e7814dd771f740509bbb668d251d485a6e21f12e287be7cc2275e0eab1d1/68747470733a2f2f7867626f6f73742e61692f696d616765732f6c6f676f2f7867626f6f73742d6c6f676f2e737667' height=64> | XGBoost                                |       [GitHub](https://github.com/dmlc/xgboost)        |                 ✅                    | **WrapXGB**<br />`from fold_wrappers import WrapXGB`               |
-| <img alt='LightGBM Logo' src='https://lightgbm.readthedocs.io/en/latest/_images/LightGBM_logo_black_text.svg' height=64> | LightGBM                                |       [GitHub](https://github.com/Microsoft/LightGBM)        |                 ✅                    | **WrapLGBM**<br />`from fold_wrappers import WrapLGBM`               |
-| <img alt='Sktime Logo' src='https://github.com/sktime/sktime/raw/main/docs/source/images/sktime-logo.jpg?raw=true' height=64>                                                                                                               | SKTime (beta)                                 |       [GitHub](https://github.com/sktime/sktime)       |                 ✅                  | **WrapSktime**<br />`from fold_wrappers import WrapSktime`                |
-| <img alt='Statsmodels Logo' src='https://github.com/statsmodels/statsmodels/raw/main/docs/source/images/statsmodels-logo-v2-horizontal.svg' width=160>                                                                                      | Statsmodels                            |  [GitHub](https://github.com/statsmodels/statsmodels)  |                 ✅                  | **WrapStatsModels**<br />`from fold_wrappers import WrapStatsModels` |
-| <img alt='Prophet Logo' src='https://miro.medium.com/v2/resize:fit:964/0*tVCene42rgUTNv9Q.png' width=160>                                                                                                                                   | Prophet                                |     [GitHub](https://github.com/facebook/prophet)      |                 ✅                  | **WrapProphet**<br />`from fold_wrappers import WrapProphet`             |
-| <img alt='Scikit-Learn Logo' src='https://raw.githubusercontent.com/scikit-learn/scikit-learn/main/doc/logos/scikit-learn-logo.png' width=160>                                                                                              | Sklearn <br/>(natively available in `fold`) | [GitHub](https://github.com/scikit-learn/scikit-learn) |             🟡<br/>(some)              | Sklearn doesn't need to be wrapped,<br />just pass in the models.              |
+|                                                                                                                                                                                                                                             | Name                                        |                          Link                          | Supports<br />Online <br />updating | Wrapper Name<br />& Import Location                                        |
+|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------|:------------------------------------------------------:|:-----------------------------------:|----------------------------------------------------------------------------|
+|                                                   <img alt='StatsDorecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                    | StatsForecast                               |   [GitHub](https://github.com/Nixtla/statsforecast)    |                  ❌                  | **WrapStatsForecast**<br />`from fold_wrappers import WrapStatsForecast`   |
+|                                                   <img alt='NeuralForecast Logo' src='https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png' height=64>                                                   | NeuralForecast (beta)                       |   [GitHub](https://github.com/Nixtla/neuralforecast)   |                  ❌                  | **WrapNeuralForecast**<br />`from fold_wrappers import WrapNeuralForecast` |
+| <img alt='XGBoost Logo' src='https://camo.githubusercontent.com/0ea6e7814dd771f740509bbb668d251d485a6e21f12e287be7cc2275e0eab1d1/68747470733a2f2f7867626f6f73742e61692f696d616765732f6c6f676f2f7867626f6f73742d6c6f676f2e737667' height=64> | XGBoost                                     |       [GitHub](https://github.com/dmlc/xgboost)        |                  ✅                  | **WrapXGB**<br />`from fold_wrappers import WrapXGB`                       |
+|                                                          <img alt='LightGBM Logo' src='https://lightgbm.readthedocs.io/en/latest/_images/LightGBM_logo_black_text.svg' height=64>                                                           | LightGBM                                    |    [GitHub](https://github.com/Microsoft/LightGBM)     |                  ✅                  | **WrapLGBM**<br />`from fold_wrappers import WrapLGBM`                     |
+|                                                        <img alt='Sktime Logo' src='https://github.com/sktime/sktime/raw/main/docs/source/images/sktime-logo.jpg?raw=true' height=64>                                                        | SKTime (beta)                               |       [GitHub](https://github.com/sktime/sktime)       |                  ✅                  | **WrapSktime**<br />`from fold_wrappers import WrapSktime`                 |
+|                                           <img alt='Statsmodels Logo' src='https://github.com/statsmodels/statsmodels/raw/main/docs/source/images/statsmodels-logo-v2-horizontal.svg' width=160>                                            | Statsmodels                                 |  [GitHub](https://github.com/statsmodels/statsmodels)  |                  ✅                  | **WrapStatsModels**<br />`from fold_wrappers import WrapStatsModels`       |
+|                                                                  <img alt='Prophet Logo' src='https://miro.medium.com/v2/resize:fit:964/0*tVCene42rgUTNv9Q.png' width=160>                                                                  | Prophet                                     |     [GitHub](https://github.com/facebook/prophet)      |                  ✅                  | **WrapProphet**<br />`from fold_wrappers import WrapProphet`               |
+|                                               <img alt='Scikit-Learn Logo' src='https://raw.githubusercontent.com/scikit-learn/scikit-learn/main/doc/logos/scikit-learn-logo.png' width=160>                                                | Sklearn <br/>(natively available in `fold`) | [GitHub](https://github.com/scikit-learn/scikit-learn) |            🟡<br/>(some)            | Sklearn doesn't need to be wrapped,<br />just pass in the models.          |
 
 # Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold-wrappers/archive/main.zip
+  pip install fold-wrappers
   ```
 - Depending on what model you'd like to wrap, you can either install the library directly or run
    ```
-  pip install "git+https://github.com/dream-faster/fold-wrappers.git#egg=fold-wrappers[<your_library_name>]"
+  pip install "fold-wrappers[<your_library_name>]"
   ```
 
 # Quickstart
```

