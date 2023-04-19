# Comparing `tmp/viddiffusion-0.1.0.tar.gz` & `tmp/viddiffusion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viddiffusion-0.1.0.tar", last modified: Wed Apr 19 06:10:38 2023, max compression
+gzip compressed data, was "viddiffusion-0.1.1.tar", last modified: Wed Apr 19 06:13:22 2023, max compression
```

## Comparing `viddiffusion-0.1.0.tar` & `viddiffusion-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:10:38.155029 viddiffusion-0.1.0/
--rw-r--r--   0 masaishi   (501) staff       (20)    11357 2023-04-18 02:31:33.000000 viddiffusion-0.1.0/LICENSE
--rw-r--r--   0 masaishi   (501) staff       (20)     7652 2023-04-19 06:10:38.154697 viddiffusion-0.1.0/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)     7160 2023-04-19 06:09:52.000000 viddiffusion-0.1.0/README.md
--rw-r--r--   0 masaishi   (501) staff       (20)       38 2023-04-19 06:10:38.155088 viddiffusion-0.1.0/setup.cfg
--rw-r--r--   0 masaishi   (501) staff       (20)      834 2023-04-18 18:52:48.000000 viddiffusion-0.1.0/setup.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:10:38.153607 viddiffusion-0.1.0/viddiffusion/
--rw-r--r--   0 masaishi   (501) staff       (20)       78 2023-04-19 06:08:08.000000 viddiffusion-0.1.0/viddiffusion/__init__.py
--rw-r--r--   0 masaishi   (501) staff       (20)      723 2023-04-18 18:31:45.000000 viddiffusion-0.1.0/viddiffusion/image_utils.py
--rw-r--r--   0 masaishi   (501) staff       (20)     8484 2023-04-19 03:58:47.000000 viddiffusion-0.1.0/viddiffusion/pipeline_viddiffusion.py
--rw-r--r--   0 masaishi   (501) staff       (20)     2824 2023-04-18 18:32:08.000000 viddiffusion-0.1.0/viddiffusion/video_utils.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:10:38.154393 viddiffusion-0.1.0/viddiffusion.egg-info/
--rw-r--r--   0 masaishi   (501) staff       (20)     7652 2023-04-19 06:10:38.000000 viddiffusion-0.1.0/viddiffusion.egg-info/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)      324 2023-04-19 06:10:38.000000 viddiffusion-0.1.0/viddiffusion.egg-info/SOURCES.txt
--rw-r--r--   0 masaishi   (501) staff       (20)        1 2023-04-19 06:10:38.000000 viddiffusion-0.1.0/viddiffusion.egg-info/dependency_links.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       66 2023-04-19 06:10:38.000000 viddiffusion-0.1.0/viddiffusion.egg-info/requires.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       13 2023-04-19 06:10:38.000000 viddiffusion-0.1.0/viddiffusion.egg-info/top_level.txt
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.754214 viddiffusion-0.1.1/
+-rw-r--r--   0 masaishi   (501) staff       (20)    11357 2023-04-18 02:31:33.000000 viddiffusion-0.1.1/LICENSE
+-rw-r--r--   0 masaishi   (501) staff       (20)     7653 2023-04-19 06:13:22.754057 viddiffusion-0.1.1/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)     7161 2023-04-19 06:12:03.000000 viddiffusion-0.1.1/README.md
+-rw-r--r--   0 masaishi   (501) staff       (20)       38 2023-04-19 06:13:22.754265 viddiffusion-0.1.1/setup.cfg
+-rw-r--r--   0 masaishi   (501) staff       (20)      834 2023-04-18 18:52:48.000000 viddiffusion-0.1.1/setup.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.753104 viddiffusion-0.1.1/viddiffusion/
+-rw-r--r--   0 masaishi   (501) staff       (20)       78 2023-04-19 06:13:05.000000 viddiffusion-0.1.1/viddiffusion/__init__.py
+-rw-r--r--   0 masaishi   (501) staff       (20)      723 2023-04-18 18:31:45.000000 viddiffusion-0.1.1/viddiffusion/image_utils.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     8484 2023-04-19 03:58:47.000000 viddiffusion-0.1.1/viddiffusion/pipeline_viddiffusion.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     2824 2023-04-18 18:32:08.000000 viddiffusion-0.1.1/viddiffusion/video_utils.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2023-04-19 06:13:22.753825 viddiffusion-0.1.1/viddiffusion.egg-info/
+-rw-r--r--   0 masaishi   (501) staff       (20)     7653 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)      324 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)        1 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       66 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/requires.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       13 2023-04-19 06:13:22.000000 viddiffusion-0.1.1/viddiffusion.egg-info/top_level.txt
```

### Comparing `viddiffusion-0.1.0/LICENSE` & `viddiffusion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.0/PKG-INFO` & `viddiffusion-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viddiffusion
-Version: 0.1.0
+Version: 0.1.1
 Summary: VidDiffusion is a Python library that provides vid2vid pipeline by using Hugging Face's `diffusers`.
 Home-page: https://github.com/masaishi/VidDiffusion
 Author: Masamune Ishihara
 Author-email: masaishi_masa@yahoo.co.jp
 Maintainer: Masamune Ishihara
 Maintainer-email: masaishi_masa@yahoo.co.jp
 License: Apache License 2.0
