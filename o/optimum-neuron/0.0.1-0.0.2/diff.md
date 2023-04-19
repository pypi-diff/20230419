# Comparing `tmp/optimum-neuron-0.0.1.tar.gz` & `tmp/optimum-neuron-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.1.tar", last modified: Mon Mar 13 14:09:29 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.2.tar", last modified: Wed Apr 19 16:48:44 2023, max compression
```

## Comparing `optimum-neuron-0.0.1.tar` & `optimum-neuron-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,51 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.537550 optimum-neuron-0.0.1/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.1/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.1/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10718 2023-03-13 14:09:29.537550 optimum-neuron-0.0.1/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-03-13 13:15:30.000000 optimum-neuron-0.0.1/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.533549 optimum-neuron-0.0.1/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.533549 optimum-neuron-0.0.1/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      918 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/optimum/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-13 09:50:20.000000 optimum-neuron-0.0.1/optimum/neuron/hf_argparser.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5358 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/optimum/neuron/trainers.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.533549 optimum-neuron-0.0.1/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)      621 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3750 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9068 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-03-13 13:17:43.000000 optimum-neuron-0.0.1/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.537550 optimum-neuron-0.0.1/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10718 2023-03-13 14:09:29.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      554 2023-03-13 14:09:29.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-03-13 14:09:29.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      136 2023-03-13 14:09:29.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-03-13 14:09:29.000000 optimum-neuron-0.0.1/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1034 2023-02-10 14:28:23.000000 optimum-neuron-0.0.1/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-03-13 14:09:29.537550 optimum-neuron-0.0.1/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2229 2023-03-13 14:09:20.000000 optimum-neuron-0.0.1/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-13 14:09:29.537550 optimum-neuron-0.0.1/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    26359 2023-03-13 13:15:21.000000 optimum-neuron-0.0.1/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-10 14:24:28.000000 optimum-neuron-0.0.1/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.2/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.2/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4755 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4523 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4655 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12023 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/model_configs.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.2/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/neuron/trainers.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4745 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17609 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.2/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1193 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      277 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2549 2023-04-19 16:48:33.000000 optimum-neuron-0.0.2/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    23763 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    26361 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.2/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.1/LICENSE` & `optimum-neuron-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.1/MANIFEST.in` & `optimum-neuron-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.1/PKG-INFO` & `optimum-neuron-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.1
+Version: 0.0.2
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: quality
+Provides-Extra: neuron
+Provides-Extra: neuronx
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `optimum-neuron-0.0.1/README.md` & `optimum-neuron-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.1/optimum/neuron/__init__.py` & `optimum-neuron-0.0.2/optimum/neuron/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # coding=utf-8
-# Copyright 2023 The HuggingFace Team. All rights reserved.
+# Copyright 2023 The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 
-from .hf_argparser import TrainiumHfArgumentParser
-from .trainers import Seq2SeqTrainiumTrainer, TrainiumTrainer
-from .utils.training_utils import patch_transformers_for_neuron_sdk
-
-
-if not os.environ.get("DISABLE_TRANSFORMERS_PATCHING", False):
-    patch_transformers_for_neuron_sdk()
+from .argument_utils import convert_neuronx_compiler_args_to_neuron
+from .import_utils import is_neuron_available, is_neuronx_available
+from .training_utils import (
+    FirstAndLastDataset,
+    Patcher,
+    is_model_officially_supported,
+    is_precompilation,
+    patch_forward,
+    patch_model,
+    patch_transformers_for_neuron_sdk,
+    patched_finfo,
+    prepare_environment_for_neuron,
+)
```

### Comparing `optimum-neuron-0.0.1/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.2/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.1/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.2/optimum/neuron/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# coding=utf-8
-# Copyright 2023 The HuggingFace Team. All rights reserved.
+#  Copyright 2022 The HuggingFace Team. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+__version__ = "0.0.2"
```

### Comparing `optimum-neuron-0.0.1/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.2/optimum/neuron/utils/argument_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -82,7 +82,40 @@
             logger.warning(error_msg)
         else:
             raise_error_msg = (
                 "Aborting training. To disable automatic failure when an argument value is inferred to be wrong for "
                 "Tranium, set the environment variable OPTIMUM_DISABLE_STRICT_MODE to 1."
             )
             raise ValueError(f"{error_msg}\n{raise_error_msg}")
