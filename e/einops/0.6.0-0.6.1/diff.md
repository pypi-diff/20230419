# Comparing `tmp/einops-0.6.0.tar.gz` & `tmp/einops-0.6.1.tar.gz`

## Comparing `einops-0.6.0.tar` & `einops-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 einops-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 einops-0.6.0/test.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 einops-0.6.0/einops/__init__.py
--rw-r--r--   0        0        0    20964 2020-02-02 00:00:00.000000 einops-0.6.0/einops/_backends.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 einops-0.6.0/einops/_torch_specific.py
--rw-r--r--   0        0        0    33737 2020-02-02 00:00:00.000000 einops-0.6.0/einops/einops.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.6.0/einops/packing.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.6.0/einops/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.0/einops/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.0/einops/experimental/__init__.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.6.0/einops/experimental/data_api_packing.py
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.6.0/einops/experimental/indexing.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/__init__.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/_einmix.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/chainer.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/flax.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/gluon.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/keras.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/oneflow.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/tensorflow.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 einops-0.6.0/einops/layers/torch.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.6.0/scripts/convert_readme.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 einops-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_einsum.py
--rw-r--r--   0        0        0    11236 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_examples.py
--rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_layers.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_notebooks.py
--rw-r--r--   0        0        0    23226 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_ops.py
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_other.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_packing.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.6.0/tests/test_parsing.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 einops-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.6.0/LICENSE
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 einops-0.6.0/README.md
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 einops-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 einops-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 einops-0.6.1/mkdocs.yml
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.6.1/test.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 einops-0.6.1/einops/__init__.py
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 einops-0.6.1/einops/_backends.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 einops-0.6.1/einops/_torch_specific.py
+-rw-r--r--   0        0        0    33690 2020-02-02 00:00:00.000000 einops-0.6.1/einops/einops.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.6.1/einops/packing.py
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.6.1/einops/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.1/einops/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/__init__.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/data_api_packing.py
+-rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.6.1/einops/experimental/indexing.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/__init__.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/_einmix.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/chainer.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/flax.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/gluon.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/keras.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/oneflow.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/paddle.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/tensorflow.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 einops-0.6.1/einops/layers/torch.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.6.1/scripts/convert_readme.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 einops-0.6.1/scripts/setup.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 einops-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_einsum.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_examples.py
+-rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_layers.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_ops.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_other.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_packing.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.6.1/tests/test_parsing.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 einops-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.6.1/LICENSE
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 einops-0.6.1/README.md
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 einops-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 einops-0.6.1/PKG-INFO
```

### Comparing `einops-0.6.0/mkdocs.yml` & `einops-0.6.1/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       - parse_shape: api/parse_shape.md
       - rearrange: api/rearrange.md
       - reduce: api/reduce.md
       - repeat: api/repeat.md
       - einsum: api/einsum.md
       - pack and unpack: api/pack_unpack.md
   - Testimonials: pages/testimonials.md
-  - Projects: pages/projects.md
+  - Community/Ecosystem: pages/projects.md
 extra:
   search:
     language: en
 markdown_extensions:
   - admonition
   - codehilite
   - pymdownx.arithmatex
```

### Comparing `einops-0.6.0/einops/_backends.py` & `einops-0.6.1/einops/_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -244,78 +244,14 @@
         return 'float' in str(x.dtype)
 
     def layers(self):
         from .layers import gluon
         return gluon
 
 
-class MXNetBackend(AbstractBackend):
-    framework_name = 'mxnet.symbol'
-
-    def __init__(self):
-        import mxnet
-        self.mx = mxnet
-
-    def is_appropriate_type(self, tensor):
-        return isinstance(tensor, self.mx.symbol.Symbol)
-
-    def create_symbol(self, shape, dtype='float32'):
-        # mxnet accepts zeros as undefined dimensions
-        shape = tuple(0 if d is None else d for d in shape)
-        var = self.mx.symbol.Variable('input', shape=shape, dtype=dtype)
-        return var
-
-    def eval_symbol(self, symbol, input_dict):
-        args = {var.name: self.mx.nd.array(val) for var, val in input_dict}
-        ex = symbol.bind(ctx=self.mx.cpu(), args=args)
-        ex.forward()
-        return ex.outputs[0].asnumpy()
-
-    def shape(self, x):
-        # mxnet has problems with shape inference - it does not provide shape symbols
-        # shape_array seems to be impossible to use in shape inference
-        # infer_shape_partial returns empty tuple if was not able to infer shape
-        # reductions such as sum can't return scalars, but return 1-element vectors
-        shape = x.infer_shape_partial()[1][0]
-        if len(shape) == 0:
-            warnings.warn('mxnet inferred shape to be (), which probably means it could not be inferred')
-        shape = tuple(UnknownSize() if d == 0 else d for d in shape)
-        return shape
-
-    def reshape(self, x, shape):
-        if len(shape) == 0:
-            return x  # poor support of scalars in mxnet
-        if any(isinstance(dimension, UnknownSize) for dimension in shape):
-            from einops import EinopsError
-            raise EinopsError("Mxnet couldn't infer all dimensions statically, please provide those with axes_lengths")
-        return x.reshape(shape)
-
-    def arange(self, start, stop):
-        return self.mx.symbol.arange(start, stop)
-
-    def stack_on_zeroth_dimension(self, tensors: list):
-        return self.mx.symbol.stack(*tensors)
-
-    def tile(self, x, repeats):
-        return self.mx.symbol.tile(x, repeats)
-
-    def concat(self, tensors, axis: int):
-        return self.mx.symbol.concat(tensors, dim=axis)
-
-    def add_axis(self, x, new_position):
-        return self.mx.symbol.expand_dims(x, new_position)
-
-    def is_float_type(self, x):
-        return 'float' in str(x.infer_type()[1][0])
-
-    def layers(self):
-        from .layers import gluon
-        return gluon
-
-
 class TorchBackend(AbstractBackend):
     framework_name = 'torch'
 
     def __init__(self):
         import torch
         self.torch = torch
 
@@ -364,15 +300,15 @@
             repeats[axis_position] = axis_length
         return x.expand(repeats)
 
     def tile(self, x, repeats):
         return x.repeat(repeats)
 
     def concat(self, tensors, axis: int):
-        return self.torch.concat(tensors, dim=axis)
+        return self.torch.cat(tensors, dim=axis)
 
     def add_axis(self, x, new_position):
         return self.torch.unsqueeze(x, new_position)
 
     def is_float_type(self, x):
         return x.dtype in [self.torch.float16, self.torch.float32, self.torch.float64, self.torch.bfloat16]
 
@@ -613,15 +549,14 @@
 
 class OneFlowBackend(AbstractBackend):
     framework_name = "oneflow"
 
     def __init__(self):
         import oneflow as flow
         self.flow = flow
-        print("using oneflow")
 
     def is_appropriate_type(self, tensor):
         return isinstance(tensor, self.flow.Tensor)
 
     def from_numpy(self, x):
         variable = self.flow.from_numpy(x)
         if self.is_float_type(variable):
@@ -673,8 +608,75 @@
         return x.dtype in [self.flow.float16, self.flow.float32, self.flow.float64]
 
     def layers(self):
         from .layers import oneflow
         return oneflow
 
     def einsum(self, pattern, *x):
-        return self.flow.einsum(pattern, *x)
+        return self.flow.einsum(pattern, *x)
+
+
+class PaddleBackend(AbstractBackend):
+    framework_name = "paddle"
+
+    def __init__(self):
+        import paddle
+        self.paddle = paddle
+
+    def is_appropriate_type(self, tensor):
+        return isinstance(tensor, (self.paddle.Tensor, self.paddle.static.Variable))
+
+    def from_numpy(self, x):
+        tensor = self.paddle.to_tensor(x)
+        tensor.stop_gradient = False
+        return tensor
+
+    def to_numpy(self, x):
+        return x.detach().numpy()
+
+    def arange(self, start, stop):
+        return self.paddle.arange(start, stop, dtype=self.paddle.int64)
+
+    def reduce(self, x, operation, axes):
+        # TODO: Support the reduce operation to output a 0D Tensor
+        if len(axes) == x.ndim:
+            return super().reduce(x, operation, axes).squeeze(0)
+        else:
+            return super().reduce(x, operation, axes)
+
+    def transpose(self, x, axes):
+        return x.transpose(axes)
+
+    def add_axes(self, x, n_axes, pos2len):
+        repeats = [-1] * n_axes
+        for axis_position, axis_length in pos2len.items():
+            x = self.add_axis(x, axis_position)
+            repeats[axis_position] = axis_length
+        return x.expand(repeats)
+
+    def stack_on_zeroth_dimension(self, tensors: list):
+        return self.paddle.stack(tensors)
+
+    def reshape(self, x, shape):
+        return x.reshape(shape)
+
+    def tile(self, x, repeats):
+        return x.tile(repeats)
+
+    def concat(self, tensors, axis: int):
+        return self.paddle.concat(tensors, axis=axis)
+
+    def add_axis(self, x, new_position):
+        return x.unsqueeze(new_position)
+
+    def is_float_type(self, x):
+        return x.dtype in [self.paddle.float16, self.paddle.float32, self.paddle.float64]
+
+    def layers(self):
+        from .layers import paddle
+        return paddle
+
+    def einsum(self, pattern, *x):
+        return self.paddle.einsum(pattern, *x)
+
+    def shape(self, x):
+        return tuple(x.shape)
```

### Comparing `einops-0.6.0/einops/_torch_specific.py` & `einops-0.6.1/einops/_torch_specific.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Unfortunately, torch's jit scripting mechanism isn't strong enough,
 and to have scripting supported at least for layers,
 a number of changes is required, and this layer helps.
 
 Importantly, whole lib is designed so that you can't use it
 """
-
+import warnings
 from typing import Dict, List
 
 import torch
 from einops.einops import TransformRecipe, _reconstruct_from_shape_uncached
 
 
 class TorchJitBackend:
@@ -78,7 +78,25 @@
     tensor = backend.reshape(tensor, init_shapes)
     if len(reduced_axes) > 0:
         tensor = backend.reduce(tensor, operation=reduction_type, reduced_axes=reduced_axes)
     tensor = backend.transpose(tensor, axes_reordering)
     if len(added_axes) > 0:
         tensor = backend.add_axes(tensor, n_axes=len(axes_reordering) + len(added_axes), pos2len=added_axes)
     return backend.reshape(tensor, final_shapes)
+
+
+def allow_ops_in_compiled_graph():
+    try:
+        from torch._dynamo import allow_in_graph
+    except ImportError:
+        from warnings import warn
+        warnings.warn("allow_ops_in_compiled_graph failed to import torch: ensure pytorch >=2.0", ImportWarning)
+
+    from .einops import rearrange, reduce, repeat, einsum
+    from .packing import pack, unpack
+
+    allow_in_graph(rearrange)
+    allow_in_graph(reduce)
+    allow_in_graph(repeat)
+    allow_in_graph(einsum)
+    allow_in_graph(pack)
+    allow_in_graph(unpack)
```

### Comparing `einops-0.6.0/einops/einops.py` & `einops-0.6.1/einops/einops.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
     # Subtracting per-image mean for each channel
     >>> y = x - reduce(x, 'b c h w -> b c () ()', 'mean')
 
     ```
 
     Parameters:
-        tensor: tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch, mxnet.ndarray).
+        tensor: tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch).
             list of tensors is also accepted, those should be of the same type and shape
         pattern: string, reduction pattern
         reduction: one of available reductions ('min', 'max', 'sum', 'mean', 'prod'), case-sensitive
             alternatively, a callable f(tensor, reduced_axes) -> tensor can be provided.
             This allows using various reductions, examples: np.max, tf.reduce_logsumexp, torch.var, etc.
         axes_lengths: any additional specifications for dimensions
 
@@ -463,15 +463,15 @@
 
     ```
 
     When composing axes, C-order enumeration used (consecutive elements have different last axis)
     Find more examples in einops tutorial.
 
     Parameters:
-        tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch, mxnet.ndarray).
+        tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch).
                 list of tensors is also accepted, those should be of the same type and shape
         pattern: string, rearrangement pattern
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         tensor of the same type as input. If possible, a view to the original tensor is returned.
 
@@ -517,15 +517,15 @@
 
     ```
 
     When composing axes, C-order enumeration used (consecutive elements have different last axis)
     Find more examples in einops tutorial.
 
     Parameters:
-        tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch, mxnet.ndarray).
+        tensor: tensor of any supported library (e.g. numpy.ndarray, tensorflow, pytorch).
             list of tensors is also accepted, those should be of the same type and shape
         pattern: string, rearrangement pattern
         axes_lengths: any additional specifications for dimensions
 
     Returns:
         Tensor of the same type as input. If possible, a view to the original tensor is returned.
 
@@ -611,15 +611,15 @@
 
 # to avoid importing numpy
 np_ndarray = Any
 
 
 def asnumpy(tensor) -> np_ndarray:
     """
