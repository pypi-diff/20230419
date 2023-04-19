# Comparing `tmp/bigdl_nano-2.3.0b20230418-py3-none-win_amd64.whl.zip` & `tmp/bigdl_nano-2.3.0b20230419-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2993492 bytes, number of entries: 226
+Zip file size: 2993860 bytes, number of entries: 226
 -rw-r--r--  2.0 unx      956 b- defN 22-Oct-25 01:39 bigdl/__init__.py
 -rw-r--r--  2.0 unx     1554 b- defN 23-Feb-09 11:06 bigdl/nano/__init__.py
 -rw-r--r--  2.0 unx      684 b- defN 22-Oct-25 01:39 bigdl/nano/openvino.py
 -rw-r--r--  2.0 unx      734 b- defN 22-Oct-25 01:39 bigdl/nano/automl/__init__.py
 -rw-r--r--  2.0 unx      633 b- defN 22-Oct-25 01:39 bigdl/nano/automl/hpo/__init__.py
 -rw-r--r--  2.0 unx     1888 b- defN 22-Oct-25 01:39 bigdl/nano/automl/hpo/backend.py
 -rw-r--r--  2.0 unx     8486 b- defN 23-Feb-09 11:06 bigdl/nano/automl/hpo/callgraph.py
@@ -96,17 +96,17 @@
 -rw-r--r--  2.0 unx      586 b- defN 22-Oct-25 01:39 bigdl/nano/deps/ray/__init__.py
 -rw-r--r--  2.0 unx     1265 b- defN 23-Feb-09 11:06 bigdl/nano/deps/ray/ray_api.py
 -rw-r--r--  2.0 unx     1530 b- defN 23-Feb-09 11:06 bigdl/nano/deps/ray/ray_backend.py
 -rw-r--r--  2.0 unx    18650 b- defN 23-Mar-01 03:16 bigdl/nano/deps/ray/ray_distributed.py
 -rw-r--r--  2.0 unx     3705 b- defN 22-Oct-25 01:39 bigdl/nano/deps/ray/ray_envbase.py
 -rw-r--r--  2.0 unx      618 b- defN 22-Oct-25 01:39 bigdl/nano/k8s/__init__.py
 -rw-r--r--  2.0 unx    13183 b- defN 23-Feb-09 11:06 bigdl/nano/k8s/bigdl_submit.py
--rwxr--r--  2.0 unx  5460184 b- defN 23-Apr-18 11:08 bigdl/nano/libs/libjemalloc.so
--rwxr--r--  2.0 unx  1432624 b- defN 23-Apr-18 11:09 bigdl/nano/libs/libtcmalloc.so
--rwxr--r--  2.0 unx   918296 b- defN 23-Apr-18 11:09 bigdl/nano/libs/libturbojpeg.so.0.2.0
+-rwxr--r--  2.0 unx  5460184 b- defN 23-Apr-19 11:08 bigdl/nano/libs/libjemalloc.so
+-rwxr--r--  2.0 unx  1432624 b- defN 23-Apr-19 11:09 bigdl/nano/libs/libtcmalloc.so
+-rwxr--r--  2.0 unx   918296 b- defN 23-Apr-19 11:08 bigdl/nano/libs/libturbojpeg.so.0.2.0
 -rw-r--r--  2.0 unx     2113 b- defN 23-Mar-09 11:07 bigdl/nano/pytorch/__init__.py
 -rw-r--r--  2.0 unx     5657 b- defN 23-Apr-07 11:07 bigdl/nano/pytorch/context_manager.py
 -rw-r--r--  2.0 unx     3245 b- defN 22-Dec-16 11:06 bigdl/nano/pytorch/dispatcher.py
 -rw-r--r--  2.0 unx     5818 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/lightning.py
 -rw-r--r--  2.0 unx     3063 b- defN 23-Apr-13 11:07 bigdl/nano/pytorch/model.py
 -rw-r--r--  2.0 unx    18937 b- defN 23-Mar-01 07:03 bigdl/nano/pytorch/torch_nano.py
 -rw-r--r--  2.0 unx      706 b- defN 22-Oct-25 01:39 bigdl/nano/pytorch/algorithms/__init__.py
@@ -118,15 +118,15 @@
 -rw-r--r--  2.0 unx      640 b- defN 23-Jan-09 11:06 bigdl/nano/pytorch/encryption/__init__.py
 -rw-r--r--  2.0 unx     6480 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/encryption/encryption.py
 -rw-r--r--  2.0 unx      661 b- defN 23-Feb-23 11:07 bigdl/nano/pytorch/inference/__init__.py
 -rw-r--r--  2.0 unx     4231 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/inference/multi_instance.py
 -rw-r--r--  2.0 unx    88302 b- defN 23-Apr-18 11:06 bigdl/nano/pytorch/inference/optimizer.py
 -rw-r--r--  2.0 unx     4593 b- defN 23-Feb-27 07:35 bigdl/nano/pytorch/inference/pipeline.py
 -rw-r--r--  2.0 unx     3430 b- defN 23-Apr-18 11:06 bigdl/nano/pytorch/low_precision/jit_int8_api.py
