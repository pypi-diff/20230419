# Comparing `tmp/segment-anything-py-0.2.tar.gz` & `tmp/segment-anything-py-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-anything-py-0.2.tar", last modified: Wed Apr 19 01:43:47 2023, max compression
+gzip compressed data, was "segment-anything-py-0.3.tar", last modified: Wed Apr 19 01:47:27 2023, max compression
```

## Comparing `segment-anything-py-0.2.tar` & `segment-anything-py-0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:43:47.932587 segment-anything-py-0.2/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.2/LICENSE
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      629 2023-04-19 01:43:47.932587 segment-anything-py-0.2/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8488 2023-04-18 22:22:47.000000 segment-anything-py-0.2/README.md
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:43:47.929254 segment-anything-py-0.2/segment_anything/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/build_sam.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:43:47.929254 segment-anything-py-0.2/segment_anything/modeling/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/common.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/sam.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/modeling/transformer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/predictor.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:43:47.932587 segment-anything-py-0.2/segment_anything/utils/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/utils/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/utils/amg.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/utils/onnx.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.2/segment_anything/utils/transforms.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:43:47.932587 segment-anything-py-0.2/segment_anything_py.egg-info/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      629 2023-04-19 01:43:47.000000 segment-anything-py-0.2/segment_anything_py.egg-info/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      794 2023-04-19 01:43:47.000000 segment-anything-py-0.2/segment_anything_py.egg-info/SOURCES.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 01:43:47.000000 segment-anything-py-0.2/segment_anything_py.egg-info/dependency_links.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 01:43:47.000000 segment-anything-py-0.2/segment_anything_py.egg-info/requires.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 01:43:47.000000 segment-anything-py-0.2/segment_anything_py.egg-info/top_level.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 01:43:47.932587 segment-anything-py-0.2/setup.cfg
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1189 2023-04-19 01:43:44.000000 segment-anything-py-0.2/setup.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:47:27.518407 segment-anything-py-0.3/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11357 2023-04-18 22:22:47.000000 segment-anything-py-0.3/LICENSE
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9158 2023-04-19 01:47:27.518407 segment-anything-py-0.3/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8488 2023-04-18 22:22:47.000000 segment-anything-py-0.3/README.md
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:47:27.515074 segment-anything-py-0.3/segment_anything/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      427 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    15148 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     2941 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/build_sam.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:47:27.515074 segment-anything-py-0.3/segment_anything/modeling/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      385 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1479 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/common.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    14420 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     6615 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8594 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     7226 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/sam.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     8397 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/modeling/transformer.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    11649 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/predictor.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:47:27.518407 segment-anything-py-0.3/segment_anything/utils/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      197 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/utils/__init__.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)    12712 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/utils/amg.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     5812 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/utils/onnx.py
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     3972 2023-04-18 22:22:47.000000 segment-anything-py-0.3/segment_anything/utils/transforms.py
+drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1001)        0 2023-04-19 01:47:27.518407 segment-anything-py-0.3/segment_anything_py.egg-info/
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     9158 2023-04-19 01:47:27.000000 segment-anything-py-0.3/segment_anything_py.egg-info/PKG-INFO
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      794 2023-04-19 01:47:27.000000 segment-anything-py-0.3/segment_anything_py.egg-info/SOURCES.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)        1 2023-04-19 01:47:27.000000 segment-anything-py-0.3/segment_anything_py.egg-info/dependency_links.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      120 2023-04-19 01:47:27.000000 segment-anything-py-0.3/segment_anything_py.egg-info/requires.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)       17 2023-04-19 01:47:27.000000 segment-anything-py-0.3/segment_anything_py.egg-info/top_level.txt
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)      430 2023-04-19 01:47:27.518407 segment-anything-py-0.3/setup.cfg
+-rw-r--r--   0 qiusheng  (1000) qiusheng  (1001)     1341 2023-04-19 01:47:20.000000 segment-anything-py-0.3/setup.py
```

### Comparing `segment-anything-py-0.2/LICENSE` & `segment-anything-py-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/README.md` & `segment-anything-py-0.3/README.md`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/automatic_mask_generator.py` & `segment-anything-py-0.3/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/build_sam.py` & `segment-anything-py-0.3/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/common.py` & `segment-anything-py-0.3/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/image_encoder.py` & `segment-anything-py-0.3/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/mask_decoder.py` & `segment-anything-py-0.3/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/prompt_encoder.py` & `segment-anything-py-0.3/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/sam.py` & `segment-anything-py-0.3/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/modeling/transformer.py` & `segment-anything-py-0.3/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/predictor.py` & `segment-anything-py-0.3/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/utils/amg.py` & `segment-anything-py-0.3/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/utils/onnx.py` & `segment-anything-py-0.3/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything/utils/transforms.py` & `segment-anything-py-0.3/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/segment_anything_py.egg-info/SOURCES.txt` & `segment-anything-py-0.3/segment_anything_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segment-anything-py-0.2/setup.py` & `segment-anything-py-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from setuptools import find_packages, setup
 
+with open("README.md") as readme_file:
+    readme = readme_file.read()
+
 setup(
     author="Qiusheng Wu",
     author_email="giswqs@gmail.com",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -18,16 +21,18 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="A unofficial Python package for Meta AI's Segment Anything Model",
     rl="https://github.com/opengeos/segment-anything",
     name="segment-anything-py",
-    version="0.2",
+    version="0.3",
     install_requires=["torch>=1.7", "torchvision>=0.8"],
     license="MIT license",
+    long_description=readme,
+    long_description_content_type="text/markdown",
     packages=find_packages(exclude="notebooks"),
     extras_require={
         "all": ["matplotlib", "pycocotools", "opencv-python", "onnx", "onnxruntime"],
         "dev": ["flake8", "isort", "black", "mypy"],
     },
 )
```

