# Comparing `tmp/fold_core-0.0.6.tar.gz` & `tmp/fold_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.0.6.tar", max compression
+gzip compressed data, was "fold_core-0.1.0.tar", max compression
```

## Comparing `fold_core-0.0.6.tar` & `fold_core-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3870 2023-04-19 12:58:38.109536 fold_core-0.0.6/LICENSE
--rw-r--r--   0        0        0    10163 2023-04-19 12:58:38.109536 fold_core-0.0.6/README.md
--rw-r--r--   0        0        0     3601 2023-04-19 12:58:38.141536 fold_core-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      298 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/__init__.py
--rw-r--r--   0        0        0     5097 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/base.py
--rw-r--r--   0        0        0      353 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10085 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1401 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/common.py
--rw-r--r--   0        0        0     6096 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2050 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6183 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4584 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3085 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/sample.py
--rw-r--r--   0        0        0     1888 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/select.py
--rw-r--r--   0        0        0     4369 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/composites/target.py
--rw-r--r--   0        0        0      169 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2232 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1755 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3022 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      414 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9746 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/common.py
--rw-r--r--   0        0        0     1933 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     6962 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2817 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5559 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/training.py
--rw-r--r--   0        0        0     1669 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/loop/types.py
--rw-r--r--   0        0        0      205 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3036 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/base.py
--rw-r--r--   0        0        0     1751 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4173 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2011 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/random.py
--rw-r--r--   0        0        0     4134 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/py.typed
--rw-r--r--   0        0        0     6548 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/splitters.py
--rw-r--r--   0        0        0      752 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     5858 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8417 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4088 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2730 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      622 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6393 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5499 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7397 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3558 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      711 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4238 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/transformations/window.py
--rw-r--r--   0        0        0     1995 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2064 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1415 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/list.py
--rw-r--r--   0        0        0     2779 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1540 2023-04-19 12:58:38.141536 fold_core-0.0.6/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12781 1970-01-01 00:00:00.000000 fold_core-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-19 14:22:30.042023 fold_core-0.1.0/LICENSE
+-rw-r--r--   0        0        0    10111 2023-04-19 14:22:30.042023 fold_core-0.1.0/README.md
+-rw-r--r--   0        0        0     3768 2023-04-19 14:22:30.074022 fold_core-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/__init__.py
+-rw-r--r--   0        0        0     5273 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/base.py
+-rw-r--r--   0        0        0      529 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6359 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4760 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2064 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4545 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1931 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      590 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9922 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/common.py
+-rw-r--r--   0        0        0     2109 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     7138 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2993 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     5735 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/types.py
+-rw-r--r--   0        0        0      381 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3212 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/base.py
+-rw-r--r--   0        0        0     1927 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/random.py
+-rw-r--r--   0        0        0     4310 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/splitters.py
+-rw-r--r--   0        0        0      928 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4264 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2906 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5675 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7573 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3734 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2171 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     2240 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2955 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12881 1970-01-01 00:00:00.000000 fold_core-0.1.0/PKG-INFO
```

### Comparing `fold_core-0.0.6/LICENSE` & `fold_core-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.0.6/README.md` & `fold_core-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- # Fold -->
+<!-- # fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://dream-faster.github.io/fold/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/fold/docs.yaml?logo=readthedocs"></a>
   <a style="margin:2px" href="https://codecov.io/gh/dream-faster/fold" ><img src="https://codecov.io/gh/dream-faster/fold/branch/main/graph/badge.svg?token=Z7I2XSF188"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/fold/actions/workflows/tests.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
   <a style="margin:2px" href="https://calendly.com/nowcasting/consultation"><img alt="Book a call with us!" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
@@ -35,17 +35,17 @@
 
 <!-- GETTING STARTED -->
 
 ## Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold/archive/main.zip
+  pip install fold-core
   ```
 
 ## Quickstart
 
 You can quickly train your chosen models and get predictions by running:
 
 ```py
```

#### html2text {}

```diff
@@ -14,22 +14,21 @@
 main/docs/images/overview_diagrams/main_features.svg) - Composite Models with
 Continuous Validation - [What does that mean?](https://dream-faster.github.io/
 fold/concepts/continuous-validation/) - Distributed computing - [Why is this
 important?](#Fold-is-different) - Update deployed models (coming in May) - [Why
 is this important?](#Fold-is-different) ![Fold works with many third party
 libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/
 images/overview_diagrams/third_party.svg)  ## Installation - Prerequisites:
-`python >= 3.7` and `pip` - Install from git directly: ``` pip install https://
-github.com/dream-faster/fold/archive/main.zip ``` ## Quickstart You can quickly
-train your chosen models and get predictions by running: ```py from
-sklearn.ensemble import RandomForestRegressor from statsforecast.models import
-ARIMA from fold import ExpandingWindowSplitter, train_evaluate from
-fold.composites import Ensemble from fold.transformations import
-OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset X, y =
-get_preprocessed_dataset( "weather/historical_hourly_la",
+`python >= 3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ##
+Quickstart You can quickly train your chosen models and get predictions by
+running: ```py from sklearn.ensemble import RandomForestRegressor from
+statsforecast.models import ARIMA from fold import ExpandingWindowSplitter,
+train_evaluate from fold.composites import Ensemble from fold.transformations
+import OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset
+X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
 target_col="temperature", shorten=1000 ) pipeline = [ Ensemble(
 [ RandomForestRegressor(), ARIMA(order=(1, 1, 0)), ] ), OnlyPredictions(), ]
 splitter = ExpandingWindowSplitter(initial_train_window=0.2, step=0.2)
 scorecard, prediction, trained_pipelines = train_evaluate(pipeline, X, y,
 splitter) ``` Thinking of using `fold`? We'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! (If you install `krisi` by running `pip install
```

### Comparing `fold_core-0.0.6/pyproject.toml` & `fold_core-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.0.6"
+version = "0.1.0"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: Other/Proprietary License",
   "Operating System :: OS Independent",
 ]
 description = "A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour."
