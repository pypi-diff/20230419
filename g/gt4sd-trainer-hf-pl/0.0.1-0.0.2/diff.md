# Comparing `tmp/gt4sd-trainer-hf-pl-0.0.1.tar.gz` & `tmp/gt4sd-trainer-hf-pl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt4sd-trainer-hf-pl-0.0.1.tar", last modified: Tue Feb 14 16:32:21 2023, max compression
+gzip compressed data, was "gt4sd-trainer-hf-pl-0.0.2.tar", last modified: Wed Apr 19 15:34:57 2023, max compression
```

## Comparing `gt4sd-trainer-hf-pl-0.0.1.tar` & `gt4sd-trainer-hf-pl-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.113350 gt4sd-trainer-hf-pl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-02-14 16:32:21.113350 gt4sd-trainer-hf-pl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-02-14 16:32:21.113350 gt4sd-trainer-hf-pl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.105350 gt4sd-trainer-hf-pl-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.105350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.105350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.109350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/cli_pl_to_hf_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/cli_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.109350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/datasets/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.109350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/pytorch_lightning_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.109350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/lm_example.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-02-14 16:32:06.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/test_lm_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 16:32:21.109350 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-14 16:32:21.000000 gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-19 15:34:57.809082 gt4sd-trainer-hf-pl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.801082 gt4sd-trainer-hf-pl-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.801082 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/cli_pl_to_hf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/cli_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/datasets/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/pytorch_lightning_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/lm_example.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-19 15:34:48.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/test_lm_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:34:57.805081 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 15:34:57.000000 gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/top_level.txt
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/LICENSE` & `gt4sd-trainer-hf-pl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/PKG-INFO` & `gt4sd-trainer-hf-pl-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd-trainer-hf-pl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Transformers trainer submodule of GT4SD.
 Author: GT4SD team
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/README.md` & `gt4sd-trainer-hf-pl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/setup.cfg` & `gt4sd-trainer-hf-pl-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gt4sd-trainer-hf-pl
-version = attr: gt4sd.trainer.hf_pl.__version__
+version = attr: gt4sd_trainer.hf_pl.__version__
 description = Transformers trainer submodule of GT4SD.
 author = GT4SD team
 long_description_content_type = text/markdown
 long_description = file: README.md
 python_requires = >= 3.7.*
 classifiers = 
 	Operating System :: OS Independent
@@ -39,19 +39,19 @@
 package_dir = 
 	= src
 packages = find_namespace:
 include_package_data = False  # would break package_data
 
 [options.entry_points]
 console_scripts = 
-	gt4sd-trainer-hf-pl = gt4sd.trainer.hf_pl.cli_trainer:main
-	gt4sd-pl-to-hf = gt4sd.trainer.hf_pl.cli_pl_to_hf_converter:main
+	gt4sd-trainer-hf-pl = gt4sd_trainer.hf_pl.cli_trainer:main
+	gt4sd-pl-to-hf = gt4sd_trainer.hf_pl.cli_pl_to_hf_converter:main
 
 [options.package_data]
