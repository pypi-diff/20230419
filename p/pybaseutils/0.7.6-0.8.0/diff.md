# Comparing `tmp/pybaseutils-0.7.6.tar.gz` & `tmp/pybaseutils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.7.6.tar", last modified: Fri Mar 17 07:17:10 2023, max compression
+gzip compressed data, was "dist/pybaseutils-0.8.0.tar", last modified: Wed Apr 19 09:08:10 2023, max compression
```

## Comparing `pybaseutils-0.7.6.tar` & `pybaseutils-0.8.0.tar`

### file list

```diff
@@ -1,114 +1,119 @@
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.7.6/LICENCE
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3955 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/PKG-INFO
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5099 2022-06-22 03:40:56.000000 pybaseutils-0.7.6/pybaseutils/base64_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2160 2022-07-27 07:00:03.000000 pybaseutils-0.7.6/pybaseutils/batch_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/cluster/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1957 2022-11-25 09:01:44.000000 pybaseutils-0.7.6/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3043 2022-11-25 05:37:15.000000 pybaseutils-0.7.6/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2749 2022-11-25 05:37:15.000000 pybaseutils-0.7.6/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-09-05 11:49:47.000000 pybaseutils-0.7.6/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.7.6/pybaseutils/color_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.7.6/pybaseutils/config_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    10081 2022-08-10 02:34:08.000000 pybaseutils-0.7.6/pybaseutils/coords_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/cvutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.7.6/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8270 2022-11-25 02:19:35.000000 pybaseutils-0.7.6/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7739 2023-03-13 11:14:07.000000 pybaseutils-0.7.6/pybaseutils/cvutils/video_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.7.6/pybaseutils/cvutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/dataloader/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7368 2022-11-16 02:01:19.000000 pybaseutils-0.7.6/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    12141 2023-02-14 09:23:56.000000 pybaseutils-0.7.6/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    11902 2022-11-28 09:33:24.000000 pybaseutils-0.7.6/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19255 2023-03-12 01:44:07.000000 pybaseutils-0.7.6/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-06-29 10:58:17.000000 pybaseutils-0.7.6/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    30318 2023-03-16 08:36:20.000000 pybaseutils-0.7.6/pybaseutils/file_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/font_style/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      542 2022-06-02 06:53:27.000000 pybaseutils-0.7.6/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6697 2023-01-13 09:18:47.000000 pybaseutils-0.7.6/pybaseutils/font_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13058 2022-03-31 02:23:17.000000 pybaseutils-0.7.6/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5311 2022-07-25 07:52:13.000000 pybaseutils-0.7.6/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    95360 2023-03-13 07:40:19.000000 pybaseutils-0.7.6/pybaseutils/image_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4260 2022-05-20 03:29:01.000000 pybaseutils-0.7.6/pybaseutils/json_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6815 2022-12-30 05:59:58.000000 pybaseutils-0.7.6/pybaseutils/log.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.7.6/pybaseutils/logger.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/maker/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4602 2023-02-14 09:27:54.000000 pybaseutils-0.7.6/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5179 2022-12-07 08:09:58.000000 pybaseutils-0.7.6/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6209 2022-12-07 06:35:47.000000 pybaseutils-0.7.6/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3513 2022-12-07 06:32:33.000000 pybaseutils-0.7.6/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1656 2022-09-05 11:49:24.000000 pybaseutils-0.7.6/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    17370 2023-02-24 07:56:04.000000 pybaseutils-0.7.6/pybaseutils/maker/maker_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-09-05 11:49:47.000000 pybaseutils-0.7.6/pybaseutils/maker/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/metrics/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      800 2022-11-14 03:43:13.000000 pybaseutils-0.7.6/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2196 2022-11-14 03:34:54.000000 pybaseutils-0.7.6/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5473 2022-09-06 09:00:14.000000 pybaseutils-0.7.6/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5581 2022-08-12 07:06:49.000000 pybaseutils-0.7.6/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5380 2022-08-12 07:05:42.000000 pybaseutils-0.7.6/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-08-11 07:42:38.000000 pybaseutils-0.7.6/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19293 2022-12-29 02:38:43.000000 pybaseutils-0.7.6/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2095 2022-10-13 10:31:05.000000 pybaseutils-0.7.6/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7527 2023-03-17 05:43:46.000000 pybaseutils-0.7.6/pybaseutils/plot_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/pycpp/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.7.6/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4314 2022-10-26 10:42:32.000000 pybaseutils-0.7.6/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.7.6/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.7.6/pybaseutils/setup_config.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7201 2023-02-23 10:37:54.000000 pybaseutils-0.7.6/pybaseutils/thread_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3311 2022-10-11 07:25:16.000000 pybaseutils-0.7.6/pybaseutils/time_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4990 2023-02-28 03:50:01.000000 pybaseutils-0.7.6/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.7.6/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils/transforms/
--rwxrwxrwx   0 dm        (1000) dm        (1000)    24121 2022-08-12 09:32:18.000000 pybaseutils-0.7.6/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-07-26 07:00:42.000000 pybaseutils-0.7.6/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13630 2023-03-02 06:16:50.000000 pybaseutils-0.7.6/pybaseutils/word_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4100 2022-05-06 02:33:14.000000 pybaseutils-0.7.6/pybaseutils/worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.7.6/pybaseutils/yaml_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      142 2023-03-17 07:17:05.000000 pybaseutils-0.7.6/pybaseutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils.egg-info/
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.7.6/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3955 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2891 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.7.6/README.md
--rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/setup.cfg
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2221 2022-06-02 02:42:02.000000 pybaseutils-0.7.6/setup.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/test_py/
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-03-17 07:17:10.000000 pybaseutils-0.7.6/test_py/converter/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.7.6/test_py/converter/AffectNet.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.7.6/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.7.6/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.7.6/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.7.6/test_py/converter/CCPD.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.7.6/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4942 2023-03-14 10:27:29.000000 pybaseutils-0.7.6/test_py/converter/detect_face_person.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7597 2022-12-13 08:38:36.000000 pybaseutils-0.7.6/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-11-17 06:50:23.000000 pybaseutils-0.7.6/test_py/converter/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1429 2023-02-08 03:20:15.000000 pybaseutils-0.7.6/test_py/demo1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      800 2023-03-10 03:31:13.000000 pybaseutils-0.7.6/test_py/demo2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1879 2023-03-17 06:23:53.000000 pybaseutils-0.7.6/test_py/demo_copy_files.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.7.6/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.7.6/test_py/demo_correction_v1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5662 2022-11-30 03:34:38.000000 pybaseutils-0.7.6/test_py/demo_correction_v2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1563 2022-11-30 07:11:05.000000 pybaseutils-0.7.6/test_py/demo_correction_v3.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.7.6/test_py/demo_for_trt.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2909 2023-02-28 05:42:39.000000 pybaseutils-0.7.6/test_py/demo_get_file_list.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      672 2022-12-08 08:49:19.000000 pybaseutils-0.7.6/test_py/demo_gif.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2644 2022-10-10 09:04:31.000000 pybaseutils-0.7.6/test_py/demo_metrics.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1680 2022-11-25 02:19:35.000000 pybaseutils-0.7.6/test_py/demo_mouse.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2022-10-13 11:35:18.000000 pybaseutils-0.7.6/test_py/demo_pandas.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.7.6/test_py/demo_plot.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1588 2023-03-09 07:27:27.000000 pybaseutils-0.7.6/test_py/demo_standard_image .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      754 2022-12-29 02:39:54.000000 pybaseutils-0.7.6/test_py/demo_taichi.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1806 2023-03-13 11:19:13.000000 pybaseutils-0.7.6/test_py/demo_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3014 2023-02-28 09:11:41.000000 pybaseutils-0.7.6/test_py/demo_voc_crop.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2088 2023-03-02 10:36:38.000000 pybaseutils-0.7.6/test_py/demo_voc_vis.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1396 2023-03-07 06:44:31.000000 pybaseutils-0.7.6/test_py/demo_word_similar.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2911 2022-05-05 07:01:30.000000 pybaseutils-0.7.6/test_py/demo_worker1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3156 2022-05-06 02:50:52.000000 pybaseutils-0.7.6/test_py/demo_worker2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.7.6/test_py/men_tracemalloc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.7.6/test_py/performance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      133 2022-10-21 01:09:27.000000 pybaseutils-0.7.6/test_py/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.0/LICENCE
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/PKG-INFO
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/batch_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/cluster/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.0/pybaseutils/color_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.0/pybaseutils/config_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/coords_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/cvutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.0/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7784 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cvutils/video_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.0/pybaseutils/cvutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/dataloader/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/file_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/font_style/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/font_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    95465 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/image_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/json_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/log.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.0/pybaseutils/logger.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/maker/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/maker/maker_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/maker/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/metrics/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/plot_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/pycpp/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.0/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/pycpp/main.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.0/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.0/pybaseutils/setup_config.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/time_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.0/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/transforms/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13621 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/word_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4095 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/worker.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.0/pybaseutils/yaml_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-04-19 09:08:03.000000 pybaseutils-0.8.0/pybaseutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.0/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3054 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.0/README.md
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/setup.cfg
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/setup.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/test_py/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.0/test_py/class_names.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/test_py/converter/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.0/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.0/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.0/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.0/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.0/test_py/converter/CCPD.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.0/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4942 2023-03-14 10:27:29.000000 pybaseutils-0.8.0/test_py/converter/detect_face_person.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.0/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.0/test_py/converter/TT100K.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.0/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/converter/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      830 2023-04-12 02:15:23.000000 pybaseutils-0.8.0/test_py/demo1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1111 2023-03-31 03:30:19.000000 pybaseutils-0.8.0/test_py/demo2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4533 2023-04-15 03:49:32.000000 pybaseutils-0.8.0/test_py/demo_copy_files.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.0/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.0/test_py/demo_correction_v1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_correction_v2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_correction_v3.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.0/test_py/demo_for_trt.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_gif.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_metrics.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_mouse.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_pandas.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.0/test_py/demo_plot.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.0/test_py/demo_standard_image .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      861 2023-03-21 08:22:16.000000 pybaseutils-0.8.0/test_py/demo_standard_video .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_taichi.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1891 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_video.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.0/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.0/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.0/test_py/demo_word_similar.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_worker1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_worker2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.0/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.0/test_py/performance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/__init__.py
```

### Comparing `pybaseutils-0.7.6/LICENCE` & `pybaseutils-0.8.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/PKG-INFO` & `pybaseutils-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.7.6
+Version: 0.8.0
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
-Author-email: pan_jinquan@163.com
+Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
```

### Comparing `pybaseutils-0.7.6/pybaseutils/base64_utils.py` & `pybaseutils-0.8.0/pybaseutils/base64_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-03-22 09:11:35
     @Brief  :
 """
 import sys
 import os
 import cv2
 import base64
```

### Comparing `pybaseutils-0.7.6/pybaseutils/batch_utils.py` & `pybaseutils-0.8.0/pybaseutils/batch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-06-06 14:34:38
     @Brief  :
 """
 from typing import Tuple, List, Dict
 
 
 def get_batch_sample(data_list: List, batch_size: int):
