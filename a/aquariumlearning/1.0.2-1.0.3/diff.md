# Comparing `tmp/aquariumlearning-1.0.2.tar.gz` & `tmp/aquariumlearning-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquariumlearning-1.0.2.tar", last modified: Thu Mar 23 18:37:05 2023, max compression
+gzip compressed data, was "dist/aquariumlearning-1.0.3.tar", last modified: Wed Apr 19 20:02:08 2023, max compression
```

## Comparing `aquariumlearning-1.0.2.tar` & `aquariumlearning-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/README.md
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning/
--rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/__init__.py
--rw-r--r--   0 robinyang   (501) staff       (20)    27774 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/base_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/class_map.py
--rw-r--r--   0 robinyang   (501) staff       (20)    82398 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/collection_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/coordinate_frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/dataset_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-03-23 18:34:10.000000 aquariumlearning-1.0.2/aquariumlearning/datasets.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-03-23 18:34:10.000000 aquariumlearning-1.0.2/aquariumlearning/datasharing.py
--rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/embedding_distance_sampling.py
--rw-r--r--   0 robinyang   (501) staff       (20)    36142 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17452 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/inferences.py
--rw-r--r--   0 robinyang   (501) staff       (20)    18285 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/metrics_manager.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17179 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/modified_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/sampling_agent.py
--rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/segments.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19456 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/sensor_data.py
--rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.2/aquariumlearning/turbo.py
--rw-r--r--   0 robinyang   (501) staff       (20)    18335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/util.py
--rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.2/aquariumlearning/viridis.py
--rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-03-15 18:23:45.000000 aquariumlearning-1.0.2/aquariumlearning/work_queues.py
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/SOURCES.txt
--rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/dependency_links.txt
--rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/requires.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/aquariumlearning.egg-info/top_level.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-03-23 18:37:05.000000 aquariumlearning-1.0.2/setup.cfg
--rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-03-23 18:34:46.000000 aquariumlearning-1.0.2/setup.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/README.md
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning/
+-rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/__init__.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    27866 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/base_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/class_map.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    82398 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/collection_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/coordinate_frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/dataset_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-03-27 18:45:55.000000 aquariumlearning-1.0.3/aquariumlearning/datasets.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-03-27 18:45:55.000000 aquariumlearning-1.0.3/aquariumlearning/datasharing.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/embedding_distance_sampling.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    36142 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17446 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/inferences.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    18378 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/metrics_manager.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17181 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/modified_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/sampling_agent.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/segments.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19457 2023-04-10 17:47:19.000000 aquariumlearning-1.0.3/aquariumlearning/sensor_data.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.3/aquariumlearning/turbo.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    18392 2023-04-12 17:37:02.000000 aquariumlearning-1.0.3/aquariumlearning/util.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.3/aquariumlearning/viridis.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/work_queues.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/requires.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/top_level.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/setup.cfg
+-rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/setup.py
```

### Comparing `aquariumlearning-1.0.2/PKG-INFO` & `aquariumlearning-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.2
+Version: 1.0.3
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/__init__.py` & `aquariumlearning-1.0.3/aquariumlearning/__init__.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/base_labels.py` & `aquariumlearning-1.0.3/aquariumlearning/base_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
 FRIENDLY_SENSOR_NAMES: Dict[Sensor, str] = {
     _BaseSensor2D: "2D Sensor Data",
     _BaseSensor3D: "3D Sensor Data",
     _BaseSensor: ", ".join(["2D Sensor Data", "3D Sensor Data"]),
 }
 