--rw-r--r--  2.0 unx    11050 b- defN 23-Apr-18 11:06 bigdl/nano/pytorch/low_precision/jit_int8_model.py
+-rw-r--r--  2.0 unx     9886 b- defN 23-Apr-19 11:06 bigdl/nano/pytorch/low_precision/jit_int8_model.py
 -rw-r--r--  2.0 unx      646 b- defN 22-Oct-25 01:39 bigdl/nano/pytorch/optim/__init__.py
 -rw-r--r--  2.0 unx     8351 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/optim/sparseadam.py
 -rw-r--r--  2.0 unx      804 b- defN 23-Jan-06 11:06 bigdl/nano/pytorch/patching/__init__.py
 -rw-r--r--  2.0 unx      627 b- defN 22-Dec-16 11:06 bigdl/nano/pytorch/patching/dtype_patching/__init__.py
 -rw-r--r--  2.0 unx     4206 b- defN 23-Feb-09 11:06 bigdl/nano/pytorch/patching/dtype_patching/dtype_patching.py
 -rw-r--r--  2.0 unx      637 b- defN 23-Jan-06 11:06 bigdl/nano/pytorch/patching/encryption_patching/__init__.py
 -rw-r--r--  2.0 unx     1854 b- defN 23-Jan-11 11:06 bigdl/nano/pytorch/patching/encryption_patching/encryption_patching.py
@@ -151,15 +151,15 @@
 -rw-r--r--  2.0 unx    31603 b- defN 23-Feb-19 03:08 bigdl/nano/pytorch/vision/transforms/transforms.py
 -rw-r--r--  2.0 unx     1618 b- defN 23-Feb-18 11:06 bigdl/nano/tf/__init__.py
 -rw-r--r--  2.0 unx     4369 b- defN 23-Feb-09 11:06 bigdl/nano/tf/dispatcher.py
 -rw-r--r--  2.0 unx     4894 b- defN 23-Mar-13 11:07 bigdl/nano/tf/model.py
 -rw-r--r--  2.0 unx     1294 b- defN 23-Jan-11 11:06 bigdl/nano/tf/keras/Model.py
 -rw-r--r--  2.0 unx     1076 b- defN 22-Oct-25 01:39 bigdl/nano/tf/keras/Sequential.py
 -rw-r--r--  2.0 unx      845 b- defN 23-Apr-04 11:07 bigdl/nano/tf/keras/__init__.py
--rw-r--r--  2.0 unx    10780 b- defN 23-Apr-07 11:07 bigdl/nano/tf/keras/customized_training_utils.py
+-rw-r--r--  2.0 unx    12580 b- defN 23-Apr-19 11:06 bigdl/nano/tf/keras/customized_training_utils.py
 -rw-r--r--  2.0 unx     4929 b- defN 23-Feb-09 11:06 bigdl/nano/tf/keras/distributed_utils.py
 -rw-r--r--  2.0 unx    11245 b- defN 23-Feb-09 11:06 bigdl/nano/tf/keras/inference_utils.py
 -rw-r--r--  2.0 unx     1244 b- defN 22-Oct-25 01:39 bigdl/nano/tf/keras/inheritance_utils.py
 -rw-r--r--  2.0 unx     5393 b- defN 23-Feb-09 11:06 bigdl/nano/tf/keras/training_utils.py
 -rw-r--r--  2.0 unx      586 b- defN 22-Oct-25 01:39 bigdl/nano/tf/keras/activations/__init__.py
 -rw-r--r--  2.0 unx      609 b- defN 23-Jan-10 11:06 bigdl/nano/tf/keras/amp/__init__.py
 -rw-r--r--  2.0 unx      798 b- defN 23-Feb-02 11:06 bigdl/nano/tf/keras/amp/amp_api.py
@@ -193,36 +193,36 @@
 -rw-r--r--  2.0 unx      709 b- defN 23-Feb-09 11:07 bigdl/nano/utils/common/optimizer/metric.py
 -rw-r--r--  2.0 unx     8336 b- defN 23-Mar-07 11:07 bigdl/nano/utils/common/optimizer/optimizer.py
 -rw-r--r--  2.0 unx     1939 b- defN 23-Apr-18 11:06 bigdl/nano/utils/pytorch/__init__.py
 -rw-r--r--  2.0 unx     1100 b- defN 23-Feb-19 03:08 bigdl/nano/utils/pytorch/attributes.py
 -rw-r--r--  2.0 unx     4527 b- defN 23-Feb-19 03:08 bigdl/nano/utils/pytorch/channel_last.py
 -rw-r--r--  2.0 unx     1807 b- defN 23-Mar-01 07:03 bigdl/nano/utils/pytorch/check_deps.py
 -rw-r--r--  2.0 unx     3358 b- defN 23-Feb-19 03:08 bigdl/nano/utils/pytorch/convert.py