```

### Comparing `pybaseutils-0.7.6/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.0/pybaseutils/cluster/kmean.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-09-02 19:04:10
 """
 import numpy as np
 from sklearn.cluster import KMeans
 
 
 def sklearn_kmeans(feature, n_clusters, max_iter=300):
```

### Comparing `pybaseutils-0.7.6/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.0/pybaseutils/cluster/maxmin_distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 """
     @Project: IntelligentManufacture
     @File   : maxmin_distance.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-02-14 18:41:30
 """
 import math
 import numpy as np
 from pybaseutils.cluster import similarity
```

### Comparing `pybaseutils-0.7.6/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.0/pybaseutils/cluster/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-09-02 17:04:52
 """
 
 import cv2
 import numpy as np
 import math
```

### Comparing `pybaseutils-0.7.6/pybaseutils/color_utils.py` & `pybaseutils-0.8.0/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/config_utils.py` & `pybaseutils-0.8.0/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/coords_utils.py` & `pybaseutils-0.8.0/pybaseutils/coords_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2021-09-08 16:58:52
 """
 
 import math
 import random
 import cv2
 import numbers
```

### Comparing `pybaseutils-0.7.6/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.0/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.0/pybaseutils/cvutils/mouse_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-07-27 15:23:24
     @Brief  :
 """
 import cv2
 import numpy as np
 from typing import Callable
 from pybaseutils import image_utils
```

### Comparing `pybaseutils-0.7.6/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.0/pybaseutils/cvutils/video_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-05-24 16:46:51
     @Brief  :
 """
 import os
 import cv2
 import numpy as np
 from tqdm import tqdm
@@ -148,15 +148,16 @@
     """
     video_cap = get_video_capture(video_file)
     width, height, num_frames, fps = get_video_info(video_cap)
     video_writer = get_video_writer(save_video, width, height, fps)
     # freq = int(fps / detect_freq)
     count = 0
     while True:
-        if count % interval == 0:
+        # if count % interval == 0:
+        if count % interval == 0 and count > 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
             if not isSuccess:
                 break
             if vis: image_utils.cv_show_image("frame", frame, use_rgb=False, delay=delay)
             video_writer.write(frame)
```

### Comparing `pybaseutils-0.7.6/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.0/pybaseutils/dataloader/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-06-29 18:58:33
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 import glob
```

### Comparing `pybaseutils-0.7.6/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.0/pybaseutils/dataloader/parser_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-06-29 18:31:12
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 import glob
```

### Comparing `pybaseutils-0.7.6/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.0/pybaseutils/dataloader/parser_textdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-06-29 18:31:12
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 import glob
```

### Comparing `pybaseutils-0.7.6/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.0/pybaseutils/dataloader/parser_voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
-# @Author : panjq
-# @E-mail : pan_jinquan@163.com
+# @Author : Pan
+# @E-mail : 390737991@qq.com
 # @Date   : 2020-02-05 11:01:49
 # --------------------------------------------------------
 """
 import os
 import xmltodict
 import numpy as np
 import cv2
@@ -103,14 +103,16 @@
         dst_ids = []
         # image_ids = image_ids[:100]
         # image_ids = image_ids[100:]
         class_set = []
         for image_id in tqdm(image_ids):
             image_file, annotation_file = self.get_image_anno_file(image_id)
             if not os.path.exists(annotation_file):
+                # print(image_file)
+                # os.remove(image_file)
                 continue
             if not os.path.exists(image_file):
                 continue
             objects = self.get_annotation(annotation_file)
             bboxes, labels, is_difficult = objects["bboxes"], objects["labels"], objects["is_difficult"]
             class_set = labels.reshape(-1).tolist() + class_set
             class_set = list(set(class_set))
@@ -443,15 +445,16 @@
                           shuffle=shuffle,
                           check=check)
         datasets.append(data)
     datasets = ConcatDataset(datasets, shuffle=shuffle)
     return datasets
 
 
-def show_target_image(image, bboxes, labels, normal=False, transpose=False, class_name=None, use_rgb=True):
+def show_target_image(image, bboxes, labels, normal=False, transpose=False, class_name=None, use_rgb=True,
+                      thickness=-1, fontScale=-1.0):
     """
     :param image:
     :param targets_t:
                 bboxes = targets[idx][:, :4].data
                 keypoints = targets[idx][:, 4:14].data
                 labels = targets[idx][:, -1].data
     :return:
@@ -469,15 +472,16 @@
     h, w, _ = image.shape
     landms_scale = np.asarray([w, h] * 5)
     bboxes_scale = np.asarray([w, h] * 2)
     if normal:
         bboxes = bboxes * bboxes_scale
     # image = image_processing.untranspose(image)
     # image = image_processing.convert_color_space(image, colorSpace="RGB")