+Coordinate2D = Tuple[Union[int, float], Union[int, float]]
+
 
 class LabelAsset(BaseLabelAssetDict):
     pass
 
 
 class _BaseSingleCrop(_BaseEntity):
     """The base class for all crops (labels and inferences)
@@ -72,26 +74,27 @@
     _add_to_coordinate_frame: bool = False
     # check if confidence is required
     _require_confidence: Optional[bool] = False
     classification: Optional[str] = None
     classification_id: Optional[int] = None  # to also pass to the backend?
     embedding: Optional[List[float]] = None
     embedding_dim: Optional[int] = None
+    label_type: LabelType
 
     def __init__(
         self,
         id: str,
         update_type: UpdateType,
         label_type: LabelType,
         classification: Optional[str] = None,
         sensor_id: Optional[str] = None,
         coordinate_frame_id: Optional[str] = None,
         confidence: Optional[float] = None,
         iscrowd: Optional[bool] = None,
-        attributes: Dict[str, Any] = None,
+        attributes: Optional[Dict[str, Any]] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
         super().__init__(id)
 
         # validate that we're passing the right flag
         if update_type == "ADD":
@@ -296,21 +299,21 @@
     def __init__(
         self,
         update_type: UpdateType,
         id: str,
         classification: Optional[str] = None,
         sensor_id: Optional[str] = None,
         confidence: Optional[float] = None,
-        keypoints: List[Dict[KEYPOINT_KEYS, Union[int, float, str]]] = None,
+        keypoints: Optional[List[Dict[KEYPOINT_KEYS, Union[int, float, str]]]] = None,
         top: Optional[Union[int, float]] = None,
         left: Optional[Union[int, float]] = None,
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
         polygons: Optional[
-            List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]]
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
         attributes: Dict[str, Any] = {}
@@ -387,16 +390,16 @@
     def __init__(
         self,
         update_type: UpdateType,
         id: str,
         classification: Optional[str] = None,
         sensor_id: Optional[str] = None,
         confidence: Optional[float] = None,
-        polygons: List[
-            Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]
+        polygons: Optional[
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
         if polygons:
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/class_map.py` & `aquariumlearning-1.0.3/aquariumlearning/class_map.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/client.py` & `aquariumlearning-1.0.3/aquariumlearning/client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/collection_client.py` & `aquariumlearning-1.0.3/aquariumlearning/collection_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/coordinate_frames.py` & `aquariumlearning-1.0.3/aquariumlearning/coordinate_frames.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/dataset_client.py` & `aquariumlearning-1.0.3/aquariumlearning/dataset_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/datasets.py` & `aquariumlearning-1.0.3/aquariumlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/datasharing.py` & `aquariumlearning-1.0.3/aquariumlearning/datasharing.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/embedding_distance_sampling.py` & `aquariumlearning-1.0.3/aquariumlearning/embedding_distance_sampling.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/frames.py` & `aquariumlearning-1.0.3/aquariumlearning/frames.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/inferences.py` & `aquariumlearning-1.0.3/aquariumlearning/inferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 from .dataset_client import DatasetClient
 from .base_labels import (
+    Coordinate2D,
     _BaseCrop,
     _BaseSingleCrop,
     _BaseCropSet,
     _Bbox2D,
     _Classification2D,
     _Classification3D,
     _Cuboid3D,
@@ -169,15 +170,15 @@
         confidence: float,
         keypoints: List[Dict[KEYPOINT_KEYS, Union[int, float, str]]],
         top: Optional[Union[int, float]] = None,
         left: Optional[Union[int, float]] = None,
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
         polygons: Optional[
-            List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]]
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
         sensor_id: str = DEFAULT_SENSOR_ID,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
@@ -200,26 +201,26 @@
         )
 
 
 class PolygonList2DInference(_Inference, _PolygonList2D):
     """Create an inference for a 2D Polygon List.
 
     Polygons are dictionaries of the form:
-        'vertices': List of (x, y) vertices (e.g. [[x1,y1], [x2,y2], ...])
+        'vertices': List of (x, y) vertices (e.g. [(x1,y1), (x2,y2), ...])
             The polygon does not need to be closed with (x1, y1).
             As an example, a bounding box in polygon representation would look like:
 
             .. code-block::
 
                 {
                     'vertices': [
-                        [left, top],
-                        [left + width, top],
-                        [left + width, top + height],
-                        [left, top + height]
+                        (left, top),
+                        (left + width, top),
+                        (left + width, top + height),
+                        (left, top + height)
                     ]
                 }
 
     Args:
         id: Id which is unique across datasets and inferences.
         classification: The classification of this inference
         confidence: The model's confidence of the inference
