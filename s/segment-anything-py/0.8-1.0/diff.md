# Comparing `tmp/segment-anything-py-0.8.tar.gz` & `tmp/segment-anything-py-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-anything-py-0.8.tar", last modified: Wed Apr 19 02:19:48 2023, max compression
+gzip compressed data, was "segment-anything-py-1.0.tar", last modified: Wed Apr 19 02:25:46 2023, max compression
```

## Comparing `segment-anything-py-0.8.tar` & `segment-anything-py-1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:19:48.976925 segment-anything-py-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:19:37.000000 segment-anything-py-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-19 02:19:48.976925 segment-anything-py-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-19 02:19:37.000000 segment-anything-py-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:19:48.976925 segment-anything-py-0.8/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:19:48.976925 segment-anything-py-0.8/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:19:48.976925 segment-anything-py-0.8/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-19 02:19:37.000000 segment-anything-py-0.8/segment_anything/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:19:48.976925 segment-anything-py-0.8/segment_anything_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-19 02:19:48.000000 segment-anything-py-0.8/segment_anything_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 02:19:48.000000 segment-anything-py-0.8/segment_anything_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:19:48.000000 segment-anything-py-0.8/segment_anything_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 02:19:48.000000 segment-anything-py-0.8/segment_anything_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 02:19:48.000000 segment-anything-py-0.8/segment_anything_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-19 02:19:48.976925 segment-anything-py-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-19 02:19:37.000000 segment-anything-py-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:25:46.680804 segment-anything-py-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:25:30.000000 segment-anything-py-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-19 02:25:46.684804 segment-anything-py-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-19 02:25:30.000000 segment-anything-py-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:25:46.680804 segment-anything-py-1.0/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:25:46.680804 segment-anything-py-1.0/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:25:46.680804 segment-anything-py-1.0/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-19 02:25:30.000000 segment-anything-py-1.0/segment_anything/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:25:46.680804 segment-anything-py-1.0/segment_anything_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-19 02:25:46.000000 segment-anything-py-1.0/segment_anything_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 02:25:46.000000 segment-anything-py-1.0/segment_anything_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:25:46.000000 segment-anything-py-1.0/segment_anything_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 02:25:46.000000 segment-anything-py-1.0/segment_anything_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 02:25:46.000000 segment-anything-py-1.0/segment_anything_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-19 02:25:46.684804 segment-anything-py-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-19 02:25:30.000000 segment-anything-py-1.0/setup.py
```

### Comparing `segment-anything-py-0.8/LICENSE` & `segment-anything-py-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/PKG-INFO` & `segment-anything-py-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.8
+Version: 1.0
 Summary: An unofficial Python package for Meta AI's Segment Anything Model
 Home-page: https://github.com/opengeos/segment-anything
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segment-anything-py-0.8/README.md` & `segment-anything-py-1.0/README.md`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/automatic_mask_generator.py` & `segment-anything-py-1.0/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/build_sam.py` & `segment-anything-py-1.0/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/common.py` & `segment-anything-py-1.0/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/image_encoder.py` & `segment-anything-py-1.0/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/mask_decoder.py` & `segment-anything-py-1.0/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/prompt_encoder.py` & `segment-anything-py-1.0/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/sam.py` & `segment-anything-py-1.0/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/modeling/transformer.py` & `segment-anything-py-1.0/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/predictor.py` & `segment-anything-py-1.0/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/utils/amg.py` & `segment-anything-py-1.0/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/utils/onnx.py` & `segment-anything-py-1.0/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything/utils/transforms.py` & `segment-anything-py-1.0/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/segment_anything_py.egg-info/PKG-INFO` & `segment-anything-py-1.0/segment_anything_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.8
+Version: 1.0
 Summary: An unofficial Python package for Meta AI's Segment Anything Model
 Home-page: https://github.com/opengeos/segment-anything
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `segment-anything-py-0.8/segment_anything_py.egg-info/SOURCES.txt` & `segment-anything-py-1.0/segment_anything_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.8/setup.py` & `segment-anything-py-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="An unofficial Python package for Meta AI's Segment Anything Model",
     url="https://github.com/opengeos/segment-anything",
     name="segment-anything-py",
-    version="0.8",
+    version="1.0",
     install_requires=["torch>=1.7", "torchvision>=0.8"],
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude="notebooks"),
     extras_require={
         "all": ["matplotlib", "pycocotools", "opencv-python", "onnx", "onnxruntime"],
```

