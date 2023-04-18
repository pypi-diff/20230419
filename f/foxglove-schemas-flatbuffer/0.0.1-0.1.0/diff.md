# Comparing `tmp/foxglove-schemas-flatbuffer-0.0.1.tar.gz` & `tmp/foxglove-schemas-flatbuffer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-schemas-flatbuffer-0.0.1.tar", last modified: Thu Feb 16 05:05:46 2023, max compression
+gzip compressed data, was "foxglove-schemas-flatbuffer-0.1.0.tar", last modified: Tue Apr 18 22:45:24 2023, max compression
```

## Comparing `foxglove-schemas-flatbuffer-0.0.1.tar` & `foxglove-schemas-flatbuffer-0.1.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-16 05:05:05.000000 foxglove-schemas-flatbuffer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ArrowPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ByteVector.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ByteVector.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CameraCalibration.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CameraCalibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CircleAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Color.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CompressedImage.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CompressedImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CubePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CubePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CylinderPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Duration.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/FrameTransform.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/FrameTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/GeoJSON.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/GeoJSON.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Grid.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ImageAnnotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/KeyValuePair.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/KeyValuePair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LaserScan.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LaserScan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LinePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LinePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LineType.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LocationFix.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LocationFix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Log.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LogLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ModelPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/NumericType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PackedElementField.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PackedElementField.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point2.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point2.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point3.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointCloud.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointCloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointsAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointsAnnotationType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Pose.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PoseInFrame.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PoseInFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PosesInFrame.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PosesInFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PositionCovarianceType.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Quaternion.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/RawImage.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/RawImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntity.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntityDeletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntityDeletionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneUpdate.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SpherePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TextPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TextPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Time.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TriangleListPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector2.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector2.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector3.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector3.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-16 05:05:41.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-16 05:05:46.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-02-16 05:05:46.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 05:05:46.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-16 05:05:46.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-16 05:05:46.000000 foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-16 05:05:05.000000 foxglove-schemas-flatbuffer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 05:05:46.672229 foxglove-schemas-flatbuffer-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-16 05:05:05.000000 foxglove-schemas-flatbuffer-0.0.1/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LineType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LogLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/NumericType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PositionCovarianceType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.bfbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/tests/test_schemas.py
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/PKG-INFO` & `foxglove-schemas-flatbuffer-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-flatbuffer
-Version: 0.0.1
+Version: 0.1.0
 Summary: Flatbuffer classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/README.md` & `foxglove-schemas-flatbuffer-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ArrowPrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ByteVector.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CameraCalibration.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CameraCalibration.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CircleAnnotation.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,35 +33,35 @@
             x = o + self._tab.Pos
             from .Time import Time
             obj = Time()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Center of the circle in 2D image coordinates