-    image = image_utils.draw_image_bboxes_labels(image, bboxes, labels, class_name=class_name,drawType="custom")
+    image = image_utils.draw_image_bboxes_labels(image, bboxes, labels, class_name=class_name,
+                                                 thickness=thickness, fontScale=fontScale, drawType="custom")
     image_utils.cv_show_image("image", image, delay=0, use_rgb=use_rgb)
     print("===" * 10)
     return image
 
 
 if __name__ == "__main__":
     # from models.transforms import data_transforms
```

### Comparing `pybaseutils-0.7.6/pybaseutils/file_utils.py` & `pybaseutils-0.8.0/pybaseutils/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
-# @Author : panjq
-# @E-mail : pan_jinquan@163.com
+# @Author : Pan
+# @E-mail : 390737991@qq.com
 # @Date   : 2019-12-31 09:11:25
 # --------------------------------------------------------
 """
 import os
 import time
 import shutil
 import numpy as np
@@ -206,19 +206,19 @@
                     else:
                         line_data.append(l)
                 content_list[i] = line_data
     return content_list
 
 
 def read_line_image_label(line_image_label):
-    '''
+    """
     line_image_label:[image_id,boxes_nums,x1, y1, w, h, label_id,x1, y1, w, h, label_id,...]
     :param line_image_label:
     :return:
-    '''
+    """
     line_image_label = line_image_label.strip().split()
     image_id = line_image_label[0]
     boxes_nums = int(line_image_label[1])
     box = []
     label = []
     for i in range(boxes_nums):
         x = float(line_image_label[2 + 5 * i])
@@ -323,14 +323,27 @@
     :param dir:
     :return:
     """
     if os.path.exists(dir):
         shutil.rmtree(dir)
 
 
+def get_config_file(file_dir, prefix="*.yaml"):
+    """
+    获得config.yaml文件
+    :param file_dir:
+    :param prefix:
+    :return:
+    """
+    if os.path.isfile(file_dir): file_dir = os.path.dirname(file_dir)
+    files = get_prefix_files(file_dir, prefix)
+    file = files[0] if len(files) > 0 else ""
+    return file
+
+
 def get_prefix_files(file_dir, prefix):
     """
     获得符合前缀条件所有文件
     :param file_dir:
     :param prefix: "best*"
     :return:
     """
@@ -459,14 +472,31 @@
         for filename in files:
             copy_file(
                 os.path.join(root, filename),
                 os.path.join(dest_path, filename)
             )
 
 
+def move_dir(src, dst, sub=False):
+    """ copy src-directory to dst-directory, will cover the same files"""
+    if not os.path.exists(src):
+        print("\nno src path:{}".format(src))
+        return
+    if sub: dst = os.path.join(dst, os.path.basename(src))
+    for root, dirs, files in os.walk(src, topdown=False):
+        dest_path = os.path.join(dst, os.path.relpath(root, src))
+        if not os.path.exists(dest_path):
+            os.makedirs(dest_path)
+        for filename in files:
+            move_file(
+                os.path.join(root, filename),
+                os.path.join(dest_path, filename)
+            )
+
+
 def move_file(srcfile, dstfile):
     """ 移动文件或重命名"""
     if not os.path.isfile(srcfile):
         print("%s not exist!" % (srcfile))
     else:
         fpath, fname = os.path.split(dstfile)  # 分离文件名和路径
         if not os.path.exists(fpath):
@@ -513,14 +543,21 @@
         if not os.path.exists(des_dir):
             os.makedirs(des_dir)  # 创建路径
         dstfile = os.path.join(des_dir, fname)
         # shutil.copyfile(srcfile, dstfile)  # 复制文件
         move_file(srcfile, dstfile)  # 复制文件
 
 
+def copy_file_list(file_list, dst_dir):
+    [copy_file_to_dir(file, dst_dir) for file in file_list]
+
+
+def move_file_list(file_list, dst_dir):
+    [move_file_to_dir(file, dst_dir) for file in file_list]
+
 def merge_dir(src, dst, sub, merge_same):
     src_dir = os.path.join(src, sub)
     dst_dir = os.path.join(dst, sub)
 
     if not os.path.exists(src_dir):
         print("\nno src path:{}".format(src))
         return
@@ -560,19 +597,19 @@
     basename = os.path.basename(filename)
     dirname = os.path.dirname(filename)
     out_path = create_dir(dirname, dir1=None, filename=basename)
     return out_path
 
 
 def get_sub_paths(input_dir):
-    '''
+    """
     当前路径下所有子目录
     :param input_dir:
     :return:
-    '''
+    """
     sub_list = []
     for root, dirs, files in os.walk(input_dir):
         sub_list = dirs
         break
     # print(root)   # 当前目录路径
     # print(dirs)   # 当前路径下所有子目录
     # print(files)  # 当前路径下所有非目录子文件
@@ -818,20 +855,21 @@
         faces_list2 = faces_list2.tolist()
         issames_data = issames_data.tolist()
         return faces_list1, faces_list2, issames_data
     return content_list
 
 
 def check_files(files_list, sizeTh=1 * 1024, isRemove=False):
-    ''' 去除不存的文件和文件过小的文件列表
+    """
+    去除不存的文件和文件过小的文件列表
     :param files_list:
     :param sizeTh: 文件大小阈值,单位：字节B，默认1000B ,33049513/1024/1024=33.0MB
     :param isRemove: 是否在硬盘上删除被损坏的原文件
     :return:
-    '''
+    """
     i = 0
     while i < len(files_list):
         path = files_list[i]
         # 判断文件是否存在
         if not (os.path.exists(path)):
             print(" non-existent file:{}".format(path))
             files_list.pop(i)
@@ -972,42 +1010,70 @@
 
 
 def load_pickle(file):
     with open(file, 'rb') as f: obj = pickle.load(f)
     return obj
 
 
-def copy_move_file_dir(file_dir, out_dir, postfix=None, sub_names=None, max_nums=None, shuffle=True, move=False):
+def copy_move_file_dir(src, dst, postfix=None, sub_names=None, max_nums=None, shuffle=True, move=False):
     """
     复制/移动文件夹
-    :param file_dir: 原始目录
-    :param out_dir: 输出目录
+    :param src: 原始目录
+    :param dst: 输出目录
     :param sub_names: 需要复制/移动的子文件夹名称，默认全部
     :param max_nums: 最大移动数量，默认不限制
     :param shuffle:
     :param move: True表示移动，False表示复制
     :return: out_list 返回复制/移动后，out_dir的文件列表
     """
-    file_list = get_files_list(file_dir, prefix="", postfix=postfix, basename=False)
-    file_list = get_sub_list(file_list, file_dir)
+    file_list = get_files_list(src, prefix="", postfix=postfix, basename=False)
+    file_list = get_sub_list(file_list, src)
     if shuffle:
         random.seed(100)
         random.shuffle(file_list)
         random.shuffle(file_list)
     if max_nums: file_list = file_list[:min(max_nums, len(file_list))]
     for file_name in tqdm(file_list):
         sub = os.path.dirname(file_name)
         if sub_names and (sub not in sub_names): continue
-        src_file = os.path.join(file_dir, file_name)
-        out_file = os.path.join(out_dir, file_name)
+        src_file = os.path.join(src, file_name)
+        out_file = os.path.join(dst, file_name)
         if move:
             move_file(src_file, out_file)
         else:
             copy_file(src_file, out_file)
-    out_list = get_files_list(out_dir, prefix="", postfix=postfix, basename=False)
+    out_list = get_files_list(dst, prefix="", postfix=postfix, basename=False)
+    return out_list
+
+
+def copy_move_dir_dir(src, dst, postfix=None, sub_names=None, per_nums=None, shuffle=True, move=False):
+    """
+    复制/移动文件夹
+    :param src: 原始目录
+    :param out_dir_: 输出目录
+    :param sub_names: 需要复制/移动的子文件夹名称，默认全部
+    :param per_nums: 每个子文件夹最大移动数量，默认全部
+    :param shuffle:
+    :param move: True表示移动，False表示复制
+    :return: out_list 返回复制/移动后，out_dir的文件列表
+    """
+    sub_list = get_sub_paths(src)
+    for sub in tqdm(sub_list):
+        if sub_names and (sub not in sub_names): continue
+        src_dir_ = os.path.join(src, sub)
+        out_dir_ = os.path.join(dst, sub)
+        if per_nums is None:
+            if move:
+                move_dir(src_dir_, out_dir_)
+            else:
+                copy_dir(src_dir_, out_dir_)
+        else:
+            copy_move_file_dir(src_dir_, out_dir_, postfix=postfix, sub_names=postfix,
+                               max_nums=per_nums, shuffle=shuffle, move=move)
+    out_list = get_files_list(dst, prefix="", postfix=postfix, basename=False)
     return out_list
 
 
 if __name__ == '__main__':
     dir = "/home/dm/nasdata/dataset-dmai/handwriting/word-class/trainval/unknown"
     file_list, label_list = get_files_labels(dir)
     print(label_list)
```

### Comparing `pybaseutils-0.7.6/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.0/pybaseutils/font_style/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-05-07 17:40:27
 """
 import os
 
 # windows: C:\Windows\Fonts可查看系统支持的字体
 # Linux  : /usr/share/fonts/truetype可查看系统支持的字体
