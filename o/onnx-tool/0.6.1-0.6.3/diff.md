# Comparing `tmp/onnx-tool-0.6.1.tar.gz` & `tmp/onnx-tool-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-tool-0.6.1.tar", last modified: Thu Mar  2 11:57:04 2023, max compression
+gzip compressed data, was "onnx-tool-0.6.3.tar", last modified: Wed Apr 19 12:50:23 2023, max compression
```

## Comparing `onnx-tool-0.6.1.tar` & `onnx-tool-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 11:57:04.305692 onnx-tool-0.6.1/
--rw-rw-rw-   0        0        0     1092 2022-06-28 15:38:19.000000 onnx-tool-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     8941 2023-03-02 11:57:04.304691 onnx-tool-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     8482 2023-02-24 14:19:15.000000 onnx-tool-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 11:57:04.287654 onnx-tool-0.6.1/onnx_tool/
--rw-rw-rw-   0        0        0    15652 2023-02-24 14:18:33.000000 onnx-tool-0.6.1/onnx_tool/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-02-07 11:56:14.000000 onnx-tool-0.6.1/onnx_tool/__main__.py
--rw-rw-rw-   0        0        0    38630 2023-03-02 11:41:13.000000 onnx-tool-0.6.1/onnx_tool/graph.py
--rw-rw-rw-   0        0        0    58037 2023-03-02 11:41:43.000000 onnx-tool-0.6.1/onnx_tool/node.py
--rw-rw-rw-   0        0        0     5596 2023-02-24 14:18:33.000000 onnx-tool-0.6.1/onnx_tool/serialization.py
--rw-rw-rw-   0        0        0    14393 2023-02-07 11:56:14.000000 onnx-tool-0.6.1/onnx_tool/tensor.py
--rw-rw-rw-   0        0        0     3685 2023-03-02 11:52:37.000000 onnx-tool-0.6.1/onnx_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-02 11:57:04.302691 onnx-tool-0.6.1/onnx_tool.egg-info/
--rw-rw-rw-   0        0        0     8941 2023-03-02 11:57:04.000000 onnx-tool-0.6.1/onnx_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-03-02 11:57:04.000000 onnx-tool-0.6.1/onnx_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 11:57:04.000000 onnx-tool-0.6.1/onnx_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-03-02 11:57:04.000000 onnx-tool-0.6.1/onnx_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-02 11:57:04.000000 onnx-tool-0.6.1/onnx_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-06-28 15:40:35.000000 onnx-tool-0.6.1/onnx_tool.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-03-02 11:57:04.305692 onnx-tool-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      972 2023-03-02 11:52:37.000000 onnx-tool-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:50:23.938199 onnx-tool-0.6.3/
+-rw-rw-rw-   0        0        0     1092 2022-06-28 15:38:19.000000 onnx-tool-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0    10342 2023-04-19 12:50:23.937199 onnx-tool-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9883 2023-04-16 06:54:51.000000 onnx-tool-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:50:23.918171 onnx-tool-0.6.3/onnx_tool/
+-rw-rw-rw-   0        0        0    15585 2023-04-10 11:33:26.000000 onnx-tool-0.6.3/onnx_tool/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-02-07 11:56:14.000000 onnx-tool-0.6.3/onnx_tool/__main__.py
+-rw-rw-rw-   0        0        0    11847 2023-04-10 11:33:26.000000 onnx-tool-0.6.3/onnx_tool/fusion.py
+-rw-rw-rw-   0        0        0    51650 2023-04-19 12:43:18.000000 onnx-tool-0.6.3/onnx_tool/graph.py
+-rw-rw-rw-   0        0        0    60509 2023-04-10 11:31:57.000000 onnx-tool-0.6.3/onnx_tool/node.py
+-rw-rw-rw-   0        0        0     6205 2023-04-14 09:22:33.000000 onnx-tool-0.6.3/onnx_tool/serialization.py
+-rw-rw-rw-   0        0        0    15938 2023-04-19 12:37:01.000000 onnx-tool-0.6.3/onnx_tool/tensor.py
+-rw-rw-rw-   0        0        0     3685 2023-04-19 12:48:12.000000 onnx-tool-0.6.3/onnx_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:50:23.936199 onnx-tool-0.6.3/onnx_tool.egg-info/
+-rw-rw-rw-   0        0        0    10342 2023-04-19 12:50:23.000000 onnx-tool-0.6.3/onnx_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-04-19 12:50:23.000000 onnx-tool-0.6.3/onnx_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:50:23.000000 onnx-tool-0.6.3/onnx_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 12:50:23.000000 onnx-tool-0.6.3/onnx_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 12:50:23.000000 onnx-tool-0.6.3/onnx_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-06-28 15:40:35.000000 onnx-tool-0.6.3/onnx_tool.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:50:23.938199 onnx-tool-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      972 2023-04-19 12:48:06.000000 onnx-tool-0.6.3/setup.py
```

### Comparing `onnx-tool-0.6.1/LICENSE` & `onnx-tool-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.6.1/PKG-INFO` & `onnx-tool-0.6.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.6.1
+Version: 0.6.3
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
+* *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: Resnet, MobileNet, YOLO, ...
@@ -89,34 +90,55 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
+## Memory Compression
+
+For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
+The compression method achieves 5% memory compression on most models.   
+For example:
+
+ model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
+-------------------------------|------------------------|----------------------------|----------------------
+ StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
+ StableDiffusion(VAE_decoder)  | 25,417                 | 1,140                      | 4.48                 
+ StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
+ StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
+ GPT2                          | 40                     | 2                          | 6.9                  
+ BERT                          | 2,170                  | 27                         | 1.25                 
+
+code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
+
+---
+
 ## Tensor operations
-* *Export weight tensors to files*  
-* *Simplify tensor and node names, convert name from a long string to a short string*  
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*  
+
+* *Export weight tensors to files*
+* *Simplify tensor and node names, convert name from a long string to a short string*
+* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
 * *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).  
