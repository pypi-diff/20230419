# Comparing `tmp/fold_models-0.0.2.tar.gz` & `tmp/fold_models-0.1.0.tar.gz`

## Comparing `fold_models-0.0.2.tar` & `fold_models-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_models-0.0.2/.flake8
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_models-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fold_models-0.0.2/fold_models/__init__.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 fold_models-0.0.2/fold_models/ar.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 fold_models-0.0.2/fold_models/baseline.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_models-0.0.2/.gitignore
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 fold_models-0.0.2/LICENSE
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 fold_models-0.0.2/README.md
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 fold_models-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 fold_models-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_models-0.1.0/.flake8
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_models-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fold_models-0.1.0/fold_models/__init__.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 fold_models-0.1.0/fold_models/ar.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 fold_models-0.1.0/fold_models/baseline.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_models-0.1.0/.gitignore
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 fold_models-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 fold_models-0.1.0/README.md
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 fold_models-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 fold_models-0.1.0/PKG-INFO
```

### Comparing `fold_models-0.0.2/.vscode/settings.json` & `fold_models-0.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `fold_models-0.0.2/fold_models/ar.py` & `fold_models-0.1.0/fold_models/ar.py`

 * *Files identical despite different names*

### Comparing `fold_models-0.0.2/fold_models/baseline.py` & `fold_models-0.1.0/fold_models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_models-0.0.2/.gitignore` & `fold_models-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fold_models-0.0.2/LICENSE` & `fold_models-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_models-0.0.2/README.md` & `fold_models-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 NaiveSeasonal | `from fold_models import NaiveSeasonal`
 MovingAverage | `from fold_models import MovingAverage`
 
 # Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold-models/archive/main.zip
+  pip install fold-models
   ```
 - Depending on what model you'd like to wrap, you can either install the library directly or run
    ```
-  pip install "git+https://github.com/dream-faster/fold-models.git#egg=fold-models[<your_library_name>]"
+  pip install "fold-models[<your_library_name>]"
   ```
 
 # Quickstart
```

#### html2text {}

```diff
@@ -8,22 +8,21 @@
 
                               Explore_the_docs_Â»
 
 # Available models Name | Usage --------------|--------------------------------
 -------- Naive | `from fold_models import Naive` NaiveSeasonal | `from
 fold_models import NaiveSeasonal` MovingAverage | `from fold_models import
 MovingAverage` # Installation - Prerequisites: `python >= 3.7` and `pip` -
-Install from git directly: ``` pip install https://github.com/dream-faster/
-fold-models/archive/main.zip ``` - Depending on what model you'd like to wrap,
-you can either install the library directly or run ``` pip install "git+https:/
-/github.com/dream-faster/fold-models.git#egg=fold-models[]" ``` # Quickstart
-You can quickly train your chosen models and get predictions by running:
-```python from fold import ExpandingWindowSplitter, train_evaluate from
-fold.utils.dataset import get_preprocessed_dataset from fold_models import
-Naive X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
+Install from pypi: ``` pip install fold-models ``` - Depending on what model
+you'd like to wrap, you can either install the library directly or run ``` pip
+install "fold-models[]" ``` # Quickstart You can quickly train your chosen
+models and get predictions by running: ```python from fold import
+ExpandingWindowSplitter, train_evaluate from fold.utils.dataset import
+get_preprocessed_dataset from fold_models import Naive X, y =
+get_preprocessed_dataset( "weather/historical_hourly_la",
 target_col="temperature", shorten=1000 ) model = Naive() splitter =
 ExpandingWindowSplitter(initial_train_window=0.2, step=50) scorecard,
 predictions, trained_pipeline = train_evaluate(model, X, y, splitter) ``` ##
 Our Open-core Time Series Toolkit [![Krisi](https://raw.githubusercontent.com/
 dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi) [![Fold]
 (https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
```

### Comparing `fold_models-0.0.2/pyproject.toml` & `fold_models-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "fold-models" 
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -19,19 +19,19 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: Other/Proprietary License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy",
-  "fold-core~=0.0.6",
+  "fold-core~=0.1",
   "scikit-learn",
 ]
 description = "Models for fold."
-keywords = []
+keywords = ["time-series", "machine-learning", "forecasting", "forecast", "nowcast", "models", "time-series-regression", "time-series-classification", "financial-machine-learning"]
 license = { file="LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold-models"
 Issues = "https://github.com/dream-faster/fold-models/issues"
@@ -42,15 +42,15 @@
   "black~=22.10.0",
   "flake8~=4.0.1",
   "isort~=5.10.1",
   "pre-commit~=2.20.0",
 ]
 tests = [
   "pytest~=7.1.2",
-  "fold-core~=0.0.6",
+  "fold-core~=0.1",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings-python",
   "mkdocs-include-markdown-plugin",
   "mkdocs-autorefs"
 ]
@@ -106,15 +106,15 @@
 testpaths = ["tests"]
 
 [tool.hatch.build]
 sources = ["src"]
 
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

### Comparing `fold_models-0.0.2/PKG-INFO` & `fold_models-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-models
-Version: 0.0.2
+Version: 0.1.0
 Summary: Models for fold.
 Project-URL: Documentation, https://dream-faster.github.io/fold-models
 Project-URL: Issues, https://github.com/dream-faster/fold-models/issues
 Project-URL: Source, https://github.com/dream-faster/fold-models
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License:                             LICENSE
         
@@ -82,40 +82,41 @@
         GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
         USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
         DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
         PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
         EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
         SUCH DAMAGES.
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
-Requires-Dist: fold-core~=0.0.6
+Requires-Dist: fold-core~=0.1
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Provides-Extra: docs
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: flake8~=4.0.1; extra == 'quality'
 Requires-Dist: isort~=5.10.1; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Provides-Extra: tests
-Requires-Dist: fold-core~=0.0.6; extra == 'tests'
+Requires-Dist: fold-core~=0.1; extra == 'tests'
 Requires-Dist: pytest~=7.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://github.com/dream-faster/fold-models/actions/workflows/test-baselines.yaml"><img alt="Baselines Tests" src="https://github.com/dream-faster/fold-models/actions/workflows/test-baselines.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
   <a style="margin:2px" href="https://calendly.com/nowcasting/consultation"><img alt="Calendly Booking" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
@@ -146,21 +147,21 @@
 NaiveSeasonal | `from fold_models import NaiveSeasonal`
 MovingAverage | `from fold_models import MovingAverage`
 
 # Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
-- Install from git directly:
+- Install from pypi:
   ```
-  pip install https://github.com/dream-faster/fold-models/archive/main.zip
+  pip install fold-models
   ```
 - Depending on what model you'd like to wrap, you can either install the library directly or run
    ```
-  pip install "git+https://github.com/dream-faster/fold-models.git#egg=fold-models[<your_library_name>]"
+  pip install "fold-models[<your_library_name>]"
   ```
 
 # Quickstart
```