+
+
+def convert_neuronx_compiler_args_to_neuron(
+    auto_cast: Optional[str] = None,
+    auto_cast_type: Optional[str] = None,
+    disable_fast_relayout: Optional[bool] = False,
+):
+    """
+    Builds `compiler_args` for neuron compiler.
+    """
+    compiler_args = []
+
+    if auto_cast is None:
+        auto_cast = "none"
+    elif auto_cast == "matmul":
+        auto_cast = "matmult"
+
+    if auto_cast in ["none", "all"]:
+        compiler_args.extend(["--fast-math", auto_cast])
+    elif auto_cast == "matmult":
+        if auto_cast_type is None:
+            compiler_args.extend(["--fast-math", "fp32-cast-matmult"])
+        else:
+            compiler_args.extend(["--fast-math", f"fp32-cast-matmult-{auto_cast_type}"])
+    else:
+        raise ValueError(
+            f"The auto_cast value {auto_cast} is not valid. Please use one of the following: None, all or matmul."
+        )
+
+    if disable_fast_relayout is True:
+        compiler_args.append("no-fast-relayout")
+
+    return compiler_args
```

### Comparing `optimum-neuron-0.0.1/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.2/optimum/neuron/utils/training_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-"""Various utilities"""
+"""Training utilities"""
 
 import contextlib
 import functools
 import importlib
 import os
 from typing import TYPE_CHECKING, Callable, List, Optional, Tuple, Union
```

### Comparing `optimum-neuron-0.0.1/optimum/neuron/version.py` & `optimum-neuron-0.0.2/optimum/exporters/neuron/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-#  Copyright 2023 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2023 The HuggingFace Team. All rights reserved.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-__version__ = "0.0.1"
+from .base import NeuronConfig
+from .convert import export, validate_model_outputs
```

### Comparing `optimum-neuron-0.0.1/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.2/optimum_neuron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.1
+Version: 0.0.2
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: quality
+Provides-Extra: neuron
+Provides-Extra: neuronx
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `optimum-neuron-0.0.1/pyproject.toml` & `optimum-neuron-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,25 @@
 
 [tool.black]
 line-length = 119
 target-version = ['py38']
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
-ignore = ["E501", "E741", "W605"]
-select = ["E", "F", "I", "W"]
+ignore = ["C901", "E501", "E741", "W605"]
+select = ["C", "E", "F", "I", "W"]
 line-length = 119
 
 # Ignore import violations in all `__init__.py` files.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 
 [tool.ruff.isort]
 lines-after-imports = 2
 known-first-party = ["optimum.neuron"]
+
+[tool.pytest.ini_options]
+markers = [
+    "is_staging_test",
+    "is_trainium_test",
+    "is_inferentia_test",
+]
```

### Comparing `optimum-neuron-0.0.1/setup.py` & `optimum-neuron-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
-    "transformers >= 4.26.0",
+    "transformers >= 4.28.0",
     "optimum",
 ]
 
 TESTS_REQUIRE = [
     "pytest",
     "psutil",
     "parameterized",
@@ -25,28 +25,37 @@
     "sentencepiece",
     "datasets",
 ]
 
 QUALITY_REQUIRES = [
     "black",
     "ruff",
+    "isort",
     "hf_doc_builder",
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
+    "neuron": [
+        "wheel",
+        "torch-neuron==1.12.1.*",
+        "neuron-cc[tensorflow]",
+        "protobuf",
+        "torchvision",
+    ],
+    "neuronx": ["neuronx-cc==2.*", "torch-neuronx", "torchvision"],
 }
 
 setup(
     name="optimum-neuron",
     version=__version__,
     description=(
-        "Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS"
-        " Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and "
+        "Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS "
+        "Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and "
         "inference on single and multiple neuron core settings for different downstream tasks."
     ),
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: Apache Software License",
@@ -64,8 +73,9 @@
     author_email="hardware@huggingface.co",
     license="Apache",
     packages=find_namespace_packages(include=["optimum*"]),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     include_package_data=True,
     zip_safe=False,
+    entry_points={"console_scripts": ["optimum-cli=optimum.commands.optimum_cli:main"]},
 )
```

### Comparing `optimum-neuron-0.0.1/tests/test_examples.py` & `optimum-neuron-0.0.2/tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     MODEL_FOR_MULTIPLE_CHOICE_MAPPING,
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
-from utils import MODELS_TO_TEST_MAPPING
+
+from .utils import MODELS_TO_TEST_MAPPING
 
 
 def _get_supported_models_for_script(
     models_to_test: Dict[str, str], task_mapping: Dict[str, str], to_exclude: Optional[Set[str]] = None
 ) -> List[str]:
     """
     Filters models that can perform the task from models_to_test.
```

### Comparing `optimum-neuron-0.0.1/tests/test_utils.py` & `optimum-neuron-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

