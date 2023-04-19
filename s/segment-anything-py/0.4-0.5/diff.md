# Comparing `tmp/segment-anything-py-0.4.tar.gz` & `tmp/segment-anything-py-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-anything-py-0.4.tar", last modified: Wed Apr 19 01:49:32 2023, max compression
+gzip compressed data, was "segment-anything-py-0.5.tar", last modified: Wed Apr 19 01:54:28 2023, max compression
```

## Comparing `segment-anything-py-0.4.tar` & `segment-anything-py-0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.993225 segment-anything-py-0.4/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.4/LICENSE
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       26 2023-04-19 01:49:19.000000 segment-anything-py-0.4/MANIFEST.in
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9158 2023-04-19 01:49:32.993225 segment-anything-py-0.4/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8488 2023-04-18 22:22:47.000000 segment-anything-py-0.4/README.md
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.989892 segment-anything-py-0.4/assets/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  3703371 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/masks1.png
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   133278 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/masks2.jpg
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  2015643 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/minidemo.gif
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   581875 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/model_diagram.png
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   874274 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/notebook1.png
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  1221706 2023-04-18 22:22:47.000000 segment-anything-py-0.4/assets/notebook2.png
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.993225 segment-anything-py-0.4/segment_anything/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/build_sam.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.993225 segment-anything-py-0.4/segment_anything/modeling/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/common.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/sam.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/modeling/transformer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/predictor.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.993225 segment-anything-py-0.4/segment_anything/utils/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/utils/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/utils/amg.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/utils/onnx.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.4/segment_anything/utils/transforms.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:49:32.993225 segment-anything-py-0.4/segment_anything_py.egg-info/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9158 2023-04-19 01:49:32.000000 segment-anything-py-0.4/segment_anything_py.egg-info/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      929 2023-04-19 01:49:32.000000 segment-anything-py-0.4/segment_anything_py.egg-info/SOURCES.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 01:49:32.000000 segment-anything-py-0.4/segment_anything_py.egg-info/dependency_links.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 01:49:32.000000 segment-anything-py-0.4/segment_anything_py.egg-info/requires.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 01:49:32.000000 segment-anything-py-0.4/segment_anything_py.egg-info/top_level.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 01:49:32.993225 segment-anything-py-0.4/setup.cfg
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1341 2023-04-19 01:49:26.000000 segment-anything-py-0.4/setup.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.226842 segment-anything-py-0.5/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.5/LICENSE
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:52:31.000000 segment-anything-py-0.5/MANIFEST.in
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9483 2023-04-19 01:54:28.226842 segment-anything-py-0.5/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8813 2023-04-19 01:54:04.000000 segment-anything-py-0.5/README.md
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.223508 segment-anything-py-0.5/assets/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  3703371 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/masks1.png
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   133278 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/masks2.jpg
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  2015643 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/minidemo.gif
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   581875 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/model_diagram.png
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)   874274 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/notebook1.png
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)  1221706 2023-04-18 22:22:47.000000 segment-anything-py-0.5/assets/notebook2.png
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.223508 segment-anything-py-0.5/segment_anything/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/build_sam.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.223508 segment-anything-py-0.5/segment_anything/modeling/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/common.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/sam.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/modeling/transformer.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/predictor.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.226842 segment-anything-py-0.5/segment_anything/utils/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/utils/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/utils/amg.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/utils/onnx.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.5/segment_anything/utils/transforms.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:54:28.226842 segment-anything-py-0.5/segment_anything_py.egg-info/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9483 2023-04-19 01:54:28.000000 segment-anything-py-0.5/segment_anything_py.egg-info/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      929 2023-04-19 01:54:28.000000 segment-anything-py-0.5/segment_anything_py.egg-info/SOURCES.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 01:54:28.000000 segment-anything-py-0.5/segment_anything_py.egg-info/dependency_links.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 01:54:28.000000 segment-anything-py-0.5/segment_anything_py.egg-info/requires.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 01:54:28.000000 segment-anything-py-0.5/segment_anything_py.egg-info/top_level.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 01:54:28.226842 segment-anything-py-0.5/setup.cfg
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1341 2023-04-19 01:52:23.000000 segment-anything-py-0.5/setup.py
```

### Comparing `segment-anything-py-0.4/LICENSE` & `segment-anything-py-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/PKG-INFO` & `segment-anything-py-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.4
+Version: 0.5
 Summary: A unofficial Python package for Meta AI's Segment Anything Model
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -22,21 +22,21 @@
 
 **[Meta AI Research, FAIR](https://ai.facebook.com/research/)**
 
 [Alexander Kirillov](https://alexander-kirillov.github.io/), [Eric Mintun](https://ericmintun.github.io/), [Nikhila Ravi](https://nikhilaravi.com/), [Hanzi Mao](https://hanzimao.me/), Chloe Rolland, Laura Gustafson, [Tete Xiao](https://tetexiao.com), [Spencer Whitehead](https://www.spencerwhitehead.com/), Alex Berg, Wan-Yen Lo, [Piotr Dollar](https://pdollar.github.io/), [Ross Girshick](https://www.rossgirshick.info/)
 
 [[`Paper`](https://ai.facebook.com/research/publications/segment-anything/)] [[`Project`](https://segment-anything.com/)] [[`Demo`](https://segment-anything.com/demo)] [[`Dataset`](https://segment-anything.com/dataset/index.html)] [[`Blog`](https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/)] [[`BibTeX`](#citing-segment-anything)]
 
-![SAM design](assets/model_diagram.png?raw=true)
+![SAM design](https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/model_diagram.png?raw=true)
 
 The **Segment Anything Model (SAM)** produces high quality object masks from input prompts such as points or boxes, and it can be used to generate masks for all objects in an image. It has been trained on a [dataset](https://segment-anything.com/dataset/index.html) of 11 million images and 1.1 billion masks, and has strong zero-shot performance on a variety of segmentation tasks.
 
 <p float="left">
-  <img src="assets/masks1.png?raw=true" width="37.25%" />
-  <img src="assets/masks2.jpg?raw=true" width="61.5%" /> 
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks1.png?raw=true" width="37.25%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks2.jpg?raw=true" width="61.5%" /> 
 </p>
 
 ## Installation
 
 The code requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions [here](https://pytorch.org/get-started/locally/) to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
 Install Segment Anything:
@@ -84,16 +84,16 @@
 ```
 python scripts/amg.py --checkpoint <path/to/checkpoint> --model-type <model_type> --input <image_or_folder> --output <path/to/output>
 ```
 
 See the examples notebooks on [using SAM with prompts](/notebooks/predictor_example.ipynb) and [automatically generating masks](/notebooks/automatic_mask_generator_example.ipynb) for more details.
 
 <p float="left">
-  <img src="assets/notebook1.png?raw=true" width="49.1%" />
-  <img src="assets/notebook2.png?raw=true" width="48.9%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook1.png?raw=true" width="49.1%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook2.png?raw=true" width="48.9%" />
 </p>
 
 ## ONNX Export
 
 SAM's lightweight mask decoder can be exported to ONNX format so that it can be run in any environment that supports ONNX runtime, such as in-browser as showcased in the [demo](https://segment-anything.com/demo). Export the model with
 
 ```
```

### Comparing `segment-anything-py-0.4/README.md` & `segment-anything-py-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 **[Meta AI Research, FAIR](https://ai.facebook.com/research/)**
 
 [Alexander Kirillov](https://alexander-kirillov.github.io/), [Eric Mintun](https://ericmintun.github.io/), [Nikhila Ravi](https://nikhilaravi.com/), [Hanzi Mao](https://hanzimao.me/), Chloe Rolland, Laura Gustafson, [Tete Xiao](https://tetexiao.com), [Spencer Whitehead](https://www.spencerwhitehead.com/), Alex Berg, Wan-Yen Lo, [Piotr Dollar](https://pdollar.github.io/), [Ross Girshick](https://www.rossgirshick.info/)
 
 [[`Paper`](https://ai.facebook.com/research/publications/segment-anything/)] [[`Project`](https://segment-anything.com/)] [[`Demo`](https://segment-anything.com/demo)] [[`Dataset`](https://segment-anything.com/dataset/index.html)] [[`Blog`](https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/)] [[`BibTeX`](#citing-segment-anything)]
 
-![SAM design](assets/model_diagram.png?raw=true)
+![SAM design](https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/model_diagram.png?raw=true)
 
 The **Segment Anything Model (SAM)** produces high quality object masks from input prompts such as points or boxes, and it can be used to generate masks for all objects in an image. It has been trained on a [dataset](https://segment-anything.com/dataset/index.html) of 11 million images and 1.1 billion masks, and has strong zero-shot performance on a variety of segmentation tasks.
 
 <p float="left">
-  <img src="assets/masks1.png?raw=true" width="37.25%" />
-  <img src="assets/masks2.jpg?raw=true" width="61.5%" /> 
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks1.png?raw=true" width="37.25%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks2.jpg?raw=true" width="61.5%" /> 
 </p>
 
 ## Installation
 
 The code requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions [here](https://pytorch.org/get-started/locally/) to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
 Install Segment Anything:
@@ -64,16 +64,16 @@
 ```
 python scripts/amg.py --checkpoint <path/to/checkpoint> --model-type <model_type> --input <image_or_folder> --output <path/to/output>
 ```
 
 See the examples notebooks on [using SAM with prompts](/notebooks/predictor_example.ipynb) and [automatically generating masks](/notebooks/automatic_mask_generator_example.ipynb) for more details.
 
 <p float="left">
-  <img src="assets/notebook1.png?raw=true" width="49.1%" />
-  <img src="assets/notebook2.png?raw=true" width="48.9%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook1.png?raw=true" width="49.1%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook2.png?raw=true" width="48.9%" />
 </p>
 
 ## ONNX Export
 
 SAM's lightweight mask decoder can be exported to ONNX format so that it can be run in any environment that supports ONNX runtime, such as in-browser as showcased in the [demo](https://segment-anything.com/demo). Export the model with
 
 ```
```

### Comparing `segment-anything-py-0.4/assets/masks1.png` & `segment-anything-py-0.5/assets/masks1.png`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/assets/masks2.jpg` & `segment-anything-py-0.5/assets/masks2.jpg`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/assets/minidemo.gif` & `segment-anything-py-0.5/assets/minidemo.gif`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/assets/model_diagram.png` & `segment-anything-py-0.5/assets/model_diagram.png`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/assets/notebook1.png` & `segment-anything-py-0.5/assets/notebook1.png`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/assets/notebook2.png` & `segment-anything-py-0.5/assets/notebook2.png`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/automatic_mask_generator.py` & `segment-anything-py-0.5/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/build_sam.py` & `segment-anything-py-0.5/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/common.py` & `segment-anything-py-0.5/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/image_encoder.py` & `segment-anything-py-0.5/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/mask_decoder.py` & `segment-anything-py-0.5/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/prompt_encoder.py` & `segment-anything-py-0.5/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/sam.py` & `segment-anything-py-0.5/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/modeling/transformer.py` & `segment-anything-py-0.5/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/predictor.py` & `segment-anything-py-0.5/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/utils/amg.py` & `segment-anything-py-0.5/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/utils/onnx.py` & `segment-anything-py-0.5/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything/utils/transforms.py` & `segment-anything-py-0.5/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/segment_anything_py.egg-info/PKG-INFO` & `segment-anything-py-0.5/segment_anything_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.4
+Version: 0.5
 Summary: A unofficial Python package for Meta AI's Segment Anything Model
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -22,21 +22,21 @@
 
 **[Meta AI Research, FAIR](https://ai.facebook.com/research/)**
 
 [Alexander Kirillov](https://alexander-kirillov.github.io/), [Eric Mintun](https://ericmintun.github.io/), [Nikhila Ravi](https://nikhilaravi.com/), [Hanzi Mao](https://hanzimao.me/), Chloe Rolland, Laura Gustafson, [Tete Xiao](https://tetexiao.com), [Spencer Whitehead](https://www.spencerwhitehead.com/), Alex Berg, Wan-Yen Lo, [Piotr Dollar](https://pdollar.github.io/), [Ross Girshick](https://www.rossgirshick.info/)
 
 [[`Paper`](https://ai.facebook.com/research/publications/segment-anything/)] [[`Project`](https://segment-anything.com/)] [[`Demo`](https://segment-anything.com/demo)] [[`Dataset`](https://segment-anything.com/dataset/index.html)] [[`Blog`](https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/)] [[`BibTeX`](#citing-segment-anything)]
 
-![SAM design](assets/model_diagram.png?raw=true)
+![SAM design](https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/model_diagram.png?raw=true)
 
 The **Segment Anything Model (SAM)** produces high quality object masks from input prompts such as points or boxes, and it can be used to generate masks for all objects in an image. It has been trained on a [dataset](https://segment-anything.com/dataset/index.html) of 11 million images and 1.1 billion masks, and has strong zero-shot performance on a variety of segmentation tasks.
 
 <p float="left">
-  <img src="assets/masks1.png?raw=true" width="37.25%" />
-  <img src="assets/masks2.jpg?raw=true" width="61.5%" /> 
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks1.png?raw=true" width="37.25%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/masks2.jpg?raw=true" width="61.5%" /> 
 </p>
 
 ## Installation
 
 The code requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions [here](https://pytorch.org/get-started/locally/) to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
 Install Segment Anything:
@@ -84,16 +84,16 @@
 ```
 python scripts/amg.py --checkpoint <path/to/checkpoint> --model-type <model_type> --input <image_or_folder> --output <path/to/output>
 ```
 
 See the examples notebooks on [using SAM with prompts](/notebooks/predictor_example.ipynb) and [automatically generating masks](/notebooks/automatic_mask_generator_example.ipynb) for more details.
 
 <p float="left">
-  <img src="assets/notebook1.png?raw=true" width="49.1%" />
-  <img src="assets/notebook2.png?raw=true" width="48.9%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook1.png?raw=true" width="49.1%" />
+  <img src="https://raw.githubusercontent.com/opengeos/segment-anything/pypi/assets/notebook2.png?raw=true" width="48.9%" />
 </p>
 
 ## ONNX Export
 
 SAM's lightweight mask decoder can be exported to ONNX format so that it can be run in any environment that supports ONNX runtime, such as in-browser as showcased in the [demo](https://segment-anything.com/demo). Export the model with
 
 ```
```

### Comparing `segment-anything-py-0.4/segment_anything_py.egg-info/SOURCES.txt` & `segment-anything-py-0.5/segment_anything_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.4/setup.py` & `segment-anything-py-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="A unofficial Python package for Meta AI's Segment Anything Model",
     rl="https://github.com/opengeos/segment-anything",
     name="segment-anything-py",
-    version="0.4",
+    version="0.5",
     install_requires=["torch>=1.7", "torchvision>=0.8"],
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude="notebooks"),
     extras_require={
         "all": ["matplotlib", "pycocotools", "opencv-python", "onnx", "onnxruntime"],
```