+  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
```

### Comparing `onnx-tool-0.6.1/README.md` & `onnx-tool-0.6.3/onnx_tool.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,28 @@
+Metadata-Version: 2.1
+Name: onnx-tool
+Version: 0.6.3
+Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
+Home-page: https://github.com/ThanatosShinji/onnx-tool
+Author: Luo Yu
+Author-email: luoyu888888@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # onnx-tool
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
+* *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: Resnet, MobileNet, YOLO, ...
@@ -77,34 +90,55 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
+## Memory Compression
+
+For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
+The compression method achieves 5% memory compression on most models.   
+For example:
+
+ model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
+-------------------------------|------------------------|----------------------------|----------------------
+ StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
+ StableDiffusion(VAE_decoder)  | 25,417                 | 1,140                      | 4.48                 
+ StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
+ StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
+ GPT2                          | 40                     | 2                          | 6.9                  
+ BERT                          | 2,170                  | 27                         | 1.25                 
+
+code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
+
+---
+
 ## Tensor operations
-* *Export weight tensors to files*  
-* *Simplify tensor and node names, convert name from a long string to a short string*  
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*  
+
+* *Export weight tensors to files*
+* *Simplify tensor and node names, convert name from a long string to a short string*
+* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
 * *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).  
+  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
 
@@ -172,8 +206,8 @@
 [FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29 | 37,056
 [MobileNet v2-1.0-fp32](https://github.com/onnx/models/blob/main/vision/classification/mobilenet) | 3.3 | 300
 [ResNet50_fp32](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25 | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

### Comparing `onnx-tool-0.6.1/onnx_tool/__init__.py` & `onnx-tool-0.6.3/onnx_tool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,17 +105,15 @@
 def model_shape_regress(m, input_desc: {}, input_range: {}):
     if isinstance(m, str):
         m = onnx.load_model(m)
     if isinstance(m, onnx.ModelProto):
         G = Graph(m.graph)
         G.graph_reorder()
         shape_engine = G.shape_regress(input_desc, input_range)
-        g = G.get_compute_graph()
-        cg = Graph(g)
-        cg.save_model('compute_graph.onnx')
+        cg = G.get_compute_graph()
         return shape_engine, cg
 
 
 def model_remove_Identity(m, f: str):
     if isinstance(m, str):
         m = onnx.load_model(m)
     if isinstance(m, onnx.ModelProto):
```

### Comparing `onnx-tool-0.6.1/onnx_tool/__main__.py` & `onnx-tool-0.6.3/onnx_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.6.1/onnx_tool/graph.py` & `onnx-tool-0.6.3/onnx_tool/graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import copy
 import math
 import warnings
 
 import numpy
 import onnx
 
+import onnx_tool
 from .node import create_node
 from .tensor import get_attribute_data, Tensor, volume
 from .utils import VERSION, tuple2str
 
 
 def __shape_of_initializer__(initial):
     shape = []
@@ -163,19 +165,30 @@
         self.rawgraph = g
         self.initials = []
         self.dynamics = []
         self.input = []
         self.output = []
         self.__init_graph_from_onnxproto__(g, noderename)
         self.__find_shape_tensors__()
+        self.valid_shape = False
+        self.valid_profile = False
 
     def log(self, str):
         if self.verbose:
             print(str)
 
+    def remove_constant(self):
+        rmlist = []
+        for key in self.nodemap:
+            if self.nodemap[key].op_type == 'Constant':
+                rmlist.append(key)
+
+        for key in rmlist:
+            self.nodemap.pop(key)
+
     def __init_graph_from_onnxproto__(self, g, noderename, remove_dummytensors=True):
         if g is None:
             return
         ncount = 0
         from .utils import timer
 
         tm = timer()
@@ -344,14 +357,22 @@
 
         for node in self.nodemap.keys():
             if node not in graph_level1 and node not in graph_level2:
                 graph_level0.append(node)
 
         return graph_level0, graph_level1, graph_level2
 
+    def add_initial(self, name, data):
+        from .tensor import create_initial_Tensor
+        self.initials.add(name)
+        if isinstance(data, numpy.ndarray):
+            self.tensormap[name] = create_initial_Tensor(name, data)
+        else:
+            raise NotImplementedError('unsupported data type')
+
     def get_subgraph(self, inputs: [], outputs: []):
         graph_level0, graph_level1, graph_level2 = self.__get_subnodes_byio__(inputs, outputs)
 
         graph_level0 = Graph(self.get_onnxgraph_by_nodenames(graph_level0))
         graph_level1 = Graph(self.get_onnxgraph_by_nodenames(graph_level1))
         graph_level2 = Graph(self.get_onnxgraph_by_nodenames(graph_level2))
 
@@ -378,100 +399,179 @@
             warnings.warn("subgraph input and output tensors can not reverse to raw graph.")
 
         if len(extern_outputs) != len(self.output):
             warnings.warn("subgraph input and output tensors can not reverse to raw graph.")
 
         return graph_level0, graph_level1, graph_level2
 
-    def fuse_subgraph_node_names(self, nodes: [str], nodeop: str, name: str, keep_attr=True):
+    def get_initials_from_nodenames(self, nodenames):
+        initializer = []
+        for name in nodenames:
+            for input in self.nodemap[name].input:
+                if input in self.initials:
+                    initializer.append(self.tensormap[input].proto)
+        return initializer
+
+    def remove_node(self, nodename):
+        node = self.nodemap[nodename]
+        # update producer
+        for o in node.output:
+            self.producedby[o].remove(nodename)
+            if len(self.producedby[o]) == 0:
+                self.producedby.pop(o)
+        # update consumer
+        for i in node.input:
+            if i in self.consumedby.keys():
+                self.consumedby[i].remove(nodename)
+        self.nodemap.pop(nodename)
+
+    def skip_node(self, nodename):
+        node = self.nodemap[nodename]
+        count = 0
+        for input in node.input:
+            if input in self.dynamics:
+                count += 1
+                indtensor = input
+        if count == 1 and len(node.output) == 1:
+            self.consumedby[indtensor].remove(nodename)
+            for con in self.consumedby[node.output[0]]:
+                con_node = self.nodemap[con]
+                for i in range(len(con_node.input)):
+                    if con_node.input[i] == node.output[0]:
+                        con_node.input[i] = indtensor
+                        self.consumedby[indtensor].append(con)
+                        break
+
+    def fuse_subgraph_node_names(self, nodes: [str], nodeop: str, nodename: str, keep_attr=True):
         _inputs, _outputs = self.get_iotensors(nodes, remove_initials=False)
-        newnode = onnx.helper.make_node(nodeop, _inputs, _outputs, name=name)
+        newnode = onnx.helper.make_node(nodeop, _inputs, _outputs, name=nodename)
         count = 0
         if keep_attr:
             for node in nodes:
                 for attribute in self.nodemap[node].proto.attribute:
-                    attr = onnx.helper.make_attribute(self.nodemap[node].proto.name + '_' + attribute.name,
-                                                      get_attribute_data(attribute))
+                    attr = onnx.helper.make_attribute(
+                        self.nodemap[node].proto.op_type + str(count) + '_' + attribute.name,
+                        get_attribute_data(attribute))
                     newnode.attribute.append(attr)
                 count += 1
+        from .node import Node
+        for name in nodes:
+            self.remove_node(name)
+        newnode = Node(newnode)
+        newnode.input = _inputs
+        newnode.output = _outputs
+        for i in _inputs:
+            self.consumedby[i].append(nodename)
+            if i in self.producedby.keys():
+                newnode.prevnodes.append(self.producedby[i])
+        for o in _outputs:
+            self.producedby[o] = [nodename]
+            if o in self.consumedby.keys():
+                newnode.nextnodes.append(self.consumedby[o])
+        self.nodemap[nodename] = newnode
 
-        allnodes = set(self.nodemap.keys())
-        remainnodes = allnodes - set(nodes)
-        nodes = []
-        for name in remainnodes:
-            nodes.append(self.nodemap[name].proto)
-        nodes.append(newnode)
-        inputs = []
-        outputs = []
-        for name in self.input:
-            if name in self.tensormap:
-                inputs.append(self.tensormap[name].proto)
-            else:
-                inputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
-        for name in self.output:
-            if name in self.tensormap:
-                outputs.append(self.tensormap[name].proto)
+    def fuse_postop_node_names(self, nodes: [str], append_attr: bool, **extrakeys):
+        _inputs, _outputs = self.get_iotensors(nodes, remove_initials=False)
+        mainnode = self.nodemap[nodes[0]]
+        newnode = onnx.helper.make_node(mainnode.op_type, _inputs, _outputs, name=mainnode.name)
+        count = 0
+        for attr in mainnode.proto.attribute:
+            if attr.name == 'postop_count':
+                count = onnx.helper.get_attribute_value(attr)
             else:
-                outputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
-        graph = onnx.helper.make_graph(nodes=nodes, name='fused_graph', inputs=inputs, outputs=outputs,
-                                       initializer=self.rawgraph.initializer)
-        newgraph = Graph(graph)
-        return newgraph
+                newnode.attribute.append(attr)
+
+        for key in extrakeys:
+            attr = onnx.helper.make_attribute(key, extrakeys[key])
+            newnode.attribute.append(attr)
+
+        if append_attr:
+            for nname in nodes:
+                if nname == mainnode.name:
+                    continue
+                pnode = self.nodemap[nname]
+                attr = onnx.helper.make_attribute(
+                    'postop_' + str(count), pnode.op_type)
+                newnode.attribute.append(attr)
+                for attribute in pnode.proto.attribute:
+                    attr = onnx.helper.make_attribute(
+                        'postop_' + str(count) + '_' + attribute.name,
+                        get_attribute_data(attribute))
+                    newnode.attribute.append(attr)
+                count += 1
+
+        attr = onnx.helper.make_attribute('postop_count', count)
+        newnode.attribute.append(attr)
+
+        for name in nodes:
+            self.remove_node(name)
+        newnode = create_node(newnode)
+        newnode.input = _inputs
+        newnode.output = _outputs
+        for i in _inputs:
+            if i in self.consumedby.keys():
+                self.consumedby[i].append(mainnode.name)
+            if i in self.producedby.keys():
+                newnode.prevnodes.append(self.producedby[i])
+        for o in _outputs:
+            self.producedby[o] = [mainnode.name]
+            if o in self.consumedby.keys():
+                newnode.nextnodes.append(self.consumedby[o])
+        self.nodemap[mainnode.name] = newnode
 
     def fuse_subgraph_iotensors(self, inputs: [], outputs: [], nodeop: str, name: str, keep_attr=True):
         _, nodes, _ = self.__get_subnodes_byio__(inputs, outputs)
         _inputs, _outputs = self.get_iotensors(nodes, remove_initials=True)
         nodes = self.reorder_nodes(nodes, _inputs)
         return self.fuse_subgraph_node_names(nodes, nodeop, name, keep_attr)
 
     def get_onnxgraph_by_nodenames(self, nodenames):
         if len(nodenames):
             _inputs0, _outputs0 = self.get_iotensors(nodenames)
             graph_level0 = self.reorder_nodes(nodenames, _inputs0)
-            subgraph = self.make_graph(graph_level0, 'subgraph', _inputs0, _outputs0)
+            subgraph = self.make_graph_onnx(graph_level0, 'subgraph', _inputs0, _outputs0)
             return subgraph
         return None
 
-    def save_model(self, f: str, shape_only: bool = False):
-        graph = self.make_graph(self.nodemap.keys(), 'graph', self.input, self.output, not shape_only)
+    def save_model(self, f: str, shape_only: bool = False, rawmodel: onnx.ModelProto = None):
+        graph = self.make_graph_onnx(self.nodemap.keys(), 'graph', self.input, self.output, not shape_only)
         if graph is not None and f is not None:
-            model = onnx.helper.make_model(graph, producer_name='onnx-tool', producer_version='v' + VERSION)
+            attr = {}
+            attr['producer_name'] = 'onnx_tool'
+            attr['producer_version'] = 'v' + VERSION
+            model = onnx.helper.make_model(graph, **attr)
+            if rawmodel is not None:
+                model.ir_version = rawmodel.ir_version
+                model.opset_import[0].version = rawmodel.opset_import[0].version
             onnx.save_model(model, f)
 
-    def make_graph(self, nodenames, gname, inputnames, outputnames, with_initializer=True):
+    def make_graph_onnx(self, nodenames, gname, inputnames, outputnames, with_initializer=True):
         nodes = []
         for name in nodenames:
             nodes.append(self.nodemap[name].make_nodeproto())
 
         initializer = None
         if with_initializer:
-            names = []
-            for name in nodenames:
-                for input in self.nodemap[name].input:
-                    if input in self.initials:
-                        names.append(input)
-            initializer = []
-            for initial in self.rawgraph.initializer:
-                if initial.name in names:
-                    initializer.append(initial)
+            initializer = self.get_initials_from_nodenames(nodenames)
 
         inputs = []
         outputs = []
         for name in inputnames:
             if name in self.tensormap:
                 inputs.append(self.tensormap[name].make_value_proto())
             else:
                 inputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
         for name in outputnames:
             if name in self.tensormap:
-                outputs.append(self.tensormap[name].make_value_proto())
-            else:
-                outputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
+                proto = self.tensormap[name].make_value_proto(make_dummy=True)
+                outputs.append(proto)
         value_infos = []
         for key in self.dynamics:
+            if key in self.input or key in self.output:
+                continue
             tensor = self.tensormap[key]
             vinfo = tensor.make_value_proto()
             if vinfo is None:
                 continue
             value_infos.append(vinfo)
         graph = onnx.helper.make_graph(nodes=nodes, name=gname, inputs=inputs, outputs=outputs, initializer=initializer,
                                        value_info=value_infos)
@@ -486,15 +586,15 @@
     def graph_reorder(self):
         old_order = self.nodemap.keys()
         ordered_nodes = self.reorder_nodes(old_order, self.input)
         new_map = {}
         for nname in ordered_nodes:
             new_map[nname] = self.nodemap[nname]
         self.nodemap = new_map
-        self.rawgraph = self.make_graph(self.nodemap.keys(), 'reordered', self.input, self.output)
+        self.rawgraph = self.make_graph_onnx(self.nodemap.keys(), 'reordered', self.input, self.output)
 
     def reorder_nodes(self, nodenames, itnames):
         tensor_consumed = []
         tensor_produced = []
         nextnodes = []
         reorderednode = []
         search_flag = {}
@@ -530,14 +630,16 @@
             for node in nextnodes:
                 produced = True
                 for input in self.nodemap[node].input:
                     if len(input) == 0:
                         continue
                     if input in self.initials:
                         continue
+                    if input not in self.producedby:
+                        continue
                     if input not in tensor_produced:
                         produced = False
                         break
                 if produced:
                     execnodes.append(node)
 
             newnodes = []
@@ -610,17 +712,32 @@
     def get_dynamic_tensors(self):
         dtensors = {}
         import copy
         for key in self.dynamics:
             dtensors[key] = copy.deepcopy(self.tensormap[key])
         return dtensors
 
+    def check_inputs(self):
+        for name in self.input:
+            shape = self.tensormap[name].shape
+            for val in shape:
+                if isinstance(val, str):
+                    return False, name
+                if val < 0:
+                    return False, name
+        return True, None
+
     def shape_infer(self, inputs: {} = None):
+        self.valid_shape = False
         if inputs is not None:
             self.update_input_by_map(inputs)
+        in_valid, tname = self.check_inputs()
+        if not in_valid:
+            raise ValueError(
+                f"The input tensor {tname}'s shape {self.tensormap[tname].shape2str()} is not valid, Please set it to a valid shape.")
         self.shapeinfer_optime_map = {}
         from .utils import timer
         tm = timer()
         for key in self.nodemap.keys():
             tm.start()
             node = self.nodemap[key]
             if node.shape_calc:
@@ -647,14 +764,15 @@
                     for i, output in enumerate(node.output):
                         self.tensormap[output].update_shape(oshapes[i])
             if node.op_type in self.shapeinfer_optime_map.keys():
                 self.shapeinfer_optime_map[node.op_type] += tm.stop()
             else:
                 self.shapeinfer_optime_map[node.op_type] = tm.stop()
         self.log(self.shapeinfer_optime_map)
+        self.valid_shape = True
 
     def value_infer(self, inputs: {}):
         self.update_input_by_map(inputs)
         for key in self.nodemap.keys():
             node = self.nodemap[key]
             itensors = []
             for input in node.input:
@@ -666,15 +784,16 @@
         for output in self.output:
             outputs.append(self.tensormap[output].numpy)
         return outputs
 
     def add_dump_tensors(self, dump_tensor_names: []):
         for name in dump_tensor_names:
             if name in self.tensormap.keys():
-                self.output.append(name)
+                if name not in self.output:
+                    self.output.append(name)
 
     def shape_regress(self, input_desc: {}, input_range: {}):
         shapeengine = ShapeEngine(input_desc)
 
         for key in input_range.keys():
             shapeengine.update_variable(key, input_range[key][1])
         tmp_input = shapeengine.generate_input()
@@ -770,15 +889,159 @@
                             else:
                                 vidx = vcount + idx
                                 valkey = str(vidx)
                         shapeengine.update_tensor_desc(vkey, i, valkey)
             vcount += len(dstranges)
         return shapeengine
 
-    def get_compute_graph(self):
+    def compress_memory(self, size_padding=64):
+        self.remove_constant()
+        tensor_in_mem = copy.deepcopy(self.input)
+        tensor_mem_per_node = []
+        tensor_consumed = {}
+        for node in self.nodemap.keys():
+            node_ = self.nodemap[node]
+            for name in node_.output:
+                tensor_in_mem.append(name)
+            new_list = copy.deepcopy(tensor_in_mem)
+            tensor_mem_per_node.append(new_list)
+            for name in node_.input:
+                if name in self.consumedby:
+                    if name in tensor_consumed:
+                        tensor_consumed[name].append(node)
+                    else:
+                        tensor_consumed[name] = [node]
+                    consumers = self.consumedby[name]
+                    if len(tensor_consumed[name]) == len(consumers):
+                        if name in tensor_in_mem:
+                            tensor_in_mem.remove(name)
+        for output in self.output:
+            if output not in tensor_in_mem:
+                warnings.warn(f'tensor list is wrong, {output} is missing!')
+        # print(tensor_mem_per_node)
+        compress_mem = {}
+        mem_tags = []
+        mem_block = []
+        for nodetensors in tensor_mem_per_node:
+            # clear mem tags
+            for i, tag in enumerate(mem_tags):
+                if tag == "":
+                    continue
+                if tag not in nodetensors:
+                    premerge = False
+                    if i >= 1 and mem_tags[i - 1] == "":
+                        premerge = True
+                    nextmerge = False
+                    if i < len(mem_tags) - 1 and mem_tags[i + 1] == "":
+                        nextmerge = True
+                    if premerge and nextmerge:
+                        newblock = [mem_block[i - 1][0], mem_block[i + 1][0] + mem_block[i + 1][1]
+                                    - mem_block[i - 1][0]]
+                        mem_tags.pop(i)
+                        mem_tags.pop(i)
+                        mem_block.pop(i)
+                        mem_block.pop(i)
+                        mem_tags[i - 1] = ""
+                        mem_block[i - 1] = newblock
+                    elif premerge:
+                        newblock = [mem_block[i - 1][0], mem_block[i][0] + mem_block[i][1]
+                                    - mem_block[i - 1][0]]
+                        mem_tags.pop(i)
+                        mem_block.pop(i)
+                        mem_tags[i - 1] = ""
+                        mem_block[i - 1] = newblock
+                    elif nextmerge:
+                        newblock = [mem_block[i][0], mem_block[i + 1][0] + mem_block[i + 1][1]
+                                    - mem_block[i][0]]
+                        mem_tags.pop(i)
+                        mem_block.pop(i)
+                        mem_tags[i] = ""
+                        mem_block[i] = newblock
+                    else:
+                        mem_tags[i] = ""
+
+            # push tensor mem to block
+            for tname in nodetensors:
+                t_ = self.tensormap[tname]
+                size_ = t_.get_memsize()
+                size_ = int((size_ + size_padding - 1) // size_padding * size_padding)
+                if tname in mem_tags:
+                    continue
+                block_found = False
+                for i, tag in enumerate(mem_tags):
+                    if tag == "":
+                        if mem_block[i][1] >= size_:
+                            remain_size = mem_block[i][1] - size_
+                            if remain_size > 1024 * 1024:
+                                remain_block = [mem_block[i][0] + size_, remain_size]
+                                mem_tags[i] = tname
+                                mem_block[i][1] = size_
+                                mem_tags.insert(i + 1, "")
+                                mem_block.insert(i + 1, remain_block)
+                            else:
+                                mem_tags[i] = tname
+                            block_found = True
+                            break
+                if not block_found:
+                    lastidx = len(mem_tags) - 1
+                    if lastidx >= 0 and mem_tags[lastidx] == "":
+                        mem_block[lastidx][1] = size_
+                        mem_tags[lastidx] = tname
+                    else:
+                        mem_tags.append(tname)
+                        if lastidx >= 0:
+                            mem_block.append([mem_block[lastidx][0] + mem_block[lastidx][1], size_])
+                        else:
+                            mem_block.append([0, size_])
+
+                idx = mem_tags.index(tname)
+                compress_mem[tname] = mem_block[idx]
+
+        lastblock = mem_block[-1]
+        compress_size = lastblock[0] + lastblock[1]
+        # print(compress_mem)
+        # validate memory
+        for nodetensors in tensor_mem_per_node:
+            maxmem = 0
+            overlap = False
+            for tname in nodetensors:
+                block = compress_mem[tname]
+                if block[0] + block[1] > maxmem:
+                    maxmem = block[0] + block[1]
+            for tname in nodetensors:
+                block0 = compress_mem[tname]
+                for tname1 in nodetensors:
+                    if tname1 == tname:
+                        continue
+                    block1 = compress_mem[tname1]
+                    if block0[0] >= block1[0] and block0[0] < block1[0] + block1[1]:
+                        overlap = True
+                        laptensor = [tname, tname1]
+                        break
+                    if block1[0] >= block0[0] and block1[0] < block0[0] + block0[1]:
+                        overlap = True
+                        laptensor = [tname, tname1]
+                        break
+            if maxmem > compress_size:
+                warnings.warn(f'Wrong compress total memory size:{compress_size}. larger size detected:{maxmem}')
+            if overlap:
+                warnings.warn(f'Memory overlap detected!{laptensor[0]} v.s. {laptensor[1]}')
+
+        raw_memsize = 0
+        for tname in self.dynamics:
+            if tname in self.input or tname in self.output:
+                continue
+            raw_memsize += self.tensormap[tname].get_memsize()
+
+        print(f"Raw memory size: {raw_memsize:,} bytes")
+        print(f"Compressed memory size: {compress_size:,} bytes")
+        print(f'Comression ratio: {compress_size / raw_memsize * 100:.3f}%')
+        return compress_mem, compress_size
+
+    def get_compute_graph_onnx(self):
         nodes = []
         for key in self.nodemap.keys():
             node = self.nodemap[key]
             if node.shape_calc:
                 continue
             dummy_node = True
             for output in node.output:
@@ -793,18 +1056,59 @@
                 dummy_node = dummy_node and dummy
             if dummy_node:
                 continue
             nodes.append(node.name)
 
         _inputs0, _outputs0 = self.get_iotensors(nodes)
         graph_level0 = self.reorder_nodes(nodes, _inputs0)
-        subgraph = self.make_graph(graph_level0, 'compute_graph', self.input, _outputs0)
+        subgraph = self.make_graph_onnx(graph_level0, 'compute_graph', self.input, self.output)
         return subgraph
 
+    def get_compute_graph(self):
+        cg = self
+        nodes = []
+        rmnodes = []
+        for key in cg.nodemap.keys():
+            node = cg.nodemap[key]
+            if node.shape_calc:
+                rmnodes.append(key)
+                continue
+            dummy_node = True
+            for output in node.output:
+                dummy = True
+                if output in cg.consumedby.keys():
+                    for consumer in cg.consumedby[output]:
+                        if not cg.nodemap[consumer].shape_calc:
+                            dummy = False
+                            break
+                else:
+                    dummy = False
+                dummy_node = dummy_node and dummy
+            if dummy_node:
+                rmnodes.append(key)
+                continue
+            nodes.append(node.name)
+
+        for key in rmnodes:
+            cg.remove_node(key)
+        cg.graph_reorder()
+        cg.dynamics = []
+        cg.dynamics.extend(cg.input)
+        cg.dynamics.extend(cg.output)
+        for name in cg.nodemap.keys():
+            for output in cg.nodemap[name].output:
+                if name not in cg.dynamics:
+                    cg.dynamics.append(output)
+        return cg
+
     def profile(self):
+        self.valid_profile = False
+        if not self.valid_shape:
+            warnings.warn('Please perform a valid shape_infer() before profile().')
+            return
         params_flag_map = {}
         for key in self.initials:
             params_flag_map[key] = 0
 
         self.macs = 0.0
         self.params = 0
         self.memory = 0
@@ -852,16 +1156,20 @@
             node.outshape = outshape
             node.params = _params
             node.memory = _memory
             node.sparsity = block_sparsity
             self.macs += macs
             self.params += _params
             self.memory += _memory
+        self.valid_profile = True
 
     def print_node_map(self, f: str = None, metric='MACs', exclude_nodes=None):
+        if not self.valid_profile:
+            warnings.warn('Please perform a valid profile() before print_node_map().')
+            return
         from tabulate import tabulate
         assert (metric in ['MACs', 'FLOPs'])
         print_sparse_table = self.sparse_model
         saveformat = 'txt'
         splitch = 'x'
 
         if f is not None and '.csv' in f:
@@ -909,15 +1217,15 @@
 
         params += 1e-18
         macs += 1e-18
         for key in self.nodemap.keys():
             node = self.nodemap[key]
             if exclude_nodes is not None and node.op_type in exclude_nodes:
                 continue
-            row = [key]
+            row = [key, self.nodemap[key].op_type]
             if print_sparse_table:
                 sparsity = node.sparsity
                 row.append(tuple2str(sparsity['blocksize'], splitch))
                 row.append('{:.2%}'.format(sparsity['blockratio']))
                 row.append('{:.2%}'.format(sparsity['ratio']))
             row.append(num2str(int(node.macs) * factor, csvformat))
             row.append('{:.2%}'.format(node.macs / macs))
@@ -925,30 +1233,30 @@
             row.append('{:.2%}'.format(node.memory / memory))
             row.append(num2str(int(node.params), csvformat))
             row.append('{:.2%}'.format(node.params / params))
             row.append(tuple2str(node.inshape, splitch))
             row.append(tuple2str(node.outshape, splitch))
 
             ptable.append(row)
-        row = ['Total']
+        row = ['Total', '_']
         if print_sparse_table:
             row.append('_')
             row.append('_')
             row.append('_')
         row.append(num2str(int(macs * factor), csvformat))
         row.append('100%')
         row.append(num2str(int(memory), csvformat))
         row.append('100%')
         row.append(num2str(int(params), csvformat))
         row.append('100%')
         row.append('_')
         row.append('_')
 
         ptable.append(row)
-        header = ['Name']
+        header = ['Name', 'Type']
         if print_sparse_table:
             header.append('Sparse Pattern')
             header.append('Sparse Block Ratio')
             header.append('Sparse Ratio')
         header.extend([metric, 'CPercent', 'Memory', 'MPercent', 'Params', 'PPercent', 'InShape',
                        'OutShape'])
```

### Comparing `onnx-tool-0.6.1/onnx_tool/node.py` & `onnx-tool-0.6.3/onnx_tool/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,14 +862,29 @@
                                         self.strides[0],
                                         self.ceil_mode),
                     _pooling_shape_calc(inshape[3], self.pads[1] + self.pads[3], self.kernel_shape[1],
                                         self.dilations[1],
                                         self.strides[1],
                                         self.ceil_mode),
                 ]
+            if len(self.kernel_shape) == 3:
+                outshape = inshape[:2] + [
+                    _pooling_shape_calc(inshape[2], self.pads[0] + self.pads[0], self.kernel_shape[0],
+                                        self.dilations[0],
+                                        self.strides[0],
+                                        self.ceil_mode),
+                    _pooling_shape_calc(inshape[3], self.pads[1] + self.pads[1], self.kernel_shape[1],
+                                        self.dilations[1],
+                                        self.strides[1],
+                                        self.ceil_mode),
+                    _pooling_shape_calc(inshape[4], self.pads[2] + self.pads[2], self.kernel_shape[2],
+                                        self.dilations[1],
+                                        self.strides[2],
+                                        self.ceil_mode),
+                ]
         return [outshape, ]
 
     def profile(self, intensors: [], outtensors: []):
         outshape = _get_shape(outtensors[0])
         outvol = volume(outshape)
         macs = outvol * CMP_MACS * self.kernel_shape[0]
         if len(self.kernel_shape) == 2:
@@ -1337,14 +1352,22 @@
                 if len(xshape) == 4:
                     ow = math.ceil((xshape[3] - wshape[3] + 1) / self.strides[1])
                     shape += (ow,)
             else:
                 assert 0
 
         else:
+            if len(xshape) == 5:
+                od = _conv_output_shape(xshape[2], self.pads[0] + self.pads[3], wshape[2], self.strides[0],
+                                        self.dilations[0])
+                oh = _conv_output_shape(xshape[3], self.pads[1] + self.pads[4], wshape[3], self.strides[1],
+                                        self.dilations[1])
+                ow = _conv_output_shape(xshape[4], self.pads[2] + self.pads[5], wshape[4], self.strides[2],
+                                        self.dilations[2])
+                shape = (xshape[0], wshape[0], od, oh, ow)
             if len(xshape) == 4:
                 oh = _conv_output_shape(xshape[2], self.pads[0] + self.pads[2], wshape[2], self.strides[0],
                                         self.dilations[0])
                 ow = _conv_output_shape(xshape[3], self.pads[1] + self.pads[3], wshape[3], self.strides[1],
                                         self.dilations[1])
                 shape = (xshape[0], wshape[0], oh, ow)
             elif len(xshape) == 3:
@@ -1607,14 +1630,27 @@
         self.add_default_value('group', 1)
 
     def shape_infer(self, intensors: []):
         xshape = _get_shape(intensors[0])
         wshape = _get_shape(intensors[1])
         shape = []
         outc = self.group * wshape[1]
+        if len(xshape) == 5:
+            od = _convtranspose_output_shape(xshape[2], self.output_padding[0], self.pads[0] + self.pads[3], wshape[2],
+                                             self.strides[0],
+                                             self.dilations[0])
+            ow = _convtranspose_output_shape(xshape[3], self.output_padding[1], self.pads[1] + self.pads[4], wshape[3],
+                                             self.strides[1],
+                                             self.dilations[1])
+            oh = _convtranspose_output_shape(xshape[4], self.output_padding[2], self.pads[2] + self.pads[5], wshape[4],
+                                             self.strides[2],
+                                             self.dilations[2])
+            shape = [xshape[0], outc, od, ow, oh]
+            if volume(self.output_shape) != 0:
+                shape[2:] = self.output_shape
         if len(xshape) == 4:
             ow = _convtranspose_output_shape(xshape[2], self.output_padding[0], self.pads[0] + self.pads[2], wshape[2],
                                              self.strides[0],
                                              self.dilations[0])
             oh = _convtranspose_output_shape(xshape[3], self.output_padding[1], self.pads[1] + self.pads[3], wshape[3],
                                              self.strides[1],
                                              self.dilations[1])
```

### Comparing `onnx-tool-0.6.1/onnx_tool/serialization.py` & `onnx-tool-0.6.3/onnx_tool/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 def __write_float2buf(buf, f):
     ba = struct.pack('f', f)
     buf += ba
     return buf
 
 
-def __write_int2buf(buf, i):
-    ba = i.to_bytes(4, 'little', signed=True)
+def __write_int2buf(buf, i, bytes=4):
+    ba = i.to_bytes(bytes, 'little', signed=True)
     buf += ba
     return buf
 
 
-def __write_len2buf(buf, src):
-    ba = len(src).to_bytes(4, 'little', signed=True)
+def __write_len2buf(buf, src, bytes=4):
+    ba = len(src).to_bytes(bytes, 'little', signed=True)
     buf += ba
     return buf
 
 
 def __write_str2buf(buf, string):
     if not '\0' in string:
         string += '\0'
@@ -40,15 +40,15 @@
 DTYPE_UINT8 = 6
 DTYPE_INT16 = 7
 DTYPE_UINT16 = 8
 DTYPE_INT64 = 9
 
 
 def __write_data_type(buf, data):
-    if isinstance(data, str):
+    if isinstance(data, str) or isinstance(data, bytes):
         buf = __write_int2buf(buf, DTYPE_STR)
     if isinstance(data, int):
         buf = __write_int2buf(buf, DTYPE_INT)
     if isinstance(data, float):
         buf = __write_int2buf(buf, DTYPE_FLOAT)
     return buf
 
@@ -141,34 +141,48 @@
 
         writebuf = __write_len2buf(writebuf, node.attr.keys())
 
         def write_attribute(buf, attrval):
             def write_value(buf, val):
                 if isinstance(val, str):
                     buf = __write_str2buf(buf, val)
+                if isinstance(val, bytes):
+                    buf += val + b'\0'
                 if isinstance(val, int):
                     buf = __write_int2buf(buf, val)
                 if isinstance(val, float):
                     buf = __write_float2buf(buf, val)
                 return buf
 
             if not isinstance(attrval, list):
                 attrval = [attrval]
             buf = __write_len2buf(buf, attrval)
-            if isinstance(attrval, list):
-                buf = __write_data_type(buf, attrval[0])
-            else:
-                buf = __write_data_type(buf, attrval)
+            buf = __write_data_type(buf, attrval[0])
             for val in attrval:
                 buf = write_value(buf, val)
             return buf
 
         for key in node.attr.keys():
             writebuf = __write_str2buf(writebuf, key)
             writebuf = write_attribute(writebuf, node.attr[key])
     writebuf = __write_len2buf(writebuf, graph.initials)
     for name in graph.initials:
         writebuf = __write_str2buf(writebuf, name)
         tensor = graph.tensormap[name]
         writebuf = __write_ndarray(writebuf, tensor.numpy)
     binfile.write(writebuf)
     binfile.close()
+
+
+def serialize_memory_compression(compressed_mem: {}, filepath):
+    binfile = open(filepath, 'wb')
+    writebuf = bytearray(0)
+    writebuf = __write_int2buf(writebuf, compressed_mem[1], 8)
+    compress_map = compressed_mem[0]
+    writebuf = __write_len2buf(writebuf, compress_map.keys(), 8)
+    for key in compress_map.keys():
+        block = compress_map[key]
+        writebuf = __write_str2buf(writebuf, key)
+        writebuf = __write_int2buf(writebuf, block[0], 8)
+        writebuf = __write_int2buf(writebuf, block[1], 8)
+    binfile.write(writebuf)
+    binfile.close()
```

### Comparing `onnx-tool-0.6.1/onnx_tool/tensor.py` & `onnx-tool-0.6.3/onnx_tool/tensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import warnings
+
 import numpy
 import onnx
 
 from .utils import GLOBAL_VARS
 
+
 def create_ndarray_f32(shape):
     return numpy.ones(shape, dtype=numpy.float32)
 
 
 def create_ndarray_int64(shape):
     return numpy.zeros(shape, dtype=numpy.int64)
 
@@ -29,14 +32,16 @@
         shape.append(nb)
     return shape
 
 
 def onnxdtype2npdtype(data_type):
     if data_type == onnx.TensorProto.FLOAT:
         return numpy.float32
+    if data_type == onnx.TensorProto.DOUBLE:
+        return numpy.float64
     if data_type == onnx.TensorProto.FLOAT16:
         return numpy.float16
     if data_type == onnx.TensorProto.INT32:
         return numpy.int32
     if data_type == onnx.TensorProto.INT16:
         return numpy.int16
     if data_type == onnx.TensorProto.INT64:
@@ -44,15 +49,15 @@
     if data_type == onnx.TensorProto.INT8:
         return numpy.int8
     if data_type == onnx.TensorProto.UINT8:
         return numpy.uint8
     if data_type == onnx.TensorProto.BOOL:
         return numpy.bool
     if data_type == onnx.TensorProto.STRING:
-        return numpy.str
+        return numpy.string_
 
 
 def npdtype2onnxdtype(npdtype):
     if npdtype == numpy.float32:
         return onnx.TensorProto.FLOAT
     if npdtype == numpy.float64:
         return onnx.TensorProto.DOUBLE
@@ -78,31 +83,31 @@
     shape = shape_of_initializer(initial)
     ndtype = onnxdtype2npdtype(initial.data_type)
     if initial.raw_data == b'':
         arr = numpy.zeros(shape, ndtype).reshape((-1))
         if ndtype == numpy.float32:
             arr = numpy.fromiter(initial.float_data, dtype=ndtype)
 
-        if ndtype == numpy.int32:
+        elif ndtype == numpy.int32:
             arr = numpy.fromiter(initial.int32_data, dtype=ndtype)
 
-        if ndtype == numpy.float16:
+        elif ndtype == numpy.float16:
             raw = list(initial.int32_data)
             raw = numpy.fromiter(raw, dtype=numpy.uint16)
             mem = raw.tobytes()
             arr = numpy.frombuffer(mem, dtype=numpy.float16).reshape(shape)
 
-        if ndtype == numpy.int64:
+        elif ndtype == numpy.int64:
             arr = numpy.fromiter(initial.int64_data, dtype=ndtype)
 
-        if ndtype == numpy.float64:
+        elif ndtype == numpy.float64:
             arr = numpy.fromiter(initial.double_data, dtype=ndtype)
 
-        if ndtype == numpy.str:
-            arr = numpy.array(initial.string_data, dtype="S")
+        elif ndtype == numpy.string_:
+            arr = numpy.array(initial.string_data, dtype=ndtype)
     else:
         arr = numpy.frombuffer(initial.raw_data, dtype=ndtype)
     # if len(shape):
     arr = arr.reshape(shape)
     return arr
 
 def get_attribute_data(att):
@@ -360,39 +365,56 @@
             self.proto = t
             self.numpy = tensorproto2ndarray(t)
             self.shape = self.numpy.shape
             self.type = STATIC_TENSOR
         elif isinstance(t, Node):
             if t.op_type == 'Constant':
                 self.name = t.output[0]
-                self.numpy = t.value
+                self.update_proto(t.value)
                 self.shape = self.numpy.shape
                 self.type = STATIC_TENSOR
         else:
             assert 0
         self.sparsity_search()
 
     def update_tensor(self, data: numpy.ndarray):
         if not isinstance(data, numpy.ndarray):
             data = numpy.array(data)
         self.numpy = data
         self.shape = data.shape
 
+    def update_proto(self, data: numpy.ndarray):
+        self.update_tensor(data)
+        self.proto = self.make_tensor_proto()
+
     def update_shape(self, shape: list):
         if isinstance(shape, numpy.ndarray):
             assert 0
         self.shape = shape
 
+    def shape2str(self):
+        st = '['
+        for val in self.shape:
+            if isinstance(val, str):
+                st += val + ','
+            else:
+                st += str(val) + ','
+        st = st[:-1]
+        st += ']'
+        return st
+
     def get_shape(self):
         shape = []
         for s in self.shape:
             if isinstance(s, str):
                 shape.append(s)
             else:
                 shape.append(int(s))
+        if len(shape) == 0:  # scalar
+            return [1, ]
         return shape
 
     def get_valueorshape(self):
         if self.numpy is not None:
             return self.numpy
         return self.shape
 
@@ -414,19 +436,42 @@
         ratio = 0
         if (volume(shape) > thres_size) and self.numpy is not None:
             ratio = narray_calc_sparsity(self.numpy)
             if ratio is not None and ratio > thres_ratio:
                 blocksize, blockratio = search_sparse_blocksize(self.numpy, ratio, deltar_thres=0.1)
         self.sparsity = {'blocksize': blocksize, 'blockratio': blockratio, 'ratio': ratio}
 
-    def make_value_proto(self):
+    def make_value_proto(self, make_dummy=False):
         if len(self.shape) == 0:
+            if self.proto is None and make_dummy:
+                warnings.warn('Creating a dummpy tensor proto:' + self.name)
+                return onnx.helper.make_tensor_value_info(self.name, 1, None)
             return self.proto
         else:
             shape = self.get_shape()
         if self.numpy is None:
             dtype = onnx.TensorProto.FLOAT
         else:
             dtype = npdtype2onnxdtype(self.numpy.dtype)
         # shape = [int(i) for i in shape]
         vinf = onnx.helper.make_tensor_value_info(self.name, dtype, shape)
         return vinf
+
+    def make_tensor_proto(self):
+        if self.numpy is None:
+            return None
+        if len(self.numpy.shape) == 0:
+            tproto = onnx.helper.make_tensor(self.name, npdtype2onnxdtype(self.numpy.dtype)
+                                             , [], [self.numpy])
+        else:
+            tproto = onnx.helper.make_tensor(self.name, npdtype2onnxdtype(self.numpy.dtype)
+                                             , self.numpy.shape, self.numpy.flatten())
+        return tproto
+
+
+def create_initial_Tensor(name: str, ndarray: numpy.ndarray):
+    t = Tensor(name)
+    t.type = STATIC_TENSOR
+    t.numpy = ndarray
+    t.shape = t.numpy.shape
+    t.proto = t.make_tensor_proto()
+    return t
```

### Comparing `onnx-tool-0.6.1/onnx_tool/utils.py` & `onnx-tool-0.6.3/onnx_tool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import warnings
 
-VERSION = "0.6.1"
+VERSION = "0.6.3"
 
 
 class timer():
     def __init__(self):
         self._startt = time.time()
 
     def start(self):
```

### Comparing `onnx-tool-0.6.1/onnx_tool.egg-info/PKG-INFO` & `onnx-tool-0.6.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-Metadata-Version: 2.1
-Name: onnx-tool
-Version: 0.6.1
-Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
-Home-page: https://github.com/ThanatosShinji/onnx-tool
-Author: Luo Yu
-Author-email: luoyu888888@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # onnx-tool
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
+* *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: Resnet, MobileNet, YOLO, ...
@@ -89,34 +78,55 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
+## Memory Compression
+
+For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
+The compression method achieves 5% memory compression on most models.   
+For example:
+
+ model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
+-------------------------------|------------------------|----------------------------|----------------------
+ StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
+ StableDiffusion(VAE_decoder)  | 25,417                 | 1,140                      | 4.48                 
+ StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
+ StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
+ GPT2                          | 40                     | 2                          | 6.9                  
+ BERT                          | 2,170                  | 27                         | 1.25                 
+
+code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
+
+---
+
 ## Tensor operations
-* *Export weight tensors to files*  
-* *Simplify tensor and node names, convert name from a long string to a short string*  
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*  
+
+* *Export weight tensors to files*
+* *Simplify tensor and node names, convert name from a long string to a short string*
+* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
 * *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).  
+  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
 
@@ -184,8 +194,8 @@
 [FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29 | 37,056
 [MobileNet v2-1.0-fp32](https://github.com/onnx/models/blob/main/vision/classification/mobilenet) | 3.3 | 300
 [ResNet50_fp32](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25 | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

### Comparing `onnx-tool-0.6.1/setup.py` & `onnx-tool-0.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 readme = open("README.md").read()
-VERSION = "0.6.1"
+VERSION = "0.6.3"
 
 
 requirements = [
     "onnx",
     "numpy",
     'tabulate'
 ]
```