```

### Comparing `pybaseutils-0.7.6/pybaseutils/font_utils.py` & `pybaseutils-0.8.0/pybaseutils/font_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
-# @Author : panjq
-# @E-mail : pan_jinquan@163.com
+# @Author : Pan
+# @E-mail : 390737991@qq.com
 # @Date   : 2019-12-31 09:11:25
 # --------------------------------------------------------
 """
 import os
 import cv2
 import re
 import PIL
+import platform
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 from pybaseutils import image_utils, file_utils
 from pybaseutils.font_style import FONT_TYPE, FONT_ROOT
 from fontTools.ttLib import TTFont
 
+ROOT = os.path.dirname(__file__)
+
 
 class FontType(object):
     def __init__(self, root=FONT_ROOT, style="宋体", size=20):
         """
         :param root: 安装字体的路径
         :param style: 选择字体风格
         :param size: 旋转字体大小
@@ -49,14 +52,37 @@
     def get_font_type(self):
         return self.font_type
 
 
 font_type = FontType()
 
 
+def get_font_type(size, font=""):
+    """
+    Windows字体路径      : /usr/share/fonts/楷体.ttf
+    Linux(Ubuntu)字体路径：/usr/share/fonts/楷体.ttf
+     >> fc-list             查看所有的字体
+     >> fc-list :lang=zh    查看所有的中文字体
+    :param size: 字体大小
+    :param font:  simsun.ttc 宋体;simhei.ttf 黑体
+    :return:
+    """
+    # 参数1：字体文件路径，参数2：字体大小；Windows系统“simhei.ttf”默认存储在路径：
+    if font:
+        font = ImageFont.truetype(font, size, encoding="utf-8")
+    elif platform.system().lower() == 'windows':
+        font = ImageFont.truetype("simhei.ttf", size, encoding="utf-8")  # simsun.ttc 宋体
+    elif platform.system().lower() == 'linux':
+        # font = ImageFont.truetype("uming.ttc", size, encoding="utf-8")
+        font = ImageFont.truetype("NotoSansCJK-Regular.ttc", size, encoding="utf-8")
+    else:
+        font = ImageFont.truetype(os.path.join(ROOT, "font_style/simhei.ttf"), size, encoding="utf-8")
+    return font
+
+
 def draw_image_text(image, point, text, style="楷体", size=20, color=(255, 255, 255)):
     """
     在图像中显示汉字
     https://blog.csdn.net/weixin_44237337/article/details/119817801
     :param image: RGB字体背景
     :param point:
     :param text:
@@ -154,15 +180,15 @@
     string = "你3.39好@、/、小，*、明&，在 %%%么100（）"
     去除所有特殊字符
     :param string:
     :param repl:
     :return:
     """
     # new = re.sub(r"[^\w]", repl, string)  # 删除特殊字符，数字除外
-    new = re.sub('[0-9’!"#$%&\'()（）*+,-./:;<=>?@，。?★、…【】《》？“”‘’！[\\]^_`{|}~\s]+', repl, string) # 删除特殊字符，数字也删除
+    new = re.sub('[0-9’!"#$%&\'()（）*+,-./:;<=>?@，。?★、…【】《》？“”‘’！[\\]^_`{|}~\s]+', repl, string)  # 删除特殊字符，数字也删除
     return new
 
 
 def get_font_char(font_file, only_chinese=False):
     """
     返回字库支持的所有字符
     ord()返回字符对应的ascii码
```

### Comparing `pybaseutils-0.7.6/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.0/pybaseutils/geometry_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 """
     @Project: PyKinect2-OpenCV
     @File   : geometry_tools.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-10-11 09:23:21
 """
 # -*- coding: utf-8 -*-
 
 import numpy as np
```

### Comparing `pybaseutils-0.7.6/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.0/pybaseutils/heatmap_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2021-04-14 14:29:30
 """
 import cv2
 import numpy as np
 import numpy.matlib
```

### Comparing `pybaseutils-0.7.6/pybaseutils/image_utils.py` & `pybaseutils-0.8.0/pybaseutils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-02-14 15:34:50
 """
 
 import os
 import copy
 import re
 import cv2
@@ -1301,14 +1301,16 @@
         cv2.rectangle(image, (text_loc[0] - 2 // 2, text_loc[1] - 2 - baseline),
                       (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color=color, thickness=thickness)
         # draw score value
         cv2.putText(image, str(text), (text_loc[0], text_loc[1] + baseline), fontFace, fontScale,
                     (255, 255, 255), text_thickness, 2)
     elif drawType == "simple":
         cv2.putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
+    if drawType == "chinese":
+        cv2_putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
     return image
 
 
 def draw_text_line(image, point, text_line: str, bg_color=(255, 0, 0), thickness=-1, fontScale=-1.0, drawType="custom"):
     """
     :param image:
     :param point:
@@ -1806,43 +1808,45 @@
     :param bbox:
     :return:
     """
     crops = [get_bbox_crop(image, box) for box in bboxes]
     return crops
 
 
-def get_bboxes_crop_padding(image, bboxes, size, color=(0, 0, 0)):
+def get_bboxes_crop_padding(image, bboxes, size=(), color=(0, 0, 0)):
     """
     :param image:
     :param bboxes:
     :param size:
+    :param color:
     :return:
     """
     rects = bboxes2rects(bboxes)
-    roi_images = []
+    crops = []
     for rect in rects:
-        roi_image = get_rect_crop_padding(image, rect, color=color)
-        roi_image = resize_image(roi_image, size=size)
-        roi_images.append(roi_image)
-    return roi_images
+        roi = get_rect_crop_padding(image, rect, color=color)
+        if size: roi = resize_image(roi, size=size)
+        crops.append(roi)
+    return crops
 
 
-def get_rects_crop_padding(image, rects, size, color=(0, 0, 0)):
+def get_rects_crop_padding(image, rects, size=(), color=(0, 0, 0)):
     """
     :param image:
     :param rects:
-    :param resize:
+    :param size:
+    :param color:
     :return:
     """
-    roi_images = []
+    crops = []
     for rect in rects:
-        roi_image = get_rect_crop_padding(image, rect, color=color)
-        roi_image = resize_image(roi_image, size=size)
-        roi_images.append(roi_image)
-    return roi_images
+        roi = get_rect_crop_padding(image, rect, color=color)
+        if size: roi = resize_image(roi, size=size)
+        crops.append(roi)
+    return crops
 
 
 def center_crop(image, crop_size=[112, 112]):
     """
     central_crop
     :param image: input numpy type image
     :param crop_size: (W,H) crop_size must less than x.shape[:2]=[crop_h,crop_w]
