# Comparing `tmp/supervision-0.5.2.tar.gz` & `tmp/supervision-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.5.2.tar", last modified: Thu Apr 13 08:57:26 2023, max compression
+gzip compressed data, was "supervision-0.6.0.tar", last modified: Wed Apr 19 21:02:56 2023, max compression
```

## Comparing `supervision-0.5.2.tar` & `supervision-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.829212 supervision-0.5.2/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.5.2/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-13 08:57:26.829055 supervision-0.5.2/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.5.2/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-13 08:57:26.829270 supervision-0.5.2/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.5.2/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.823825 supervision-0.5.2/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)      876 2023-04-13 08:56:47.000000 supervision-0.5.2/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.824981 supervision-0.5.2/supervision/annotation/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-05 15:18:58.000000 supervision-0.5.2/supervision/annotation/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3279 2023-04-05 15:18:58.000000 supervision-0.5.2/supervision/annotation/voc.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.825698 supervision-0.5.2/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6166 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    14744 2023-04-13 08:56:47.000000 supervision-0.5.2/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7162 2023-04-13 08:46:01.000000 supervision-0.5.2/supervision/detection/line_counter.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.825971 supervision-0.5.2/supervision/detection/tools/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/tools/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5058 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/tools/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5527 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.826380 supervision-0.5.2/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.5.2/supervision/draw/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.826779 supervision-0.5.2/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.2/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/geometry/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827054 supervision-0.5.2/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.5.2/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.5.2/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.824705 supervision-0.5.2/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     1007 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-13 08:57:26.000000 supervision-0.5.2/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827198 supervision-0.5.2/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.827782 supervision-0.5.2/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.2/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.5.2/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     4916 2023-03-14 12:33:54.000000 supervision-0.5.2/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.828265 supervision-0.5.2/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.2/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.5.2/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-13 08:57:26.828685 supervision-0.5.2/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.2/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.5.2/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.969612 supervision-0.6.0/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.6.0/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-19 21:02:56.969431 supervision-0.6.0/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.6.0/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-19 21:02:56.969689 supervision-0.6.0/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.6.0/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.959638 supervision-0.6.0/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1044 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.961377 supervision-0.6.0/supervision/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/dataset/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5189 2023-04-19 21:02:26.000000 supervision-0.6.0/supervision/dataset/core.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.961966 supervision-0.6.0/supervision/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5912 2023-04-19 21:02:26.000000 supervision-0.6.0/supervision/dataset/formats/pascal_voc.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.963585 supervision-0.6.0/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6171 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    14736 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7162 2023-04-13 08:46:01.000000 supervision-0.6.0/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.963997 supervision-0.6.0/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.6.0/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9634 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.965674 supervision-0.6.0/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.6.0/supervision/draw/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      621 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/file.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.966660 supervision-0.6.0/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.6.0/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/geometry/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967008 supervision-0.6.0/supervision/notebook/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/supervision/notebook/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.6.0/supervision/notebook/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.960948 supervision-0.6.0/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1104 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967269 supervision-0.6.0/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967812 supervision-0.6.0/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.6.0/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.6.0/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.6.0/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.968124 supervision-0.6.0/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.6.0/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.969039 supervision-0.6.0/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.6.0/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.6.0/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.5.2/LICENSE.md` & `supervision-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/PKG-INFO` & `supervision-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.5.2
+Version: 0.6.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.5.2 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.6.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.5.2/README.md` & `supervision-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/setup.py` & `supervision-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/detection/annotate.py` & `supervision-0.6.0/supervision/detection/annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,18 @@
             scene (np.ndarray): The image on which the masks will be overlaid
             detections (Detections): The detections for which the masks will be overlaid
             opacity (float): The opacity of the masks, between 0 and 1, default is 0.5
 
         Returns:
             np.ndarray: The image with the masks overlaid
         """
-        for i in range(len(detections.xyxy)):
-            if detections.mask is None:
-                continue
+        if detections.mask is None:
+            return scene
 
+        for i in np.flip(np.argsort(detections.area)):
             class_id = (
                 detections.class_id[i] if detections.class_id is not None else None
             )
             idx = class_id if class_id is not None else i
             color = (
                 self.color.by_idx(idx)
                 if isinstance(self.color, ColorPalette)
```

### Comparing `supervision-0.5.2/supervision/detection/core.py` & `supervision-0.6.0/supervision/detection/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, Iterator, List, Optional, Tuple, Union
+from typing import Any, Iterator, List, Optional, Tuple
 
 import numpy as np
 
 from supervision.detection.utils import non_max_suppression, xywh_to_xyxy
 from supervision.geometry.core import Position
 
 
@@ -47,27 +47,26 @@
         raise ValueError("tracker_id must be None or 1d np.ndarray with (n,) shape")
 
 
 @dataclass
 class Detections:
     """
     Data class containing information about the detections in a video frame.
