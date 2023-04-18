# Comparing `tmp/foxglove-schemas-protobuf-0.0.3.tar.gz` & `tmp/foxglove-schemas-protobuf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-schemas-protobuf-0.0.3.tar", last modified: Tue Nov 29 17:28:58 2022, max compression
+gzip compressed data, was "foxglove-schemas-protobuf-0.1.0.tar", last modified: Tue Apr 18 22:45:48 2023, max compression
```

## Comparing `foxglove-schemas-protobuf-0.0.3.tar` & `foxglove-schemas-protobuf-0.1.0.tar`

### file list

```diff
@@ -1,84 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:28:58.855772 foxglove-schemas-protobuf-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-11-29 17:28:58.855772 foxglove-schemas-protobuf-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2022-11-29 17:28:25.000000 foxglove-schemas-protobuf-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:28:58.851772 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CameraCalibration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Color_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Color_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CompressedImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CubePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/FrameTransform_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/GeoJSON_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Grid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Grid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/KeyValuePair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LaserScan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LaserScan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LinePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LocationFix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LocationFix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PackedElementField_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointCloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointCloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PoseInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Pose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Pose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PosesInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Quaternion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Quaternion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/RawImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/RawImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneUpdate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TextPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-11-29 17:28:54.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-29 17:28:25.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-29 17:28:25.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 17:28:58.855772 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-11-29 17:28:58.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2022-11-29 17:28:58.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 17:28:58.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-11-29 17:28:58.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-11-29 17:28:58.000000 foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-11-29 17:28:25.000000 foxglove-schemas-protobuf-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2022-11-29 17:28:58.855772 foxglove-schemas-protobuf-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 22:45:48.243672 foxglove-schemas-protobuf-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/tests/test_schemas.py
```

### Comparing `foxglove-schemas-protobuf-0.0.3/PKG-INFO` & `foxglove-schemas-protobuf-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.0.3
+Version: 0.1.0
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 
 ```bash
 pipenv install foxglove-schemas-protobuf
 ```
 
 ## Usage
 
-Import types from the `foxglove` module as follows:
+Import types from the `foxglove_schemas_protobuf` module as follows:
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
```

### Comparing `foxglove-schemas-protobuf-0.0.3/README.md` & `foxglove-schemas-protobuf-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```bash
 pipenv install foxglove-schemas-protobuf
 ```
 
 ## Usage
 