```

### Comparing `pybaseutils-0.7.6/pybaseutils/json_utils.py` & `pybaseutils-0.8.0/pybaseutils/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-04-19 10:40:26
     @Brief  :
 """
 import os
 import toolz
 import json
 import numbers
```

### Comparing `pybaseutils-0.7.6/pybaseutils/log.py` & `pybaseutils-0.8.0/pybaseutils/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
-# @Author : panjq
+# @Author : Pan
 # @Date   : 2019-9-20 13:18:34
 # --------------------------------------------------------
 """
 import os
 import datetime
 import logging
 import threading
```

### Comparing `pybaseutils-0.7.6/pybaseutils/logger.py` & `pybaseutils-0.8.0/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.0/pybaseutils/maker/convert_labelme2voc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
 # @Project: AlphaPose
-# @Author : panjq
-# @E-mail : pan_jinquan@163.com
+# @Author : Pan
+# @E-mail : 390737991@qq.com
 # @Date   : 2020-02-14 09:15:52
 # --------------------------------------------------------
 """
 import sys
 import os
 
 sys.path.insert(0, os.getcwd())
@@ -32,18 +32,18 @@
                                                      image_dir=image_dir,
                                                      class_name=None,
                                                      use_rgb=False,
                                                      check=False,
                                                      phase="val",
                                                      shuffle=False)
 
-    def convert_dataset2voc(self, out_root, class_name=None, out_image_dir=None, crop=True, rename=False, vis=True):
+    def convert_dataset2voc(self, out_root, class_dict={}, out_image_dir=None, crop=False, rename=False, vis=True):
         """
         :param out_root: VOC输出根目录
-        :param class_name: label映射 list或dict
+        :param class_dict: label映射 list或dict
         :param out_image_dir: 保存 JPEGImages
         :param crop: 是否进行目标裁剪
         :param rename: 是否重命名
         :param vis: 是否可视化
         :return:
         """
         out_xml_dir = os.path.join(out_root, "Annotations")
@@ -60,25 +60,25 @@
             format = os.path.basename(image_file).split(".")[-1]
             image_id = os.path.basename(image_file)[:-len(format) - 1]
             if rename:
                 image_id = "{}_{:0=4d}".format(rename, i)
                 format = "jpg"
             newname = "{}.{}".format(image_id, format)
             xml_path = file_utils.create_dir(out_xml_dir, None, "{}.xml".format(image_id))
-            objects = maker_voc.create_objects(bboxes, labels, keypoints=None, class_name=class_name)
+            objects = maker_voc.create_objects(bboxes, labels, keypoints=None, class_name=class_dict)
             maker_voc.write_voc_xml_objects(newname, image_shape, objects, xml_path)
             if crop and out_crop_dir:
                 self.save_object_crops(objects, image, out_crop_dir, image_id)
             if out_image_dir:
                 dst_file = file_utils.create_dir(out_image_dir, None, newname)
                 file_utils.copy_file(image_file, dst_file)
                 # cv2.imwrite(dst_file, image)
             if vis:
                 self.show_object_image(image, objects)
-        if not out_image_dir: out_image_dir =self.image_dir
+        if not out_image_dir: out_image_dir = self.image_dir
         file_utils.save_file_list(out_image_dir, filename=None, prefix="", postfix=file_utils.IMG_POSTFIX,
                                   only_id=False, shuffle=False, max_num=None)
 
     def save_object_crops(self, objects, image, out_dir, image_id):
         for i, item in enumerate(objects):
             label = item["name"]
             box = item["bndbox"]
@@ -92,13 +92,14 @@
             label = item["name"]
             box = item["bndbox"]
             image = image_utils.draw_image_bboxes_text(image, [box], [label])
         image_utils.cv_show_image("image", image, use_rgb=False, delay=0)
 
 
 if __name__ == "__main__":
-    json_dir = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/competition-v2/json"
+    json_dir = "/home/dm/nasdata/dataset/tmp/fall/fall-v3/json"
     out_root = os.path.dirname(json_dir)
     image_dir = os.path.join(out_root, "JPEGImages")
-    class_name = None
+    class_dict = None
+    # class_dict = {"person": "up", "squat": "bending", "fall": "down"}
     lm = LabelMeDemo(json_dir, image_dir)
-    lm.convert_dataset2voc(out_root, class_name=class_name, vis=False, crop=False)
+    lm.convert_dataset2voc(out_root, class_dict=class_dict, vis=False, crop=False)
```

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.0/pybaseutils/maker/convert_voc2voc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-12 16:21:55
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 from tqdm import tqdm
@@ -89,36 +89,14 @@
     if out_image_dir:
         file_utils.save_file_list(out_image_dir, filename=None, prefix="", postfix=file_utils.IMG_POSTFIX,
                                   only_id=False, shuffle=False, max_num=None)
     print("class_set:{}".format(class_set))
 
 
 if __name__ == "__main__":
-    filename = "/home/dm/nasdata/dataset/csdn/traffic light/Traffic-Lights-Dataset-v3/train/train.txt"
+    filename = "/home/dm/nasdata/dataset/tmp/fall/fall-v1/train.txt"
     out_xml_dir = os.path.join(os.path.dirname(filename), "VOC/Annotations")
-    class_name = ["Red",
-                  "Green",
-                  "Yellow",
-                  "off",
-                  "GreenLeft",
-                  "GreenRight",
-                  "GreenStraight",
-                  "GreenStraightLeft",
-                  "GreenStraightRight",
-                  "RedLeft",
-                  "RedRight",
-                  "RedStraight",
-                  "RedStraightLeft"]
-    class_dict = {"Red": "red", "Green": "green", "Yellow": "yellow", "off": "off",
-                  "GreenLeft": "green",
-                  "GreenRight": "green",
-                  "GreenStraight": "green",
-                  "GreenStraightLeft": "green",
-                  "GreenStraightRight": "green",
-                  "RedLeft": "red",
-                  "RedRight": "red",
-                  "RedStraight": "red",
-                  "RedStraightLeft": "red"
-                  }
+    class_name = ['fall', 'falling', 'normal']
+    class_dict = {'fall': "down", 'falling': "bending", 'normal': "up"}
 
     convert_voc2voc(filename, out_xml_dir, out_image_dir=None, class_name=class_name, class_dict=class_dict, rename="",
                     vis=False)
```

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.0/pybaseutils/maker/convert_voc2yolo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-12 16:21:55
     @Brief  :
 """
 import os
 import numpy as np
 from tqdm import tqdm
 from pybaseutils.dataloader import parser_voc
```

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.0/pybaseutils/maker/convert_yolo2voc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-12 16:21:55
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 from tqdm import tqdm
```

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.0/pybaseutils/maker/maker_labelme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-09-05 19:48:52
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 from pybaseutils import image_utils, file_utils, coords_utils
```

### Comparing `pybaseutils-0.7.6/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.0/pybaseutils/maker/maker_voc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-09-05 19:48:52
     @Brief  :
 """
 
 import cv2
 import os
 import codecs
```

### Comparing `pybaseutils-0.7.6/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.0/pybaseutils/metrics/accuracy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-11-14 11:35:42
     @Brief  :
 """
 import torch
 import numpy as np
 from sklearn import metrics
```

### Comparing `pybaseutils-0.7.6/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.0/pybaseutils/metrics/average_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-08 08:56:25
     @Brief  :
 """
 import numpy as np
 
 
 class AverageMeter(object):
```

### Comparing `pybaseutils-0.7.6/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.0/pybaseutils/metrics/class_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*-coding: utf-8 -*-
 """