-    Convert a tensor of an imperative framework (i.e. numpy/cupy/torch/gluon/etc.) to `numpy.ndarray`
+    Convert a tensor of an imperative framework (i.e. numpy/cupy/torch/jax/etc.) to `numpy.ndarray`
 
     Parameters:
         tensor: tensor of any of known imperative framework
 
     Returns:
         `numpy.ndarray`, converted to numpy
     """
```

### Comparing `einops-0.6.0/einops/packing.py` & `einops-0.6.1/einops/packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/parsing.py` & `einops-0.6.1/einops/parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/experimental/data_api_packing.py` & `einops-0.6.1/einops/experimental/data_api_packing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/experimental/indexing.py` & `einops-0.6.1/einops/experimental/indexing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/__init__.py` & `einops-0.6.1/einops/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/_einmix.py` & `einops-0.6.1/einops/layers/_einmix.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/chainer.py` & `einops-0.6.1/einops/layers/chainer.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/flax.py` & `einops-0.6.1/einops/layers/flax.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/gluon.py` & `einops-0.6.1/einops/layers/gluon.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/oneflow.py` & `einops-0.6.1/einops/layers/oneflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/tensorflow.py` & `einops-0.6.1/einops/layers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/einops/layers/torch.py` & `einops-0.6.1/einops/layers/torch.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/scripts/convert_readme.py` & `einops-0.6.1/scripts/convert_readme.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/tests/test_einsum.py` & `einops-0.6.1/tests/test_einsum.py`

 * *Files 14% similar despite different names*

```diff
@@ -163,28 +163,28 @@
         (()),
     ),
 ]
 
 
 def test_layer():
     for backend in collect_test_backends(layers=True, symbolic=False):
-        if backend.framework_name in ['tensorflow', 'torch', 'chainer', 'oneflow']:
+        if backend.framework_name in ['tensorflow', 'torch', 'chainer', 'oneflow', 'paddle']:
             layer_type = backend.layers().EinMix
             for args, in_shape, out_shape in test_layer_cases:
                 layer = args(layer_type)
                 print('Running', layer.einsum_pattern, 'for', backend.framework_name)
                 input = np.random.uniform(size=in_shape).astype('float32')
                 input_framework = backend.from_numpy(input)
                 output_framework = layer(input_framework)
                 output = backend.to_numpy(output_framework)
                 assert output.shape == out_shape
 
 
 valid_backends_functional = ['tensorflow', 'torch', 'jax', 'numpy',
-                             'chainer', 'oneflow', 'cupy', 'tensorflow.keras']
+                             'chainer', 'oneflow', 'cupy', 'tensorflow.keras', 'paddle']
 
 def test_functional():
     # Functional tests:
     backends = filter(lambda x: x.framework_name in valid_backends_functional,
                       collect_test_backends())
     for backend in backends:
         for einops_pattern, true_pattern, in_shapes, out_shape in test_functional_cases:
@@ -210,15 +210,15 @@
                 # Actually run einsum:
                 if do_manual_call:
                     out_array = backend.einsum(predicted_pattern, *in_arrays_framework)
                 else:
                     out_array = einsum(*in_arrays_framework, einops_pattern)
 
                 # Check shape:
-                if out_array.shape != out_shape:
+                if tuple(out_array.shape) != out_shape:
                     raise ValueError(
                         f"Expected output shape {out_shape} but got {out_array.shape}"
                     )
 
                 # Check values:
                 true_out_array = np.einsum(true_pattern, *in_arrays)
                 predicted_out_array = backend.to_numpy(out_array)
@@ -348,27 +348,7 @@
         )
     with pytest.raises(ValueError, match="^`einops.einsum` takes"):
         einsum(
             create_tensor(5, 1),
         )
 
     # TODO: Include check for giving normal einsum pattern rather than einops.
-
-# mxnet/gluon do not support einsum without changing to numpy. which doesn't work with the rest
-# in future, after gluon migrated to a new codebase, all testing code will be moved to a new setup
-# def test_gluon():
-#     for backend in collect_test_backends(layers=True, symbolic=False):
-#         if backend.framework_name == 'mxnet.ndarray':
-#             import mxnet as mx
-#
-#             mx.npx.set_np()
-#             layer_type = backend.layers().EinMix
-#
-#             for args, in_shape, out_shape in test_cases:
-#                 layer = args(layer_type)
-#                 # gluon requires initialization
-#                 layer.initialize()
-#                 input = np.random.uniform(size=in_shape).astype('float32')
-#                 input_framework = mx.np.array(input)
-#                 output_framework = layer(input_framework)
-#                 output = backend.to_numpy(output_framework)
-#                 assert output.shape == out_shape
```

### Comparing `einops-0.6.0/tests/test_examples.py` & `einops-0.6.1/tests/test_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 import numpy
+import pytest
 
 from einops import rearrange, parse_shape, reduce
-from tests import collect_test_backends
+from tests import is_backend_tested
 from tests.test_ops import imp_op_backends
 
 
 def test_rearrange_examples():
     def test1(x):
         # transpose
         y = rearrange(x, 'b c h w -> b h w c')
-        assert y.shape == (10, 30, 40, 20)
+        assert tuple(y.shape) == (10, 30, 40, 20)
         return y
 
     def test2(x):
         # view / reshape
         y = rearrange(x, 'b c h w -> b (c h w)')
-        assert y.shape == (10, 20 * 30 * 40)
+        assert tuple(y.shape) == (10, 20 * 30 * 40)
         return y
 
     def test3(x):
         # depth-to-space
         y = rearrange(x, 'b (c h1 w1) h w -> b c (h h1) (w w1)', h1=2, w1=2)
-        assert y.shape == (10, 5, 30 * 2, 40 * 2)
+        assert tuple(y.shape) == (10, 5, 30 * 2, 40 * 2)
         return y
 
     def test4(x):
         # space-to-depth
         y = rearrange(x, 'b c (h h1) (w w1) -> b (h1 w1 c) h w', h1=2, w1=2)
-        assert y.shape == (10, 20 * 4, 30 // 2, 40 // 2)
+        assert tuple(y.shape) == (10, 20 * 4, 30 // 2, 40 // 2)
         return y
 
     def test5(x):
         # simple transposition
         y = rearrange(x, 'b1 sound b2 letter -> b1 b2 sound letter')
-        assert y.shape == (10, 30, 20, 40)
+        assert tuple(y.shape) == (10, 30, 20, 40)
         return y
 
     def test6(x):
         # parsing parameters
         t = rearrange(x, 'b c h w -> (b h w) c')
         t = t[:, ::2]  # replacement for dot-product, just changes size of second axis
-        assert t.shape == (10 * 30 * 40, 10)
+        assert tuple(t.shape) == (10 * 30 * 40, 10)
 
         y = rearrange(t, '(b h w) c2 -> b c2 h w', **parse_shape(x, 'b _ h w'))
-        assert y.shape == (10, 10, 30, 40)
+        assert tuple(y.shape) == (10, 10, 30, 40)
         return y
 
     def test7(x):
         # split of embedding into groups
         y1, y2 = rearrange(x, 'b (c g) h w -> g b c h w', g=2)
-        assert y1.shape == (10, 10, 30, 40)
-        assert y2.shape == (10, 10, 30, 40)
+        assert tuple(y1.shape) == (10, 10, 30, 40)
+        assert tuple(y2.shape) == (10, 10, 30, 40)
         return y1 + y2  # only one tensor is expected in output
 
     def test8(x):
         # max-pooling
         y = reduce(x, 'b c (h h1) (w w1) -> b c h w', reduction='max', h1=2, w1=2)
-        assert y.shape == (10, 20, 30 // 2, 40 // 2)
+        assert tuple(y.shape) == (10, 20, 30 // 2, 40 // 2)
         return y
 
     def test9(x):
         # squeeze - unsqueeze
         y = reduce(x, 'b c h w -> b c () ()', reduction='max')
-        assert y.shape == (10, 20, 1, 1)
+        assert tuple(y.shape) == (10, 20, 1, 1)
         y = rearrange(y, 'b c () () -> c b')
-        assert y.shape == (20, 10)
+        assert tuple(y.shape) == (20, 10)
         return y
 
     def test10(x):
         # stack
         tensors = list(x + 0)  # 0 is needed https://github.com/tensorflow/tensorflow/issues/23185
         tensors = rearrange(tensors, 'b c h w -> b h w c')
-        assert tensors.shape == (10, 30, 40, 20)
+        assert tuple(tensors.shape) == (10, 30, 40, 20)
         return tensors
 
     def test11(x):
         # concatenate
         tensors = list(x + 0)  # 0 is needed https://github.com/tensorflow/tensorflow/issues/23185
         tensors = rearrange(tensors, 'b c h w -> h (b w) c')
-        assert tensors.shape == (30, 10 * 40, 20)
+        assert tuple(tensors.shape) == (30, 10 * 40, 20)
         return tensors
 
     def shufflenet(x, convolve, c1, c2):
         # shufflenet reordering example
         x = convolve(x)
         x = rearrange(x, 'b (c1 c2) h w-> b (c2 c1) h w', c1=c1, c2=c2)
         x = convolve(x)
@@ -175,18 +176,18 @@
         y = rearrange(y, 'i ... (j alpha) -> ... j (alpha i)', alpha=alpha, i=i)
         y = y @ rearrange(G, 'i j alpha beta -> (alpha i) (j beta)')
     y3 = y.reshape(-1)
     assert numpy.allclose(y1, y3)
 
 
 def test_pytorch_yolo_fragment():
-    if not any(b.framework_name == 'torch' for b in collect_test_backends(symbolic=False, layers=False)):
-        return
-    import torch
+    if not is_backend_tested('torch'):
+        pytest.skip()
 
+    import torch
     def old_way(input, num_classes, num_anchors, anchors, stride_h, stride_w):
         # https://github.com/BobLiu20/YOLOv3_PyTorch/blob/c6b483743598b5f64d520d81e7e5f47ba936d4c9/nets/yolo_loss.py#L28-L44
         bs = input.size(0)
         in_h = input.size(2)
         in_w = input.size(3)
         scaled_anchors = [(a_w / stride_w, a_h / stride_h) for a_w, a_h in anchors]
```

### Comparing `einops-0.6.0/tests/test_layers.py` & `einops-0.6.1/tests/test_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,86 @@
 import pickle
 import tempfile
 from collections import namedtuple
 
 import numpy
-import torch.jit
+import pytest
 
 from einops import rearrange, reduce
 from einops.einops import _reductions
-from . import collect_test_backends
+from . import collect_test_backends, is_backend_tested
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
-testcase = namedtuple('testcase', ['pattern', 'axes_lengths', 'input_shape', 'wrong_shapes'])
+testcase = namedtuple("testcase", ["pattern", "axes_lengths", "input_shape", "wrong_shapes"])
 
 rearrangement_patterns = [
-    testcase('b c h w -> b (c h w)', dict(c=20), (10, 20, 30, 40),
-             [(), (10,), (10, 10, 10), (10, 21, 30, 40), [1, 20, 1, 1, 1]]),
-    testcase('b c (h1 h2) (w1 w2) -> b (c h2 w2) h1 w1', dict(h2=2, w2=2), (10, 20, 30, 40),
-             [(), (1, 1, 1, 1), (1, 10, 3), ()]),
-    testcase('b ... c -> c b ...', dict(b=10), (10, 20, 30),
-             [(), (10,), (5, 10)]),
+    testcase(
+        "b c h w -> b (c h w)",
+        dict(c=20),
+        (10, 20, 30, 40),
+        [(), (10,), (10, 10, 10), (10, 21, 30, 40), [1, 20, 1, 1, 1]],
+    ),
+    testcase(
+        "b c (h1 h2) (w1 w2) -> b (c h2 w2) h1 w1",
+        dict(h2=2, w2=2),
+        (10, 20, 30, 40),
+        [(), (1, 1, 1, 1), (1, 10, 3), ()],
+    ),
+    testcase(
+        "b ... c -> c b ...",
+        dict(b=10),
+        (10, 20, 30),
+        [(), (10,), (5, 10)],
+    ),
 ]
 
 
 def test_rearrange_imperative():
     for backend in collect_test_backends(symbolic=False, layers=True):
-        print('Test layer for ', backend.framework_name)
+        print("Test layer for ", backend.framework_name)
 
         for pattern, axes_lengths, input_shape, wrong_shapes in rearrangement_patterns:
-            x = numpy.arange(numpy.prod(input_shape), dtype='float32').reshape(input_shape)
+            x = numpy.arange(numpy.prod(input_shape), dtype="float32").reshape(input_shape)
             result_numpy = rearrange(x, pattern, **axes_lengths)
             layer = backend.layers().Rearrange(pattern, **axes_lengths)
             for shape in wrong_shapes:
                 try:
-                    layer(backend.from_numpy(numpy.zeros(shape, dtype='float32')))
+                    layer(backend.from_numpy(numpy.zeros(shape, dtype="float32")))
                 except:
                     pass
                 else:
-                    raise AssertionError('Failure expected')
+                    raise AssertionError("Failure expected")
 
             # simple pickling / unpickling
             layer2 = pickle.loads(pickle.dumps(layer))
             result1 = backend.to_numpy(layer(backend.from_numpy(x)))
             result2 = backend.to_numpy(layer2(backend.from_numpy(x)))
             assert numpy.allclose(result_numpy, result1)
             assert numpy.allclose(result1, result2)
 
-            just_sum = backend.layers().Reduce('...->', reduction='sum')
+            just_sum = backend.layers().Reduce("...->", reduction="sum")
 
-            if 'mxnet' in backend.framework_name:
-                with backend.mx.autograd.record():
-                    variable = backend.from_numpy(x)
-                    result = just_sum(layer(variable))
-            else:
-                variable = backend.from_numpy(x)
-                result = just_sum(layer(variable))
+            variable = backend.from_numpy(x)
+            result = just_sum(layer(variable))
 
             result.backward()
             assert numpy.allclose(backend.to_numpy(variable.grad), 1)
 
 
 def test_rearrange_symbolic():
     for backend in collect_test_backends(symbolic=True, layers=True):
-        print('Test layer for ', backend.framework_name)
+        print("Test layer for ", backend.framework_name)
 
         for pattern, axes_lengths, input_shape, wrong_shapes in rearrangement_patterns:
-            x = numpy.arange(numpy.prod(input_shape), dtype='float32').reshape(input_shape)
+            x = numpy.arange(numpy.prod(input_shape), dtype="float32").reshape(input_shape)
             result_numpy = rearrange(x, pattern, **axes_lengths)
             layer = backend.layers().Rearrange(pattern, **axes_lengths)
-            shapes = [input_shape]
-            if 'mxnet' not in backend.framework_name:
-                shapes.append([None] * len(input_shape))
+            input_shape_of_nones = [None] * len(input_shape)
+            shapes = [input_shape, input_shape_of_nones]
 
             for shape in shapes:
                 symbol = backend.create_symbol(shape)
                 eval_inputs = [(symbol, x)]
 
                 result_symbol1 = layer(symbol)
                 result1 = backend.eval_symbol(result_symbol1, eval_inputs)
@@ -82,90 +88,81 @@
 
                 layer2 = pickle.loads(pickle.dumps(layer))
                 result_symbol2 = layer2(symbol)
                 result2 = backend.eval_symbol(result_symbol2, eval_inputs)
                 assert numpy.allclose(result1, result2)
 
                 # now testing back-propagation
-                just_sum = backend.layers().Reduce('...->', reduction='sum')
+                just_sum = backend.layers().Reduce("...->", reduction="sum")
 
                 result_sum1 = backend.eval_symbol(just_sum(result_symbol1), eval_inputs)
                 result_sum2 = numpy.sum(x)
 
                 assert numpy.allclose(result_sum1, result_sum2)
 
 
 reduction_patterns = rearrangement_patterns + [
-    testcase('b c h w -> b ()', dict(b=10), (10, 20, 30, 40),
-             [(10,), (10, 20, 30)]),
-    testcase('b c (h1 h2) (w1 w2) -> b c h1 w1', dict(h1=15, h2=2, w2=2), (10, 20, 30, 40),
-             [(10, 20, 31, 40)]),
-    testcase('b ... c -> b', dict(b=10), (10, 20, 30, 40),
-             [(10,), (11, 10)]),
+    testcase("b c h w -> b ()", dict(b=10), (10, 20, 30, 40), [(10,), (10, 20, 30)]),
+    testcase("b c (h1 h2) (w1 w2) -> b c h1 w1", dict(h1=15, h2=2, w2=2), (10, 20, 30, 40), [(10, 20, 31, 40)]),
+    testcase("b ... c -> b", dict(b=10), (10, 20, 30, 40), [(10,), (11, 10)]),
 ]
 
 
 def test_reduce_imperative():
     for backend in collect_test_backends(symbolic=False, layers=True):
-        print('Test layer for ', backend.framework_name)
+        print("Test layer for ", backend.framework_name)
         for reduction in _reductions:
             for pattern, axes_lengths, input_shape, wrong_shapes in reduction_patterns:
                 print(backend, reduction, pattern, axes_lengths, input_shape, wrong_shapes)
-                x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype='float32').reshape(input_shape)
+                x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype="float32").reshape(input_shape)
                 x /= x.mean()
                 result_numpy = reduce(x, pattern, reduction, **axes_lengths)
                 layer = backend.layers().Reduce(pattern, reduction, **axes_lengths)
                 for shape in wrong_shapes:
                     try:
-                        layer(backend.from_numpy(numpy.zeros(shape, dtype='float32')))
+                        layer(backend.from_numpy(numpy.zeros(shape, dtype="float32")))
                     except:
                         pass
                     else:
-                        raise AssertionError('Failure expected')
+                        raise AssertionError("Failure expected")
 
                 # simple pickling / unpickling
                 layer2 = pickle.loads(pickle.dumps(layer))
                 result1 = backend.to_numpy(layer(backend.from_numpy(x)))
                 result2 = backend.to_numpy(layer2(backend.from_numpy(x)))
                 assert numpy.allclose(result_numpy, result1)
                 assert numpy.allclose(result1, result2)
 
-                just_sum = backend.layers().Reduce('...->', reduction='sum')
+                just_sum = backend.layers().Reduce("...->", reduction="sum")
 
-                if 'mxnet' in backend.framework_name:
-                    with backend.mx.autograd.record():
-                        variable = backend.from_numpy(x)
-                        result = just_sum(layer(variable))
-                else:
-                    variable = backend.from_numpy(x)
-                    result = just_sum(layer(variable))
+                variable = backend.from_numpy(x)
+                result = just_sum(layer(variable))
 
                 result.backward()
                 grad = backend.to_numpy(variable.grad)
-                if reduction == 'sum':
+                if reduction == "sum":
                     assert numpy.allclose(grad, 1)
-                if reduction == 'mean':
+                if reduction == "mean":
                     assert numpy.allclose(grad, grad.min())
-                if reduction in ['max', 'min']:
+                if reduction in ["max", "min"]:
                     assert numpy.all(numpy.in1d(grad, [0, 1]))
                     assert numpy.sum(grad) > 0.5
 
 
 def test_reduce_symbolic():
     for backend in collect_test_backends(symbolic=True, layers=True):
-        print('Test layer for ', backend.framework_name)
+        print("Test layer for ", backend.framework_name)
         for reduction in _reductions:
             for pattern, axes_lengths, input_shape, wrong_shapes in reduction_patterns:
-                x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype='float32').reshape(input_shape)
+                x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype="float32").reshape(input_shape)
                 x /= x.mean()
                 result_numpy = reduce(x, pattern, reduction, **axes_lengths)
                 layer = backend.layers().Reduce(pattern, reduction, **axes_lengths)
-                shapes = [input_shape]
-                if 'mxnet' not in backend.framework_name:
-                    shapes.append([None] * len(input_shape))
+                input_shape_of_nones = [None] * len(input_shape)
+                shapes = [input_shape, input_shape_of_nones]
 
                 for shape in shapes:
                     symbol = backend.create_symbol(shape)
                     eval_inputs = [(symbol, x)]
 
                     result_symbol1 = layer(symbol)
                     result1 = backend.eval_symbol(result_symbol1, eval_inputs)
@@ -174,38 +171,46 @@
                     layer2 = pickle.loads(pickle.dumps(layer))
                     result_symbol2 = layer2(symbol)
                     result2 = backend.eval_symbol(result_symbol2, eval_inputs)
                     assert numpy.allclose(result1, result2)
 
 
 def create_torch_model(use_reduce=False, add_scripted_layer=False):
-    from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
-    from einops.layers.torch import Rearrange, Reduce, EinMix
-    return Sequential(
-        Conv2d(3, 6, kernel_size=(5, 5)),
-        Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2) if use_reduce else MaxPool2d(kernel_size=2),
-        Conv2d(6, 16, kernel_size=(5, 5)),
-        Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-        torch.jit.script(Rearrange('b c h w -> b (c h w)'))
-        if add_scripted_layer else Rearrange('b c h w -> b (c h w)'),
-        Linear(16 * 5 * 5, 120),
-        ReLU(),
-        Linear(120, 84),
-        ReLU(),
-        EinMix('b c1 -> (b c2)', weight_shape='c1 c2', bias_shape='c2', c1=84, c2=84),
-        EinMix('(b c2) -> b c3', weight_shape='c2 c3', bias_shape='c3', c2=84, c3=84),
-        Linear(84, 10),
-    )
+    if not is_backend_tested("torch"):
+        pytest.skip()
+    else:
+        from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU
+        from einops.layers.torch import Rearrange, Reduce, EinMix
+        import torch.jit
+
+        return Sequential(
+            Conv2d(3, 6, kernel_size=(5, 5)),
+            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2) if use_reduce else MaxPool2d(kernel_size=2),
+            Conv2d(6, 16, kernel_size=(5, 5)),
+            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+            torch.jit.script(Rearrange("b c h w -> b (c h w)"))
+            if add_scripted_layer
+            else Rearrange("b c h w -> b (c h w)"),
+            Linear(16 * 5 * 5, 120),
+            ReLU(),
+            Linear(120, 84),
+            ReLU(),
+            EinMix("b c1 -> (b c2)", weight_shape="c1 c2", bias_shape="c2", c1=84, c2=84),
+            EinMix("(b c2) -> b c3", weight_shape="c2 c3", bias_shape="c3", c2=84, c3=84),
+            Linear(84, 10),
+        )
 
 
 def test_torch_layer():
-    has_torch = any(backend.framework_name == 'torch' for backend in collect_test_backends(symbolic=False, layers=True))
-    if has_torch:
+    if not is_backend_tested("torch"):
+        pytest.skip()
+    else:
         # checked that torch present
         import torch
+        import torch.jit
 
         model1 = create_torch_model(use_reduce=True)
         model2 = create_torch_model(use_reduce=False)
         input = torch.randn([10, 3, 32, 32])
         # random models have different predictions
         assert not torch.allclose(model1(input), model2(input))
         model2.load_state_dict(pickle.loads(pickle.dumps(model1.state_dict())))
@@ -218,209 +223,213 @@
 
         model4 = torch.jit.trace(model2, example_inputs=input)
         torch.testing.assert_close(model1(input), model4(input), atol=1e-3, rtol=1e-3)
         torch.testing.assert_close(model1(input + 1), model4(input + 1), atol=1e-3, rtol=1e-3)
 
 
 def test_torch_layers_scripting():
-    import torch
-    for script_layer in [False, True]:
-        model1 = create_torch_model(use_reduce=True, add_scripted_layer=script_layer)
-        model2 = torch.jit.script(model1)
-        input = torch.randn([10, 3, 32, 32])
+    if not is_backend_tested("torch"):
+        pytest.skip()
+    else:
+        import torch
 
-        torch.testing.assert_close(model1(input), model2(input), atol=1e-3, rtol=1e-3)
+        for script_layer in [False, True]:
+            model1 = create_torch_model(use_reduce=True, add_scripted_layer=script_layer)
+            model2 = torch.jit.script(model1)
+            input = torch.randn([10, 3, 32, 32])
 
+            torch.testing.assert_close(model1(input), model2(input), atol=1e-3, rtol=1e-3)
 
-def test_keras_layer():
-    if any(backend.framework_name == 'tensorflow.keras' for backend in collect_test_backends(symbolic=True, layers=True)):
-        # checked that keras present
 
+def test_keras_layer():
+    if not is_backend_tested("tensorflow"):
+        pytest.skip()
+    else:
         import tensorflow as tf
         from tensorflow.keras.models import Sequential
         from tensorflow.keras.layers import Conv2D as Conv2d, Dense as Linear, ReLU
         from einops.layers.keras import Rearrange, Reduce, EinMix, keras_custom_objects
 
         def create_keras_model():
-            return Sequential([
-                Conv2d(6, kernel_size=5, input_shape=[32, 32, 3]),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-                Conv2d(16, kernel_size=5),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-                Rearrange('b c h w -> b (c h w)'),
-                Linear(120),
-                ReLU(),
-                Linear(84),
-                ReLU(),
-                EinMix('b c1 -> (b c2)', weight_shape='c1 c2', bias_shape='c2', c1=84, c2=84),
-                EinMix('(b c2) -> b c3', weight_shape='c2 c3', bias_shape='c3', c2=84, c3=84),
-                Linear(10),
-            ])
+            return Sequential(
+                [
+                    Conv2d(6, kernel_size=5, input_shape=[32, 32, 3]),
+                    Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+                    Conv2d(16, kernel_size=5),
+                    Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+                    Rearrange("b c h w -> b (c h w)"),
+                    Linear(120),
+                    ReLU(),
+                    Linear(84),
+                    ReLU(),
+                    EinMix("b c1 -> (b c2)", weight_shape="c1 c2", bias_shape="c2", c1=84, c2=84),
+                    EinMix("(b c2) -> b c3", weight_shape="c2 c3", bias_shape="c3", c2=84, c3=84),
+                    Linear(10),
+                ]
+            )
 
         model1 = create_keras_model()
         model2 = create_keras_model()
-        input = numpy.random.normal(size=[10, 32, 32, 3]).astype('float32')
+        input = numpy.random.normal(size=[10, 32, 32, 3]).astype("float32")
         assert not numpy.allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
 
         # get some temp filename
-        with tempfile.NamedTemporaryFile(mode='r+b') as f:
+        with tempfile.NamedTemporaryFile(mode="r+b") as f:
             tmp_filename = f.name
         # save arch + weights
-        print('temp_path_keras1', tmp_filename)
+        print("temp_path_keras1", tmp_filename)
         tf.keras.models.save_model(model1, tmp_filename)
         model3 = tf.keras.models.load_model(tmp_filename, custom_objects=keras_custom_objects)
         assert numpy.allclose(model1.predict_on_batch(input), model3.predict_on_batch(input))
 
         # save arch as json
         model4 = tf.keras.models.model_from_json(model1.to_json(), custom_objects=keras_custom_objects)
         model1.save_weights(tmp_filename)
         model4.load_weights(tmp_filename)
         model2.load_weights(tmp_filename)
         assert numpy.allclose(model1.predict_on_batch(input), model4.predict_on_batch(input))
         assert numpy.allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
 
 
-def test_gluon_layer():
-    gluon_is_present = any(
-        'mxnet' in backend.framework_name for backend in collect_test_backends(symbolic=False, layers=True)
-    )
-    if gluon_is_present:
-        # checked that gluon present
-        import mxnet
-        from mxnet.gluon.nn import HybridSequential, Dense, Conv2D, LeakyReLU
-        from einops.layers.gluon import Rearrange, Reduce, EinMix
-        from einops import asnumpy
-
-        def create_model():
-            model = HybridSequential()
-            layers = [
-                Conv2D(6, kernel_size=5),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-                Conv2D(16, kernel_size=5),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-                Rearrange('b c h w -> b (c h w)'),
-                Dense(120),
-                LeakyReLU(alpha=0.0),
-                Dense(84),
-                LeakyReLU(alpha=0.0),
-                Dense(10),
-            ]
-            for layer in layers:
-                model.add(layer)
-            model.initialize(mxnet.init.Xavier(), ctx=mxnet.cpu())
-            return model
-
-        model1 = create_model()
-        model2 = create_model()
-        x = mxnet.ndarray.random_normal(shape=[10, 3, 32, 32])
-        assert not numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
-
-        with tempfile.NamedTemporaryFile(mode='r+b') as fp:
-            model1.save_parameters(fp.name)
-            model2.load_parameters(fp.name)
-
-        assert numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
-
-        # testing with symbolic (NB with fixed dimensions!)
-        input = mxnet.sym.Variable('data', shape=x.shape)
-        json = model1(input).tojson()
-        model3 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
-        model4 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
-        model3.initialize(ctx=mxnet.cpu())
-        model3(x)
-
-        with tempfile.NamedTemporaryFile(mode='r+b') as fp:
-            model3.save_parameters(fp.name)
-            model4.load_parameters(fp.name)
-        assert numpy.allclose(asnumpy(model3(x)), asnumpy(model4(x)))
-
-        try:
-            model1.hybridize(static_alloc=True, static_shape=True)
-            model1(x)
-        except:
-            # hybridization is not supported
-            pass
+def _deprecated_check_gluon_layer():
+    # currently gluon is not tested, and will be removed
+    import mxnet
+    from mxnet.gluon.nn import HybridSequential, Dense, Conv2D, LeakyReLU
+    from einops.layers.gluon import Rearrange, Reduce, EinMix
+    from einops import asnumpy
+
+    def create_model():
+        model = HybridSequential()
+        layers = [
+            Conv2D(6, kernel_size=5),
+            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+            Conv2D(16, kernel_size=5),
+            Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+            Rearrange("b c h w -> b (c h w)"),
+            Dense(120),
+            LeakyReLU(alpha=0.0),
+            Dense(84),
+            LeakyReLU(alpha=0.0),
+            Dense(10),
+        ]
+        for layer in layers:
+            model.add(layer)
+        model.initialize(mxnet.init.Xavier(), ctx=mxnet.cpu())
+        return model
+
+    model1 = create_model()
+    model2 = create_model()
+    x = mxnet.ndarray.random_normal(shape=[10, 3, 32, 32])
+    assert not numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
+
+    with tempfile.NamedTemporaryFile(mode="r+b") as fp:
+        model1.save_parameters(fp.name)
+        model2.load_parameters(fp.name)
+
+    assert numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
+
+    # testing with symbolic (NB with fixed dimensions!)
+    input = mxnet.sym.Variable("data", shape=x.shape)
+    json = model1(input).tojson()
+    model3 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
+    model4 = mxnet.gluon.SymbolBlock(outputs=mxnet.sym.load_json(json), inputs=input)
+    model3.initialize(ctx=mxnet.cpu())
+    model3(x)
+
+    with tempfile.NamedTemporaryFile(mode="r+b") as fp:
+        model3.save_parameters(fp.name)
+        model4.load_parameters(fp.name)
+    assert numpy.allclose(asnumpy(model3(x)), asnumpy(model4(x)))
+
+    try:
+        model1.hybridize(static_alloc=True, static_shape=True)
+        model1(x)
+    except:
+        # hybridization is not supported
+        pass
 
 
 def test_chainer_layer():
     chainer_is_present = any(
-        'chainer' in backend.framework_name for backend in collect_test_backends(symbolic=False, layers=True)
+        "chainer" in backend.framework_name for backend in collect_test_backends(symbolic=False, layers=True)
     )
     if chainer_is_present:
         # checked that gluon present
         import chainer
         import chainer.links as L
         import chainer.functions as F
         from einops.layers.chainer import Rearrange, Reduce, EinMix
         from einops import asnumpy
         import numpy as np
 
         def create_model():
             return chainer.Sequential(
                 L.Convolution2D(3, 6, ksize=(5, 5)),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
+                Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
                 L.Convolution2D(6, 16, ksize=(5, 5)),
-                Reduce('b c (h h2) (w w2) -> b c h w', 'max', h2=2, w2=2),
-                Rearrange('b c h w -> b (c h w)'),
+                Reduce("b c (h h2) (w w2) -> b c h w", "max", h2=2, w2=2),
+                Rearrange("b c h w -> b (c h w)"),
                 L.Linear(16 * 5 * 5, 120),
                 L.Linear(120, 84),
                 F.relu,
-                EinMix('b c1 -> (b c2)', weight_shape='c1 c2', bias_shape='c2', c1=84, c2=84),
-                EinMix('(b c2) -> b c3', weight_shape='c2 c3', bias_shape='c3', c2=84, c3=84),
+                EinMix("b c1 -> (b c2)", weight_shape="c1 c2", bias_shape="c2", c1=84, c2=84),
+                EinMix("(b c2) -> b c3", weight_shape="c2 c3", bias_shape="c3", c2=84, c3=84),
                 L.Linear(84, 10),
             )
 
         model1 = create_model()
         model2 = create_model()
-        x = np.random.normal(size=[10, 3, 32, 32]).astype('float32')
+        x = np.random.normal(size=[10, 3, 32, 32]).astype("float32")
         x = chainer.Variable(x)
         assert not numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
 
         with tempfile.TemporaryDirectory() as dir:
-            filename = f'{dir}/file.npz'
+            filename = f"{dir}/file.npz"
             chainer.serializers.save_npz(filename, model1)
             chainer.serializers.load_npz(filename, model2)
 
         assert numpy.allclose(asnumpy(model1(x)), asnumpy(model2(x)))
 
 
 def test_flax_layers():
     """
     One-off simple tests for Flax layers.
     Unfortunately, Flax layers have a different interface from other layers.
     """
-    import jax
-    import jax.numpy as jnp
-
-    import flax
-    from flax import linen as nn
-    from einops.layers.flax import EinMix, Reduce, Rearrange
-
-    class NN(nn.Module):
-        @nn.compact
-        def __call__(self, x):
-            x = EinMix('b (h h2) (w w2) c -> b h w c_out', 'h2 w2 c c_out', 'c_out', sizes=dict(h2=2, w2=3, c=4, c_out=5) )(x)
-            x = Rearrange('b h w c -> b (w h c)', sizes=dict(c=5))(x)
-            x = Reduce('b hwc -> b', 'mean', dict(hwc=2 * 3 * 5))(x)
-            return x
-
-    model = NN()
-    fixed_input = jnp.ones([10, 2 * 2, 3 * 3, 4])
-    params = model.init(jax.random.PRNGKey(0), fixed_input)
-    eval_at_point = lambda params: jnp.linalg.norm(model.apply(params, fixed_input))
-
-    vandg = jax.value_and_grad(eval_at_point)
-    value0 = eval_at_point(params)
-    value1, grad1 = vandg(params)
-    assert jnp.allclose(value0, value1)
-
-    params2 = jax.tree_map(
-        lambda x1, x2: x1 - x2 * 0.001,
-        params, grad1
-    )
-
-    value2 = eval_at_point(params2)
-    assert value0 >= value2, (value0, value2)
-
-    # check serialization
-    fbytes = flax.serialization.to_bytes(params)
-    _loaded = flax.serialization.from_bytes(params, fbytes)
+    if not is_backend_tested("jax"):
+        pytest.skip()
+    else:
+        import jax
+        import jax.numpy as jnp
+
+        import flax
+        from flax import linen as nn
+        from einops.layers.flax import EinMix, Reduce, Rearrange
+
+        class NN(nn.Module):
+            @nn.compact
+            def __call__(self, x):
+                x = EinMix(
+                    "b (h h2) (w w2) c -> b h w c_out", "h2 w2 c c_out", "c_out", sizes=dict(h2=2, w2=3, c=4, c_out=5)
+                )(x)
+                x = Rearrange("b h w c -> b (w h c)", sizes=dict(c=5))(x)
+                x = Reduce("b hwc -> b", "mean", dict(hwc=2 * 3 * 5))(x)
+                return x
+
+        model = NN()
+        fixed_input = jnp.ones([10, 2 * 2, 3 * 3, 4])
+        params = model.init(jax.random.PRNGKey(0), fixed_input)
+        eval_at_point = lambda params: jnp.linalg.norm(model.apply(params, fixed_input))
+
+        vandg = jax.value_and_grad(eval_at_point)
+        value0 = eval_at_point(params)
+        value1, grad1 = vandg(params)
+        assert jnp.allclose(value0, value1)
+
+        params2 = jax.tree_map(lambda x1, x2: x1 - x2 * 0.001, params, grad1)
+
+        value2 = eval_at_point(params2)
+        assert value0 >= value2, (value0, value2)
+
+        # check serialization
+        fbytes = flax.serialization.to_bytes(params)
+        _loaded = flax.serialization.from_bytes(params, fbytes)
```

### Comparing `einops-0.6.0/tests/test_notebooks.py` & `einops-0.6.1/tests/test_notebooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,73 @@
 from typing import Dict
 
 from io import StringIO
 
-from tests import collect_test_backends
+from tests import parse_backends_to_test, is_backend_tested
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 from pathlib import Path
 import nbformat
+import pytest
 from nbconvert.preprocessors import ExecutePreprocessor
 
 
 def render_notebook(filename: Path, replacements: Dict[str, str]) -> str:
-    """ Takes path to the notebook, returns executed and rendered version
+    """Takes path to the notebook, returns executed and rendered version
     :param filename: notebook
     :param replacements: dictionary with text replacements done before executing
     :return: notebook, rendered as string
     """