+    # Center of the circle in 2D image coordinates (pixels)
     # CircleAnnotation
     def Position(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             from .Point2 import Point2
             obj = Point2()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Circle diameter
+    # Circle diameter in pixels
     # CircleAnnotation
     def Diameter(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
 
-    # Line thickness
+    # Line thickness in pixels
     # CircleAnnotation
     def Thickness(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Color.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CompressedImage.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CompressedImage.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CubePrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CubePrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/CylinderPrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Duration.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/FrameTransform.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/FrameTransform.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/GeoJSON.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Grid.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Grid.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,192 @@
 00000000: 2000 0000 4246 4253 0000 0000 1400 2000   ...BFBS...... .
 00000010: 0400 0800 0c00 1000 1400 1800 0000 1c00  ................
 00000020: 1400 0000 3800 0000 2c00 0000 2000 0000  ....8...,... ...
-00000030: 1400 0000 7402 0000 0800 0000 3c00 0000  ....t.......<...
+00000030: 1400 0000 a002 0000 0800 0000 4000 0000  ............@...
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0100 0000 d000 0000 0600 0000  ................
-00000060: f404 0000 5808 0000 4002 0000 8c07 0000  ....X...@.......
-00000070: f002 0000 d806 0000 0600 0000 7c00 0000  ............|...
-00000080: 6800 0000 4c00 0000 3800 0000 1800 0000  h...L...8.......
-00000090: 0400 0000 d4f8 ffff d006 0000 0400 0000  ................
-000000a0: 0000 0000 e4f8 ffff cc02 0000 0400 0000  ................
-000000b0: 0300 0000 1c08 0000 5407 0000 ac06 0000  ........T.......
-000000c0: 00f9 ffff 4807 0000 0400 0000 0000 0000  ....H...........
-000000d0: 10f9 ffff e801 0000 0400 0000 0200 0000  ................
-000000e0: 8804 0000 9002 0000 28f9 ffff e407 0000  ........(.......
-000000f0: 0400 0000 0000 0000 38f9 ffff 6c04 0000  ........8...l...
-00000100: 0400 0000 0300 0000 c807 0000 0007 0000  ................
-00000110: 5806 0000 0000 1200 1400 0400 0800 0000  X...............
-00000120: 0c00 0000 0000 1000 1200 0000 3c00 0000  ............<...
-00000130: 2000 0000 0800 0000 3c02 0000 48fc ffff   .......<...H...
-00000140: 0000 0004 0000 0000 0100 0000 0100 0000  ................
-00000150: 0500 0000 2001 0000 e400 0000 a000 0000  .... ...........
-00000160: 5c00 0000 2800 0000 1d00 0000 666f 7867  \...(.......foxg
-00000170: 6c6f 7665 2e50 6f69 6e74 7341 6e6e 6f74  love.PointsAnnot
-00000180: 6174 696f 6e54 7970 6500 0000 5cff ffff  ationType...\...
-00000190: 1c00 0000 0c00 0000 0400 0000 0000 0000  ................
-000001a0: 20ff ffff 0100 0000 0100 0000 0900 0000   ...............
-000001b0: 4c49 4e45 5f4c 4953 5400 0000 ccff ffff  LINE_LIST.......
-000001c0: 2000 0000 1000 0000 0300 0000 0000 0000   ...............
-000001d0: 0000 0000 54ff ffff 0100 0000 0100 0000  ....T...........
-000001e0: 0a00 0000 4c49 4e45 5f53 5452 4950 0000  ....LINE_STRIP..
-000001f0: 0c00 1800 0400 0c00 0000 0800 0c00 0000  ................
-00000200: 2000 0000 1000 0000 0200 0000 0000 0000   ...............
-00000210: 0000 0000 94ff ffff 0100 0000 0100 0000  ................
-00000220: 0900 0000 4c49 4e45 5f4c 4f4f 5000 0000  ....LINE_LOOP...
-00000230: 0c00 1400 0400 0c00 0000 0800 0c00 0000  ................
-00000240: 1c00 0000 0c00 0000 0100 0000 0000 0000  ................
-00000250: d0ff ffff 0100 0000 0100 0000 0600 0000  ................
-00000260: 504f 494e 5453 0000 0c00 0c00 0400 0000  POINTS..........
-00000270: 0000 0800 0c00 0000 2400 0000 1400 0000  ........$.......
-00000280: 1000 0c00 0000 0000 0000 0000 0400 0800  ................
-00000290: 1000 0000 0100 0000 0100 0000 0700 0000  ................
-000002a0: 554e 4b4e 4f57 4e00 00fa ffff 3800 0000  UNKNOWN.....8...
-000002b0: 2800 0000 0100 0000 0400 0000 1600 0000  (...............
-000002c0: 2f2f 496d 6167 6541 6e6e 6f74 6174 696f  //ImageAnnotatio
-000002d0: 6e73 2e66 6273 0000 0200 0000 5800 0000  ns.fbs......X...
-000002e0: 2400 0000 1900 0000 666f 7867 6c6f 7665  $.......foxglove
-000002f0: 2e49 6d61 6765 416e 6e6f 7461 7469 6f6e  .ImageAnnotation
-00000300: 7300 0000 78fc ffff 0000 0001 0100 0600  s...x...........
-00000310: 1800 0000 0400 0000 60fe ffff 0000 0e0f  ........`.......
-00000320: 0400 0000 0400 0000 0600 0000 706f 696e  ............poin
-00000330: 7473 0000 58fc ffff 0001 0400 1800 0000  ts..X...........
-00000340: 0400 0000 8cfe ffff 0000 0e0f 0000 0000  ................
-00000350: 0400 0000 0700 0000 6369 7263 6c65 7300  ........circles.
-00000360: b8fa ffff 4c00 0000 2800 0000 0100 0000  ....L...(.......
-00000370: 0400 0000 1600 0000 2f2f 506f 696e 7473  ........//Points
-00000380: 416e 6e6f 7461 7469 6f6e 2e66 6273 0000  Annotation.fbs..
-00000390: 0700 0000 6c00 0000 d400 0000 9800 0000  ....l...........
-000003a0: 0401 0000 2c00 0000 7c01 0000 3801 0000  ....,...|...8...
-000003b0: 1900 0000 666f 7867 6c6f 7665 2e50 6f69  ....foxglove.Poi
-000003c0: 6e74 7341 6e6e 6f74 6174 696f 6e00 0000  ntsAnnotation...
-000003d0: 90fb ffff 0600 1000 1800 0000 0400 0000  ................
-000003e0: 10fa ffff 0000 000c 0800 0000 0100 0000  ................
-000003f0: 0900 0000 7468 6963 6b6e 6573 7300 0000  ....thickness...
-00000400: 74fd ffff 0000 0001 0500 0e00 1800 0000  t...............
-00000410: 0400 0000 0cfd ffff 0000 000f 0100 0000  ................
-00000420: 0100 0000 0a00 0000 6669 6c6c 5f63 6f6c  ........fill_col
-00000430: 6f72 0000 a8fd ffff 0000 0001 0400 0c00  or..............
-00000440: 1800 0000 0400 0000 90ff ffff 0000 0e0f  ................
-00000450: 0100 0000 0400 0000 0e00 0000 6f75 746c  ............outl
-00000460: 696e 655f 636f 6c6f 7273 0000 e0fd ffff  ine_colors......
-00000470: 0000 0001 0300 0a00 1800 0000 0400 0000  ................
-00000480: 78fd ffff 0000 000f 0100 0000 0100 0000  x...............
-00000490: 0d00 0000 6f75 746c 696e 655f 636f 6c6f  ....outline_colo
-000004a0: 7200 0000 18fe ffff 0000 0001 0200 0800  r...............
-000004b0: 2800 0000 1400 0000 1000 1000 0600 0700  (...............
-000004c0: 0800 0000 0000 0c00 1000 0000 0000 0e0f  ................
-000004d0: 0300 0000 0400 0000 0600 0000 706f 696e  ............poin
-000004e0: 7473 0000 a4fc ffff 0100 0600 2c00 0000  ts..........,...
-000004f0: 1400 0000 1000 1400 0700 0000 0800 0000  ................
-00000500: 0c00 1000 1000 0000 0000 0004 0000 0000  ................
-00000510: 0100 0000 0100 0000 0400 0000 7479 7065  ............type
-00000520: 0000 0000 48fe ffff 0001 0400 1800 0000  ....H...........
-00000530: 0400 0000 2cfe ffff 0000 000f 0500 0000  ....,...........
-00000540: 0100 0000 0900 0000 7469 6d65 7374 616d  ........timestam
-00000550: 7000 0000 acfc ffff 4800 0000 2800 0000  p.......H...(...
-00000560: 0100 0000 0400 0000 1600 0000 2f2f 4369  ............//Ci
-00000570: 7263 6c65 416e 6e6f 7461 7469 6f6e 2e66  rcleAnnotation.f
-00000580: 6273 0000 0600 0000 d400 0000 6c00 0000  bs..........l...
-00000590: 3000 0000 1401 0000 9400 0000 5c01 0000  0...........\...
-000005a0: 1900 0000 666f 7867 6c6f 7665 2e43 6972  ....foxglove.Cir
-000005b0: 636c 6541 6e6e 6f74 6174 696f 6e00 0000  cleAnnotation...
-000005c0: 34ff ffff 0000 0001 0500 0e00 1800 0000  4...............
-000005d0: 0400 0000 ccfe ffff 0000 000f 0100 0000  ................
-000005e0: 0100 0000 0d00 0000 6f75 746c 696e 655f  ........outline_
-000005f0: 636f 6c6f 7200 0000 6cff ffff 0000 0001  color...l.......
-00000600: 0400 0c00 1800 0000 0400 0000 04ff ffff  ................
-00000610: 0000 000f 0100 0000 0100 0000 0a00 0000  ................
-00000620: 6669 6c6c 5f63 6f6c 6f72 0000 ecfd ffff  fill_color......
-00000630: 0300 0a00 1800 0000 0400 0000 6cfc ffff  ............l...
-00000640: 0000 000c 0800 0000 0100 0000 0900 0000  ................
-00000650: 7468 6963 6b6e 6573 7300 0000 1cfe ffff  thickness.......
-00000660: 0200 0800 1800 0000 0400 0000 9cfc ffff  ................
-00000670: 0000 000c 0800 0000 0100 0000 0800 0000  ................
-00000680: 6469 616d 6574 6572 0000 0000 1c00 1400  diameter........
-00000690: 0c00 1000 0800 0a00 0000 0000 0000 0000  ................
-000006a0: 0000 0000 0000 0700 1c00 0000 0000 0001  ................
-000006b0: 0100 0600 1800 0000 0400 0000 b4ff ffff  ................
-000006c0: 0000 000f 0300 0000 0100 0000 0800 0000  ................
-000006d0: 706f 7369 7469 6f6e 0000 0000 1c00 1000  position........
-000006e0: 0800 0c00 0000 0600 0000 0000 0000 0000  ................
-000006f0: 0000 0000 0000 0500 1c00 0000 0001 0400  ................
-00000700: 2800 0000 1400 0000 1000 1000 0700 0000  (...............
-00000710: 0800 0000 0000 0c00 1000 0000 0000 000f  ................
-00000720: 0500 0000 0100 0000 0900 0000 7469 6d65  ............time
-00000730: 7374 616d 7000 0000 1400 1c00 0800 0c00  stamp...........
-00000740: 0700 1000 1400 0000 0000 1800 1400 0000  ................
-00000750: 0000 0001 3000 0000 2000 0000 0400 0000  ....0... .......
-00000760: 0800 0000 0400 0000 0a00 0000 2f2f 5469  ............//Ti
-00000770: 6d65 2e66 6273 0000 0200 0000 1c00 0000  me.fbs..........
-00000780: 4800 0000 0d00 0000 666f 7867 6c6f 7665  H.......foxglove
-00000790: 2e54 696d 6500 0000 58ff ffff 0100 0400  .Time...X.......
-000007a0: 1400 0000 0400 0000 d4ff ffff 0000 0008  ................
-000007b0: 0100 0000 0400 0000 6e73 6563 0000 0000  ........nsec....
-000007c0: 0800 0c00 0400 0800 0800 0000 2400 0000  ............$...
-000007d0: 1400 0000 1000 0c00 0700 0000 0000 0000  ................
-000007e0: 0000 0800 1000 0000 0000 0008 0100 0000  ................
-000007f0: 0300 0000 7365 6300 50ff ffff 3000 0000  ....sec.P...0...
-00000800: 2000 0000 0100 0000 0400 0000 0c00 0000   ...............
-00000810: 2f2f 506f 696e 7432 2e66 6273 0000 0000  //Point2.fbs....
-00000820: 0200 0000 5c00 0000 2400 0000 0f00 0000  ....\...$.......
-00000830: 666f 7867 6c6f 7665 2e50 6f69 6e74 3200  foxglove.Point2.
-00000840: 0c00 1000 0800 0c00 0400 0600 0c00 0000  ................
-00000850: 0100 0600 1800 0000 0400 0000 8cfe ffff  ................
-00000860: 0000 000c 0800 0000 0100 0000 0100 0000  ................
-00000870: 7900 0000 0c00 1000 0800 0c00 0000 0600  y...............
-00000880: 0c00 0000 0000 0400 1800 0000 0400 0000  ................
-00000890: c0fe ffff 0000 000c 0800 0000 0100 0000  ................
-000008a0: 0100 0000 7800 0000 1400 1400 0400 0800  ....x...........
-000008b0: 0000 0c00 0000 0000 0000 1000 1400 0000  ................
-000008c0: 3400 0000 1c00 0000 0100 0000 0400 0000  4...............
-000008d0: 0b00 0000 2f2f 436f 6c6f 722e 6662 7300  ....//Color.fbs.
-000008e0: 0400 0000 2400 0000 5000 0000 8c00 0000  ....$...P.......
-000008f0: c800 0000 0e00 0000 666f 7867 6c6f 7665  ........foxglove
-00000900: 2e43 6f6c 6f72 0000 a0ff ffff 0300 0a00  .Color..........
-00000910: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
-00000920: 50ff ffff 0000 000c 0800 0000 0100 0000  P...............
-00000930: 0100 0000 6100 0000 d0ff ffff 0200 0800  ....a...........
-00000940: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
-00000950: 80ff ffff 0000 000c 0800 0000 0100 0000  ................
-00000960: 0100 0000 6200 0000 1000 1800 0800 0c00  ....b...........
-00000970: 0400 0600 0000 1000 1000 0000 0100 0600  ................
-00000980: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
-00000990: c0ff ffff 0000 000c 0800 0000 0100 0000  ................
-000009a0: 0100 0000 6700 0000 1000 1800 0800 0c00  ....g...........
-000009b0: 0000 0600 0000 1000 1000 0000 0000 0400  ................
-000009c0: 3000 0000 1c00 0000 0000 0000 0000 f03f  0..............?
-000009d0: 1000 1000 0700 0000 0000 0000 0800 0c00  ................
-000009e0: 1000 0000 0000 000c 0800 0000 0100 0000  ................
-000009f0: 0100 0000 7200 0000                      ....r...
+00000050: 0000 0000 0100 0000 f800 0000 0700 0000  ................
+00000060: f406 0000 580a 0000 6c02 0000 8c09 0000  ....X...l.......
+00000070: f004 0000 4c03 0000 d408 0000 0700 0000  ....L...........
+00000080: a000 0000 8c00 0000 6c00 0000 5800 0000  ........l...X...
+00000090: 3800 0000 1800 0000 0400 0000 dcf6 ffff  8...............
+000000a0: c808 0000 0400 0000 0000 0000 ecf6 ffff  ................
+000000b0: 2403 0000 0400 0000 0300 0000 140a 0000  $...............
+000000c0: 4c09 0000 a408 0000 08f7 ffff a804 0000  L...............
+000000d0: 0400 0000 0300 0000 f809 0000 3009 0000  ............0...
+000000e0: 8808 0000 24f7 ffff 2409 0000 0400 0000  ....$...$.......
+000000f0: 0000 0000 34f7 ffff f001 0000 0400 0000  ....4...........
+00000100: 0300 0000 6406 0000 6c04 0000 c802 0000  ....d...l.......
+00000110: 50f7 ffff bc09 0000 0400 0000 0000 0000  P...............
+00000120: 60f7 ffff 4406 0000 0400 0000 0300 0000  `...D...........
+00000130: a009 0000 d808 0000 3008 0000 0000 1200  ........0.......
+00000140: 1400 0400 0800 0000 0c00 0000 0000 1000  ................
+00000150: 1200 0000 3c00 0000 2000 0000 0800 0000  ....<... .......
+00000160: 1404 0000 70fa ffff 0000 0004 0000 0000  ....p...........
+00000170: 0100 0000 0100 0000 0500 0000 2401 0000  ............$...
+00000180: e400 0000 a000 0000 6c00 0000 2800 0000  ........l...(...
+00000190: 1d00 0000 666f 7867 6c6f 7665 2e50 6f69  ....foxglove.Poi
+000001a0: 6e74 7341 6e6e 6f74 6174 696f 6e54 7970  ntsAnnotationTyp
+000001b0: 6500 0000 5cff ffff 2000 0000 1000 0000  e...\... .......
+000001c0: 0400 0000 0000 0000 0000 0000 20ff ffff  ............ ...
+000001d0: 0100 0000 0100 0000 0900 0000 4c49 4e45  ............LINE
+000001e0: 5f4c 4953 5400 0000 0c00 1400 0400 0c00  _LIST...........
+000001f0: 0000 0800 0c00 0000 1c00 0000 0c00 0000  ................
+00000200: 0300 0000 0000 0000 5cff ffff 0100 0000  ........\.......
+00000210: 0100 0000 0a00 0000 4c49 4e45 5f53 5452  ........LINE_STR
+00000220: 4950 0000 ccff ffff 2000 0000 1000 0000  IP...... .......
+00000230: 0200 0000 0000 0000 0000 0000 90ff ffff  ................
+00000240: 0100 0000 0100 0000 0900 0000 4c49 4e45  ............LINE
+00000250: 5f4c 4f4f 5000 0000 0c00 1800 0400 0c00  _LOOP...........
+00000260: 0000 0800 0c00 0000 2000 0000 1000 0000  ........ .......
+00000270: 0100 0000 0000 0000 0000 0000 d0ff ffff  ................
+00000280: 0100 0000 0100 0000 0600 0000 504f 494e  ............POIN
+00000290: 5453 0000 0c00 0c00 0400 0000 0000 0800  TS..............
+000002a0: 0c00 0000 2400 0000 1400 0000 1000 0c00  ....$...........
+000002b0: 0000 0000 0000 0000 0400 0800 1000 0000  ................
+000002c0: 0100 0000 0100 0000 0700 0000 554e 4b4e  ............UNKN
+000002d0: 4f57 4e00 2cf8 ffff 3c00 0000 2800 0000  OWN.,...<...(...
+000002e0: 0100 0000 0400 0000 1600 0000 2f2f 496d  ............//Im
+000002f0: 6167 6541 6e6e 6f74 6174 696f 6e73 2e66  ageAnnotations.f
+00000300: 6273 0000 0300 0000 8c00 0000 5800 0000  bs..........X...
+00000310: 2400 0000 1900 0000 666f 7867 6c6f 7665  $.......foxglove
+00000320: 2e49 6d61 6765 416e 6e6f 7461 7469 6f6e  .ImageAnnotation
+00000330: 7300 0000 a8fa ffff 0000 0001 0200 0800  s...............
+00000340: 1800 0000 0400 0000 90fc ffff 0000 0e0f  ................
+00000350: 0500 0000 0400 0000 0500 0000 7465 7874  ............text
+00000360: 7300 0000 d8fa ffff 0000 0001 0100 0600  s...............
+00000370: 1800 0000 0400 0000 c0fc ffff 0000 0e0f  ................
+00000380: 0400 0000 0400 0000 0600 0000 706f 696e  ............poin
+00000390: 7473 0000 b8fa ffff 0001 0400 1800 0000  ts..............
+000003a0: 0400 0000 ecfc ffff 0000 0e0f 0000 0000  ................
+000003b0: 0400 0000 0700 0000 6369 7263 6c65 7300  ........circles.
+000003c0: 18f9 ffff 4800 0000 2800 0000 0100 0000  ....H...(.......
+000003d0: 0400 0000 1400 0000 2f2f 5465 7874 416e  ........//TextAn
+000003e0: 6e6f 7461 7469 6f6e 2e66 6273 0000 0000  notation.fbs....
+000003f0: 0600 0000 3400 0000 a000 0000 0001 0000  ....4...........
+00000400: d000 0000 6000 0000 2801 0000 1700 0000  ....`...(.......
+00000410: 666f 7867 6c6f 7665 2e54 6578 7441 6e6e  foxglove.TextAnn
+00000420: 6f74 6174 696f 6e00 9cfb ffff 0000 0001  otation.........
+00000430: 0500 0e00 1800 0000 0400 0000 34fb ffff  ............4...
+00000440: 0000 000f 0100 0000 0100 0000 1000 0000  ................
+00000450: 6261 636b 6772 6f75 6e64 5f63 6f6c 6f72  background_color
+00000460: 0000 0000 d8fb ffff 0000 0001 0400 0c00  ................
+00000470: 1800 0000 0400 0000 70fb ffff 0000 000f  ........p.......
+00000480: 0100 0000 0100 0000 0a00 0000 7465 7874  ............text
+00000490: 5f63 6f6c 6f72 0000 30f9 ffff 0300 0a00  _color..0.......
+000004a0: 2000 0000 0c00 0000 0000 0000 0000 2840   .............(@
+000004b0: e0f8 ffff 0000 000c 0800 0000 0100 0000  ................
+000004c0: 0900 0000 666f 6e74 5f73 697a 6500 0000  ....font_size...
+000004d0: 44fc ffff 0000 0001 0200 0800 1400 0000  D...............
+000004e0: 0400 0000 10fb ffff 0000 000d 0100 0000  ................
+000004f0: 0400 0000 7465 7874 0000 0000 70fc ffff  ....text....p...
+00000500: 0000 0001 0100 0600 1800 0000 0400 0000  ................
+00000510: 08fc ffff 0000 000f 0300 0000 0100 0000  ................
+00000520: 0800 0000 706f 7369 7469 6f6e 0000 0000  ....position....
+00000530: 54fc ffff 0001 0400 1800 0000 0400 0000  T...............
+00000540: 38fc ffff 0000 000f 0600 0000 0100 0000  8...............
+00000550: 0900 0000 7469 6d65 7374 616d 7000 0000  ....timestamp...
+00000560: b8fa ffff 4c00 0000 2800 0000 0100 0000  ....L...(.......
+00000570: 0400 0000 1600 0000 2f2f 506f 696e 7473  ........//Points
+00000580: 416e 6e6f 7461 7469 6f6e 2e66 6273 0000  Annotation.fbs..
+00000590: 0700 0000 6c00 0000 d400 0000 9800 0000  ....l...........
+000005a0: 0401 0000 2c00 0000 7c01 0000 3801 0000  ....,...|...8...
+000005b0: 1900 0000 666f 7867 6c6f 7665 2e50 6f69  ....foxglove.Poi
+000005c0: 6e74 7341 6e6e 6f74 6174 696f 6e00 0000  ntsAnnotation...
+000005d0: 90fb ffff 0600 1000 1800 0000 0400 0000  ................
+000005e0: 10fa ffff 0000 000c 0800 0000 0100 0000  ................
+000005f0: 0900 0000 7468 6963 6b6e 6573 7300 0000  ....thickness...
+00000600: 74fd ffff 0000 0001 0500 0e00 1800 0000  t...............
+00000610: 0400 0000 0cfd ffff 0000 000f 0100 0000  ................
+00000620: 0100 0000 0a00 0000 6669 6c6c 5f63 6f6c  ........fill_col
+00000630: 6f72 0000 a8fd ffff 0000 0001 0400 0c00  or..............
+00000640: 1800 0000 0400 0000 90ff ffff 0000 0e0f  ................
+00000650: 0100 0000 0400 0000 0e00 0000 6f75 746c  ............outl
+00000660: 696e 655f 636f 6c6f 7273 0000 e0fd ffff  ine_colors......
+00000670: 0000 0001 0300 0a00 1800 0000 0400 0000  ................
+00000680: 78fd ffff 0000 000f 0100 0000 0100 0000  x...............
+00000690: 0d00 0000 6f75 746c 696e 655f 636f 6c6f  ....outline_colo
+000006a0: 7200 0000 18fe ffff 0000 0001 0200 0800  r...............
+000006b0: 2800 0000 1400 0000 1000 1000 0600 0700  (...............
+000006c0: 0800 0000 0000 0c00 1000 0000 0000 0e0f  ................
+000006d0: 0300 0000 0400 0000 0600 0000 706f 696e  ............poin
+000006e0: 7473 0000 a4fc ffff 0100 0600 2c00 0000  ts..........,...
+000006f0: 1400 0000 1000 1400 0700 0000 0800 0000  ................
+00000700: 0c00 1000 1000 0000 0000 0004 0000 0000  ................
+00000710: 0100 0000 0100 0000 0400 0000 7479 7065  ............type
+00000720: 0000 0000 48fe ffff 0001 0400 1800 0000  ....H...........
+00000730: 0400 0000 2cfe ffff 0000 000f 0600 0000  ....,...........
+00000740: 0100 0000 0900 0000 7469 6d65 7374 616d  ........timestam
+00000750: 7000 0000 acfc ffff 4800 0000 2800 0000  p.......H...(...
+00000760: 0100 0000 0400 0000 1600 0000 2f2f 4369  ............//Ci
+00000770: 7263 6c65 416e 6e6f 7461 7469 6f6e 2e66  rcleAnnotation.f
+00000780: 6273 0000 0600 0000 d400 0000 6c00 0000  bs..........l...
+00000790: 3000 0000 1401 0000 9400 0000 5c01 0000  0...........\...
+000007a0: 1900 0000 666f 7867 6c6f 7665 2e43 6972  ....foxglove.Cir
+000007b0: 636c 6541 6e6e 6f74 6174 696f 6e00 0000  cleAnnotation...
+000007c0: 34ff ffff 0000 0001 0500 0e00 1800 0000  4...............
+000007d0: 0400 0000 ccfe ffff 0000 000f 0100 0000  ................
+000007e0: 0100 0000 0d00 0000 6f75 746c 696e 655f  ........outline_
+000007f0: 636f 6c6f 7200 0000 6cff ffff 0000 0001  color...l.......
+00000800: 0400 0c00 1800 0000 0400 0000 04ff ffff  ................
+00000810: 0000 000f 0100 0000 0100 0000 0a00 0000  ................
+00000820: 6669 6c6c 5f63 6f6c 6f72 0000 ecfd ffff  fill_color......
+00000830: 0300 0a00 1800 0000 0400 0000 6cfc ffff  ............l...
+00000840: 0000 000c 0800 0000 0100 0000 0900 0000  ................
+00000850: 7468 6963 6b6e 6573 7300 0000 1cfe ffff  thickness.......
+00000860: 0200 0800 1800 0000 0400 0000 9cfc ffff  ................
+00000870: 0000 000c 0800 0000 0100 0000 0800 0000  ................
+00000880: 6469 616d 6574 6572 0000 0000 1c00 1400  diameter........
+00000890: 0c00 1000 0800 0a00 0000 0000 0000 0000  ................
+000008a0: 0000 0000 0000 0700 1c00 0000 0000 0001  ................
+000008b0: 0100 0600 1800 0000 0400 0000 b4ff ffff  ................
+000008c0: 0000 000f 0300 0000 0100 0000 0800 0000  ................
+000008d0: 706f 7369 7469 6f6e 0000 0000 1c00 1000  position........
+000008e0: 0800 0c00 0000 0600 0000 0000 0000 0000  ................
+000008f0: 0000 0000 0000 0500 1c00 0000 0001 0400  ................
+00000900: 2800 0000 1400 0000 1000 1000 0700 0000  (...............
+00000910: 0800 0000 0000 0c00 1000 0000 0000 000f  ................
+00000920: 0600 0000 0100 0000 0900 0000 7469 6d65  ............time
+00000930: 7374 616d 7000 0000 1400 1c00 0800 0c00  stamp...........
+00000940: 0700 1000 1400 0000 0000 1800 1400 0000  ................
+00000950: 0000 0001 3000 0000 2000 0000 0400 0000  ....0... .......
+00000960: 0800 0000 0400 0000 0a00 0000 2f2f 5469  ............//Ti
+00000970: 6d65 2e66 6273 0000 0200 0000 1c00 0000  me.fbs..........
+00000980: 4800 0000 0d00 0000 666f 7867 6c6f 7665  H.......foxglove
+00000990: 2e54 696d 6500 0000 58ff ffff 0100 0400  .Time...X.......
+000009a0: 1400 0000 0400 0000 d4ff ffff 0000 0008  ................
+000009b0: 0100 0000 0400 0000 6e73 6563 0000 0000  ........nsec....
+000009c0: 0800 0c00 0400 0800 0800 0000 2400 0000  ............$...
+000009d0: 1400 0000 1000 0c00 0700 0000 0000 0000  ................
+000009e0: 0000 0800 1000 0000 0000 0008 0100 0000  ................
+000009f0: 0300 0000 7365 6300 50ff ffff 3000 0000  ....sec.P...0...
+00000a00: 2000 0000 0100 0000 0400 0000 0c00 0000   ...............
+00000a10: 2f2f 506f 696e 7432 2e66 6273 0000 0000  //Point2.fbs....
+00000a20: 0200 0000 5c00 0000 2400 0000 0f00 0000  ....\...$.......
+00000a30: 666f 7867 6c6f 7665 2e50 6f69 6e74 3200  foxglove.Point2.
+00000a40: 0c00 1000 0800 0c00 0400 0600 0c00 0000  ................
+00000a50: 0100 0600 1800 0000 0400 0000 8cfe ffff  ................
+00000a60: 0000 000c 0800 0000 0100 0000 0100 0000  ................
+00000a70: 7900 0000 0c00 1000 0800 0c00 0000 0600  y...............
+00000a80: 0c00 0000 0000 0400 1800 0000 0400 0000  ................
+00000a90: c0fe ffff 0000 000c 0800 0000 0100 0000  ................
+00000aa0: 0100 0000 7800 0000 1400 1400 0400 0800  ....x...........
+00000ab0: 0000 0c00 0000 0000 0000 1000 1400 0000  ................
+00000ac0: 3400 0000 1c00 0000 0100 0000 0400 0000  4...............
+00000ad0: 0b00 0000 2f2f 436f 6c6f 722e 6662 7300  ....//Color.fbs.
+00000ae0: 0400 0000 2400 0000 5000 0000 8c00 0000  ....$...P.......
+00000af0: c800 0000 0e00 0000 666f 7867 6c6f 7665  ........foxglove
+00000b00: 2e43 6f6c 6f72 0000 a0ff ffff 0300 0a00  .Color..........
+00000b10: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
+00000b20: 50ff ffff 0000 000c 0800 0000 0100 0000  P...............
+00000b30: 0100 0000 6100 0000 d0ff ffff 0200 0800  ....a...........
+00000b40: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
+00000b50: 80ff ffff 0000 000c 0800 0000 0100 0000  ................
+00000b60: 0100 0000 6200 0000 1000 1800 0800 0c00  ....b...........
+00000b70: 0400 0600 0000 1000 1000 0000 0100 0600  ................
+00000b80: 2000 0000 0c00 0000 0000 0000 0000 f03f   ..............?
+00000b90: c0ff ffff 0000 000c 0800 0000 0100 0000  ................
+00000ba0: 0100 0000 6700 0000 1000 1800 0800 0c00  ....g...........
+00000bb0: 0000 0600 0000 1000 1000 0000 0000 0400  ................
+00000bc0: 3000 0000 1c00 0000 0000 0000 0000 f03f  0..............?
+00000bd0: 1000 1000 0700 0000 0000 0000 0800 0c00  ................
+00000be0: 1000 0000 0000 000c 0800 0000 0100 0000  ................
+00000bf0: 0100 0000 7200 0000                      ....r...
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ImageAnnotations.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.py`

 * *Files 13% similar despite different names*

```diff
@@ -73,25 +73,57 @@
         return 0
 
     # ImageAnnotations
     def PointsIsNone(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         return o == 0
 
-def ImageAnnotationsStart(builder): builder.StartObject(2)
+    # Text annotations
+    # ImageAnnotations
+    def Texts(self, j):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            x = self._tab.Vector(o)
+            x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
+            x = self._tab.Indirect(x)
+            from .TextAnnotation import TextAnnotation
+            obj = TextAnnotation()
+            obj.Init(self._tab.Bytes, x)
+            return obj
+        return None
+
+    # ImageAnnotations
+    def TextsLength(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.VectorLen(o)
+        return 0
+
+    # ImageAnnotations
+    def TextsIsNone(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        return o == 0
+
+def ImageAnnotationsStart(builder): builder.StartObject(3)
 def Start(builder):
     return ImageAnnotationsStart(builder)
 def ImageAnnotationsAddCircles(builder, circles): builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(circles), 0)
 def AddCircles(builder, circles):
     return ImageAnnotationsAddCircles(builder, circles)
 def ImageAnnotationsStartCirclesVector(builder, numElems): return builder.StartVector(4, numElems, 4)
 def StartCirclesVector(builder, numElems):
     return ImageAnnotationsStartCirclesVector(builder, numElems)
 def ImageAnnotationsAddPoints(builder, points): builder.PrependUOffsetTRelativeSlot(1, flatbuffers.number_types.UOffsetTFlags.py_type(points), 0)
 def AddPoints(builder, points):
     return ImageAnnotationsAddPoints(builder, points)
 def ImageAnnotationsStartPointsVector(builder, numElems): return builder.StartVector(4, numElems, 4)
 def StartPointsVector(builder, numElems):
     return ImageAnnotationsStartPointsVector(builder, numElems)
+def ImageAnnotationsAddTexts(builder, texts): builder.PrependUOffsetTRelativeSlot(2, flatbuffers.number_types.UOffsetTFlags.py_type(texts), 0)
+def AddTexts(builder, texts):
+    return ImageAnnotationsAddTexts(builder, texts)
+def ImageAnnotationsStartTextsVector(builder, numElems): return builder.StartVector(4, numElems, 4)
+def StartTextsVector(builder, numElems):
+    return ImageAnnotationsStartTextsVector(builder, numElems)
 def ImageAnnotationsEnd(builder): return builder.EndObject()
 def End(builder):
     return ImageAnnotationsEnd(builder)
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/KeyValuePair.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LaserScan.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LaserScan.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LinePrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LinePrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LocationFix.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/LocationFix.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Log.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Log.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/ModelPrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PackedElementField.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PackedElementField.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point2.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Point3.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointCloud.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointCloud.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # PointCloud
     def PointStride(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Uint32Flags, o + self._tab.Pos)
         return 0
 
-    # Fields in `data`. At least 2 coordinate fields from `x`, `y`, and `z` (all `float64`s) are required for each point's position; `red`, `green`, `blue`, and `alpha` (all `float64`s) are optional for customizing each point's color.
+    # Fields in `data`. At least 2 coordinate fields from `x`, `y`, and `z` are required for each point's position; `red`, `green`, `blue`, and `alpha` are optional for customizing each point's color.
     # PointCloud
     def Fields(self, j):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             x = self._tab.Vector(o)
             x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
             x = self._tab.Indirect(x)
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PointsAnnotation.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # PointsAnnotation
     def Type(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Uint8Flags, o + self._tab.Pos)
         return 0
 
-    # Points in 2D image coordinates
+    # Points in 2D image coordinates (pixels)
     # PointsAnnotation
     def Points(self, j):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             x = self._tab.Vector(o)
             x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
             x = self._tab.Indirect(x)
@@ -117,15 +117,15 @@
             x = self._tab.Indirect(o + self._tab.Pos)
             from .Color import Color
             obj = Color()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Stroke thickness
+    # Stroke thickness in pixels
     # PointsAnnotation
     def Thickness(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Pose.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Pose.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PoseInFrame.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PoseInFrame.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PosesInFrame.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/PosesInFrame.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Quaternion.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/RawImage.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/RawImage.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntity.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntity.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneEntityDeletion.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneUpdate.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SceneUpdate.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/SpherePrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TextPrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TextPrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Time.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/TriangleListPrimitive.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector2.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer/Vector3.py` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/PKG-INFO` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-flatbuffer
-Version: 0.0.1
+Version: 0.1.0
 Summary: Flatbuffer classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt` & `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 foxglove_schemas_flatbuffer/CubePrimitive.py
 foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
 foxglove_schemas_flatbuffer/CylinderPrimitive.py
 foxglove_schemas_flatbuffer/Duration.bfbs
 foxglove_schemas_flatbuffer/Duration.py
 foxglove_schemas_flatbuffer/FrameTransform.bfbs
 foxglove_schemas_flatbuffer/FrameTransform.py
+foxglove_schemas_flatbuffer/FrameTransforms.bfbs
+foxglove_schemas_flatbuffer/FrameTransforms.py
 foxglove_schemas_flatbuffer/GeoJSON.bfbs
 foxglove_schemas_flatbuffer/GeoJSON.py
 foxglove_schemas_flatbuffer/Grid.bfbs
 foxglove_schemas_flatbuffer/Grid.py
 foxglove_schemas_flatbuffer/ImageAnnotations.bfbs
 foxglove_schemas_flatbuffer/ImageAnnotations.py
 foxglove_schemas_flatbuffer/KeyValuePair.bfbs
@@ -69,14 +71,16 @@
 foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs
 foxglove_schemas_flatbuffer/SceneEntityDeletion.py
 foxglove_schemas_flatbuffer/SceneEntityDeletionType.py
 foxglove_schemas_flatbuffer/SceneUpdate.bfbs
 foxglove_schemas_flatbuffer/SceneUpdate.py
 foxglove_schemas_flatbuffer/SpherePrimitive.bfbs
 foxglove_schemas_flatbuffer/SpherePrimitive.py
+foxglove_schemas_flatbuffer/TextAnnotation.bfbs
+foxglove_schemas_flatbuffer/TextAnnotation.py
 foxglove_schemas_flatbuffer/TextPrimitive.bfbs
 foxglove_schemas_flatbuffer/TextPrimitive.py
 foxglove_schemas_flatbuffer/Time.bfbs
 foxglove_schemas_flatbuffer/Time.py
 foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs
 foxglove_schemas_flatbuffer/TriangleListPrimitive.py
 foxglove_schemas_flatbuffer/Vector2.bfbs
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/setup.cfg` & `foxglove-schemas-flatbuffer-0.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-schemas-flatbuffer
-version = 0.0.1
+version = 0.1.0
 description = Flatbuffer classes for Foxglove Schemas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/schemas
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-schemas-flatbuffer-0.0.1/tests/test_schemas.py` & `foxglove-schemas-flatbuffer-0.1.0/tests/test_schemas.py`

 * *Files identical despite different names*