@@ -21,14 +21,15 @@
 ### Openjourney V4
 
 
 
 https://user-images.githubusercontent.com/1396267/232981471-33406bff-6b2b-44d8-a294-7b8268c57552.mov
 
 
+
 ### Anime style
 
 
 https://user-images.githubusercontent.com/1396267/232980819-02f7e15a-af37-4d2d-a66d-f82f4163eb87.mov
 
 
 Original Video: https://mixkit.co/free-stock-video/girl-dancing-with-her-headphones-while-taking-a-walk-4823/
```

### Comparing `viddiffusion-0.1.0/README.md` & `viddiffusion-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ### Openjourney V4
 
 
 
 https://user-images.githubusercontent.com/1396267/232981471-33406bff-6b2b-44d8-a294-7b8268c57552.mov
 
 
+
 ### Anime style
 
 
 https://user-images.githubusercontent.com/1396267/232980819-02f7e15a-af37-4d2d-a66d-f82f4163eb87.mov
 
 
 Original Video: https://mixkit.co/free-stock-video/girl-dancing-with-her-headphones-while-taking-a-walk-4823/
```

### Comparing `viddiffusion-0.1.0/setup.py` & `viddiffusion-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.0/viddiffusion/image_utils.py` & `viddiffusion-0.1.1/viddiffusion/image_utils.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.0/viddiffusion/pipeline_viddiffusion.py` & `viddiffusion-0.1.1/viddiffusion/pipeline_viddiffusion.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.0/viddiffusion/video_utils.py` & `viddiffusion-0.1.1/viddiffusion/video_utils.py`

 * *Files identical despite different names*

### Comparing `viddiffusion-0.1.0/viddiffusion.egg-info/PKG-INFO` & `viddiffusion-0.1.1/viddiffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viddiffusion
-Version: 0.1.0
+Version: 0.1.1
 Summary: VidDiffusion is a Python library that provides vid2vid pipeline by using Hugging Face's `diffusers`.
 Home-page: https://github.com/masaishi/VidDiffusion
 Author: Masamune Ishihara
 Author-email: masaishi_masa@yahoo.co.jp
 Maintainer: Masamune Ishihara
 Maintainer-email: masaishi_masa@yahoo.co.jp
 License: Apache License 2.0
@@ -21,14 +21,15 @@
 ### Openjourney V4
 
 
 
 https://user-images.githubusercontent.com/1396267/232981471-33406bff-6b2b-44d8-a294-7b8268c57552.mov
 
 
+
 ### Anime style
 
 
 https://user-images.githubusercontent.com/1396267/232980819-02f7e15a-af37-4d2d-a66d-f82f4163eb87.mov
 
 
 Original Video: https://mixkit.co/free-stock-video/girl-dancing-with-her-headphones-while-taking-a-walk-4823/
```