-    with filename.open('r') as f:
+    with filename.open("r") as f:
         nb_as_str = f.read()
     for original, replacement in replacements.items():
         nb_as_str = nb_as_str.replace(original, replacement)
 
     nb = nbformat.read(StringIO(nb_as_str), nbformat.NO_CONVERT)
-    ep = ExecutePreprocessor(timeout=60, kernel_name='python3')
-    ep.preprocess(nb, {'metadata': {'path': str(filename.parent.absolute())}})
+    ep = ExecutePreprocessor(timeout=60, kernel_name="python3")
+    ep.preprocess(nb, {"metadata": {"path": str(filename.parent.absolute())}})
 
     result_as_stream = StringIO()
     nbformat.write(nb, result_as_stream)
     return result_as_stream.getvalue()
 
 
-def test_all_notebooks():
-    notebooks = Path(__file__).parent.with_name('docs').glob('*.ipynb')
-    for notebook in notebooks:
-        render_notebook(notebook, replacements={})
+def test_notebook_1():
+    [notebook] = Path(__file__).parent.with_name("docs").glob("1-*.ipynb")
+    render_notebook(notebook, replacements={})
+
+
+def test_notebook_2_with_all_backends():
+    [notebook] = Path(__file__).parent.with_name("docs").glob("2-*.ipynb")
+    backends = []
+    if is_backend_tested("torch"):
+        # notebook uses name pytorch
+        backends.append("pytorch")
+    if is_backend_tested("tensorflow"):
+        backends.append("tensorflow")
+    if is_backend_tested("chainer"):
+        backends.append("chainer")
 