--rw-r--r--  2.0 unx     6234 b- defN 23-Feb-23 11:07 bigdl/nano/utils/pytorch/dataloader.py
+-rw-r--r--  2.0 unx     6197 b- defN 23-Apr-19 11:06 bigdl/nano/utils/pytorch/dataloader.py
 -rw-r--r--  2.0 unx     1321 b- defN 23-Feb-09 11:07 bigdl/nano/utils/pytorch/dataset.py
 -rw-r--r--  2.0 unx     3881 b- defN 23-Feb-10 11:06 bigdl/nano/utils/pytorch/input_sample.py
 -rw-r--r--  2.0 unx     4952 b- defN 23-Feb-19 03:08 bigdl/nano/utils/pytorch/inspect.py
 -rw-r--r--  2.0 unx     2595 b- defN 23-Apr-18 11:06 bigdl/nano/utils/pytorch/jit_method.py
 -rw-r--r--  2.0 unx     6270 b- defN 23-Apr-18 11:06 bigdl/nano/utils/pytorch/load.py
--rw-r--r--  2.0 unx     4739 b- defN 23-Apr-18 11:06 bigdl/nano/utils/pytorch/metadata.py
+-rw-r--r--  2.0 unx     5951 b- defN 23-Apr-19 11:06 bigdl/nano/utils/pytorch/metadata.py
 -rw-r--r--  2.0 unx     1391 b- defN 23-Feb-09 11:07 bigdl/nano/utils/pytorch/metric.py
 -rw-r--r--  2.0 unx     5531 b- defN 23-Mar-03 11:07 bigdl/nano/utils/pytorch/model_info.py
 -rw-r--r--  2.0 unx     2878 b- defN 23-Feb-23 11:07 bigdl/nano/utils/pytorch/save.py
 -rw-r--r--  2.0 unx     1189 b- defN 23-Apr-11 11:07 bigdl/nano/utils/pytorch/version.py
 -rw-r--r--  2.0 unx     1012 b- defN 23-Apr-07 11:07 bigdl/nano/utils/pytorch/xpu.py
 -rw-r--r--  2.0 unx     1057 b- defN 23-Mar-09 11:07 bigdl/nano/utils/tf/__init__.py
 -rw-r--r--  2.0 unx     4300 b- defN 23-Feb-19 03:08 bigdl/nano/utils/tf/attributes.py
 -rw-r--r--  2.0 unx     2816 b- defN 23-Apr-04 11:07 bigdl/nano/utils/tf/backend.py
 -rw-r--r--  2.0 unx     7421 b- defN 23-Mar-13 11:07 bigdl/nano/utils/tf/data.py
 -rw-r--r--  2.0 unx     2582 b- defN 23-Mar-09 11:07 bigdl/nano/utils/tf/preprocess.py
 -rw-r--r--  2.0 unx     1347 b- defN 23-Apr-04 11:07 bigdl/nano/utils/tf/subprocess_worker.py
 -rw-r--r--  2.0 unx      823 b- defN 23-Feb-19 03:08 bigdl/nano/utils/tf/version.py
--rwxr-xr-x  2.0 unx    12068 b- defN 23-Apr-07 11:07 bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init
--rwxr-xr-x  2.0 unx      909 b- defN 22-Dec-29 11:06 bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init.ps1
--rwxr-xr-x  2.0 unx      214 b- defN 23-Feb-02 11:06 bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env
--rwxr-xr-x  2.0 unx      127 b- defN 22-Dec-29 11:06 bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env.ps1
--rw-r--r--  2.0 unx    10112 b- defN 23-Apr-18 11:09 bigdl_nano-2.3.0b20230418.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-18 11:09 bigdl_nano-2.3.0b20230418.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Apr-18 11:09 bigdl_nano-2.3.0b20230418.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-18 11:09 bigdl_nano-2.3.0b20230418.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    21966 b- defN 23-Apr-18 11:09 bigdl_nano-2.3.0b20230418.dist-info/RECORD
-226 files, 8832020 bytes uncompressed, 2957946 bytes compressed:  66.5%
+-rwxr-xr-x  2.0 unx    12068 b- defN 23-Apr-07 11:07 bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init
+-rwxr-xr-x  2.0 unx      909 b- defN 22-Dec-29 11:06 bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init.ps1
+-rwxr-xr-x  2.0 unx      214 b- defN 23-Feb-02 11:06 bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env
+-rwxr-xr-x  2.0 unx      127 b- defN 22-Dec-29 11:06 bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env.ps1
+-rw-r--r--  2.0 unx    10112 b- defN 23-Apr-19 11:09 bigdl_nano-2.3.0b20230419.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-19 11:09 bigdl_nano-2.3.0b20230419.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Apr-19 11:09 bigdl_nano-2.3.0b20230419.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-19 11:09 bigdl_nano-2.3.0b20230419.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    21965 b- defN 23-Apr-19 11:09 bigdl_nano-2.3.0b20230419.dist-info/RECORD
+226 files, 8833830 bytes uncompressed, 2958314 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -645,35 +645,35 @@
 
 Filename: bigdl/nano/utils/tf/subprocess_worker.py
 Comment: 
 
 Filename: bigdl/nano/utils/tf/version.py
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init
+Filename: bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init.ps1
+Filename: bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init.ps1
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env
+Filename: bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env.ps1
+Filename: bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env.ps1
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.dist-info/METADATA
+Filename: bigdl_nano-2.3.0b20230419.dist-info/METADATA
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.dist-info/WHEEL
+Filename: bigdl_nano-2.3.0b20230419.dist-info/WHEEL
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.dist-info/entry_points.txt
+Filename: bigdl_nano-2.3.0b20230419.dist-info/entry_points.txt
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.dist-info/top_level.txt
+Filename: bigdl_nano-2.3.0b20230419.dist-info/top_level.txt
 Comment: 
 