-gt4sd.trainer.hf_pl = 
+gt4sd_trainer.hf_pl = 
 	py.typed
 	tests/*.jsonl
 
 [options.packages.find]
 where = src
 
 [flake8]
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/__init__.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/argument_parser.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/cli_pl_to_hf_converter.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/cli_pl_to_hf_converter.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/cli_trainer.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/cli_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         Returns:
             parsed arguments in a tuple of dataclasses.
         """
         number_of_dataclass_types = len(self.dataclass_types)  # type:ignore
         self.dataclass_types = [
             dataclass_type
             for dataclass_type in self.dataclass_types  # type:ignore
-            if "gt4sd.trainer.hf_pl.TrainerArguments" not in str(dataclass_type)
+            if "gt4sd_trainer.hf_pl.TrainerArguments" not in str(dataclass_type)
         ]
         try:
             parsed_arguments = super().parse_json_file(  # type:ignore
                 json_file=json_file, allow_extra_keys=True
             )
         except Exception:
             logger.exception(
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/core.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/datasets/__init__.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/datasets/core.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/datasets/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/models/__init__.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/models/core.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/models/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/pytorch_lightning_trainer.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/pytorch_lightning_trainer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/__init__.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/lm_example.jsonl` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/lm_example.jsonl`

 * *Files identical despite different names*

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd/trainer/hf_pl/tests/test_lm_trainer.py` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer/hf_pl/tests/test_lm_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 #
 """Language modeling trainer unit tests."""
 
 import sentencepiece as _sentencepiece
 import importlib_resources
 from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint
 
-from gt4sd.trainer.hf_pl.core import LanguageModelingTrainingPipeline  # type: ignore
-from gt4sd.trainer.hf_pl.datasets.core import (  # type: ignore
+from gt4sd_trainer.hf_pl.core import LanguageModelingTrainingPipeline  # type: ignore
+from gt4sd_trainer.hf_pl.datasets.core import (  # type: ignore
     CGMDataModule,
     CLMDataModule,
     MLMDataModule,
     PLMDataModule,
 )
-from gt4sd.trainer.hf_pl.models.core import (  # type: ignore
+from gt4sd_trainer.hf_pl.models.core import (  # type: ignore
     CGMModule,
     CLMModule,
     MLMModule,
     PLMModule,
 )
 
 # sentencepiece has to be loaded before lightning to avoid segfaults
@@ -83,15 +83,15 @@
     test_pipeline = LanguageModelingTrainingPipeline()
 
     assert test_pipeline is not None
 
     config = template_config.copy()
 
     with importlib_resources.as_file(
-        importlib_resources.files("gt4sd") / "trainer/hf_pl/tests/lm_example.jsonl"
+        importlib_resources.files("gt4sd_trainer") / "hf_pl/tests/lm_example.jsonl"
     ) as file_path:
         config["dataset_args"]["train_file"] = file_path
 
         config["dataset_args"]["validation_file"] = file_path
         config["model_args"]["type"] = "mlm"
 
         data_module, model_module = test_pipeline.get_data_and_model_modules(
@@ -109,15 +109,15 @@
     test_pipeline = LanguageModelingTrainingPipeline()
 
     assert test_pipeline is not None
 
     config = template_config.copy()
 
     with importlib_resources.as_file(
-        importlib_resources.files("gt4sd") / "trainer/hf_pl/tests/lm_example.jsonl"
+        importlib_resources.files("gt4sd_trainer") / "hf_pl/tests/lm_example.jsonl"
     ) as file_path:
         config["dataset_args"]["train_file"] = file_path
         config["dataset_args"]["validation_file"] = file_path
         config["model_args"]["type"] = "clm"
         config["model_args"]["model_name_or_path"] = "gpt2"
 
         data_module, model_module = test_pipeline.get_data_and_model_modules(
@@ -135,15 +135,15 @@
     test_pipeline = LanguageModelingTrainingPipeline()
 
     assert test_pipeline is not None
 
     config = template_config.copy()
 
     with importlib_resources.as_file(
-        importlib_resources.files("gt4sd") / "trainer/hf_pl/tests/lm_example.jsonl"
+        importlib_resources.files("gt4sd_trainer") / "hf_pl/tests/lm_example.jsonl"
     ) as file_path:
         config["dataset_args"]["train_file"] = file_path
         config["dataset_args"]["validation_file"] = file_path
         config["model_args"]["type"] = "cgm"
         config["model_args"]["model_name_or_path"] = "t5-small"
 
         data_module, model_module = test_pipeline.get_data_and_model_modules(
@@ -161,15 +161,15 @@
     test_pipeline = LanguageModelingTrainingPipeline()
 
     assert test_pipeline is not None
 
     config = template_config.copy()
 
     with importlib_resources.as_file(
-        importlib_resources.files("gt4sd") / "trainer/hf_pl/tests/lm_example.jsonl"
+        importlib_resources.files("gt4sd_trainer") / "hf_pl/tests/lm_example.jsonl"
     ) as file_path:
         config["dataset_args"]["train_file"] = file_path
         config["dataset_args"]["validation_file"] = file_path
         config["model_args"]["type"] = "plm"
         config["model_args"]["model_name_or_path"] = "xlnet-base-cased"
 
         data_module, model_module = test_pipeline.get_data_and_model_modules(
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/PKG-INFO` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd-trainer-hf-pl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Transformers trainer submodule of GT4SD.
 Author: GT4SD team
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gt4sd-trainer-hf-pl-0.0.1/src/gt4sd_trainer_hf_pl.egg-info/SOURCES.txt` & `gt4sd-trainer-hf-pl-0.0.2/src/gt4sd_trainer_hf_pl.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-src/gt4sd/trainer/hf_pl/__init__.py
-src/gt4sd/trainer/hf_pl/argument_parser.py
-src/gt4sd/trainer/hf_pl/cli_pl_to_hf_converter.py
-src/gt4sd/trainer/hf_pl/cli_trainer.py
-src/gt4sd/trainer/hf_pl/core.py
-src/gt4sd/trainer/hf_pl/pytorch_lightning_trainer.py
-src/gt4sd/trainer/hf_pl/datasets/__init__.py
-src/gt4sd/trainer/hf_pl/datasets/core.py
-src/gt4sd/trainer/hf_pl/models/__init__.py
-src/gt4sd/trainer/hf_pl/models/core.py
-src/gt4sd/trainer/hf_pl/tests/__init__.py
-src/gt4sd/trainer/hf_pl/tests/lm_example.jsonl
-src/gt4sd/trainer/hf_pl/tests/test_lm_trainer.py
+src/gt4sd_trainer/hf_pl/__init__.py
+src/gt4sd_trainer/hf_pl/argument_parser.py
+src/gt4sd_trainer/hf_pl/cli_pl_to_hf_converter.py
+src/gt4sd_trainer/hf_pl/cli_trainer.py
+src/gt4sd_trainer/hf_pl/core.py
+src/gt4sd_trainer/hf_pl/pytorch_lightning_trainer.py
+src/gt4sd_trainer/hf_pl/datasets/__init__.py
+src/gt4sd_trainer/hf_pl/datasets/core.py
+src/gt4sd_trainer/hf_pl/models/__init__.py
+src/gt4sd_trainer/hf_pl/models/core.py
+src/gt4sd_trainer/hf_pl/tests/__init__.py
+src/gt4sd_trainer/hf_pl/tests/lm_example.jsonl
+src/gt4sd_trainer/hf_pl/tests/test_lm_trainer.py
 src/gt4sd_trainer_hf_pl.egg-info/PKG-INFO
 src/gt4sd_trainer_hf_pl.egg-info/SOURCES.txt
 src/gt4sd_trainer_hf_pl.egg-info/dependency_links.txt
 src/gt4sd_trainer_hf_pl.egg-info/entry_points.txt
 src/gt4sd_trainer_hf_pl.egg-info/requires.txt
 src/gt4sd_trainer_hf_pl.egg-info/top_level.txt
```