-    @Project: python-learning-notes
-    @File   : classification_report.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-07-13 13:23:05
 """
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn import metrics
 from pybaseutils import pandas_utils
 
+
 def plot_confusion_matrix(conf_matrix, labels_name, title, normalization=True):
     if normalization:
         conf_matrix = conf_matrix.astype('float') / conf_matrix.sum(axis=1)[:, np.newaxis]  # 归一化
     plt.imshow(conf_matrix, interpolation='nearest')  # 在特定的窗口上显示图像
     plt.title(title)  # 图像标题
     plt.colorbar()
     num_local = np.array(range(len(labels_name)))
@@ -25,25 +24,31 @@
     plt.ylabel('True label')
     plt.xlabel('Predicted label')
     plt.show()
 
 
 def get_confusion_matrix(true_labels, pred_labels, target_names=None, filename=None, normalization=True, plot=False,
                          title="Confusion Matrix"):
-    '''
+    """
+    混淆矩阵说明：(./docs/confusion_matrix.png)
+    （0）表行表示pred_labels，表列表示true_labels
+    （1）每一行之和表示该类别的真实样本数量
+    （2）每一列之和表示被预测为该类别的样本数量
+    （3）对角线每个元素表示该类别预测正确的样本数
+    （4）每列非对角线的数值，表示预测样本被识别错误的个数
     :param true_labels: Y-ylabel
     :param pred_labels: X-xlabel
     :param target_names: 如果输入的true_labels和pred_labels都是Int类型的label,
                          则可以使用target_names映射为class_name
     :param filename: 保存混淆矩阵文件
     :param normalization: 是将混淆矩阵转换为概率形式
     :param plot: 是否绘制混淆矩阵
     :param title:
     :return:
-    '''
+    """
     if target_names is None:
         target_names = list(set(pred_labels) | set(true_labels))
         target_names.sort()
     else:
         true_labels = [target_names[int(i)] for i in true_labels]
         pred_labels = [target_names[int(i)] for i in pred_labels]
     conf_matrix = metrics.confusion_matrix(true_labels, pred_labels, labels=target_names)
@@ -107,15 +112,15 @@
     :param dir1:
     :param filename:
     :return:
     """
     out_path = parent_dir
     if dir1:
         out_path = os.path.join(parent_dir, dir1)
-    if not os.path.exists(out_path):
+    if out_path and (not os.path.exists(out_path)):
         os.makedirs(out_path)
     if filename:
         out_path = os.path.join(out_path, filename)
     return out_path
 
 
 def create_file_path(filename):
@@ -128,14 +133,16 @@
     dirname = os.path.dirname(filename)
     out_path = create_dir(dirname, dir1=None, filename=basename)
     return out_path
 
 
 if __name__ == "__main__":
     true_labels = [0, 1, 2, 3, 3, 1, 1]  # Y
-    pred_labels = [0, 1, 2, 2, 2, 1, 0]  # X
+    pred_labels = [1, 1, 2, 2, 2, 1, 0]  # X
     # true_labels = [0, 1, 1, 2, 2]
     # pred_labels = [0, 1, 1, 2, 2]
-    target_names = ["A", "B", "C", "D"]
+    target_names = ["A0", "B1", "C2", "D3"]
+    confuse_file = "confuse.csv"
     out_result = get_classification_report(true_labels, pred_labels, target_names=target_names, output_dict=False)
     print(out_result)
-    get_confusion_matrix(true_labels, pred_labels, target_names=target_names, normalization=False,plot=True, title="NVR Confusion Matrix")
+    get_confusion_matrix(true_labels, pred_labels, target_names=target_names,
+                         normalization=False, filename=confuse_file, plot=True, title="Confusion Matrix")
```

### Comparing `pybaseutils-0.7.6/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.0/pybaseutils/metrics/plot_pr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-08-11 16:11:13
     @Brief  : https://www.cnblogs.com/volcao/p/9401304.html
     @Brief  : https://blog.csdn.net/u012370185/article/details/98244530
 """
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn import metrics
```

### Comparing `pybaseutils-0.7.6/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.0/pybaseutils/metrics/plot_roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-08-11 16:11:13
     @Brief  : https://www.cnblogs.com/volcao/p/9401304.html
     @Brief  : https://blog.csdn.net/u012370185/article/details/98244530
 """
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn import metrics
```

### Comparing `pybaseutils-0.7.6/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.0/pybaseutils/numpy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 """
     @Project: python-learning-notes
     @File   : numpy_tools.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-10-23 12:01:36
 """
 import numpy as np
 import math
 from sklearn import metrics, preprocessing
 import heapq
```

### Comparing `pybaseutils-0.7.6/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.0/pybaseutils/pandas_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 """
     @Project: python-learning-notes
     @File   : pandas_tools.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-07-30 20:13:59
 """
 import numpy as np
 import pandas as pd
 
 
 def read_csv(filename, usecols=None):
```

### Comparing `pybaseutils-0.7.6/pybaseutils/plot_utils.py` & `pybaseutils-0.8.0/pybaseutils/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 """
     @Project: python-learning-notes
     @File   : plot_utils.py
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-07-13 16:30:10
 """
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import PIL.Image as Image
 import platform
```

### Comparing `pybaseutils-0.7.6/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.0/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.0/pybaseutils/pycpp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-25 16:39:57
     @Brief  : ctypes例子：https://blog.csdn.net/milkhoko/article/details/119326249
               ctypes例子：https://blog.csdn.net/u012819437/article/details/89642312
               ctypes指针: https://blog.csdn.net/weixin_39636057/article/details/109948238
 """
 import ctypes
 import cv2
```

### Comparing `pybaseutils-0.7.6/pybaseutils/setup_config.py` & `pybaseutils-0.8.0/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/thread_utils.py` & `pybaseutils-0.8.0/pybaseutils/thread_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-05-01 16:36:18
-    @Url    : https://blog.csdn.net/xiaoyu_wu/article/details/102820384
+    @Url    : 官方API说明：https://docs.python.org/zh-tw/3.6/library/threading.html
+            https://blog.csdn.net/xiaoyu_wu/article/details/102820384
             python多进程&多线程
             由于多线程受GIL全局解释器锁的影响，多进程比多线程性能好，
             python多线程采用GIL(全局解释器锁)加锁机制，线程在执行代码时，必须先获得这把锁，才获得CPU执行代码指令。
             如果这把锁被其他线程占用，该线程就只能等待，等到占有该锁的线程释放锁。在进行数值计算时，python的多线程可能会更慢；
             但在进行网络爬虫，文件读写的时候，使用多线程会更快（因为每个线程执行的时候都是在请求外部的资源，而非CPU内部的计算
             参考：https://blog.csdn.net/weixin_42176112/article/details/117790945
 """
```

### Comparing `pybaseutils-0.7.6/pybaseutils/time_utils.py` & `pybaseutils-0.8.0/pybaseutils/time_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-05-25 18:19:34
     @Brief  :
 """
 import time
 import numpy as np
 from typing import Dict, List
```

### Comparing `pybaseutils-0.7.6/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.0/pybaseutils/tracemalloc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-05-25 18:19:34
     @Brief  : https://zhuanlan.zhihu.com/p/494763838
     @Brief  : https://zhuanlan.zhihu.com/p/38600861(不要在Python 3中缓存Exception对象)
 """
 import cv2
 import copy
 import numpy as np
```

### Comparing `pybaseutils-0.7.6/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.0/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.0/pybaseutils/transforms/affine_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2021-05-25 09:31:17
 """
 import numpy as np
 import cv2
 import numbers
 import random
 import PIL.Image as Image
```

### Comparing `pybaseutils-0.7.6/pybaseutils/word_utils.py` & `pybaseutils-0.8.0/pybaseutils/word_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-03-29 16:15:09
     @Brief  :
 """
 import cv2
 import numpy as np
 from typing import List, Tuple, Dict
 from pybaseutils import image_utils, json_utils, file_utils
@@ -87,16 +87,16 @@
         text = ["{}={}".format(key, hw_word[key]) for key in keys if key in hw_word]
         print("\t".join(text))
         if hw_word['mask'] is None:
             continue
         if gt_word['mask'] is None:
             hw_gt_images.append({"image": hw_word['mask'], "label": label})
             continue
-        stroke_scores = hw_word['stroke_scores'] if 'stroke_scores' in hw_word else []
-        hw_texts = ["{:3.3f}".format(s) for s in stroke_scores]
+        stroke_score = hw_word['stroke_score'] if 'stroke_score' in hw_word else []
+        hw_texts = ["{:3.3f}".format(s) for s in stroke_score]
         hw_gt_image = concat_hw_gt_stroke_image(hw_mask=hw_word['mask'], hw_segs=hw_word['stroke_segs'],
                                                 gt_mask=gt_word['mask'], gt_segs=gt_word['stroke_segs'],
                                                 hw_texts=hw_texts, vis=vis)
         hw_gt_images.append({"image": hw_gt_image, "label": label})
 
         for i in range(len(hw_word['piece_segs'])):
             hw_stroke = hw_word['stroke_segs'][i]
```

### Comparing `pybaseutils-0.7.6/pybaseutils/worker.py` & `pybaseutils-0.8.0/pybaseutils/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-05-01 16:36:18
     @Url    : https://blog.csdn.net/xiaoyu_wu/article/details/102820384
 """
 
 import threading
 from queue import Queue
 from typing import List
```

### Comparing `pybaseutils-0.7.6/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.0/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.0/pybaseutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.7.6
+Version: 0.8.0
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
-Author-email: pan_jinquan@163.com
+Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
```

### Comparing `pybaseutils-0.7.6/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.0/pybaseutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 pybaseutils/metrics/plot_roc.py
 pybaseutils/pycpp/__init__.py
 pybaseutils/pycpp/demo.py
 pybaseutils/pycpp/main.py
 pybaseutils/transforms/__init__.py
 pybaseutils/transforms/affine_transform.py
 test_py/__init__.py
+test_py/class_names.py
 test_py/demo1.py
 test_py/demo2.py
 test_py/demo_copy_files.py
 test_py/demo_copy_files_for_voc.py
 test_py/demo_correction_v1.py
 test_py/demo_correction_v2.py
 test_py/demo_correction_v3.py
@@ -75,14 +76,15 @@
 test_py/demo_get_file_list.py
 test_py/demo_gif.py
 test_py/demo_metrics.py
 test_py/demo_mouse.py
 test_py/demo_pandas.py
 test_py/demo_plot.py
 test_py/demo_standard_image .py
+test_py/demo_standard_video .py
 test_py/demo_taichi.py
 test_py/demo_video.py
 test_py/demo_voc_crop.py
 test_py/demo_voc_vis.py
 test_py/demo_word_similar.py
 test_py/demo_worker1.py
 test_py/demo_worker2.py
@@ -90,10 +92,13 @@
 test_py/performance.py
 test_py/converter/AffectNet.py
 test_py/converter/AsianMovie.py
 test_py/converter/BITVehicle2voc.py
 test_py/converter/BSTLD2voc.py
 test_py/converter/CCPD.py
 test_py/converter/CCPD2voc.py
+test_py/converter/TT100K.py
 test_py/converter/__init__.py
 test_py/converter/detect_face_person.py
+test_py/converter/insects_for_aichallenger.py
+test_py/converter/tt100k_utils.py
 test_py/converter/ua_detrac2voc.py
```

### Comparing `pybaseutils-0.7.6/README.md` & `pybaseutils-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/setup.py` & `pybaseutils-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2019-06-12 20:13:04
 """
 import os
 import pybaseutils
 import pypandoc
 from setuptools import setup, find_packages
 
@@ -13,15 +13,15 @@
 long_description = pypandoc.convert('README.md', 'rst')
 setup(name='pybaseutils',
       version=pybaseutils.__version__,
       description='pybaseutils',
       long_description=long_description,
       url='https://github.com/PanJinquan/base-utils',
       author='PanJinquan',
-      author_email='pan_jinquan@163.com',
+      author_email='390737991@qq.com',
       license='MIT',
       packages=find_packages(where=".",
                              exclude=["build", "configs", "data", "dist", "basetrainer.egg-info", "test",
                                       '.idea', ".gitignore",
                                       ]),  # 为空为全部
       package_data={
           # 如果包中含有.txt文件，则包含它
```

### Comparing `pybaseutils-0.7.6/test_py/converter/AffectNet.py` & `pybaseutils-0.8.0/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.0/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.0/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.0/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/CCPD.py` & `pybaseutils-0.8.0/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.0/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/detect_face_person.py` & `pybaseutils-0.8.0/test_py/converter/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.0/test_py/converter/ua_detrac2voc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-12 16:21:55
     @Brief  :
 """
 import os
 import cv2
 import xmltodict
 from tqdm import tqdm
```

### Comparing `pybaseutils-0.7.6/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.0/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/demo_correction_v1.py` & `pybaseutils-0.8.0/test_py/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/demo_correction_v2.py` & `pybaseutils-0.8.0/test_py/demo_correction_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-07-27 15:23:24
     @Brief  :
 """
 import cv2
 import numpy as np
 from pybaseutils.cvutils import mouse_utils, corner_utils
 from pybaseutils import file_utils, image_utils
```

### Comparing `pybaseutils-0.7.6/test_py/demo_correction_v3.py` & `pybaseutils-0.8.0/test_py/demo_correction_v3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-07-27 15:23:24
     @Brief  :
 """
 import cv2
 from page_dewarp.image import WarpedImage
 # from page_dewarp.options import cfg
 # from page_dewarp.pdf import save_pdf
```

### Comparing `pybaseutils-0.7.6/test_py/demo_get_file_list.py` & `pybaseutils-0.8.0/test_py/demo_get_file_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 # --------------------------------------------------------
 # @Project: python-learning-notes
-# @Author : panjq
-# @E-mail : pan_jinquan@163.com
+# @Author : Pan
+# @E-mail : 390737991@qq.com
 # @Date   : 2020-06-18 21:53:04
 # --------------------------------------------------------
 """
 import os
 import random
 from tqdm import tqdm
 from pybaseutils import file_utils, image_utils
@@ -63,10 +63,10 @@
         max_num = min(max_num, len(file_list))
         file_list = file_list[0:max_num]
     file_utils.write_list_data(filename, file_list)
     print("num files:{},out_path:{}".format(len(file_list), filename))
 
 
 if __name__ == "__main__":
-    file_dir = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/eyeglasses-v2/face-eyeglasses/JPEGImages"
-    save_file_list(file_dir, prefix="", postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=True,
+    file_dir = "/home/dm/nasdata/dataset/tmp/fall/Fall-Down-Det-v3/JPEGImages"
+    save_file_list(file_dir, prefix="", postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=False,
                    max_num=None)
```

### Comparing `pybaseutils-0.7.6/test_py/demo_gif.py` & `pybaseutils-0.8.0/test_py/demo_gif.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-11-17 18:43:21
     @Brief  :
 """
 from pybaseutils import file_utils, image_utils
 
 if __name__ == "__main__":
     """深度学习目标检测"""
```

### Comparing `pybaseutils-0.7.6/test_py/demo_metrics.py` & `pybaseutils-0.8.0/test_py/demo_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-07-26 15:55:30
     @Brief  :
 """
 from pybaseutils.metrics import class_report
 
 
 def binary_class_example():
```

### Comparing `pybaseutils-0.7.6/test_py/demo_mouse.py` & `pybaseutils-0.8.0/test_py/demo_mouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-07-27 15:23:24
     @Brief  :
 """
 import cv2
 import numpy as np
 from pybaseutils import image_utils
 from pybaseutils.cvutils import mouse_utils
```

### Comparing `pybaseutils-0.7.6/test_py/demo_pandas.py` & `pybaseutils-0.8.0/test_py/demo_pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-10-13 18:14:53
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 from pybaseutils import pandas_utils, image_utils, file_utils
```

### Comparing `pybaseutils-0.7.6/test_py/demo_plot.py` & `pybaseutils-0.8.0/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/demo_taichi.py` & `pybaseutils-0.8.0/test_py/demo_taichi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-09-08 09:22:01
     @Brief  :
 """
 
 import time
 import taichi as ti
 import cv2
```

### Comparing `pybaseutils-0.7.6/test_py/demo_video.py` & `pybaseutils-0.8.0/test_py/demo_video.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-11-24 14:03:56
     @Brief  :
 """
 from pybaseutils import image_utils, file_utils
 from pybaseutils.cvutils import video_utils
 
 
@@ -14,28 +14,29 @@
     h, w = frame.shape[:2]
     frame = image_utils.get_bbox_crop(frame, bbox=[60, 5, 1280, 815])
     return frame
 
 
 def resize_android(frame):
     h, w = frame.shape[:2]
-    frame = image_utils.resize_image(frame, size=(None, 640))  # android-video
+    frame = image_utils.resize_image(frame, size=(None, 580))  # android-video
     return frame
 
 
 def resize_fun(frame):
     h, w = frame.shape[:2]
     frame = image_utils.resize_image(frame, size=(360, None))
     # frame = image_utils.resize_image(frame, size=(None, 640))  # android-video
     return frame
 
 
 def android_gif():
-    video_file = "/home/dm/nasdata/dataset/csdn/emotion/demo/emotion-android.mp4"
-    video_utils.video2gif(video_file, interval=6, func=resize_android, fps=4, use_pil=False, vis=True)
+    # video_file = "/media/dm/新加卷/SDK/CSDN/双目测距/demo/image-nouse-wls.mp4"
+    video_file = "/media/dm/新加卷/SDK/CSDN/双目测距/demo/image-use-wls.mp4"
+    video_utils.video2gif(video_file, interval=6, func=resize_android, fps=3, use_pil=False, vis=True)
 
 
 def python_gif():
     video_file = "/home/dm/nasdata/dataset/csdn/emotion/demo/emotion-python.avi"
     video_utils.video2gif(video_file, interval=5, func=resize_fun, fps=6, use_pil=False, vis=True)
 
 
@@ -46,9 +47,9 @@
     # video2video(video_file, dst_file, vis=True)
     # image_dir = "/home/dm/视频/Kazam_screencast_00000"
     # video_utils.frames2video(image_dir,interval=1, fps=1)
     # image_utils.image_dir2gif(image_dir, size=(None, 600), interval=6, fps=2, loop=0, padding=False, use_pil=False)
 
 
 if __name__ == "__main__":
-    # android_gif()
-    python_gif()
+    android_gif()
+    # python_gif()
```

### Comparing `pybaseutils-0.7.6/test_py/demo_voc_vis.py` & `pybaseutils-0.8.0/test_py/demo_voc_vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,33 +10,38 @@
 if __name__ == "__main__":
     # from models.transforms import data_transforms
     # filename = "/home/dm/nasdata/dataset/csdn/traffic light/VOC/train.txt"
     # class_name = "/home/dm/nasdata/dataset/csdn/traffic light/VOC/class_name.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v1/train.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/face_person/MPII/test.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/face-eyeglasses/trainval.txt"
-    filename = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/eyeglasses-test/face/test.txt"
+    # filename = "/home/dm/nasdata/dataset/tmp/insects/VOC2/VOC/VOCdevkit/trainval.txt"
+    filename = "/home/dm/cv/panjinquan/dataset/tmp/fall/Fall-Down-Det-v2/train.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-old/train.txt"
-    class_name = ["face", "face-eyeglasses"]
+    # class_name = ["face", "face-eyeglasses"]
+    # class_name = "/home/dm/nasdata/dataset/tmp/traffic-sign/TT100K/VOC/train/class_name.txt"
     # class_name = ["unique"]
     # class_name =None
+    # class_name =['10+', 'dog', 'down', 'person']
     use_rgb = False
+    class_name = None
     dataset = parser_voc.VOCDataset(filename=filename,
                                     data_root=None,
                                     anno_dir=None,
                                     image_dir=None,
                                     class_name=class_name,
                                     transform=None,
                                     use_rgb=use_rgb,
                                     check=False,
-                                    shuffle=True)
+                                    shuffle=False)
     print("have num:{}".format(len(dataset)))
     class_name = dataset.class_name
     for i in range(len(dataset)):
+        i=113
         print(i)
         data = dataset.__getitem__(i)
         image, targets, image_id = data["image"], data["target"], data["image_id"]
         print(image_id)
         bboxes, labels = targets[:, 0:4], targets[:, 4:5]
         image = parser_voc.show_target_image(image, bboxes, labels, normal=False, transpose=False,
-                                             class_name=class_name, use_rgb=use_rgb)
+                                             class_name=class_name, use_rgb=use_rgb,thickness=2, fontScale=1)
         # image = show_boxes_image(image, Dataset.cxcywh2xyxy(bboxes, 0, 0), labels, normal=False, transpose=True)
```

### Comparing `pybaseutils-0.7.6/test_py/demo_word_similar.py` & `pybaseutils-0.8.0/test_py/demo_word_similar.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 from tqdm import tqdm
 from multiprocessing import Pool
 import numpy as np
 from pybaseutils import file_utils, image_utils, base64_utils, time_utils, font_utils, json_utils
 
 
 def read_word_file(file):
-    words = file_utils.read_data(file, split=None)
-    words_ = []
-    for ws in words:
-        ws = font_utils.get_string_chinese(ws)
-        ws = [w for w in ws]
-        words_ += ws
-    words_ = list(set(words_))
-    return words_
+    words_list = file_utils.read_data(file, split=None)
+    words_dict = {}
+    count = 0
+    for ws in words_list:
+        # ws = font_utils.get_string_chinese(ws)
+        for w in ws:
+            assert w not in words_dict, Exception(f"Error:该组:[{ws}]的字:[{w}],在其他组中存在了,请合并")
+            words_dict[w] = count
+            count += 1
+    words = list(words_dict.keys())
+    print(words_dict)
+    print("have:{}".format(len(words_dict)))
+    filename = file_utils.create_dir(os.path.dirname(file), None, "word.txt")
+    file_utils.write_list_data(filename, words)
+    print("num files:{},out_path:{}".format(len(words), filename))
+    return words_dict
 
 
 def filter_words(classes, target):
     classes = [c for c in classes if c in target]
     return classes
 
 
 if __name__ == "__main__":
-    file = "/home/dm/nasdata/dataset-dmai/handwriting/word-class/trainval/class_name3594.txt"
-    file1 = "/home/dm/nasdata/dataset-dmai/handwriting/word-class/word-similar/【DMICE0084】书法评测研发项目-字库v4形近字表梳理_第二批_1135字.txt"
-    file2 = "/home/dm/nasdata/dataset-dmai/handwriting/word-class/word-similar/【DMICE0084】书法评测研发项目-字库v4形近字表梳理_第一批_2459字.txt"
-    target = read_word_file(file)
-    class1 = read_word_file(file1)
-    class2 = read_word_file(file2)
-    classes = list(set(class1 + class2))
-    classes = filter_words(classes, target)
-    print(len(classes))
-    print(classes)
+    file = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/trainval/similar/形近字表v2.txt"
+    classes = read_word_file(file)
```

### Comparing `pybaseutils-0.7.6/test_py/demo_worker1.py` & `pybaseutils-0.8.0/test_py/demo_worker1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-04-25 16:20:17
     @Brief  :
 """
 import threading
 import time
 import queue
 from concurrent.futures import ThreadPoolExecutor
```

### Comparing `pybaseutils-0.7.6/test_py/demo_worker2.py` & `pybaseutils-0.8.0/test_py/demo_worker2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : panjq
-    @E-mail : pan_jinquan@163.com
+    @Author : Pan
+    @E-mail : 390737991@qq.com
     @Date   : 2022-04-25 16:20:17
     @Brief  :
 """
 import threading
 import time
 import random
 from pybaseutils.worker import Worker, Compose
```

### Comparing `pybaseutils-0.7.6/test_py/men_tracemalloc.py` & `pybaseutils-0.8.0/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.7.6/test_py/performance.py` & `pybaseutils-0.8.0/test_py/performance.py`

 * *Files identical despite different names*