+    if len(backends) == 0:
+        pytest.skip()
 
-def test_dl_notebook_with_all_backends():
-    notebook, = Path(__file__).parent.with_name('docs').glob('2-*.ipynb')
-    backends = ['chainer', 'gluon', 'pytorch']
-    if 'tensorflow' in collect_test_backends(symbolic=False, layers=False):
-        backends += ['tensorflow']
     for backend in backends:
-        print('Testing {} with backend {}'.format(notebook, backend))
+        print("Testing {} with backend {}".format(notebook, backend))
         replacements = {"flavour = 'pytorch'": "flavour = '{}'".format(backend)}
-        expected_string = 'selected {} backend'.format(backend)
+        expected_string = "selected {} backend".format(backend)
         result = render_notebook(notebook, replacements=replacements)
         assert expected_string in result
+
+
+def test_notebook_3():
+    [notebook] = Path(__file__).parent.with_name("docs").glob("3-*.ipynb")
+    if not is_backend_tested("torch"):
+        pytest.skip()
+    render_notebook(notebook, replacements={})
+
+
+def test_notebook_4():
+    [notebook] = Path(__file__).parent.with_name("docs").glob("4-*.ipynb")
+    if not is_backend_tested("torch"):
+        pytest.skip()
+    render_notebook(notebook, replacements={})
```

### Comparing `einops-0.6.0/tests/test_ops.py` & `einops-0.6.1/tests/test_ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,19 +79,14 @@
             return rearrange(x, pattern, **axes_lengths)
         else:
             return reduce(x, pattern, reduction, **axes_lengths)
 
     numpy_result = operation(numpy_input)
     check_equal = numpy.array_equal
     p_none_dimension = 0.5
