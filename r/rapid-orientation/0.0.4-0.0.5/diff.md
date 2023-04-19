# Comparing `tmp/rapid_orientation-0.0.4-py3-none-any.whl.zip` & `tmp/rapid_orientation-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6289282 bytes, number of entries: 10
--rw-r--r--  2.0 unx      122 b- defN 23-Feb-12 06:42 rapid_orientation/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Feb-12 06:42 rapid_orientation/config.yaml
--rw-r--r--  2.0 unx     2644 b- defN 23-Feb-12 06:42 rapid_orientation/rapid_orientation.py
--rw-r--r--  2.0 unx     5730 b- defN 23-Feb-12 06:42 rapid_orientation/utils.py
+Zip file size: 6289346 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-19 02:02 rapid_orientation/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Apr-19 02:02 rapid_orientation/config.yaml
+-rw-r--r--  2.0 unx     2644 b- defN 23-Apr-19 02:02 rapid_orientation/rapid_orientation.py
+-rw-r--r--  2.0 unx     5730 b- defN 23-Apr-19 02:02 rapid_orientation/utils.py
 -rw-rw-r--  2.0 unx  6792721 b- defN 23-Jan-20 13:53 rapid_orientation/models/rapid_orientation.onnx
--rw-r--r--  2.0 unx     2514 b- defN 23-Feb-12 06:43 rapid_orientation-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-12 06:43 rapid_orientation-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Feb-12 06:43 rapid_orientation-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Feb-12 06:43 rapid_orientation-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      898 b- defN 23-Feb-12 06:43 rapid_orientation-0.0.4.dist-info/RECORD
-10 files, 6805168 bytes uncompressed, 6287726 bytes compressed:  7.6%
+-rw-r--r--  2.0 unx     2725 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      898 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/RECORD
+10 files, 6805379 bytes uncompressed, 6287790 bytes compressed:  7.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_orientation/utils.py
 Comment: 
 
 Filename: rapid_orientation/models/rapid_orientation.onnx
 Comment: 
 
-Filename: rapid_orientation-0.0.4.dist-info/METADATA
+Filename: rapid_orientation-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: rapid_orientation-0.0.4.dist-info/WHEEL
+Filename: rapid_orientation-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_orientation-0.0.4.dist-info/entry_points.txt
+Filename: rapid_orientation-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.4.dist-info/top_level.txt
+Filename: rapid_orientation-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.4.dist-info/RECORD
+Filename: rapid_orientation-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapid_orientation-0.0.4.dist-info/METADATA` & `rapid_orientation-0.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: rapid-orientation
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for classifying the direction of images containing text based ONNXRuntime.
-Home-page: https://github.com/RapidAI/RapidOCR
+Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,layout,rapidocr,rapid_orientation
 Platform: Any
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6,<=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: onnxruntime (>=1.7.0)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: opencv-python (>=4.5.1.48)
 Requires-Dist: numpy (>=1.21.6)
 
-## rapid-orientation Package
-<p>
+## rapid-orientation
+<p align="left">
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-orientation/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-orientation"></a>
+    <a href="https://pepy.tech/project/rapid-orientation"><img src="https://static.pepy.tech/personalized-badge/rapid-orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### 1. Install package by pypi.
 ```bash
 $ pip install rapid-orientation
 ```
 
 ### 2. Run by script.
 - RapidOrientation has the default `model_path` value, you can set the different value of `model_path` to use different models, e.g. `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')`
-- See details, for [README_Layout](https://github.com/RapidAI/RapidOCR/blob/f133ff008a1c60edd6e0ed882da83873aa7b113a/python/rapid_structure/docs/README_Layout.md) .
-- 📌 `layout.png` source: [link](https://github.com/RapidAI/RapidOCR/blob/f133ff008a1c60edd6e0ed882da83873aa7b113a/python/rapid_structure/test_images/layout.png)
+- See details, for [README_Layout](https://github.com/RapidAI/RapidStructure/blob/main/docs/README_Orientation.md) .
+- 📌 `layout.png` source: [link](https://github.com/RapidAI/RapidStructure/blob/main/test_images/layout.png)
 
 ```python
 import cv2
 from rapid_orientation import RapidOrientation
 
 orientation_engine = RapidOrientation()
```

### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.4 Summary: Tools for
+Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.5 Summary: Tools for
 classifying the direction of images containing text based ONNXRuntime. Home-
-page: https://github.com/RapidAI/RapidOCR Author: SWHL Author-email:
+page: https://github.com/RapidAI/RapidStructure Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Keywords:
 ppstructure,layout,rapidocr,rapid_orientation Platform: Any Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Requires-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-
-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) ## rapid-
-orientation Package
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: >=3.6,<=3.10 Description-Content-Type: text/
+markdown Requires-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0)
+Requires-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) ##
+rapid-orientation
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
-img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI]
+img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
+static.pepy.tech/personalized-badge/rapid-
+orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### 1. Install package by pypi. ```bash $ pip install rapid-orientation ``` ###
 2. Run by script. - RapidOrientation has the default `model_path` value, you
 can set the different value of `model_path` to use different models, e.g.
 `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')` -
-See details, for [README_Layout](https://github.com/RapidAI/RapidOCR/blob/
-f133ff008a1c60edd6e0ed882da83873aa7b113a/python/rapid_structure/docs/
-README_Layout.md) . - ð `layout.png` source: [link](https://github.com/
-RapidAI/RapidOCR/blob/f133ff008a1c60edd6e0ed882da83873aa7b113a/python/
-rapid_structure/test_images/layout.png) ```python import cv2 from
-rapid_orientation import RapidOrientation orientation_engine = RapidOrientation
-() img = cv2.imread('test_images/layout.png') orientation_res, elapse =
-orientation_engine(img) print(orientation_res) ``` ### 3. Run by command line.
-- Usage: ```bash $ rapid_orientation -h usage: rapid_orientation [-h] -img
-IMG_PATH [-m MODEL_PATH] optional arguments: -h, --help show this help message
-and exit -img IMG_PATH, --img_path IMG_PATH Path to image for layout. -
-m MODEL_PATH, --model_path MODEL_PATH The model path used for inference ``` -
-Example: ```bash $ rapid_orientation -img layout.png ``` ### 4. Result.
-```python # Return str, four types:ï¼0 | 90 | 180 | 270 ```
+See details, for [README_Layout](https://github.com/RapidAI/RapidStructure/
+blob/main/docs/README_Orientation.md) . - ð `layout.png` source: [link]
+(https://github.com/RapidAI/RapidStructure/blob/main/test_images/layout.png)
+```python import cv2 from rapid_orientation import RapidOrientation
+orientation_engine = RapidOrientation() img = cv2.imread('test_images/
+layout.png') orientation_res, elapse = orientation_engine(img) print
+(orientation_res) ``` ### 3. Run by command line. - Usage: ```bash $
+rapid_orientation -h usage: rapid_orientation [-h] -img IMG_PATH [-
+m MODEL_PATH] optional arguments: -h, --help show this help message and exit -
+img IMG_PATH, --img_path IMG_PATH Path to image for layout. -m MODEL_PATH, --
+model_path MODEL_PATH The model path used for inference ``` - Example: ```bash
+$ rapid_orientation -img layout.png ``` ### 4. Result. ```python # Return str,
+four types:ï¼0 | 90 | 180 | 270 ```
```