-Filename: bigdl_nano-2.3.0b20230418.dist-info/RECORD
+Filename: bigdl_nano-2.3.0b20230419.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bigdl/nano/pytorch/low_precision/jit_int8_model.py

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 from bigdl.nano.pytorch.context_manager import generate_context_manager
 from bigdl.nano.pytorch.model import AcceleratedLightningModule
+from bigdl.nano.utils.pytorch import jit_convert
 from bigdl.nano.utils.common import compare_version
 import torch
 from torch.ao.quantization import QConfig, get_default_qconfig_mapping
 from torch.quantization.quantize_fx import prepare_fx, convert_fx
 import operator
 from collections.abc import Sequence
 
@@ -139,47 +140,20 @@
                 self.model(*x)
             else:
                 self.model(x)
 
         self.model = convert_fx(self.model)
 
         with torch.no_grad():
-            if self.jit_method == 'trace':
-                if compare_version("torch", operator.ge, "2.0"):
-                    if example_kwarg_inputs is not None:
-                        input_sample = None
-                    self.model = torch.jit.trace(
-                        self.model,
-                        example_inputs=input_sample,
-                        check_trace=False,
-                        strict=jit_strict,
-                        example_kwarg_inputs=example_kwarg_inputs)
-                else:
-                    self.model = torch.jit.trace(
-                        self.model, input_sample,
-                        check_trace=False,
-                        strict=jit_strict)
-            elif self.jit_method == 'script':
-                self.model = torch.jit.script(self.model)
-            else:
-                try:
-                    if compare_version("torch", operator.ge, "2.0"):
-                        self.model = torch.jit.trace(
-                            self.model,
-                            example_inputs=input_sample,
-                            check_trace=False,
-                            strict=jit_strict,
-                            example_kwarg_inputs=example_kwarg_inputs)
-                    else:
-                        self.model = torch.jit.trace(
-                            self.model, input_sample,
-                            check_trace=False,
-                            strict=jit_strict)
-                except Exception:
-                    self.model = torch.jit.script(self.model)
+            if example_kwarg_inputs is not None:
+                input_sample = None
+            self.model = jit_convert(self.model, input_sample,
+                                     jit_method=jit_method,
+                                     jit_strict=jit_strict,
+                                     example_kwarg_inputs=example_kwarg_inputs)
             self.model = torch.jit.freeze(self.model)
 
     def on_forward_start(self, inputs):
         return inputs
 
     def forward_step(self, *inputs):
         if self.channels_last:
```

## bigdl/nano/tf/keras/customized_training_utils.py

```diff
@@ -23,14 +23,15 @@
 import os
 import json
 
 from bigdl.nano.utils.common import schedule_processors
 from bigdl.nano.tf.keras.distributed_utils import _find_free_port
 from tensorflow.keras.losses import Loss
 import warnings
+from bigdl.nano.utils.common import invalidInputError
 
 
 def nano_bf16(func):
     """A decorator to realize mixed precision on customized training loop."""
     # todo check the func signature
     @wraps(func)
     def wrapper(*inner_args):
@@ -128,14 +129,32 @@
                         new_args.append(("dataset", train_ds_def, train_elem_spec))
                         continue
 
                 with open(os.path.join(temp_dir, f"args_{i}.pkl"), 'wb') as f:
                     cloudpickle.dump(arg, f)
                     new_args.append(("others", os.path.join(temp_dir, f"args_{i}.pkl")))
 