-    if 'mxnet' in backend.framework_name:
-        # known bug in mxnet: it can't work with scalars - so use allclose instead
-        check_equal = numpy.allclose
-        # mxnet can't work unless shape is completely specified
-        p_none_dimension = 0
     if is_symbolic:
         symbol_shape = [d if numpy.random.random() >= p_none_dimension else None for d in numpy_input.shape]
         symbol = backend.create_symbol(shape=symbol_shape)
         result_symbol = operation(symbol)
         backend_result = backend.eval_symbol(result_symbol, [(symbol, numpy_input)])
     else:
         backend_result = operation(backend.from_numpy(numpy_input))
@@ -235,18 +230,15 @@
                  getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1, 2])],
                 ['a b c d e -> (e c a)', {},
                  getattr(input, reduction)(axis=(1, 3)).transpose(2, 1, 0).reshape([-1])],
                 ['(a a2) ... -> (a2 a) ...', dict(a2=1),
                  input],
             ]
             for pattern, axes_lengths, expected_numpy_result in test_cases:
-                shapes = [input.shape]
-                if backend.framework_name != 'mxnet.symbol':
-                    # mxnet can't handle non-specified shapes
-                    shapes.append([None for _ in input.shape])
+                shapes = [input.shape, [None for _ in input.shape]]
                 for shape in shapes:
                     sym = backend.create_symbol(shape)
                     result_sym = reduce(sym, pattern, reduction=reduction, **axes_lengths)
                     result = backend.eval_symbol(result_sym, [(sym, input)])
                     assert numpy.allclose(result, expected_numpy_result)
 
                 if True:
@@ -270,32 +262,34 @@
         print('Stress-testing reduction for ', backend.framework_name)
         for reduction in _reductions + ('rearrange',):
             dtype = 'int64'
             coincide = numpy.array_equal
             if reduction in ['mean', 'prod']:
                 dtype = 'float64'
                 coincide = numpy.allclose
-            for n_axes in range(6 if 'mxnet' in backend.framework_name else (7 if 'oneflow' in backend.framework_name else 11)):
+            max_dim = 11
+            if 'oneflow' in backend.framework_name:
+                max_dim = 7
+            if 'paddle' in backend.framework_name:
+                max_dim = 9
+            for n_axes in range(max_dim):
                 shape = numpy.random.randint(2, 4, size=n_axes)
                 permutation = numpy.random.permutation(n_axes)
                 skipped = 0 if reduction == 'rearrange' else numpy.random.randint(n_axes + 1)
                 left = ' '.join('x' + str(i) for i in range(n_axes))
                 right = ' '.join('x' + str(i) for i in permutation[skipped:])
                 pattern = left + '->' + right
                 x = numpy.arange(1, 1 + numpy.prod(shape), dtype=dtype).reshape(shape)
                 if reduction == 'prod':
                     x /= x.mean()  # to avoid overflows
                 result1 = reduce(x, pattern, reduction=reduction)
                 result2 = x.transpose(permutation)
                 if skipped > 0:
                     result2 = getattr(result2, reduction)(axis=tuple(range(skipped)))
                 assert coincide(result1, result2)
-                if n_axes == 0 and 'mxnet' in backend.framework_name:
-                    # known mxnet bug, can't attach gradients to scalar
-                    continue
                 check_op_against_numpy(backend, x, pattern, reduction=reduction, axes_lengths={}, is_symbolic=False)
 
 
 def test_reduction_with_callable_imperatives():
     x_numpy = numpy.arange(2 * 3 * 4 * 5 * 6).reshape([2, 3, 4, 5, 6]).astype('float32')
     x_numpy /= x_numpy.max()
 
@@ -348,17 +342,14 @@
             )
 
 
 def test_enumerating_directions():
     for backend in imp_op_backends:
         print('testing directions for', backend.framework_name)
         for shape in [[], [1], [1, 1, 1], [2, 3, 5, 7]]:
-            if backend.framework_name == 'mxnet.ndarray' and len(shape) == 0:
-                # known bug of mxnet
-                continue
             x = numpy.arange(numpy.prod(shape)).reshape(shape)
             axes1 = _enumerate_directions(x)
             axes2 = _enumerate_directions(backend.from_numpy(x))
             assert len(axes1) == len(axes2) == len(shape)
             for ax1, ax2 in zip(axes1, axes2):
                 ax2 = backend.to_numpy(ax2)
                 assert ax1.shape == ax2.shape
@@ -367,17 +358,14 @@
 
 def test_concatenations_and_stacking():
     for backend in imp_op_backends:
         print('testing shapes for ', backend.framework_name)
         for n_arrays in [1, 2, 5]:
             shapes = [[], [1], [1, 1], [2, 3, 5, 7], [1] * 6]
             for shape in shapes:
-                if backend.framework_name == 'mxnet.ndarray' and len(shape) == 0:
-                    # known bug of mxnet
-                    continue
                 arrays1 = [numpy.arange(i, i + numpy.prod(shape)).reshape(shape) for i in range(n_arrays)]
                 arrays2 = [backend.from_numpy(array) for array in arrays1]
                 result0 = numpy.asarray(arrays1)
                 result1 = rearrange(arrays1, '...->...')
                 result2 = rearrange(arrays2, '...->...')
                 assert numpy.array_equal(result0, result1)
                 assert numpy.array_equal(result1, backend.to_numpy(result2))
@@ -392,22 +380,20 @@
     for reduction in _reductions:
         x = numpy.arange(1, 1 + 2 * 3 * 4).reshape([2, 3, 4]).astype('float32')
         results = {}
         for backend in imp_op_backends:
             y0 = backend.from_numpy(x)
             if not hasattr(y0, 'grad'):
                 continue
-            if 'mxnet' in backend.framework_name:
-                backend.mx.autograd.set_recording(True)
+
             y1 = reduce(y0, 'a b c -> c a', reduction=reduction)
             y2 = reduce(y1, 'c a -> a c', reduction=reduction)
             y3 = reduce(y2, 'a (c1 c2) -> a', reduction=reduction, c1=2)
             y4 = reduce(y3, '... -> ', reduction=reduction)
-            if 'mxnet' in backend.framework_name:
-                backend.mx.autograd.set_recording(False)
+
             y4.backward()
             grad = backend.to_numpy(y0.grad)
             results[backend.framework_name] = grad
 
         print('comparing gradients for', results.keys())
         for name1, grad1 in results.items():
             for name2, grad2 in results.items():
```

### Comparing `einops-0.6.0/tests/test_other.py` & `einops-0.6.1/tests/test_other.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,206 +9,267 @@
 from parameterized import parameterized, parameterized_class
 
 import einops
 import einops.layers
 import einops.parsing
 from einops._backends import AbstractBackend
 from einops.einops import rearrange, parse_shape, _optimize_transformation