-
     Attributes:
         xyxy (np.ndarray): An array of shape `(n, 4)` containing the bounding boxes coordinates in format `[x1, y1, x2, y2]`
         mask: (Optional[np.ndarray]): An array of shape `(n, W, H)` containing the segmentation masks.
-        class_id (Optional[np.ndarray]): An array of shape `(n,)` containing the class ids of the detections.
         confidence (Optional[np.ndarray]): An array of shape `(n,)` containing the confidence scores of the detections.
+        class_id (Optional[np.ndarray]): An array of shape `(n,)` containing the class ids of the detections.
         tracker_id (Optional[np.ndarray]): An array of shape `(n,)` containing the tracker ids of the detections.
     """
 
     xyxy: np.ndarray
     mask: np.Optional[np.ndarray] = None
-    class_id: Optional[np.ndarray] = None
     confidence: Optional[np.ndarray] = None
+    class_id: Optional[np.ndarray] = None
     tracker_id: Optional[np.ndarray] = None
 
     def __post_init__(self):
         n = len(self.xyxy)
         _validate_xyxy(xyxy=self.xyxy, n=n)
         _validate_mask(mask=self.mask, n=n)
         _validate_class_id(class_id=self.class_id, n=n)
```

### Comparing `supervision-0.5.2/supervision/detection/line_counter.py` & `supervision-0.6.0/supervision/detection/line_counter.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/detection/tools/polygon_zone.py` & `supervision-0.6.0/supervision/detection/tools/polygon_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import replace
 from typing import Optional, Tuple
 
 import cv2
 import numpy as np
 
 from supervision import Detections
-from supervision.detection.utils import clip_boxes, generate_2d_mask
+from supervision.detection.utils import clip_boxes, polygon_to_mask
 from supervision.draw.color import Color
 from supervision.draw.utils import draw_polygon, draw_text
 from supervision.geometry.core import Position
 from supervision.geometry.utils import get_polygon_center
 
 
 class PolygonZone:
@@ -32,15 +32,15 @@
     ):
         self.polygon = polygon
         self.frame_resolution_wh = frame_resolution_wh
         self.triggering_position = triggering_position
         self.current_count = 0
 
         width, height = frame_resolution_wh
-        self.mask = generate_2d_mask(
+        self.mask = polygon_to_mask(
             polygon=polygon, resolution_wh=(width + 1, height + 1)
         )
 
     def trigger(self, detections: Detections) -> np.ndarray:
         """
         Determines if the detections are within the polygon zone.
```

### Comparing `supervision-0.5.2/supervision/draw/color.py` & `supervision-0.6.0/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/draw/utils.py` & `supervision-0.6.0/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/geometry/core.py` & `supervision-0.6.0/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/geometry/utils.py` & `supervision-0.6.0/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/notebook/utils.py` & `supervision-0.6.0/supervision/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision/video.py` & `supervision-0.6.0/supervision/video.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/supervision.egg-info/PKG-INFO` & `supervision-0.6.0/supervision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.5.2
+Version: 0.6.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.5.2 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.6.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.5.2/supervision.egg-info/SOURCES.txt` & `supervision-0.6.0/supervision.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE.md
 README.md
 setup.py
 supervision/__init__.py
+supervision/file.py
 supervision/video.py
 supervision.egg-info/PKG-INFO
 supervision.egg-info/SOURCES.txt
 supervision.egg-info/dependency_links.txt
 supervision.egg-info/requires.txt
 supervision.egg-info/top_level.txt
-supervision/annotation/__init__.py
-supervision/annotation/voc.py
+supervision/dataset/__init__.py
+supervision/dataset/core.py
+supervision/dataset/formats/__init__.py
+supervision/dataset/formats/pascal_voc.py
 supervision/detection/__init__.py
 supervision/detection/annotate.py
 supervision/detection/core.py
 supervision/detection/line_counter.py
 supervision/detection/utils.py
 supervision/detection/tools/__init__.py
 supervision/detection/tools/polygon_zone.py
```

### Comparing `supervision-0.5.2/test/detection/test_core.py` & `supervision-0.6.0/test/detection/test_core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/test/draw/test_color.py` & `supervision-0.6.0/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.5.2/test/geometry/test_dataclasses.py` & `supervision-0.6.0/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