@@ -233,15 +234,15 @@
 
     def __init__(
         self,
         *,
         id: str,
         classification: str,
         confidence: float,
-        polygons: List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]],
+        polygons: List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]],
         center: Optional[List[Union[int, float]]] = None,
         sensor_id: str = DEFAULT_SENSOR_ID,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
         super(PolygonList2DInference, self).__init__(
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/labels.py` & `aquariumlearning-1.0.3/aquariumlearning/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, List, Optional, Union, Tuple, cast
 
 from .dataset_client import DatasetClient
 from .base_labels import (
+    Coordinate2D,
     _BaseCrop,
     _BaseSingleCrop,
     _BaseCropSet,
     _Bbox2D,
     _Classification2D,
     _Classification3D,
     _Cuboid3D,
@@ -51,15 +52,15 @@
         *,
         id: str,
         classification: str,
         top: Union[int, float],
         left: Union[int, float],
         width: Union[int, float],
         height: Union[int, float],
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
         super(Bbox2DLabel, self).__init__(
             "ADD",
             id=id,
@@ -96,15 +97,15 @@
         *,
         id: str,
         classification: str,
         x1: Union[int, float],
         y1: Union[int, float],
         x2: Union[int, float],
         y2: Union[int, float],
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
         super(LineSegment2DLabel, self).__init__(
             "ADD",
             id,
@@ -151,18 +152,18 @@
         classification: str,
         keypoints: List[Dict[KEYPOINT_KEYS, Union[int, float, str]]],
         top: Optional[Union[int, float]] = None,
         left: Optional[Union[int, float]] = None,
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
         polygons: Optional[
-            List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]]
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
         super(Keypoint2DLabel, self).__init__(
             "ADD",
             id=id,
@@ -181,26 +182,26 @@
         )
 
 
 class PolygonList2DLabel(_Label, _PolygonList2D):
     """Create a label for a 2D polygon list for instance segmentation
 
     Polygons are dictionaries of the form:
-        'vertices': List of (x, y) vertices (e.g. [[x1,y1], [x2,y2], ...])
+        'vertices': List of (x, y) vertices (e.g. [(x1,y1), (x2,y2), ...])
             The polygon does not need to be closed with (x1, y1).
             As an example, a bounding box in polygon representation would look like:
 
             .. code-block::
 
                 {
                     'vertices': [
-                        [left, top],
-                        [left + width, top],
-                        [left + width, top + height],
-                        [left, top + height]
+                        (left, top),
+                        (left + width, top),
+                        (left + width, top + height),
+                        (left, top + height)
                     ]
                 }
 
     Args:
         id: Id which is unique across datasets and inferences.
         classification: The classification of this label
         polygons: The polygon geometry.
@@ -212,17 +213,17 @@
     """
 
     def __init__(
         self,
         *,
         id: str,
         classification: str,
-        polygons: List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]],
+        polygons: List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]],
         center: Optional[List[Union[int, float]]] = None,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
         super(PolygonList2DLabel, self).__init__(
             "ADD",
             id=id,
@@ -249,17 +250,16 @@
 
     def __init__(
         self,
         *,
         id: str,
         mask_url: str,
         resize_mode: Optional[ResizeMode] = None,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
     ):
-
         super(Semseg2DLabel, self).__init__(
             "ADD",
             id=id,
             sensor_id=sensor_id,
             mask_url=mask_url,
             resize_mode=resize_mode,
         )
@@ -279,15 +279,15 @@
     def __init__(
         self,
         *,
         id: str,
         mask_url: str,
         instances: List[InstanceSegInstance],
         resize_mode: Optional[ResizeMode] = None,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
     ):
         for instance in instances:
             if not isinstance(instance, InstanceSegInstance):
                 raise Exception(
                     "Can only add InstanceSegInstance instances to a new InstanceSeg2D Label"
                 )
 
@@ -313,15 +313,15 @@
     """
 
     def __init__(
         self,
         *,
         id: str,
         classification: str,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         secondary_labels: Optional[Dict[str, Any]] = None,
         user_attrs: Optional[Dict[str, Any]] = {},
     ):
         super(Classification2DLabel, self).__init__(
             "ADD",
             id=id,
             classification=classification,
@@ -342,15 +342,15 @@
     """
 
     def __init__(
         self,
         *,
         id: str,
         classification: str,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         user_attrs: Optional[Dict[str, Any]] = {},
     ):
         super(Classification3DLabel, self).__init__(
             "ADD",
             id=id,
             classification=classification,
             sensor_id=sensor_id,
@@ -377,15 +377,15 @@
         self,
         *,
         id: str,
         classification: str,
         position: List[float],
         dimensions: List[float],
         rotation: List[float],
-        coordinate_frame_id: str = None,
+        coordinate_frame_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = {},
         embedding: Optional[List[float]] = None,
     ):
         super(Cuboid3DLabel, self).__init__(
             "ADD",
             id=id,
@@ -419,15 +419,15 @@
         self,
         *,
         id: str,
         classification: str,
         index: int,
         token: str,
         visible: bool,
-        sensor_id: str = None,
+        sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = {},
         embedding: Optional[List[float]] = None,
     ):
         super(TextTokenLabel, self).__init__(
             "ADD",
             id=id,
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/metrics_manager.py` & `aquariumlearning-1.0.3/aquariumlearning/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/modified_labels.py` & `aquariumlearning-1.0.3/aquariumlearning/modified_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from .dataset_client import DatasetClient
 
 from .base_labels import (
+    Coordinate2D,
     _BaseCrop,
     _BaseCropSet,
     _Bbox2D,
     _Classification2D,
     _Classification3D,
     _Cuboid3D,
     _Keypoint2D,
@@ -103,15 +104,14 @@
         x2: Optional[Union[int, float]] = None,
         y2: Optional[Union[int, float]] = None,
         sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ):
-
         super(ModifiedLineSegment2DLabel, self).__init__(
             "MODIFY",
             id,
             classification=classification,
             sensor_id=sensor_id,
             x1=x1,
             x2=x2,
@@ -148,21 +148,21 @@
     """
 
     def __init__(
         self,
         *,
         id: str,
         classification: Optional[str] = None,
-        keypoints: List[Dict[KEYPOINT_KEYS, Union[int, float, str]]] = None,
+        keypoints: Optional[List[Dict[KEYPOINT_KEYS, Union[int, float, str]]]] = None,
         top: Optional[Union[int, float]] = None,
         left: Optional[Union[int, float]] = None,
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
         polygons: Optional[
-            List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]]
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
         sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
@@ -216,15 +216,15 @@
 
     def __init__(
         self,
         *,
         id: str,
         classification: Optional[str] = None,
         polygons: Optional[
-            List[Dict[POLYGON_VERTICES_KEYS, List[Tuple[Union[int, float]]]]]
+            List[Dict[POLYGON_VERTICES_KEYS, List[Coordinate2D]]]
         ] = None,
         center: Optional[List[Union[int, float]]] = None,
         sensor_id: Optional[str] = None,
         iscrowd: Optional[bool] = None,
         user_attrs: Optional[Dict[str, Any]] = None,
         embedding: Optional[List[float]] = None,
     ) -> None:
@@ -255,15 +255,14 @@
         self,
         *,
         id: str,
         mask_url: Optional[str] = None,
         resize_mode: Optional[ResizeMode] = None,
         sensor_id: Optional[str] = None,
     ):
-
         super(ModifiedSemseg2DLabel, self).__init__(
             "MODIFY",
             id=id,
             sensor_id=sensor_id,
             mask_url=mask_url,
             resize_mode=resize_mode,
         )
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/sampling_agent.py` & `aquariumlearning-1.0.3/aquariumlearning/sampling_agent.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/segments.py` & `aquariumlearning-1.0.3/aquariumlearning/segments.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/sensor_data.py` & `aquariumlearning-1.0.3/aquariumlearning/sensor_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,15 @@
         )
 
 
 SensorData2D = Union[Image, ImageOverlay]
 SensorData3D = Union[PointCloudPCD, PointCloudBins, Obj]
 SensorData = Union[SensorData2D, SensorData3D, Text, Audio, Video]
 
+
 # TODO: figure out a less fragile way to do this? we're lucky in that we don't change any of the kwarg names when keying into metadata
 def _get_sensor_data_from_json(
     sd_json: Dict[str, Any], coordinate_frames_by_id: Dict[str, CoordinateFrame] = {}
 ) -> SensorData:
     sensor_id = sd_json["sensor_id"]
     sensor_metadata = sd_json["sensor_metadata"]
     sensor_type = sd_json["sensor_type"]
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/turbo.py` & `aquariumlearning-1.0.3/aquariumlearning/turbo.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/util.py` & `aquariumlearning-1.0.3/aquariumlearning/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,14 +538,15 @@
     ClassificationWithGeometry = "CLASSIFICATION_WITH_GEOMETRY"
     Null = None
 
     def _is_classification(self) -> bool:
         return self in [
             PrimaryTaskTypes.Classification,
             PrimaryTaskTypes.BinaryClassification,
+            PrimaryTaskTypes.ClassificationWithGeometry,
         ]
 
 
 class EmbeddingDistanceMetric(Enum):
     COSINE = "cosine"
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning/viridis.py` & `aquariumlearning-1.0.3/aquariumlearning/viridis.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning/work_queues.py` & `aquariumlearning-1.0.3/aquariumlearning/work_queues.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/aquariumlearning.egg-info/PKG-INFO` & `aquariumlearning-1.0.3/aquariumlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.2
+Version: 1.0.3
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.2/aquariumlearning.egg-info/SOURCES.txt` & `aquariumlearning-1.0.3/aquariumlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.2/setup.py` & `aquariumlearning-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aquariumlearning",  # Replace with your own username
-    version="1.0.2",
+    version="1.0.3",
     author="Quinn Johnson",
     author_email="quinn@aquarium-learn.com",
     description="Aquarium Learning Python Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aquariumlearning.com",
     packages=setuptools.find_packages(
```