+            # check necessary objects
+            arg_instance = list(map(lambda x: x[0], new_args))
+            invalidInputError("model" in arg_instance, "Please check if a model inherited from "
+                                                       "tensorflow.keras.Model or "
+                                                       "bigdl.nano.tf.keras.Model is inputted as "
+                                                       "parameter in train function.")
+            invalidInputError("optimizer" in arg_instance, "Please check if optimizer is inputted"
+                                                           " as parameter in train function.")
+            invalidInputError("loss" in arg_instance, "Please check if loss is inputted as "
+                                                      "parameter in train function. Moreover, if "
+                                                      "you use a customized loss, please add "
+                                                      "'nano_multiprocessing_loss' decorator.")
+            invalidInputError("dataset" in arg_instance, "Please check if tensorflow.data.Dataset "
+                                                         "is inputted as parameter in train "
+                                                         "function. Moreover, if dataset is "
+                                                         "created by 'from_generator', please init"
+                                                         " '_GeneratorState' of dataset first.")
+
             target_path = os.path.join(temp_dir, "target.pkl")
             with open(target_path, 'wb') as f:
                 cloudpickle.dump(self.func, f)
 
             ports = set()
             while len(ports) < self.nproc:
                 ports.add(_find_free_port())
@@ -221,15 +240,19 @@
                        isinstance(actrual_args[i], nano_multiprocessing):
                         actrual_args[i] = partial(actrual_args[i],
                                                   mirrored_strategy=mirrored_strategy)
 
         with open(target_path, 'rb') as f:
             target_func = cloudpickle.load(f)
 
-        res = target_func(*actrual_args)
+        try:
+            res = target_func(*actrual_args)
+        except TypeError:
+            invalidInputError(False, "Please check if you have added 'nano_multiprocessing' "
+                                     "decorator to the train_step function.")
 
         task_id = mirrored_strategy.cluster_resolver.task_id
         if task_id == 0:
             path = os.path.join('trained_model_weights')
             new_model.save_weights(path, overwrite=True)
 
     try:
```

## bigdl/nano/utils/pytorch/dataloader.py

```diff
@@ -114,16 +114,14 @@
             # input_sample is a Tensor
             if len(loader_input_sample) > 1:
                 return False
             return True
         if len(loader_input_sample) > len(input_sample):
             # input_sample is also a sequence
             return False
-        else:
-            return True
     if isinstance(loader_input_sample, Sequence):
         if isinstance(loader_input_sample[0], Sequence) and \
                 len(loader_input_sample[0]) == forward_args_len:
             # this means user returns a (x1, x2, ...), y
             return False
         else:
             if len(loader_input_sample) > forward_args_len:
@@ -146,8 +144,8 @@
                                 model(*loader_input_sample[0])
                                 return False
                             except Exception:
                                 # input sample don't contain label
                                 return True
                         else:
                             return True
-    return True
+    return False
```

## bigdl/nano/utils/pytorch/metadata.py

```diff
@@ -11,15 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import torch
-from ..common import invalidInputError
+
+
+class CustomDict(dict):
+    """Custom Dict class for class with dataclass, esp. for BaseOutput in diffusers
+    """
+    def __getattr__(self, key):
+        if key in self.keys():
+            return self.__getitem__(key)
+        else:
+            super().__getattr__(key)
 
 
 class BasicMetaDataInfo(object):
     """Meta info class for basic type like int, float, str
     """
     def __init__(self, input_element):
         self.type = type(input_element)
@@ -36,14 +45,41 @@
 
 
 class DictMetaDataInfo(object):
     """Meta info class for dict
     """
     def __init__(self, input_element):
         self.type = type(input_element)
+        # normal dict or custom class
+        random_key = list(input_element.keys())[0]
+        if hasattr(input_element, random_key):
+            # has attr, is custom class
+            # fake a dataclass
+            self.class_fn = CustomDict
+        else:
+            # normal dict
+            self.class_fn = dict
+        self.length = len(input_element)
+        self.keys = list(input_element.keys())
+        self.infos = []
+        for k in self.keys:
+            v = input_element[k]
+            info = get_meta_info_from_input(v)
+            if isinstance(info, ListMetaDataInfo):
+                # list inside dict requires reconstruction
+                info.need_reconstruct = True
+            self.infos.append(info)
+        self.need_reconstruct = True
+
+
+class CustomClassMetaDataInfo(object):
+    """Meta info class for custom class which is instance of dict
+    """
+    def __init__(self, input_element):
+        self.type = type(input_element)
         self.length = len(input_element)
         self.keys = list(input_element.keys())
         self.infos = []
         for k in self.keys:
             v = input_element[k]
             info = get_meta_info_from_input(v)
             if isinstance(info, ListMetaDataInfo):