-Import types from the `foxglove` module as follows:
+Import types from the `foxglove_schemas_protobuf` module as follows:
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CameraCalibration_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CircleAnnotation_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     FILL_COLOR_FIELD_NUMBER: builtins.int
     OUTLINE_COLOR_FIELD_NUMBER: builtins.int
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Timestamp of circle"""
     @property
     def position(self) -> foxglove_Point2_pb2.Point2:
-        """Center of the circle in 2D image coordinates"""
+        """Center of the circle in 2D image coordinates (pixels)"""
     diameter: builtins.float
-    """Circle diameter"""
+    """Circle diameter in pixels"""
     thickness: builtins.float
-    """Line thickness"""
+    """Line thickness in pixels"""
     @property
     def fill_color(self) -> foxglove_Color_pb2.Color:
         """Fill color"""
     @property
     def outline_color(self) -> foxglove_Color_pb2.Color:
         """Outline color"""
     def __init__(
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Color_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Color_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CompressedImage_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CompressedImage_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CubePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/FrameTransform_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/FrameTransform_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/GeoJSON_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/GeoJSON_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Grid_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Grid_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         """Size of single grid cell along x and y axes, relative to `pose`"""
     row_stride: builtins.int
     """Number of bytes between rows in `data`"""
     cell_stride: builtins.int
     """Number of bytes between cells within a row in `data`"""
     @property
     def fields(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_PackedElementField_pb2.PackedElementField]:
-        """Fields in `data`"""
+        """Fields in `data`. `red`, `green`, `blue`, and `alpha` are optional for customizing the grid's color."""
     data: builtins.bytes
     """Grid cell data, interpreted using `fields`, in row-major (y-major) order"""
     def __init__(
         self,
         *,
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         frame_id: builtins.str = ...,
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ImageAnnotations_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import CircleAnnotation_pb2 as foxglove_dot_CircleAnnotation__pb2
 from . import PointsAnnotation_pb2 as foxglove_dot_PointsAnnotation__pb2
+from . import TextAnnotation_pb2 as foxglove_dot_TextAnnotation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66oxglove/ImageAnnotations.proto\x12\x08\x66oxglove\x1a\x1f\x66oxglove/CircleAnnotation.proto\x1a\x1f\x66oxglove/PointsAnnotation.proto\"k\n\x10ImageAnnotations\x12+\n\x07\x63ircles\x18\x01 \x03(\x0b\x32\x1a.foxglove.CircleAnnotation\x12*\n\x06points\x18\x02 \x03(\x0b\x32\x1a.foxglove.PointsAnnotationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66oxglove/ImageAnnotations.proto\x12\x08\x66oxglove\x1a\x1f\x66oxglove/CircleAnnotation.proto\x1a\x1f\x66oxglove/PointsAnnotation.proto\x1a\x1d\x66oxglove/TextAnnotation.proto\"\x94\x01\n\x10ImageAnnotations\x12+\n\x07\x63ircles\x18\x01 \x03(\x0b\x32\x1a.foxglove.CircleAnnotation\x12*\n\x06points\x18\x02 \x03(\x0b\x32\x1a.foxglove.PointsAnnotation\x12\'\n\x05texts\x18\x03 \x03(\x0b\x32\x18.foxglove.TextAnnotationb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'foxglove.ImageAnnotations_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _IMAGEANNOTATIONS._serialized_start=111
-  _IMAGEANNOTATIONS._serialized_end=218
+  _IMAGEANNOTATIONS._serialized_start=143
+  _IMAGEANNOTATIONS._serialized_end=291
 # @@protoc_insertion_point(module_scope)
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Generated by https://github.com/foxglove/schemas"""
 import builtins
 import collections.abc
 from . import CircleAnnotation_pb2 as foxglove_CircleAnnotation_pb2
 from . import PointsAnnotation_pb2 as foxglove_PointsAnnotation_pb2
+from . import TextAnnotation_pb2 as foxglove_TextAnnotation_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
@@ -22,22 +23,27 @@
 class ImageAnnotations(google.protobuf.message.Message):
     """Array of annotations for a 2D image"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CIRCLES_FIELD_NUMBER: builtins.int
     POINTS_FIELD_NUMBER: builtins.int
+    TEXTS_FIELD_NUMBER: builtins.int
     @property
     def circles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_CircleAnnotation_pb2.CircleAnnotation]:
         """Circle annotations"""
     @property
     def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_PointsAnnotation_pb2.PointsAnnotation]:
         """Points annotations"""
+    @property
+    def texts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_TextAnnotation_pb2.TextAnnotation]:
+        """Text annotations"""
     def __init__(
         self,
         *,
         circles: collections.abc.Iterable[foxglove_CircleAnnotation_pb2.CircleAnnotation] | None = ...,
         points: collections.abc.Iterable[foxglove_PointsAnnotation_pb2.PointsAnnotation] | None = ...,
+        texts: collections.abc.Iterable[foxglove_TextAnnotation_pb2.TextAnnotation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["circles", b"circles", "points", b"points"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["circles", b"circles", "points", b"points", "texts", b"texts"]) -> None: ...
 
 global___ImageAnnotations = ImageAnnotations
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/KeyValuePair_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LaserScan_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LaserScan_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LinePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,29 @@
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[LinePrimitive._Type.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         LINE_STRIP: LinePrimitive._Type.ValueType  # 0
-        """0-1, 1-2, ..., (n-1)-n"""
+        """Connected line segments: 0-1, 1-2, ..., (n-1)-n"""
         LINE_LOOP: LinePrimitive._Type.ValueType  # 1
-        """0-1, 1-2, ..., (n-1)-n, n-0"""
+        """Closed polygon: 0-1, 1-2, ..., (n-1)-n, n-0"""
         LINE_LIST: LinePrimitive._Type.ValueType  # 2
-        """0-1, 2-3, 4-5, ..."""
+        """Individual line segments: 0-1, 2-3, 4-5, ..."""
 
     class Type(_Type, metaclass=_TypeEnumTypeWrapper):
         """An enumeration indicating how input points should be interpreted to create lines"""
 
     LINE_STRIP: LinePrimitive.Type.ValueType  # 0
-    """0-1, 1-2, ..., (n-1)-n"""
+    """Connected line segments: 0-1, 1-2, ..., (n-1)-n"""
     LINE_LOOP: LinePrimitive.Type.ValueType  # 1
-    """0-1, 1-2, ..., (n-1)-n, n-0"""
+    """Closed polygon: 0-1, 1-2, ..., (n-1)-n, n-0"""
     LINE_LIST: LinePrimitive.Type.ValueType  # 2
-    """0-1, 2-3, 4-5, ..."""
+    """Individual line segments: 0-1, 2-3, 4-5, ..."""
 
     TYPE_FIELD_NUMBER: builtins.int
     POSE_FIELD_NUMBER: builtins.int
     THICKNESS_FIELD_NUMBER: builtins.int
     SCALE_INVARIANT_FIELD_NUMBER: builtins.int
     POINTS_FIELD_NUMBER: builtins.int
     COLOR_FIELD_NUMBER: builtins.int
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LocationFix_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/LocationFix_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Log_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Log_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ModelPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PackedElementField_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PackedElementField_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point2_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point2_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point3_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Point3_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointCloud_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointCloud_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @property
     def pose(self) -> foxglove_Pose_pb2.Pose:
         """The origin of the point cloud relative to the frame of reference"""
     point_stride: builtins.int
     """Number of bytes between points in the `data`"""
     @property
     def fields(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_PackedElementField_pb2.PackedElementField]:
-        """Fields in the `data`"""
+        """Fields in `data`. At least 2 coordinate fields from `x`, `y`, and `z` are required for each point's position; `red`, `green`, `blue`, and `alpha` are optional for customizing each point's color."""
     data: builtins.bytes
     """Point data, interpreted using `fields`"""
     def __init__(
         self,
         *,
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         frame_id: builtins.str = ...,
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointsAnnotation_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -31,26 +31,34 @@
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[PointsAnnotation._Type.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         UNKNOWN: PointsAnnotation._Type.ValueType  # 0
         POINTS: PointsAnnotation._Type.ValueType  # 1
+        """Individual points: 0, 1, 2, ..."""
         LINE_LOOP: PointsAnnotation._Type.ValueType  # 2
+        """Closed polygon: 0-1, 1-2, ..., (n-1)-n, n-0"""
         LINE_STRIP: PointsAnnotation._Type.ValueType  # 3
+        """Connected line segments: 0-1, 1-2, ..., (n-1)-n"""
         LINE_LIST: PointsAnnotation._Type.ValueType  # 4
+        """Individual line segments: 0-1, 2-3, 4-5, ..."""
 
     class Type(_Type, metaclass=_TypeEnumTypeWrapper):
         """Type of points annotation"""
 
     UNKNOWN: PointsAnnotation.Type.ValueType  # 0
     POINTS: PointsAnnotation.Type.ValueType  # 1
+    """Individual points: 0, 1, 2, ..."""
     LINE_LOOP: PointsAnnotation.Type.ValueType  # 2
+    """Closed polygon: 0-1, 1-2, ..., (n-1)-n, n-0"""
     LINE_STRIP: PointsAnnotation.Type.ValueType  # 3
+    """Connected line segments: 0-1, 1-2, ..., (n-1)-n"""
     LINE_LIST: PointsAnnotation.Type.ValueType  # 4
+    """Individual line segments: 0-1, 2-3, 4-5, ..."""
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     POINTS_FIELD_NUMBER: builtins.int
     OUTLINE_COLOR_FIELD_NUMBER: builtins.int
     OUTLINE_COLORS_FIELD_NUMBER: builtins.int
     FILL_COLOR_FIELD_NUMBER: builtins.int
@@ -58,26 +66,26 @@
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Timestamp of annotation"""
     type: global___PointsAnnotation.Type.ValueType
     """Type of points annotation to draw"""
     @property
     def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_Point2_pb2.Point2]:
-        """Points in 2D image coordinates"""
+        """Points in 2D image coordinates (pixels)"""
     @property
     def outline_color(self) -> foxglove_Color_pb2.Color:
         """Outline color"""
     @property
     def outline_colors(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_Color_pb2.Color]:
         """Per-point colors, if `type` is `POINTS`, or per-segment stroke colors, if `type` is `LINE_LIST`."""
     @property
     def fill_color(self) -> foxglove_Color_pb2.Color:
         """Fill color"""
     thickness: builtins.float
-    """Stroke thickness"""
+    """Stroke thickness in pixels"""
     def __init__(
         self,
         *,
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         type: global___PointsAnnotation.Type.ValueType = ...,
         points: collections.abc.Iterable[foxglove_Point2_pb2.Point2] | None = ...,
         outline_color: foxglove_Color_pb2.Color | None = ...,
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PoseInFrame_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Pose_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Pose_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PosesInFrame_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Quaternion_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Quaternion_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/RawImage_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/RawImage_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntity_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneEntity_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneUpdate_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SpherePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TextPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector2_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector2_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector3_pb2.py` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf/Vector3_pb2.pyi` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/PKG-INFO` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.0.3
+Version: 0.1.0
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 
 ```bash
 pipenv install foxglove-schemas-protobuf
 ```
 
 ## Usage
 
-Import types from the `foxglove` module as follows:
+Import types from the `foxglove_schemas_protobuf` module as follows:
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
```

### Comparing `foxglove-schemas-protobuf-0.0.3/foxglove_schemas_protobuf.egg-info/SOURCES.txt` & `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 foxglove_schemas_protobuf/CompressedImage_pb2.pyi
 foxglove_schemas_protobuf/CubePrimitive_pb2.py
 foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
 foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
 foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
 foxglove_schemas_protobuf/FrameTransform_pb2.py
 foxglove_schemas_protobuf/FrameTransform_pb2.pyi
+foxglove_schemas_protobuf/FrameTransforms_pb2.py
+foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
 foxglove_schemas_protobuf/GeoJSON_pb2.py
 foxglove_schemas_protobuf/GeoJSON_pb2.pyi
 foxglove_schemas_protobuf/Grid_pb2.py
 foxglove_schemas_protobuf/Grid_pb2.pyi
 foxglove_schemas_protobuf/ImageAnnotations_pb2.py
 foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
 foxglove_schemas_protobuf/KeyValuePair_pb2.py
@@ -59,22 +61,25 @@
 foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
 foxglove_schemas_protobuf/SceneEntity_pb2.py
 foxglove_schemas_protobuf/SceneEntity_pb2.pyi
 foxglove_schemas_protobuf/SceneUpdate_pb2.py
 foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
 foxglove_schemas_protobuf/SpherePrimitive_pb2.py
 foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
+foxglove_schemas_protobuf/TextAnnotation_pb2.py
+foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
 foxglove_schemas_protobuf/TextPrimitive_pb2.py
 foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
 foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
 foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
 foxglove_schemas_protobuf/Vector2_pb2.py
 foxglove_schemas_protobuf/Vector2_pb2.pyi
 foxglove_schemas_protobuf/Vector3_pb2.py
 foxglove_schemas_protobuf/Vector3_pb2.pyi
 foxglove_schemas_protobuf/__init__.py
 foxglove_schemas_protobuf/py.typed
 foxglove_schemas_protobuf.egg-info/PKG-INFO
 foxglove_schemas_protobuf.egg-info/SOURCES.txt
 foxglove_schemas_protobuf.egg-info/dependency_links.txt
 foxglove_schemas_protobuf.egg-info/requires.txt
-foxglove_schemas_protobuf.egg-info/top_level.txt
+foxglove_schemas_protobuf.egg-info/top_level.txt
+tests/test_schemas.py
```

### Comparing `foxglove-schemas-protobuf-0.0.3/setup.cfg` & `foxglove-schemas-protobuf-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-schemas-protobuf
-version = 0.0.3
+version = 0.1.0
 description = Protobuf classes for Foxglove Schemas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/schemas
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