-from . import collect_test_backends
+from . import collect_test_backends, is_backend_tested
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 
 def test_doctests_examples():
     if sys.version_info >= (3, 6):
         # python 3.5 and lower do not keep ordered dictionaries
         testmod(einops.layers, raise_on_error=True, extraglobs=dict(np=numpy))
         testmod(einops.einops, raise_on_error=True, extraglobs=dict(np=numpy))
 
 
 def test_backends_installed():
     """
     This test will fail if some of backends are not installed or can't be imported
     Other tests will just work and only test installed backends.
     """
-    from . import skip_cupy, skip_oneflow
+    from . import parse_backends_to_test
+
+    backends_to_test = parse_backends_to_test()
     errors = []
     for backend_type in AbstractBackend.__subclasses__():
-        if skip_cupy and backend_type.framework_name == 'cupy':
-            continue
-        if skip_oneflow and backend_type.framework_name == 'oneflow':
+        if backend_type.framework_name not in backends_to_test:
             continue
         try:
             # instantiate
             backend_type()
         except Exception as e:
             errors.append(e)
     assert len(errors) == 0, errors
 
 
 def test_optimize_transformations_numpy():
-    print('Testing optimizations')
+    print("Testing optimizations")
     shapes = [[2] * n_dimensions for n_dimensions in range(14)]
     shapes += [[3] * n_dimensions for n_dimensions in range(6)]
     shapes += [[2, 3, 5, 7]]
     shapes += [[2, 3, 5, 7, 11, 17]]
 
     for shape in shapes:
         for attempt in range(5):
             n_dimensions = len(shape)
-            x = numpy.random.randint(0, 2 ** 12, size=shape).reshape([-1])
+            x = numpy.random.randint(0, 2**12, size=shape).reshape([-1])
             init_shape = shape[:]
             n_reduced = numpy.random.randint(0, n_dimensions + 1)
             reduced_axes = tuple(numpy.random.permutation(n_dimensions)[:n_reduced])
             axes_reordering = numpy.random.permutation(n_dimensions - n_reduced)
             final_shape = numpy.random.randint(0, 1024, size=333)  # just random
 
-            init_shape2, reduced_axes2, axes_reordering2, final_shape2 = combination2 = \
-                _optimize_transformation(init_shape, reduced_axes, axes_reordering, final_shape)
+            init_shape2, reduced_axes2, axes_reordering2, final_shape2 = combination2 = _optimize_transformation(
+                init_shape, reduced_axes, axes_reordering, final_shape
+            )
 
             assert numpy.array_equal(final_shape, final_shape2)
             result1 = x.reshape(init_shape).sum(axis=reduced_axes).transpose(axes_reordering).reshape([-1])
             result2 = x.reshape(init_shape2).sum(axis=reduced_axes2).transpose(axes_reordering2).reshape([-1])
             assert numpy.array_equal(result1, result2)
 
             # testing we can't optimize this formula again
             combination3 = _optimize_transformation(*combination2)
             for a, b in zip(combination2, combination3):
                 assert numpy.array_equal(a, b)
 
 
-_IMPERATIVE_BACKENDS = [{"backend": backend} for backend in
-                        (collect_test_backends(symbolic=False, layers=False) +
-                         collect_test_backends(symbolic=False, layers=True))]
+_IMPERATIVE_BACKENDS = [
+    {"backend": backend}
+    for backend in (
+        collect_test_backends(symbolic=False, layers=False) + collect_test_backends(symbolic=False, layers=True)
+    )
+]
 
 
 @parameterized_class(_IMPERATIVE_BACKENDS)
 class TestParseShapeImperative(unittest.TestCase):
+    backend: AbstractBackend
+
     def setUp(self):
         self.x = numpy.zeros([10, 20, 30, 40])
 
     def test_parse_shape_imperative(self):
-        print('Shape parsing for ', self.backend.framework_name)
-        parsed1 = parse_shape(self.x, 'a b c d')
-        parsed2 = parse_shape(self.backend.from_numpy(self.x), 'a b c d')
+        print("Shape parsing for ", self.backend.framework_name)
+        parsed1 = parse_shape(self.x, "a b c d")
+        parsed2 = parse_shape(self.backend.from_numpy(self.x), "a b c d")
         assert parsed1 == parsed2 == dict(a=10, b=20, c=30, d=40)
         assert parsed1 != dict(a=1, b=20, c=30, d=40) != parsed2
 
     def test_underscore(self):
-        parsed1 = parse_shape(self.x, '_ _ _ _')
-        parsed2 = parse_shape(self.backend.from_numpy(self.x), '_ _ _ _')
+        parsed1 = parse_shape(self.x, "_ _ _ _")
+        parsed2 = parse_shape(self.backend.from_numpy(self.x), "_ _ _ _")
         assert parsed1 == parsed2 == dict()
 
     def test_underscore_one(self):
-        parsed1 = parse_shape(self.x, '_ _ _ hello')
-        parsed2 = parse_shape(self.backend.from_numpy(self.x), '_ _ _ hello')
+        parsed1 = parse_shape(self.x, "_ _ _ hello")
+        parsed2 = parse_shape(self.backend.from_numpy(self.x), "_ _ _ hello")
         assert parsed1 == parsed2 == dict(hello=40)
 
     def test_underscore_several(self):
-        parsed1 = parse_shape(self.x, '_ _ a1 a1a111a')
-        parsed2 = parse_shape(self.backend.from_numpy(self.x), '_ _ a1 a1a111a')
+        parsed1 = parse_shape(self.x, "_ _ a1 a1a111a")
+        parsed2 = parse_shape(self.backend.from_numpy(self.x), "_ _ a1 a1a111a")
         assert parsed1 == parsed2 == dict(a1=30, a1a111a=40)
 
     def test_repeating(self):
         with pytest.raises(einops.EinopsError):
-            parse_shape(self.x, 'a a b b')
+            parse_shape(self.x, "a a b b")
 
         with pytest.raises(einops.EinopsError):
-            parse_shape(self.backend.from_numpy(self.x), 'a a b b')
+            parse_shape(self.backend.from_numpy(self.x), "a a b b")
 
-    @parameterized.expand([
-        ([10, 20], '...', dict()),
-        ([10], '... a', dict(a=10)),
-        ([10, 20], '... a', dict(a=20)),
-        ([10, 20, 30], '... a', dict(a=30)),
-        ([10, 20, 30, 40], '... a', dict(a=40)),
-        ([10], 'a ...', dict(a=10)),
-        ([10, 20], 'a ...', dict(a=10)),
-        ([10, 20, 30], 'a ...', dict(a=10)),
-        ([10, 20, 30, 40], 'a ...', dict(a=10)),
-        ([10, 20, 30, 40], ' a ... b', dict(a=10, b=40)),
-        ([10, 40], ' a ... b', dict(a=10, b=40)),
-    ])
-    def test_ellipsis(self, shape: List[int], pattern: str,
-                      expected: Dict[str, int]):
+    @parameterized.expand(
+        [
+            ([10, 20], "...", dict()),
+            ([10], "... a", dict(a=10)),
+            ([10, 20], "... a", dict(a=20)),
+            ([10, 20, 30], "... a", dict(a=30)),
+            ([10, 20, 30, 40], "... a", dict(a=40)),
+            ([10], "a ...", dict(a=10)),
+            ([10, 20], "a ...", dict(a=10)),
+            ([10, 20, 30], "a ...", dict(a=10)),
+            ([10, 20, 30, 40], "a ...", dict(a=10)),
+            ([10, 20, 30, 40], " a ... b", dict(a=10, b=40)),
+            ([10, 40], " a ... b", dict(a=10, b=40)),
+        ]
+    )
+    def test_ellipsis(self, shape: List[int], pattern: str, expected: Dict[str, int]):
         x = numpy.ones(shape)
         parsed1 = parse_shape(x, pattern)
         parsed2 = parse_shape(self.backend.from_numpy(x), pattern)
         assert parsed1 == parsed2 == expected
 
 
-_SYMBOLIC_BACKENDS = [{"backend": backend} for backend in
-                      (collect_test_backends(symbolic=True, layers=False) +
-                       collect_test_backends(symbolic=True, layers=True))
-                      if backend.framework_name != 'tensorflow.keras']
+_SYMBOLIC_BACKENDS = [
+    {"backend": backend}
+    for backend in (
+        collect_test_backends(symbolic=True, layers=False) + collect_test_backends(symbolic=True, layers=True)
+    )
+    if backend.framework_name != "tensorflow.keras"
+]
 # tensorflow.keras needs special way to compile,
 # shape vars can be used only inside layers but not as outputs
 
 
 @parameterized_class(_SYMBOLIC_BACKENDS)
 class TestParseShapeSymbolic(unittest.TestCase):
-    @parameterized.expand([
-        ([10, 20, 30, 40],),
-        ([10, 20, None, None],),
-        ([None, None, None, None],),
-    ])
+    backend: AbstractBackend
+
+    @parameterized.expand(
+        [
+            ([10, 20, 30, 40],),
+            ([10, 20, None, None],),
+            ([None, None, None, None],),
+        ]
+    )
     def test_parse_shape_symbolic(self, shape):
-        print('special shape parsing for', self.backend.framework_name)
-        if self.backend.framework_name in ['mxnet.symbol']:
-            # mxnet can't normally run inference
-            shape = [10, 20, 30, 40]
+        print("special shape parsing for", self.backend.framework_name)
         input_symbol = self.backend.create_symbol(shape)
 
-        shape_placeholder = parse_shape(input_symbol, 'a b c d')
+        shape_placeholder = parse_shape(input_symbol, "a b c d")
         shape = {}
         for name, symbol in shape_placeholder.items():
-            shape[name] = symbol if isinstance(symbol, int) \
+            shape[name] = (
+                symbol
+                if isinstance(symbol, int)
                 else self.backend.eval_symbol(symbol, [(input_symbol, numpy.zeros([10, 20, 30, 40]))])
+            )
         print(shape)
-        result_placeholder = rearrange(input_symbol, 'a b (c1 c2) (d1 d2) -> (a b d1) c1 (c2 d2)',
-                                       **parse_shape(input_symbol, 'a b c1 _'), d2=2)
+        result_placeholder = rearrange(
+            input_symbol, "a b (c1 c2) (d1 d2) -> (a b d1) c1 (c2 d2)", **parse_shape(input_symbol, "a b c1 _"), d2=2
+        )
         result = self.backend.eval_symbol(result_placeholder, [(input_symbol, numpy.zeros([10, 20, 30, 40]))])
         print(result.shape)
         assert result.shape == (10 * 20 * 20, 30, 1 * 2)
         assert numpy.allclose(result, 0)
 
-    @parameterized.expand([
-        ([10, 20], [None, None], '...', dict()),
-        ([10], [None], '... a', dict(a=10)),
-        ([10, 20], [None], '... a', dict(a=20)),
-        ([10, 20, 30], [None, None, None], '... a', dict(a=30)),
-        ([10, 20, 30, 40], [None, None, None, None], '... a', dict(a=40)),
-        ([10], [None], 'a ...', dict(a=10)),
-        ([10, 20], [None, None], 'a ...', dict(a=10)),
-        ([10, 20, 30], [None, None, None], 'a ...', dict(a=10)),
-        ([10, 20, 30, 40], [None, None, None, None], 'a ...', dict(a=10)),
-        ([10, 20, 30, 40], [None, None, None, None], ' a ... b', dict(a=10, b=40)),
-        ([10, 40], [None, None], ' a ... b', dict(a=10, b=40)),
-    ])
-    def test_ellipsis(self, static_shape: List[int], shape: List[Optional[int]],
-                      pattern: str, expected: Dict[str, int]):
-        if self.backend.framework_name in ['mxnet.symbol']:
-            # mxnet can't normally run inference
-            shape = static_shape
+    @parameterized.expand(
+        [
+            ([10, 20], [None, None], "...", dict()),
+            ([10], [None], "... a", dict(a=10)),
+            ([10, 20], [None], "... a", dict(a=20)),
+            ([10, 20, 30], [None, None, None], "... a", dict(a=30)),
+            ([10, 20, 30, 40], [None, None, None, None], "... a", dict(a=40)),
+            ([10], [None], "a ...", dict(a=10)),
+            ([10, 20], [None, None], "a ...", dict(a=10)),
+            ([10, 20, 30], [None, None, None], "a ...", dict(a=10)),
+            ([10, 20, 30, 40], [None, None, None, None], "a ...", dict(a=10)),
+            ([10, 20, 30, 40], [None, None, None, None], " a ... b", dict(a=10, b=40)),
+            ([10, 40], [None, None], " a ... b", dict(a=10, b=40)),
+        ]
+    )
+    def test_ellipsis(
+        self, static_shape: List[int], shape: List[Optional[int]], pattern: str, expected: Dict[str, int]
+    ):
         input_symbol = self.backend.create_symbol(shape)
         shape_placeholder = parse_shape(input_symbol, pattern)
         out_shape = {}
         for name, symbol in shape_placeholder.items():
             if isinstance(symbol, int):
                 out_shape[name] = symbol
             else:
-                out_shape[name] = self.backend.eval_symbol(
-                    symbol, [(input_symbol, numpy.zeros(static_shape))])
+                out_shape[name] = self.backend.eval_symbol(symbol, [(input_symbol, numpy.zeros(static_shape))])
         assert out_shape == expected
 
 
 def test_is_float_type():
     backends = collect_test_backends(symbolic=False, layers=False)
     backends += collect_test_backends(symbolic=False, layers=True)
     for backend in backends:
-        for dtype in ['int32', 'int64', 'float32', 'float64']:
-            is_float = 'float' in dtype
+        for dtype in ["int32", "int64", "float32", "float64"]:
+            is_float = "float" in dtype
             input = numpy.zeros([3, 4, 5], dtype=dtype)
             input = backend.from_numpy(input)
-            if 'chainer' in backend.framework_name and not is_float:
+            if "chainer" in backend.framework_name and not is_float:
                 continue  # chainer doesn't allow non-floating tensors
             assert backend.is_float_type(input) == is_float, (dtype, backend, input.dtype)
+
+
+def test_torch_compile():
+    """
+    Test ensures that allow_ops_in_compiled_graph allows compiling in a single graph
+    Additionally we ensure that after compilation cache works properly
+     (by changing shapes and patterns)
+    We additionally check that pack/unpack still can be handled
+     despite variable number of inputs/outputs
+    """
+    if not is_backend_tested('torch'):
+        pytest.skip()
+    import torch
+    from torch import nn
+    from einops import repeat, reduce, pack, unpack, einsum
+    from einops._torch_specific import allow_ops_in_compiled_graph
+
+    allow_ops_in_compiled_graph()
+    class TorchModuleWithOperations(nn.Module):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, x_abc, suffix=''):
+            a, b, c = x_abc.shape
+
+            def suf(pattern):
+                parts = pattern.split()
+                return ' '.join([p if p[-1] not in 'acd' else p + suffix for p in parts])
+            # patterns look a bit strange because names a, c, d will be modified on every run
+            # by suf function
+            x_abcd = repeat(x_abc, suf('a b c -> a b c 4'))
+            x_abc = reduce(x_abcd, suf('a b c d -> a b c'), 'min')
+            x_abdc, ps = pack([x_abc] * (2 + len(suffix)), suf('a b * c'))
+            x_array = unpack(rearrange(x_abdc, suf('a b d c -> (a b ) 1 c d')), ps, 'ab one1 c *')
+            x1 = x_array[0] + len(x_array)
+            x1 = rearrange(x1, suf('(a b ) 1 c -> a b c'), b=b)
+            addition = einsum(x_abc, x_abcd, suf('a b c , a b c d -> d'))[0]
+            return x1 + addition
+
+    original = TorchModuleWithOperations()
+    compiled = torch.compile(original, fullgraph=True, backend='aot_eager')
+    for size in [10, 20, 40]:
+        x = torch.rand([size, size + 1, size + 2])
+        for suffix in ['', 'suf1', 'other_suffix']:
+            result1 = compiled(x, suffix)
+            result2 = original(x, suffix)
+            assert torch.allclose(result1, result2)
```

### Comparing `einops-0.6.0/tests/test_packing.py` & `einops-0.6.1/tests/test_packing.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         assert np.allclose(asnumpy(packed), asnumpy(x))
         assert np.allclose(asnumpy(packed_np), asnumpy(x))
         assert len(unpacked) == len(unpacked_np)
         for a, b in zip(unpacked, unpacked_np):
             assert np.allclose(asnumpy(a), b)
 
 
-
 class CaptureException:
     def __enter__(self):
         self.exception = None
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.exception = exc_val
         return True
@@ -70,80 +69,80 @@
         assert np.all(a == b)
 
     r, g, b = rand(3, H, W)
     embeddings = rand(H, W, 32)
 
     check(
         np.stack([r, g, b], axis=2),
-        pack([r, g, b], 'h w *')[0],
+        pack([r, g, b], "h w *")[0],
     )
     check(
         np.stack([r, g, b], axis=1),
-        pack([r, g, b], 'h * w')[0],
+        pack([r, g, b], "h * w")[0],
     )
     check(
         np.stack([r, g, b], axis=0),
-        pack([r, g, b], '* h w')[0],
+        pack([r, g, b], "* h w")[0],
     )
 
     check(
         np.concatenate([r, g, b], axis=1),
-        pack([r, g, b], 'h *')[0],
+        pack([r, g, b], "h *")[0],
     )
     check(
         np.concatenate([r, g, b], axis=0),
-        pack([r, g, b], '* w')[0],
+        pack([r, g, b], "* w")[0],
     )
 
     i = np.index_exp[:, :, None]
     check(
         np.concatenate([r[i], g[i], b[i], embeddings], axis=2),
-        pack([r, g, b, embeddings], 'h w *')[0],
+        pack([r, g, b, embeddings], "h w *")[0],
     )
 
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], 'h w nonexisting_axis *')
+        pack([r, g, b, embeddings], "h w nonexisting_axis *")
 
-    pack([r, g, b], 'some_name_for_H some_name_for_w1 *')
+    pack([r, g, b], "some_name_for_H some_name_for_w1 *")
 
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], 'h _w *')  # no leading underscore
+        pack([r, g, b, embeddings], "h _w *")  # no leading underscore
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], 'h_ w *')  # no trailing underscore
+        pack([r, g, b, embeddings], "h_ w *")  # no trailing underscore
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], '1h_ w *')
+        pack([r, g, b, embeddings], "1h_ w *")
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], '1 w *')
+        pack([r, g, b, embeddings], "1 w *")
     with pytest.raises(EinopsError):
-        pack([r, g, b, embeddings], 'h h *')
+        pack([r, g, b, embeddings], "h h *")
     # capital and non-capital are different
-    pack([r, g, b, embeddings], 'h H *')
+    pack([r, g, b, embeddings], "h H *")
 
 
 @dataclasses.dataclass
 class UnpackTestCase:
     shape: typing.Tuple[int, ...]
     pattern: str
 
     def dim(self):
-        return self.pattern.split().index('*')
+        return self.pattern.split().index("*")
 
     def selfcheck(self):
         assert self.shape[self.dim()] == 5
 
 
 cases = [
     # NB: in all cases unpacked axis is of length 5.
     # that's actively used in tests below
-    UnpackTestCase((5,), '*'),
-    UnpackTestCase((5, 7), '* seven'),
-    UnpackTestCase((7, 5), 'seven *'),
-    UnpackTestCase((5, 3, 4), '* three four'),
-    UnpackTestCase((4, 5, 3), 'four * three'),
-    UnpackTestCase((3, 4, 5), 'three four *'),
+    UnpackTestCase((5,), "*"),
+    UnpackTestCase((5, 7), "* seven"),
+    UnpackTestCase((7, 5), "seven *"),
+    UnpackTestCase((5, 3, 4), "* three four"),
+    UnpackTestCase((4, 5, 3), "four * three"),
+    UnpackTestCase((3, 4, 5), "three four *"),
 ]
 
 
 def test_pack_unpack_with_numpy():
     case: UnpackTestCase
 
     for case in cases:
@@ -151,15 +150,15 @@
         pattern = case.pattern
 
         x = np.random.random(shape)
         # all correct, no minus 1
         unpack_and_pack(x, [[2], [1], [2]], pattern)
         # no -1, asking for wrong shapes
         with pytest.raises(BaseException):
-            unpack_and_pack(x, [[2], [1], [2]], pattern + ' non_existent_axis')
+            unpack_and_pack(x, [[2], [1], [2]], pattern + " non_existent_axis")
         with pytest.raises(BaseException):
             unpack_and_pack(x, [[2], [1], [1]], pattern)
         with pytest.raises(BaseException):
             unpack_and_pack(x, [[4], [1], [1]], pattern)
         # all correct, with -1
         unpack_and_pack(x, [[2], [1], [-1]], pattern)
         unpack_and_pack(x, [[2], [-1], [2]], pattern)
@@ -204,19 +203,16 @@
 
         # -1 takes zero, -1
         unpack_and_pack(x, [[2, -1], [1, 5]], pattern)
 
 
 def test_pack_unpack_against_numpy():
     for backend in collect_test_backends(symbolic=False, layers=False):
-        print(f'test packing against numpy for {backend.framework_name}')
+        print(f"test packing against numpy for {backend.framework_name}")
         check_zero_len = True
-        if 'mxnet' in backend.framework_name:
-            # some frameworks don't accept zero as a dimension
-            check_zero_len = False
 
         for case in cases:
             unpack_and_pack = unpack_and_pack_against_numpy
             shape = case.shape
             pattern = case.pattern
 
             x = np.random.random(shape)
@@ -267,11 +263,7 @@
                 unpack_and_pack(x, [[2], [3], [-1]], pattern)
                 unpack_and_pack(x, [[0], [5], [-1]], pattern)
                 unpack_and_pack(x, [[0], [-1], [5]], pattern)
                 unpack_and_pack(x, [[-1], [5], [0]], pattern)
 
                 # -1 takes zero, -1
                 unpack_and_pack(x, [[2, -1], [1, 5]], pattern)
-
-
-# NB there is no testing for symbolic backends
-# because mxnet symbols do not allow slicing with [...]
```

### Comparing `einops-0.6.0/tests/test_parsing.py` & `einops-0.6.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/.gitignore` & `einops-0.6.1/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -116,8 +116,11 @@
 _uncommited_explorations
 trash_notebooks
 
 # oneflow's output trash
 log
 
 # this file is auto-generated
-docs_src/index.md
+docs_src/index.md
+
+# vs code 
+*.code-workspace
```

### Comparing `einops-0.6.0/LICENSE` & `einops-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `einops-0.6.0/README.md` & `einops-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
 - [Installation](#Installation)
 - [Documentation](https://einops.rocks/)
 - [Tutorial](#Tutorials) 
 - [API micro-reference](#API)
 - [Why using einops](#Why-using-einops-notation)
 - [Supported frameworks](#Supported-frameworks)
-- [Contributing](#Contributing)
 - [Repository](https://github.com/arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/discussions)
 
 ## Installation  <a name="Installation"></a>
 
 Plain and simple:
 ```bash
 pip install einops
