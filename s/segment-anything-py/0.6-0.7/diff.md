# Comparing `tmp/segment-anything-py-0.6.tar.gz` & `tmp/segment-anything-py-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-anything-py-0.6.tar", last modified: Wed Apr 19 01:57:26 2023, max compression
+gzip compressed data, was "segment-anything-py-0.7.tar", last modified: Wed Apr 19 02:07:55 2023, max compression
```

## Comparing `segment-anything-py-0.6.tar` & `segment-anything-py-0.7.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:57:26.699085 segment-anything-py-0.6/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.6/LICENSE
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       26 2023-04-19 01:56:34.000000 segment-anything-py-0.6/MANIFEST.in
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9483 2023-04-19 01:57:26.699085 segment-anything-py-0.6/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8813 2023-04-19 01:54:04.000000 segment-anything-py-0.6/README.md
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:57:26.699085 segment-anything-py-0.6/segment_anything/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/build_sam.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:57:26.699085 segment-anything-py-0.6/segment_anything/modeling/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/common.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/sam.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/modeling/transformer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/predictor.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:57:26.699085 segment-anything-py-0.6/segment_anything/utils/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/utils/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/utils/amg.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/utils/onnx.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.6/segment_anything/utils/transforms.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:57:26.699085 segment-anything-py-0.6/segment_anything_py.egg-info/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9483 2023-04-19 01:57:26.000000 segment-anything-py-0.6/segment_anything_py.egg-info/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      806 2023-04-19 01:57:26.000000 segment-anything-py-0.6/segment_anything_py.egg-info/SOURCES.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 01:57:26.000000 segment-anything-py-0.6/segment_anything_py.egg-info/dependency_links.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 01:57:26.000000 segment-anything-py-0.6/segment_anything_py.egg-info/requires.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 01:57:26.000000 segment-anything-py-0.6/segment_anything_py.egg-info/top_level.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 01:57:26.699085 segment-anything-py-0.6/setup.cfg
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1341 2023-04-19 01:57:24.000000 segment-anything-py-0.6/setup.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 02:07:55.668839 segment-anything-py-0.7/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.7/LICENSE
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9540 2023-04-19 02:07:55.668839 segment-anything-py-0.7/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8813 2023-04-19 01:54:04.000000 segment-anything-py-0.7/README.md
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 02:07:55.668839 segment-anything-py-0.7/segment_anything/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/build_sam.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 02:07:55.668839 segment-anything-py-0.7/segment_anything/modeling/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/common.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/sam.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/modeling/transformer.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/predictor.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 02:07:55.668839 segment-anything-py-0.7/segment_anything/utils/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/utils/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/utils/amg.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/utils/onnx.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.7/segment_anything/utils/transforms.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 02:07:55.668839 segment-anything-py-0.7/segment_anything_py.egg-info/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9540 2023-04-19 02:07:55.000000 segment-anything-py-0.7/segment_anything_py.egg-info/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      794 2023-04-19 02:07:55.000000 segment-anything-py-0.7/segment_anything_py.egg-info/SOURCES.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 02:07:55.000000 segment-anything-py-0.7/segment_anything_py.egg-info/dependency_links.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 02:07:55.000000 segment-anything-py-0.7/segment_anything_py.egg-info/requires.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 02:07:55.000000 segment-anything-py-0.7/segment_anything_py.egg-info/top_level.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 02:07:55.668839 segment-anything-py-0.7/setup.cfg
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1343 2023-04-19 02:07:48.000000 segment-anything-py-0.7/setup.py
```

### Comparing `segment-anything-py-0.6/LICENSE` & `segment-anything-py-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/PKG-INFO` & `segment-anything-py-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.6
-Summary: A unofficial Python package for Meta AI's Segment Anything Model
+Version: 0.7
+Summary: An unofficial Python package for Meta AI's Segment Anything Model
+Home-page: https://github.com/opengeos/segment-anything
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `segment-anything-py-0.6/README.md` & `segment-anything-py-0.7/README.md`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/automatic_mask_generator.py` & `segment-anything-py-0.7/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/build_sam.py` & `segment-anything-py-0.7/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/common.py` & `segment-anything-py-0.7/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/image_encoder.py` & `segment-anything-py-0.7/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/mask_decoder.py` & `segment-anything-py-0.7/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/prompt_encoder.py` & `segment-anything-py-0.7/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/sam.py` & `segment-anything-py-0.7/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/modeling/transformer.py` & `segment-anything-py-0.7/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/predictor.py` & `segment-anything-py-0.7/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/utils/amg.py` & `segment-anything-py-0.7/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/utils/onnx.py` & `segment-anything-py-0.7/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything/utils/transforms.py` & `segment-anything-py-0.7/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.6/segment_anything_py.egg-info/PKG-INFO` & `segment-anything-py-0.7/segment_anything_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: segment-anything-py
-Version: 0.6
-Summary: A unofficial Python package for Meta AI's Segment Anything Model
+Version: 0.7
+Summary: An unofficial Python package for Meta AI's Segment Anything Model
+Home-page: https://github.com/opengeos/segment-anything
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `segment-anything-py-0.6/segment_anything_py.egg-info/SOURCES.txt` & `segment-anything-py-0.7/segment_anything_py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 setup.cfg
 setup.py
 segment_anything/__init__.py
 segment_anything/automatic_mask_generator.py
 segment_anything/build_sam.py
 segment_anything/predictor.py
```

### Comparing `segment-anything-py-0.6/setup.py` & `segment-anything-py-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    description="A unofficial Python package for Meta AI's Segment Anything Model",
-    rl="https://github.com/opengeos/segment-anything",
+    description="An unofficial Python package for Meta AI's Segment Anything Model",
+    url="https://github.com/opengeos/segment-anything",
     name="segment-anything-py",
-    version="0.6",
+    version="0.7",
     install_requires=["torch>=1.7", "torchvision>=0.8"],
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude="notebooks"),
     extras_require={
         "all": ["matplotlib", "pycocotools", "opencv-python", "onnx", "onnxruntime"],
```

