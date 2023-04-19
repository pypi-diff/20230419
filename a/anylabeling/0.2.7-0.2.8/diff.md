# Comparing `tmp/anylabeling-0.2.7.tar.gz` & `tmp/anylabeling-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.2.7.tar", last modified: Sun Apr 16 18:19:32 2023, max compression
+gzip compressed data, was "anylabeling-0.2.8.tar", last modified: Wed Apr 19 17:05:45 2023, max compression
```

## Comparing `anylabeling-0.2.7.tar` & `anylabeling-0.2.8.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:19:21.000000 anylabeling-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 18:19:21.000000 anylabeling-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 18:19:32.862918 anylabeling-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-16 18:19:21.000000 anylabeling-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.842918 anylabeling-0.2.7/anylabeling/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.846918 anylabeling-0.2.7/anylabeling/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/configs/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/services/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.854918 anylabeling-0.2.7/anylabeling/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.854918 anylabeling-0.2.7/anylabeling/views/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    93425 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48701 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.846918 anylabeling-0.2.7/anylabeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-16 18:19:21.000000 anylabeling-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:19:32.862918 anylabeling-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 18:19:21.000000 anylabeling-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.228251 anylabeling-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 17:05:36.000000 anylabeling-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 17:05:36.000000 anylabeling-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-19 17:05:45.228251 anylabeling-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-19 17:05:36.000000 anylabeling-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.212251 anylabeling-0.2.8/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.212251 anylabeling-0.2.8/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.212251 anylabeling-0.2.8/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.212251 anylabeling-0.2.8/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.216251 anylabeling-0.2.8/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.216251 anylabeling-0.2.8/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.216251 anylabeling-0.2.8/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.216251 anylabeling-0.2.8/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.216251 anylabeling-0.2.8/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.224251 anylabeling-0.2.8/anylabeling/views/labeling/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93549 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.224251 anylabeling-0.2.8/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.228251 anylabeling-0.2.8/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.228251 anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48701 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-19 17:05:36.000000 anylabeling-0.2.8/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:05:45.212251 anylabeling-0.2.8/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 17:05:45.000000 anylabeling-0.2.8/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-19 17:05:36.000000 anylabeling-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:05:45.228251 anylabeling-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-19 17:05:36.000000 anylabeling-0.2.8/setup.py
```

### Comparing `anylabeling-0.2.7/LICENSE` & `anylabeling-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/PKG-INFO` & `anylabeling-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.7
+Version: 0.2.8
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.7 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.8 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.2.7/README.md` & `anylabeling-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/app.py` & `anylabeling-0.2.8/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.2.8/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/models.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/models.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5l.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5m.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5n.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5s.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5x.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8l.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8m.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8n.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8s.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8x.yaml` & `anylabeling-0.2.8/anylabeling/configs/auto_labeling/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/resources/resources.py` & `anylabeling-0.2.8/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/lru_cache.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/lru_cache.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.2.8/anylabeling/services/auto_labeling/yolov8.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/common/toaster.py` & `anylabeling-0.2.8/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/__main__.py` & `anylabeling-0.2.8/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/config.py` & `anylabeling-0.2.8/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.2.8/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/label_file.py` & `anylabeling-0.2.8/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.2.8/anylabeling/views/labeling/label_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1006,14 +1006,16 @@
 
         self.populate_mode_actions()
 
         self.first_start = True
         if self.first_start:
             QWhatsThis.enterWhatsThisMode()
 
+        self.set_text_editing(False)
+
     def get_labeling_instruction(self):
         return (
             f"<b>Mode:</b> {self.canvas.get_mode()} - <b>Shortcuts:</b>"
             " Previous: <b>A</b>, Next: <b>D</b>, Rectangle: <b>R</b>,"
             " Polygon: <b>P</b>"
         )
 
@@ -2605,13 +2607,16 @@
                 self.shape_text_edit.textChanged.disconnect()
                 self.shape_text_edit.setPlainText(
                     self.other_data.get("image_text", "")
                 )
                 self.shape_text_edit.textChanged.connect(
                     self.shape_text_changed
                 )
+            self.shape_text_edit.setDisabled(False)
         else:
             self.shape_text_edit.setDisabled(True)
-            self.shape_text_label.setText("Switch to Edit mode to edit text")
+            self.shape_text_label.setText(
+                "Switch to Edit mode for text editing"
+            )
             self.shape_text_edit.textChanged.disconnect()
             self.shape_text_edit.setPlainText("")
             self.shape_text_edit.textChanged.connect(self.shape_text_changed)
```

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.2.8/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/logger.py` & `anylabeling-0.2.8/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/shape.py` & `anylabeling-0.2.8/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/testing.py` & `anylabeling-0.2.8/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.2.8/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.2.8/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.2.8/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.2.8/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.2.8/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.2.8/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling/views/mainwindow.py` & `anylabeling-0.2.8/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.2.8/anylabeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.7
+Version: 0.2.8
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.7 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.8 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.2.7/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.2.8/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.7/setup.py` & `anylabeling-0.2.8/setup.py`

 * *Files identical despite different names*