-keywords = []
+keywords = ["time-series", "machine-learning", "forecasting", "forecast", "nowcast", "models", "time-series-regression", "time-series-classification", "financial-machine-learning"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 pandas = ">=1.2"
 numpy = ">=1.16"
@@ -123,15 +123,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.0.6"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.0.6/src/fold/base.py` & `fold_core-0.1.0/src/fold/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 import enum
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Callable, List, Optional, Tuple, TypeVar, Union
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/columns.py` & `fold_core-0.1.0/src/fold/composites/columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Callable, List, Optional, Tuple
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/common.py` & `fold_core-0.1.0/src/fold/composites/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import List
 
 from ..base import Composite, Pipelines, Transformations
 from ..utils.list import flatten, wrap_in_list
 
 
 def get_flat_list_of_transformations(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/concat.py` & `fold_core-0.1.0/src/fold/composites/concat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Callable, List, Optional, Union
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/ensemble.py` & `fold_core-0.1.0/src/fold/composites/ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
 import pandas as pd
 
 from ..base import Composite, Pipelines
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/metalabeling.py` & `fold_core-0.1.0/src/fold/composites/metalabeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
 from fold.composites.common import get_concatenated_names
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/residual.py` & `fold_core-0.1.0/src/fold/composites/residual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple
 
 import pandas as pd
 
 from fold.composites.common import get_concatenated_names
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/sample.py` & `fold_core-0.1.0/src/fold/composites/sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Any, Callable, List, Optional, Tuple
 
 import pandas as pd
 
 from fold.composites.common import get_concatenated_names
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/select.py` & `fold_core-0.1.0/src/fold/composites/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
 import pandas as pd
 
 from ..base import Composite, Pipelines, Transformations
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/composites/target.py` & `fold_core-0.1.0/src/fold/composites/target.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
 from ..base import Composite, InvertibleTransformation, Pipelines, T
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/backend/ray.py` & `fold_core-0.1.0/src/fold/loop/backend/ray.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Callable, List, Optional
 
 import pandas as pd
 import ray
 
 from ...base import Composite, Transformations
 from ...splitters import Fold
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/backend/sequential.py` & `fold_core-0.1.0/src/fold/loop/backend/sequential.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Callable, List, Optional
 
 import pandas as pd
 from tqdm.auto import tqdm
 
 from ...base import Composite, Transformations
 from ...splitters import Fold
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/backtesting.py` & `fold_core-0.1.0/src/fold/loop/backtesting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Optional, Union
 
 import pandas as pd
 from tqdm.auto import tqdm
 
 from ..base import OutOfSamplePredictions, TrainedPipelines
 from ..splitters import Fold, Splitter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/common.py` & `fold_core-0.1.0/src/fold/loop/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import List, Optional
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/convenience.py` & `fold_core-0.1.0/src/fold/loop/convenience.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from importlib.util import find_spec
 from typing import Callable, List
 
 from sklearn.base import ClassifierMixin, RegressorMixin, TransformerMixin
 from sklearn.feature_selection import SelectorMixin
 from sklearn.pipeline import Pipeline as SKLearnPipeline
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/encase.py` & `fold_core-0.1.0/src/fold/loop/encase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 import importlib.util
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Union
 
 import pandas as pd
 from sklearn.metrics import mean_squared_error
 
 from ..base import OutOfSamplePredictions, Pipeline, TrainedPipelines
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/memory.py` & `fold_core-0.1.0/src/fold/loop/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Optional, Tuple
 
 import pandas as pd
 
 from ..base import Transformation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/loop/training.py` & `fold_core-0.1.0/src/fold/loop/training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
 from ..base import Composite, Pipeline, TrainedPipelines, Transformation
 from ..splitters import Fold, SlidingWindowSplitter, Splitter
 from ..utils.list import wrap_in_list
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/models/base.py` & `fold_core-0.1.0/src/fold/models/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from abc import abstractmethod
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from ..base import Transformation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/models/baseline.py` & `fold_core-0.1.0/src/fold/models/baseline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import Union
 
 import pandas as pd
 
 from ..base import fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/models/dummy.py` & `fold_core-0.1.0/src/fold/models/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import List, Union
 
 import pandas as pd
 
 from ..base import Transformation, fit_noop
 from .base import Model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/models/sklearn.py` & `fold_core-0.1.0/src/fold/models/sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Optional, Union
 
 import pandas as pd
 
 from ..base import Transformation, fit_noop
 from .base import Model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/splitters.py` & `fold_core-0.1.0/src/fold/splitters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
 
 @dataclass
 class Fold:
     order: int
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/__init__.py` & `fold_core-0.1.0/src/fold/transformations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from ..base import Transformation
 from ..composites.concat import TransformColumn
 from .columns import (
     DropColumns,
     OnlyPredictions,
     OnlyProbabilities,
     RenameColumns,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/columns.py` & `fold_core-0.1.0/src/fold/transformations/columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from typing import List, Union
 
 import pandas as pd
 
 from ..base import Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/date.py` & `fold_core-0.1.0/src/fold/transformations/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Callable, List, Union
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/dev.py` & `fold_core-0.1.0/src/fold/transformations/dev.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from inspect import getfullargspec
 from typing import Callable, Optional
 
 import pandas as pd
 
 from ..base import InvertibleTransformation, Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/difference.py` & `fold_core-0.1.0/src/fold/transformations/difference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Optional
 
 import pandas as pd
 
 from ..base import InvertibleTransformation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/function.py` & `fold_core-0.1.0/src/fold/transformations/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Callable, Optional
 
 import pandas as pd
 
 from ..base import Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/holidays.py` & `fold_core-0.1.0/src/fold/transformations/holidays.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from datetime import date
 from enum import Enum
 from typing import List, Union
 
 import pandas as pd
 
 from ..base import Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/lags.py` & `fold_core-0.1.0/src/fold/transformations/lags.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import List, Tuple, Union
 
 import pandas as pd
 
 from fold.utils.checks import is_X_available
 
 from ..base import Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/math.py` & `fold_core-0.1.0/src/fold/transformations/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from fold.base import InvertibleTransformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/sklearn.py` & `fold_core-0.1.0/src/fold/transformations/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from inspect import getfullargspec
 from typing import Optional
 
 import pandas as pd
 
 from ..base import FeatureSelector, Transformation, fit_noop
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/transformations/window.py` & `fold_core-0.1.0/src/fold/transformations/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Callable, List, Tuple, Union
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/utils/checks.py` & `fold_core-0.1.0/src/fold/utils/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import List
 
 import pandas as pd
 
 
 def is_prediction(input: pd.DataFrame) -> bool:
     if len(input.columns) == 1:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/utils/dataset.py` & `fold_core-0.1.0/src/fold/utils/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Optional, Tuple, Union
 
 import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/utils/list.py` & `fold_core-0.1.0/src/fold/utils/list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 import collections
 from collections.abc import Iterable
 from typing import List, Tuple, TypeVar, Union
 
 from iteration_utilities import unique_everseen
 
 T = TypeVar("T")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/utils/tests.py` & `fold_core-0.1.0/src/fold/utils/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from random import choices
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 
 from fold.base import Transformation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/src/fold/utils/trim.py` & `fold_core-0.1.0/src/fold/utils/trim.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
+
+
 from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 
 def trim_initial_nans(X: pd.DataFrame, y: pd.Series) -> Tuple[pd.DataFrame, pd.Series]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fold_core-0.0.6/PKG-INFO` & `fold_core-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.0.6
+Version: 0.1.0
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
+Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +49,15 @@
 Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests"
 Requires-Dist: pytest-cov (>=4.0) ; extra == "tests"
 Requires-Dist: ray (>=1.4.0) ; extra == "ray" or extra == "extras"
 Requires-Dist: scikit-learn (>=0.22)
 Requires-Dist: tqdm (>=4.0)
 Description-Content-Type: text/markdown
 
-<!-- # Fold -->
+<!-- # fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://dream-faster.github.io/fold/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/fold/docs.yaml?logo=readthedocs"></a>
   <a style="margin:2px" href="https://codecov.io/gh/dream-faster/fold" ><img src="https://codecov.io/gh/dream-faster/fold/branch/main/graph/badge.svg?token=Z7I2XSF188"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/fold/actions/workflows/tests.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
   <a style="margin:2px" href="https://calendly.com/nowcasting/consultation"><img alt="Book a call with us!" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
@@ -89,17 +90,17 @@
 
 <!-- GETTING STARTED -->
 
 ## Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold/archive/main.zip
+  pip install fold-core
   ```
 
 ## Quickstart
 
 You can quickly train your chosen models and get predictions by running:
 
 ```py
```

#### html2text {}

```diff
@@ -1,42 +1,44 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.0.6 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.0 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
-rigour. License: Proprietary Author: Mark Aron Szulyovszky Requires-Python:
->=3.7 Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: Other/Proprietary License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Provides-
-Extra: docs Provides-Extra: extras Provides-Extra: quality Provides-Extra: ray
-Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ; extra ==
-"quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality" Requires-
-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras" Requires-Dist:
-image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-learn (>=0.7.0) ;
-extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
-Requires-Dist: iteration_utilities (>=0.11) Requires-Dist: krisi
-(>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs-autorefs (>=0.4.0) ;
-extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra == "docs"
-Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs" Requires-Dist:
-mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist: mkdocs-
-jupyter (>=0.24.0) ; extra == "docs" Requires-Dist: mkdocs-material (>=9.0.0) ;
-extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
-Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2) Requires-Dist: pre-
-commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-Dist: pytest
-(>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov (>=4.0) ; extra
-== "tests" Requires-Dist: ray (>=1.4.0) ; extra == "ray" or extra == "extras"
-Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm (>=4.0) Description-
-Content-Type: text/markdown
+rigour. License: Proprietary Keywords: time-series,machine-
+learning,forecasting,forecast,nowcast,models,time-series-regression,time-
+series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
+Requires-Python: >=3.7 Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: Other/Proprietary License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Provides-Extra: docs Provides-Extra: extras Provides-Extra: quality Provides-
+Extra: ray Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ;
+extra == "quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
+Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
+Requires-Dist: image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-
+learn (>=0.7.0) ; extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ;
+extra == "quality" Requires-Dist: iteration_utilities (>=0.11) Requires-Dist:
+krisi (>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs-autorefs
+(>=0.4.0) ; extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra ==
+"docs" Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs" Requires-
+Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist:
+mkdocs-jupyter (>=0.24.0) ; extra == "docs" Requires-Dist: mkdocs-material
+(>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ;
+extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2)
+Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-
+Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov
+(>=4.0) ; extra == "tests" Requires-Dist: ray (>=1.4.0) ; extra == "ray" or
+extra == "extras" Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm
+(>=4.0) Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                  (/fold/) ****
   A Time_Series_Continuous_Validation library that lets you build, deploy and
@@ -49,22 +51,21 @@
 main/docs/images/overview_diagrams/main_features.svg) - Composite Models with
 Continuous Validation - [What does that mean?](https://dream-faster.github.io/
 fold/concepts/continuous-validation/) - Distributed computing - [Why is this
 important?](#Fold-is-different) - Update deployed models (coming in May) - [Why
 is this important?](#Fold-is-different) ![Fold works with many third party
 libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/
 images/overview_diagrams/third_party.svg)  ## Installation - Prerequisites:
-`python >= 3.7` and `pip` - Install from git directly: ``` pip install https://
-github.com/dream-faster/fold/archive/main.zip ``` ## Quickstart You can quickly
-train your chosen models and get predictions by running: ```py from
-sklearn.ensemble import RandomForestRegressor from statsforecast.models import
-ARIMA from fold import ExpandingWindowSplitter, train_evaluate from
-fold.composites import Ensemble from fold.transformations import
-OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset X, y =
-get_preprocessed_dataset( "weather/historical_hourly_la",
+`python >= 3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ##
+Quickstart You can quickly train your chosen models and get predictions by
+running: ```py from sklearn.ensemble import RandomForestRegressor from
+statsforecast.models import ARIMA from fold import ExpandingWindowSplitter,
+train_evaluate from fold.composites import Ensemble from fold.transformations
+import OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset
+X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
 target_col="temperature", shorten=1000 ) pipeline = [ Ensemble(
 [ RandomForestRegressor(), ARIMA(order=(1, 1, 0)), ] ), OnlyPredictions(), ]
 splitter = ExpandingWindowSplitter(initial_train_window=0.2, step=0.2)
 scorecard, prediction, trained_pipelines = train_evaluate(pipeline, X, y,
 splitter) ``` Thinking of using `fold`? We'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! (If you install `krisi` by running `pip install
```