@@ -101,15 +137,15 @@
     def reconstruct_output(output, metadata):
         if not metadata.need_reconstruct:
             return output
         elif isinstance(metadata, DictMetaDataInfo):
             # Single dict
             if not isinstance(output, (tuple, list)):
                 output = [output]
-            new_output = {}
+            new_output = metadata.class_fn()
             ind_out = 0
             for idx, k in enumerate(metadata.keys):
                 meta = metadata.infos[idx]
                 if not meta.need_reconstruct:
                     new_output[k] = output[ind_out]
                     ind_out += 1
                 else:
```

## Comparing `bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init` & `bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init`

 * *Files identical despite different names*

## Comparing `bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init.ps1` & `bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init.ps1`

 * *Files identical despite different names*

## Comparing `bigdl_nano-2.3.0b20230418.dist-info/METADATA` & `bigdl_nano-2.3.0b20230419.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdl-nano
-Version: 2.3.0b20230418
+Version: 2.3.0b20230419
 Summary: High-performance scalable acceleration components for intel.
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `bigdl_nano-2.3.0b20230418.dist-info/RECORD` & `bigdl_nano-2.3.0b20230419.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 bigdl/nano/pytorch/encryption/__init__.py,sha256=4e0eEjjj3iNwnCRzLtzVjS27oH-CA1ws6TJXnuUwNg8,640
 bigdl/nano/pytorch/encryption/encryption.py,sha256=UIiNtbyZ0GFlkirOHX2hOzxKXtYJ6g56SQ2lJvO40kY,6480
 bigdl/nano/pytorch/inference/__init__.py,sha256=PlFS2XblVRBXTai86gEV79sQWEJLgaOyDnjdLYNKxTA,661
 bigdl/nano/pytorch/inference/multi_instance.py,sha256=XCMQRg1BHfuQWxNTtsHpplZfSNSj0rEO71if67OsR-I,4231
 bigdl/nano/pytorch/inference/optimizer.py,sha256=XWxR_Vt39v40kCRqachrZf6Qc1SY5Op2y9l5OW1toSs,88302
 bigdl/nano/pytorch/inference/pipeline.py,sha256=lpU1OyoIjYsVf6nw0IF8JH82Z228_WSMj_qZtww1F6A,4593
 bigdl/nano/pytorch/low_precision/jit_int8_api.py,sha256=HJeNprNAa6DyCx7PLZvM26j63kEtr1luo-hjVJK-ypk,3430
-bigdl/nano/pytorch/low_precision/jit_int8_model.py,sha256=pjYvB_5Wt4CEFXr5tPyo2WIE7tpKcv7BFQ1JqEoHYXU,11050
+bigdl/nano/pytorch/low_precision/jit_int8_model.py,sha256=7XJNYiNznJDLeLyiKDOZCjB7fHLaU-hN3WMLuVKCF4s,9886
 bigdl/nano/pytorch/optim/__init__.py,sha256=JWc3YVybOcyixkTxAB2QVN9l4KZC7BXg8D2myUs2P-w,646
 bigdl/nano/pytorch/optim/sparseadam.py,sha256=22GGm0Kh2idtAgEj5mn5asMYc3CoKbbE-gwPqtXwrgA,8351
 bigdl/nano/pytorch/patching/__init__.py,sha256=LGg-BpIbWHdj_LNe4Px1m2lU-Y9LFAmWtctRF9wbCFM,804
 bigdl/nano/pytorch/patching/dtype_patching/__init__.py,sha256=P99b-m_UygHUv-c1jsfE2Q0dtGkbM_mt_GFio7bBFlQ,627
 bigdl/nano/pytorch/patching/dtype_patching/dtype_patching.py,sha256=AL054yiXtljxh9GrqNRRL1wqzPzacQV8LnyEiXOZH-c,4206
 bigdl/nano/pytorch/patching/encryption_patching/__init__.py,sha256=G8mkHd00JeSdgamd8QTemg4ZPx59VDN7N6HgbnMLxbM,637
 bigdl/nano/pytorch/patching/encryption_patching/encryption_patching.py,sha256=Ldygx4lor-gff-Cbzb05YGItBSOdCv1lNytAnqHqX0U,1854
@@ -150,15 +150,15 @@
 bigdl/nano/pytorch/vision/transforms/transforms.py,sha256=_lUA2Iia9oBoGIvs2qtuVvP1ZYi0wRf2AVFiS7_iuCQ,31603
 bigdl/nano/tf/__init__.py,sha256=ddDA5Hroej7135IqG33_AaAJWGOe2xIFofKvlYQIEHQ,1618
 bigdl/nano/tf/dispatcher.py,sha256=LQEkQ3oNIsXN8_fRJ-glZ0oafeL4pNx57Z-EezgRaTM,4369
 bigdl/nano/tf/model.py,sha256=0pMiYGU_E09ZQWrsfKIWoOHbUmYzvuetFMLxgIsS58E,4894
 bigdl/nano/tf/keras/Model.py,sha256=KSreLfjajd33pdIaquXtJ1QJZg3hy7xxsCJui-nSiPM,1294
 bigdl/nano/tf/keras/Sequential.py,sha256=kTEL-a2TJR4WfllEMFNB0uAqiNxC-QVLwYACGzL3GRE,1076
 bigdl/nano/tf/keras/__init__.py,sha256=W5yReX_Inc7OZvm921PPOj1VgdOI6UK1QXRdLF8Zkqw,845
-bigdl/nano/tf/keras/customized_training_utils.py,sha256=bf13QmVvpvuoK_CYWcT14xA-G6MpsTY9fVDfC_rHvDk,10780
+bigdl/nano/tf/keras/customized_training_utils.py,sha256=X2QaGDROHJpUs32cAWga9QjSaxylewY6x3_Vxr5JX80,12580
 bigdl/nano/tf/keras/distributed_utils.py,sha256=1azz9J_hBZm7LrrWO2YXKg_TZ1klIsR0NVSYdBpYdOM,4929
 bigdl/nano/tf/keras/inference_utils.py,sha256=Gw6tq2qhM7TgMRG4Qd_idi40wbpXCIFxqpqXV2yj6ig,11245
 bigdl/nano/tf/keras/inheritance_utils.py,sha256=DAfgLMTSDLNQTcKMy8nvpcoeKLwgvOnh2s8FH6IRyFU,1244
 bigdl/nano/tf/keras/training_utils.py,sha256=olSU29cBgKwRHJGv0Ggn_t_hOleiRDr13RU3Y04_AP8,5393
 bigdl/nano/tf/keras/activations/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 bigdl/nano/tf/keras/amp/__init__.py,sha256=5T_pNFHbS-EdK7nlbJJqb4JlCvUnPQpO-sxVZuaP6Ys,609
 bigdl/nano/tf/keras/amp/amp_api.py,sha256=yJHm-pIaPX2rQdxqmADjFv5l7H3G9fPVVpaK2YYJUJw,798
@@ -192,35 +192,35 @@
 bigdl/nano/utils/common/optimizer/metric.py,sha256=5VpF8vdUoomQnssJo1o7iF6cVMOPO0PQw1sTt29Ykqs,709
 bigdl/nano/utils/common/optimizer/optimizer.py,sha256=PgOem9vDwbhNY9rrzb9VoWBxZFA8y19kUiD6KwlrQH4,8336
 bigdl/nano/utils/pytorch/__init__.py,sha256=GQN0YyzbnQTb-sUyhrZmv_zUQhdPBZGgnbvR4NtCIog,1939
 bigdl/nano/utils/pytorch/attributes.py,sha256=vFxq074vDnw7OWuiQH-9ERJRk3CU719GxBHmWAB_3kQ,1100
 bigdl/nano/utils/pytorch/channel_last.py,sha256=iDbh_s8yFIFq0i1JRyCCYIJf67FRrf7FNU5j1js05NY,4527
 bigdl/nano/utils/pytorch/check_deps.py,sha256=oFq4BvkXQgJdpQBVwYwCd1ZN64Gfu16rmC55AO5KU-0,1807
 bigdl/nano/utils/pytorch/convert.py,sha256=kTQRSN7RZSoPXm7Q77wxUtGVBZ6KKz6pXNuFf36mobA,3358
-bigdl/nano/utils/pytorch/dataloader.py,sha256=pYC4dYKKQLH8XFtCqJ66pvhSyGBSNfM1JFTUuyf6jfQ,6234
+bigdl/nano/utils/pytorch/dataloader.py,sha256=D0vO2NdWtM-8aQQ5EsGWZqgIqBqFi8B03zEOvaWvYsk,6197
 bigdl/nano/utils/pytorch/dataset.py,sha256=8niaxA5SMmet_nVFiO9NMeL4hesCJsJxjhNJwRxfouc,1321
 bigdl/nano/utils/pytorch/input_sample.py,sha256=1wecir3d9uNn39o_StO9GZHr3TMCRC5G4eK4ykIkF-Q,3881
 bigdl/nano/utils/pytorch/inspect.py,sha256=z013opp8CfvOHFFDju2tW9v6vhdjLwQ5huychXYKpiU,4952
 bigdl/nano/utils/pytorch/jit_method.py,sha256=YuSi4LIY828eIFcVJ7VtnLhhkRzVRq_rI0AYMrTQLrk,2595
 bigdl/nano/utils/pytorch/load.py,sha256=LxJ5pQd9Ijfc-KreuihtF1p__Gl25O5a2Noqcm1UHJA,6270
-bigdl/nano/utils/pytorch/metadata.py,sha256=Igl8AXn36WaJGvJWvewaU_CrhGQssDIyImYpqlElkxs,4739
+bigdl/nano/utils/pytorch/metadata.py,sha256=bD1iTrQHntNvefJMNx2umRBGA1CDp0q0Oe3pZmRhx_M,5951
 bigdl/nano/utils/pytorch/metric.py,sha256=7TFBw2F5t_sh-2p0XbbUgUujZULBIwBMFIRt5FV4ATA,1391
 bigdl/nano/utils/pytorch/model_info.py,sha256=IT4RYtgB-YukrEudgu5j3BKDnCBlOIuKo_EyFQuG0G4,5531
 bigdl/nano/utils/pytorch/save.py,sha256=kGCz6w1Dhx4jAgo3A2TAaFv9zL6pxdEeJCJMEnGyX6k,2878
 bigdl/nano/utils/pytorch/version.py,sha256=-zK3eeKIOBgi4HAsUYTumux4axNcx8gYrh61TRm8i-4,1189
 bigdl/nano/utils/pytorch/xpu.py,sha256=anqzDwqy701n-hmSY75G7TrM56WZ6Vdcgbb53q74F6I,1012
 bigdl/nano/utils/tf/__init__.py,sha256=wxh1M-4H8NwLSNhiipdZcXs8gtycV3Cs2DcVPRUnuAE,1057
 bigdl/nano/utils/tf/attributes.py,sha256=AkRSYw0bmdpLwnWZjRXsaIVrDW9H2TJpBB3Tq-RVoGg,4300
 bigdl/nano/utils/tf/backend.py,sha256=CfI_33A-2Na8R462k592F0FlAkwu0lTKzedf_SXyUgQ,2816
 bigdl/nano/utils/tf/data.py,sha256=HyrSXuDeSC-b2X8yP7RBTTKgvLDhV5OqXf7eFOte6nc,7421
 bigdl/nano/utils/tf/preprocess.py,sha256=DHukkdJUa-3z0jK63okaJ0vhbRAJipAoBUpsyS4P93k,2582
 bigdl/nano/utils/tf/subprocess_worker.py,sha256=LitCgfBQdnMqOmGuio4y58Mh9xCoxvn3JVS0INek5mE,1347
 bigdl/nano/utils/tf/version.py,sha256=IN7ZGJJPKSUAJN2LmiJgO_C6cZM8d9023DjcwZ0x9sg,823
-bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init,sha256=A-cN-f_uxGLK3UX7AkwdCpcaMij9SE-rbySsCZRPAPY,12068
-bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-init.ps1,sha256=kX83Ue2ZJgibvddidAHzQ5zhbGlHntKlTcK5lvNmkV4,909
-bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env,sha256=rWzU73m1pflJazC6ulhItByaoudgSa8XlUAJVj3W02c,214
-bigdl_nano-2.3.0b20230418.data/scripts/bigdl-nano-unset-env.ps1,sha256=amIge9q2-1oumygXfW00qeYejEdVMESNUferj5B7txU,127
-bigdl_nano-2.3.0b20230418.dist-info/METADATA,sha256=2zEOlI1B4JoPedGH_TgNaHpZ7SLim7U3afJM1Laqqfc,10112
-bigdl_nano-2.3.0b20230418.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
-bigdl_nano-2.3.0b20230418.dist-info/entry_points.txt,sha256=NJqjgi9adpmsUUYPXsd7LzSBdoN1nYjeOyFi9Wih_oU,54
-bigdl_nano-2.3.0b20230418.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
-bigdl_nano-2.3.0b20230418.dist-info/RECORD,,
+bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init,sha256=A-cN-f_uxGLK3UX7AkwdCpcaMij9SE-rbySsCZRPAPY,12068
+bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-init.ps1,sha256=kX83Ue2ZJgibvddidAHzQ5zhbGlHntKlTcK5lvNmkV4,909
+bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env,sha256=rWzU73m1pflJazC6ulhItByaoudgSa8XlUAJVj3W02c,214
+bigdl_nano-2.3.0b20230419.data/scripts/bigdl-nano-unset-env.ps1,sha256=amIge9q2-1oumygXfW00qeYejEdVMESNUferj5B7txU,127
+bigdl_nano-2.3.0b20230419.dist-info/METADATA,sha256=_IgRbe4Bu08rGX4qAvKvRqwzP3bEEU3KLagUF1Q5q70,10112
+bigdl_nano-2.3.0b20230419.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+bigdl_nano-2.3.0b20230419.dist-info/entry_points.txt,sha256=NJqjgi9adpmsUUYPXsd7LzSBdoN1nYjeOyFi9Wih_oU,54
+bigdl_nano-2.3.0b20230419.dist-info/top_level.txt,sha256=iGuLfZARD_qANcIMfy0tbbrC3EtCg6BSiH8icc3dLWs,6
+bigdl_nano-2.3.0b20230419.dist-info/RECORD,,
```