@@ -96,14 +95,15 @@
 Tutorials are the most convenient way to see `einops` in action
 
 - part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/master/docs/1-einops-basics.ipynb) 
 - part 2: [einops for deep learning](https://github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-learning.ipynb)
 - part 3: [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - part 4: [improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)   
 
+Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/watch?v=xGy75Pjsqzo).
 
 ## API <a name="API"></a>
 
 `einops` has a minimalistic yet powerful API.
 
 Three core operations provided ([einops tutorial](https://github.com/arogozhnikov/einops/blob/master/docs/) 
 shows those cover stacking, reshape, transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous reductions)
@@ -286,18 +286,19 @@
 
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
 - [tensorflow](https://www.tensorflow.org/)
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
-- [gluon](https://gluon.mxnet.io/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
+- [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
+- [gluon](https://gluon.mxnet.io/) (deprecated)
 
 ## Citing einops <a name="Contributing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
```

#### html2text {}

```diff
@@ -27,25 +27,26 @@
 1216022614755463169) [More testimonials](https://einops.rocks/pages/
 testimonials/) ## Recordings of talk at ICLR 2022 [Screen_Shot_2022-07-03_at_1
 00_15_AM] Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603)
 focused on main problems of standard tensor manipulation methods, and how
 einops improves this process. ## Contents - [Installation](#Installation) -
 [Documentation](https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-
 reference](#API) - [Why using einops](#Why-using-einops-notation) - [Supported
-frameworks](#Supported-frameworks) - [Contributing](#Contributing) -
-[Repository](https://github.com/arogozhnikov/einops) and [discussions](https://
-github.com/arogozhnikov/einops/discussions) ## Installation  Plain and simple:
-```bash pip install einops ```  ## Tutorials  Tutorials are the most convenient
-way to see `einops` in action - part 1: [einops fundamentals](https://
-github.com/arogozhnikov/einops/blob/master/docs/1-einops-basics.ipynb) - part
-2: [einops for deep learning](https://github.com/arogozhnikov/einops/blob/
-master/docs/2-einops-for-deep-learning.ipynb) - part 3: [packing and unpacking]
-(https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-
-unpack.ipynb) - part 4: [improve pytorch code with einops](http://einops.rocks/
-pytorch-examples.html) ## API  `einops` has a minimalistic yet powerful API.
+frameworks](#Supported-frameworks) - [Repository](https://github.com/
+arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
+discussions) ## Installation  Plain and simple: ```bash pip install einops ```
+## Tutorials  Tutorials are the most convenient way to see `einops` in action -
+part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
+master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
+/github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
+learning.ipynb) - part 3: [packing and unpacking](https://github.com/
+arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - part 4:
+[improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)
+Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/
+watch?v=xGy75Pjsqzo). ## API  `einops` has a minimalistic yet powerful API.
 Three core operations provided ([einops tutorial](https://github.com/
 arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
 transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
 reductions) ```python from einops import rearrange, reduce, repeat # rearrange
 elements according to the pattern output_tensor = rearrange(input_tensor, 't b
 c -> b c t') # combine rearrangement and reduction output_tensor = reduce
 (input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
@@ -119,16 +120,17 @@
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
 Testimonials provide user's perspective on the same question. ## Supported
 frameworks  Einops works with ... - [numpy](http://www.numpy.org/) - [pytorch]
 (https://pytorch.org/) - [tensorflow](https://www.tensorflow.org/) - [jax]
 (https://github.com/google/jax) - [cupy](https://cupy.chainer.org/) - [chainer]
-(https://chainer.org/) - [gluon](https://gluon.mxnet.io/) - [tf.keras](https://
-www.tensorflow.org/guide/keras) - [oneflow](https://github.com/Oneflow-Inc/
-oneflow) (experimental) - [flax](https://github.com/google/flax) (experimental)
-## Citing einops  Please use the following bibtex record ```text @inproceedings
-{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
-with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
-{International Conference on Learning Representations}, year={2022}, url=
-{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
+(https://chainer.org/) - [tf.keras](https://www.tensorflow.org/guide/keras) -
+[oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental) - [flax]
+(https://github.com/google/flax) (experimental) - [paddle](https://github.com/
+PaddlePaddle/Paddle) (experimental) - [gluon](https://gluon.mxnet.io/)
+(deprecated) ## Citing einops  Please use the following bibtex record ```text
+@inproceedings{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor
+Manipulations with Einstein-like Notation}, author={Alex Rogozhnikov},
+booktitle={International Conference on Learning Representations}, year={2022},
+url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
 versions `einops` works with python 3.7 or later.
```

### Comparing `einops-0.6.0/pyproject.toml` & `einops-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,47 +4,53 @@
 
 [project]
 name = "einops"
 description = "A new flavour of deep learning operations"
 readme = "README.md"
 requires-python = ">=3.7"
 
-keywords = ['deep learning', 'neural networks', 'tensor manipulation', 'machine learning',
-             'scientific computations', 'einops',]
-license = {text = 'MIT'}
+keywords = [
+    'deep learning',
+    'neural networks',
+    'tensor manipulation',
+    'machine learning',
+    'scientific computations',
+    'einops',
+]
+license = { text = 'MIT' }
 classifiers = [
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
 ]
 dependencies = [
     # no run-time or installation-time dependencies
 ]
 dynamic = ["version"]
-authors = [{name = 'Alex Rogozhnikov'}]
+authors = [{ name = 'Alex Rogozhnikov' }]
 
 [project.urls]
 Homepage = 'https://github.com/arogozhnikov/einops'
 
 [tool.setuptools]
 packages = ['einops', 'einops.layers']
 
 [tool.hatch.version]
 path = "einops/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
-  "/.github",
-  "/.idea",
-  "/.pytest_cache",
-  "/build",
-  "/dist",
-  "/docs",
-  "/docs_src",
-  "/log",
+    "/.github",
+    "/.idea",
+    "/.pytest_cache",
+    "/build",
+    "/dist",
+    "/docs",
+    "/docs_src",
+    "/log",
 ]
 
 [tool.hatch.build.targets.wheel]
 # should use packages from main section
 
 
 [tool.hatch.envs.docs]
@@ -82,8 +88,12 @@
 filterwarnings = [
     "ignore:Call to deprecated create function FieldDescriptor",
     "ignore:Call to deprecated create function Descriptor",
     "ignore:Call to deprecated create function EnumDescriptor",
     "ignore:Call to deprecated create function EnumValueDescriptor",
     "ignore:Call to deprecated create function FileDescriptor",
     "ignore:Call to deprecated create function OneofDescriptor",
-]
+]
+
+[tool.black]
+line-length = 120
+target-version = ['py311']
```

### Comparing `einops-0.6.0/PKG-INFO` & `einops-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einops
-Version: 0.6.0
+Version: 0.6.1
 Summary: A new flavour of deep learning operations
 Project-URL: Homepage, https://github.com/arogozhnikov/einops
 Author: Alex Rogozhnikov
 License: MIT
 License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific computations,tensor manipulation
 Classifier: Intended Audience :: Science/Research
@@ -83,15 +83,14 @@
 
 - [Installation](#Installation)
 - [Documentation](https://einops.rocks/)
 - [Tutorial](#Tutorials) 
 - [API micro-reference](#API)
 - [Why using einops](#Why-using-einops-notation)
 - [Supported frameworks](#Supported-frameworks)
-- [Contributing](#Contributing)
 - [Repository](https://github.com/arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/discussions)
 
 ## Installation  <a name="Installation"></a>
 
 Plain and simple:
 ```bash
 pip install einops
@@ -111,14 +110,15 @@
 Tutorials are the most convenient way to see `einops` in action
 
 - part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/master/docs/1-einops-basics.ipynb) 
 - part 2: [einops for deep learning](https://github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-learning.ipynb)
 - part 3: [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - part 4: [improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)   
 
+Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/watch?v=xGy75Pjsqzo).
 
 ## API <a name="API"></a>
 
 `einops` has a minimalistic yet powerful API.
 
 Three core operations provided ([einops tutorial](https://github.com/arogozhnikov/einops/blob/master/docs/) 
 shows those cover stacking, reshape, transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous reductions)
@@ -301,18 +301,19 @@
 
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
 - [tensorflow](https://www.tensorflow.org/)
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
-- [gluon](https://gluon.mxnet.io/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
 - [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
+- [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
+- [gluon](https://gluon.mxnet.io/) (deprecated)
 
 ## Citing einops <a name="Contributing"></a>
 
 Please use the following bibtex record
 
 ```text
 @inproceedings{
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: einops Version: 0.6.0 Summary: A new flavour of
+Metadata-Version: 2.1 Name: einops Version: 0.6.1 Summary: A new flavour of
 deep learning operations Project-URL: Homepage, https://github.com/
 arogozhnikov/einops Author: Alex Rogozhnikov License: MIT License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific
 computations,tensor manipulation Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
 Type: text/markdown   https://user-images.githubusercontent.com/6318811/
@@ -34,25 +34,26 @@
 1216022614755463169) [More testimonials](https://einops.rocks/pages/
 testimonials/) ## Recordings of talk at ICLR 2022 [Screen_Shot_2022-07-03_at_1
 00_15_AM] Watch [a 15-minute talk](https://iclr.cc/virtual/2022/oral/6603)
 focused on main problems of standard tensor manipulation methods, and how
 einops improves this process. ## Contents - [Installation](#Installation) -
 [Documentation](https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-
 reference](#API) - [Why using einops](#Why-using-einops-notation) - [Supported
-frameworks](#Supported-frameworks) - [Contributing](#Contributing) -
-[Repository](https://github.com/arogozhnikov/einops) and [discussions](https://
-github.com/arogozhnikov/einops/discussions) ## Installation  Plain and simple:
-```bash pip install einops ```  ## Tutorials  Tutorials are the most convenient
-way to see `einops` in action - part 1: [einops fundamentals](https://
-github.com/arogozhnikov/einops/blob/master/docs/1-einops-basics.ipynb) - part
-2: [einops for deep learning](https://github.com/arogozhnikov/einops/blob/
-master/docs/2-einops-for-deep-learning.ipynb) - part 3: [packing and unpacking]
-(https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-
-unpack.ipynb) - part 4: [improve pytorch code with einops](http://einops.rocks/
-pytorch-examples.html) ## API  `einops` has a minimalistic yet powerful API.
+frameworks](#Supported-frameworks) - [Repository](https://github.com/
+arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
+discussions) ## Installation  Plain and simple: ```bash pip install einops ```
+## Tutorials  Tutorials are the most convenient way to see `einops` in action -
+part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
+master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
+/github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
+learning.ipynb) - part 3: [packing and unpacking](https://github.com/
+arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - part 4:
+[improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)
+Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/
+watch?v=xGy75Pjsqzo). ## API  `einops` has a minimalistic yet powerful API.
 Three core operations provided ([einops tutorial](https://github.com/
 arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
 transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
 reductions) ```python from einops import rearrange, reduce, repeat # rearrange
 elements according to the pattern output_tensor = rearrange(input_tensor, 't b
 c -> b c t') # combine rearrangement and reduction output_tensor = reduce
 (input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
@@ -126,16 +127,17 @@
 in numpy repeat(image, 'h w -> h (tile w)', tile=2) # in pytorch repeat(image,
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
 Testimonials provide user's perspective on the same question. ## Supported
 frameworks  Einops works with ... - [numpy](http://www.numpy.org/) - [pytorch]
 (https://pytorch.org/) - [tensorflow](https://www.tensorflow.org/) - [jax]
 (https://github.com/google/jax) - [cupy](https://cupy.chainer.org/) - [chainer]
-(https://chainer.org/) - [gluon](https://gluon.mxnet.io/) - [tf.keras](https://
-www.tensorflow.org/guide/keras) - [oneflow](https://github.com/Oneflow-Inc/
-oneflow) (experimental) - [flax](https://github.com/google/flax) (experimental)
-## Citing einops  Please use the following bibtex record ```text @inproceedings
-{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor Manipulations
-with Einstein-like Notation}, author={Alex Rogozhnikov}, booktitle=
-{International Conference on Learning Representations}, year={2022}, url=
-{https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
+(https://chainer.org/) - [tf.keras](https://www.tensorflow.org/guide/keras) -
+[oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental) - [flax]
+(https://github.com/google/flax) (experimental) - [paddle](https://github.com/
+PaddlePaddle/Paddle) (experimental) - [gluon](https://gluon.mxnet.io/)
+(deprecated) ## Citing einops  Please use the following bibtex record ```text
+@inproceedings{ rogozhnikov2022einops, title={Einops: Clear and Reliable Tensor
+Manipulations with Einstein-like Notation}, author={Alex Rogozhnikov},
+booktitle={International Conference on Learning Representations}, year={2022},
+url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ## Supported python
 versions `einops` works with python 3.7 or later.
```

