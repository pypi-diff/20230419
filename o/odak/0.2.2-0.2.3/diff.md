# Comparing `tmp/odak-0.2.2.tar.gz` & `tmp/odak-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odak-0.2.2.tar", last modified: Thu Feb  9 09:56:34 2023, max compression
+gzip compressed data, was "odak-0.2.3.tar", last modified: Wed Apr 19 21:12:49 2023, max compression
```

## Comparing `odak-0.2.2.tar` & `odak-0.2.3.tar`

### file list

```diff
@@ -1,137 +1,142 @@
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.431158 odak-0.2.2/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    16726 2022-07-30 19:22:11.000000 odak-0.2.2/LICENSE.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    20692 2023-02-09 09:56:34.431158 odak-0.2.2/PKG-INFO
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3737 2023-01-22 15:02:48.000000 odak-0.2.2/README.md
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      148 2022-09-08 19:26:01.000000 odak-0.2.2/THANKS.txt
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      482 2022-11-18 22:37:53.000000 odak-0.2.2/odak/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/catalog/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      186 2022-07-30 19:22:11.000000 odak-0.2.2/odak/catalog/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/catalog/data/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1788 2022-07-30 19:22:11.000000 odak-0.2.2/odak/catalog/data/plano_convex_lenses.json
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     8433 2022-07-30 19:22:11.000000 odak-0.2.2/odak/catalog/detectors.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4614 2022-07-30 19:22:11.000000 odak-0.2.2/odak/catalog/diffusers.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4347 2022-12-27 23:51:29.000000 odak-0.2.2/odak/catalog/lenses.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/fit/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4477 2022-10-28 20:57:49.000000 odak-0.2.2/odak/fit/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/jones/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1576 2022-07-30 19:22:11.000000 odak-0.2.2/odak/jones/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/learn/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      301 2022-12-02 11:09:02.000000 odak-0.2.2/odak/learn/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak/learn/models/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      190 2022-12-02 11:15:24.000000 odak-0.2.2/odak/learn/models/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7313 2022-12-10 10:40:39.000000 odak-0.2.2/odak/learn/models/components.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/learn/perception/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      481 2022-12-02 15:28:41.000000 odak-0.2.2/odak/learn/perception/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4383 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/blur_loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3511 2022-12-02 15:45:59.000000 odak-0.2.2/odak/learn/perception/color_conversion.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    13054 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/foveation.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7495 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/metamer_mse_loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    13855 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/metameric_loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     9384 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/metameric_loss_uniform.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     6933 2023-01-22 15:02:48.000000 odak-0.2.2/odak/learn/perception/radially_varying_blur.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     9549 2022-09-08 19:26:01.000000 odak-0.2.2/odak/learn/perception/spatial_steerable_pyramid.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    52251 2022-09-08 19:26:01.000000 odak-0.2.2/odak/learn/perception/steerable_pyramid_filters.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      692 2022-09-08 19:26:01.000000 odak-0.2.2/odak/learn/perception/util.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/learn/raytracing/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      303 2022-07-30 19:22:11.000000 odak-0.2.2/odak/learn/raytracing/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     6576 2022-07-30 19:22:11.000000 odak-0.2.2/odak/learn/raytracing/boundary.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     2168 2022-07-30 19:22:11.000000 odak-0.2.2/odak/learn/raytracing/primitives.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3207 2022-12-28 00:11:22.000000 odak-0.2.2/odak/learn/raytracing/ray.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/learn/tools/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      328 2022-12-03 14:01:11.000000 odak-0.2.2/odak/learn/tools/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     2830 2022-12-03 14:22:12.000000 odak-0.2.2/odak/learn/tools/file.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3319 2022-11-18 22:38:44.000000 odak-0.2.2/odak/learn/tools/fitcurve.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4408 2022-12-10 11:37:47.000000 odak-0.2.2/odak/learn/tools/loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      676 2022-11-30 13:31:07.000000 odak-0.2.2/odak/learn/tools/mask.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     6019 2022-12-02 11:08:30.000000 odak-0.2.2/odak/learn/tools/matrix.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1410 2022-07-30 19:22:11.000000 odak-0.2.2/odak/learn/tools/sample.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7178 2022-09-08 19:26:01.000000 odak-0.2.2/odak/learn/tools/transformation.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1549 2022-07-30 19:22:11.000000 odak-0.2.2/odak/learn/tools/vector.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/learn/wave/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      534 2023-02-09 09:38:40.000000 odak-0.2.2/odak/learn/wave/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    24638 2023-01-02 11:30:25.000000 odak-0.2.2/odak/learn/wave/classical.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3471 2022-09-08 19:26:01.000000 odak-0.2.2/odak/learn/wave/lens.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    12604 2023-02-09 09:47:06.000000 odak-0.2.2/odak/learn/wave/loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    17446 2023-02-09 09:42:26.000000 odak-0.2.2/odak/learn/wave/optimizer.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     5315 2023-01-22 15:04:40.000000 odak-0.2.2/odak/learn/wave/util.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/manager/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3419 2022-07-30 19:22:11.000000 odak-0.2.2/odak/manager/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/measurement/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      169 2022-07-30 19:22:11.000000 odak-0.2.2/odak/measurement/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4235 2022-07-30 19:22:11.000000 odak-0.2.2/odak/measurement/image_quality.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.423158 odak-0.2.2/odak/raytracing/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      297 2022-07-30 19:22:11.000000 odak-0.2.2/odak/raytracing/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    12385 2022-12-28 00:09:22.000000 odak-0.2.2/odak/raytracing/boundary.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7282 2022-12-27 23:52:31.000000 odak-0.2.2/odak/raytracing/primitives.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     5860 2022-12-28 00:09:22.000000 odak-0.2.2/odak/raytracing/ray.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.427158 odak-0.2.2/odak/tools/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      304 2022-10-28 20:57:49.000000 odak-0.2.2/odak/tools/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     5873 2022-12-27 23:46:55.000000 odak-0.2.2/odak/tools/asset.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      820 2022-07-30 19:22:11.000000 odak-0.2.2/odak/tools/conversions.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7196 2022-11-01 22:58:44.000000 odak-0.2.2/odak/tools/file.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     8238 2022-12-27 23:59:26.000000 odak-0.2.2/odak/tools/matrix.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     9643 2022-07-30 19:22:11.000000 odak-0.2.2/odak/tools/sample.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     5575 2022-12-27 23:53:54.000000 odak-0.2.2/odak/tools/transformation.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4461 2022-12-27 23:50:27.000000 odak-0.2.2/odak/tools/vector.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.427158 odak-0.2.2/odak/visualize/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      143 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/__init__.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.427158 odak-0.2.2/odak/visualize/blender/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1758 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/blender/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    15285 2022-12-27 23:50:12.000000 odak-0.2.2/odak/visualize/blender/libblend.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1586 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/blender/server.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     5129 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/blender/wrapper.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3541 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/export.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    19743 2022-07-30 19:22:11.000000 odak-0.2.2/odak/visualize/plotly.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.427158 odak-0.2.2/odak/wave/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     7545 2022-12-27 23:54:41.000000 odak-0.2.2/odak/wave/__init__.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    24694 2022-12-27 23:54:17.000000 odak-0.2.2/odak/wave/classical.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     4193 2022-07-30 19:22:11.000000 odak-0.2.2/odak/wave/lens.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1039 2022-07-30 19:22:11.000000 odak-0.2.2/odak/wave/utils.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3254 2022-07-30 19:22:11.000000 odak-0.2.2/odak/wave/vector.py
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.419158 odak-0.2.2/odak.egg-info/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)    20692 2023-02-09 09:56:34.000000 odak-0.2.2/odak.egg-info/PKG-INFO
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     3188 2023-02-09 09:56:34.000000 odak-0.2.2/odak.egg-info/SOURCES.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)        1 2023-02-09 09:56:34.000000 odak-0.2.2/odak.egg-info/dependency_links.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)       77 2023-02-09 09:56:34.000000 odak-0.2.2/odak.egg-info/requires.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      249 2023-02-09 09:56:34.000000 odak-0.2.2/odak.egg-info/top_level.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)       77 2022-10-28 22:57:10.000000 odak-0.2.2/requirements.txt
--rw-rw-r--   0 kaan      (1000) kaan      (1000)       38 2023-02-09 09:56:34.431158 odak-0.2.2/setup.cfg
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1859 2023-02-09 09:53:45.000000 odak-0.2.2/setup.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      305 2022-08-11 12:17:27.000000 odak-0.2.2/short_readme.md
-drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-02-09 09:56:34.431158 odak-0.2.2/test/
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1546 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_3d_gerchberg_saxton.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      603 2022-12-27 23:56:02.000000 odak-0.2.2/test/test_PLY.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1284 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_beam_propagation.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      791 2022-09-08 19:26:01.000000 odak-0.2.2/test/test_curve_fit.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1033 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_cylinder_intersection.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      878 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_detector.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1311 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_diffuser.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      394 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_export_import_PLY.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1261 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_gerchberg_saxton.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1569 2022-10-28 20:57:49.000000 odak-0.2.2/test/test_gradient_descent_1d.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      138 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_import.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1376 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_intersect_reflect.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      262 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_jones.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1439 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_learn_beam_propagation.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      568 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_learn_gerchberg_saxton.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      630 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_learn_gradient_descent.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      810 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_learn_lenses.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1122 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_learn_loss.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      526 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_learn_point_wise.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1170 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_learn_ray_intersect_w_a_triangle.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      660 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_learn_sgd.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      416 2022-10-28 20:57:49.000000 odak-0.2.2/test/test_least_square.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      816 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_lenses.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      538 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_mtf.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     2261 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_perceptron.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1281 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_perceptual_losses.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      625 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_plano_convex_lens.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1156 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_propagate_field.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      786 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_ray_intersect_w_a_surface.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1130 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_ray_intersect_w_a_triangle.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)     1380 2023-01-22 15:02:48.000000 odak-0.2.2/test/test_rayleigh.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      600 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_sample_ray.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      575 2022-10-28 22:54:32.000000 odak-0.2.2/test/test_save_load.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      994 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_sphere_intersection.py
--rw-rw-r--   0 kaan      (1000) kaan      (1000)      528 2022-07-30 19:22:11.000000 odak-0.2.2/test/test_two_rays_closest_point.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.719767 odak-0.2.3/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    16726 2022-07-30 19:22:11.000000 odak-0.2.3/LICENSE.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    20712 2023-04-19 21:12:49.719767 odak-0.2.3/PKG-INFO
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3712 2023-04-19 21:06:04.000000 odak-0.2.3/README.md
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      148 2023-04-15 22:46:01.000000 odak-0.2.3/THANKS.txt
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.611768 odak-0.2.3/odak/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      482 2023-04-15 22:46:01.000000 odak-0.2.3/odak/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/catalog/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      186 2022-07-30 19:22:11.000000 odak-0.2.3/odak/catalog/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/catalog/data/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1788 2022-07-30 19:22:11.000000 odak-0.2.3/odak/catalog/data/plano_convex_lenses.json
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     8433 2022-07-30 19:22:11.000000 odak-0.2.3/odak/catalog/detectors.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4614 2022-07-30 19:22:11.000000 odak-0.2.3/odak/catalog/diffusers.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4347 2023-04-12 08:29:59.000000 odak-0.2.3/odak/catalog/lenses.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/fit/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4477 2022-10-28 20:57:49.000000 odak-0.2.3/odak/fit/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/jones/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1576 2022-07-30 19:22:11.000000 odak-0.2.3/odak/jones/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/learn/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      301 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak/learn/models/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      212 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/models/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    19903 2023-04-15 22:46:15.000000 odak-0.2.3/odak/learn/models/components.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5565 2023-04-19 21:06:14.000000 odak-0.2.3/odak/learn/models/models.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.619768 odak-0.2.3/odak/learn/perception/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      481 2022-12-02 15:28:41.000000 odak-0.2.3/odak/learn/perception/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4383 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/blur_loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    11549 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/color_conversion.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    13054 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/foveation.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     7495 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/metamer_mse_loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    13855 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/metameric_loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     9384 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/metameric_loss_uniform.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     6933 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/perception/radially_varying_blur.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     9549 2022-09-08 19:26:01.000000 odak-0.2.3/odak/learn/perception/spatial_steerable_pyramid.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    52251 2022-09-08 19:26:01.000000 odak-0.2.3/odak/learn/perception/steerable_pyramid_filters.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      692 2022-09-08 19:26:01.000000 odak-0.2.3/odak/learn/perception/util.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.623768 odak-0.2.3/odak/learn/raytracing/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      303 2022-07-30 19:22:11.000000 odak-0.2.3/odak/learn/raytracing/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     6576 2022-07-30 19:22:11.000000 odak-0.2.3/odak/learn/raytracing/boundary.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     2168 2022-07-30 19:22:11.000000 odak-0.2.3/odak/learn/raytracing/primitives.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3207 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/raytracing/ray.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.623768 odak-0.2.3/odak/learn/tools/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      328 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/tools/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3506 2023-04-19 21:06:04.000000 odak-0.2.3/odak/learn/tools/file.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3349 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/tools/fitcurve.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     6786 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/tools/loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      676 2023-04-12 08:29:59.000000 odak-0.2.3/odak/learn/tools/mask.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     6731 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/tools/matrix.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1410 2022-07-30 19:22:11.000000 odak-0.2.3/odak/learn/tools/sample.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     7178 2022-09-08 19:26:01.000000 odak-0.2.3/odak/learn/tools/transformation.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1549 2022-07-30 19:22:11.000000 odak-0.2.3/odak/learn/tools/vector.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.627768 odak-0.2.3/odak/learn/wave/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      562 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    24686 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/classical.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5155 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/lens.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    12834 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    11249 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/optimizers.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    10871 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/propagators.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5099 2023-04-15 22:46:01.000000 odak-0.2.3/odak/learn/wave/util.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.627768 odak-0.2.3/odak/manager/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3419 2022-07-30 19:22:11.000000 odak-0.2.3/odak/manager/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.627768 odak-0.2.3/odak/measurement/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      169 2022-07-30 19:22:11.000000 odak-0.2.3/odak/measurement/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4235 2022-07-30 19:22:11.000000 odak-0.2.3/odak/measurement/image_quality.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.631768 odak-0.2.3/odak/raytracing/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      297 2022-07-30 19:22:11.000000 odak-0.2.3/odak/raytracing/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    12385 2023-04-12 08:29:59.000000 odak-0.2.3/odak/raytracing/boundary.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     7282 2023-04-12 08:29:59.000000 odak-0.2.3/odak/raytracing/primitives.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5860 2023-04-12 08:29:59.000000 odak-0.2.3/odak/raytracing/ray.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.635768 odak-0.2.3/odak/tools/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      304 2022-10-28 20:57:49.000000 odak-0.2.3/odak/tools/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5873 2023-04-12 08:29:59.000000 odak-0.2.3/odak/tools/asset.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      820 2022-07-30 19:22:11.000000 odak-0.2.3/odak/tools/conversions.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     7356 2023-04-19 21:06:04.000000 odak-0.2.3/odak/tools/file.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     8238 2023-04-12 08:29:59.000000 odak-0.2.3/odak/tools/matrix.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     9643 2022-07-30 19:22:11.000000 odak-0.2.3/odak/tools/sample.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5575 2023-04-12 08:29:59.000000 odak-0.2.3/odak/tools/transformation.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4461 2023-04-12 08:29:59.000000 odak-0.2.3/odak/tools/vector.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.643768 odak-0.2.3/odak/visualize/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      143 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/__init__.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.659767 odak-0.2.3/odak/visualize/blender/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1758 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/blender/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    15285 2023-04-12 08:29:59.000000 odak-0.2.3/odak/visualize/blender/libblend.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1586 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/blender/server.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     5129 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/blender/wrapper.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3541 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/export.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    19743 2022-07-30 19:22:11.000000 odak-0.2.3/odak/visualize/plotly.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.675767 odak-0.2.3/odak/wave/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     7545 2023-04-12 08:29:59.000000 odak-0.2.3/odak/wave/__init__.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    24694 2023-04-12 08:29:59.000000 odak-0.2.3/odak/wave/classical.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     4193 2022-07-30 19:22:11.000000 odak-0.2.3/odak/wave/lens.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1039 2022-07-30 19:22:11.000000 odak-0.2.3/odak/wave/utils.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3254 2022-07-30 19:22:11.000000 odak-0.2.3/odak/wave/vector.py
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.615768 odak-0.2.3/odak.egg-info/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)    20712 2023-04-19 21:12:49.000000 odak-0.2.3/odak.egg-info/PKG-INFO
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     3348 2023-04-19 21:12:49.000000 odak-0.2.3/odak.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)        1 2023-04-19 21:12:49.000000 odak-0.2.3/odak.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)       77 2023-04-19 21:12:49.000000 odak-0.2.3/odak.egg-info/requires.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      249 2023-04-19 21:12:49.000000 odak-0.2.3/odak.egg-info/top_level.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)       77 2022-10-28 22:57:10.000000 odak-0.2.3/requirements.txt
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)       38 2023-04-19 21:12:49.719767 odak-0.2.3/setup.cfg
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1859 2023-04-15 22:46:01.000000 odak-0.2.3/setup.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      305 2022-08-11 12:17:27.000000 odak-0.2.3/short_readme.md
+drwxrwxr-x   0 kaan      (1000) kaan      (1000)        0 2023-04-19 21:12:49.719767 odak-0.2.3/test/
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1546 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_3d_gerchberg_saxton.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      603 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_PLY.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1284 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_beam_propagation.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1181 2023-04-15 22:46:01.000000 odak-0.2.3/test/test_color_conversion.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      791 2022-09-08 19:26:01.000000 odak-0.2.3/test/test_curve_fit.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1033 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_cylinder_intersection.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      878 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_detector.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1310 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_diffuser.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      394 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_export_import_PLY.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1261 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_gerchberg_saxton.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1569 2022-10-28 20:57:49.000000 odak-0.2.3/test/test_gradient_descent_1d.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      138 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_import.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1376 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_intersect_reflect.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      262 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_jones.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1439 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_learn_beam_propagation.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1268 2023-04-15 22:59:54.000000 odak-0.2.3/test/test_learn_components.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      568 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_learn_gerchberg_saxton.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      630 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_learn_gradient_descent.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      796 2023-04-15 22:46:01.000000 odak-0.2.3/test/test_learn_lenses.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1122 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_learn_loss.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     2182 2023-04-15 22:46:01.000000 odak-0.2.3/test/test_learn_multiplane_optimizer.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      526 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_learn_point_wise.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1170 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_learn_ray_intersect_w_a_triangle.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      660 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_learn_sgd.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      416 2022-10-28 20:57:49.000000 odak-0.2.3/test/test_least_square.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      816 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_lenses.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      538 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_mtf.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     2261 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_perceptron.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1281 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_perceptual_losses.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      625 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_plano_convex_lens.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1156 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_propagate_field.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      786 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_ray_intersect_w_a_surface.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1130 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_ray_intersect_w_a_triangle.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)     1380 2023-04-12 08:29:59.000000 odak-0.2.3/test/test_rayleigh.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      600 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_sample_ray.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      575 2022-10-28 22:54:32.000000 odak-0.2.3/test/test_save_load.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      994 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_sphere_intersection.py
+-rw-rw-r--   0 kaan      (1000) kaan      (1000)      528 2022-07-30 19:22:11.000000 odak-0.2.3/test/test_two_rays_closest_point.py
```

### Comparing `odak-0.2.2/LICENSE.txt` & `odak-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/PKG-INFO` & `odak-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odak
-Version: 0.2.2
+Version: 0.2.3
 Summary: Odak, the fundamental Python library for scientific computing in optical sciences.
 Home-page: https://github.com/kaanaksit/odak
 Author: Kaan Akşit
 Author-email: kaanaksit@kaanaksit.com
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -376,19 +376,22 @@
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
 Keywords: optics,holography,perception,graphics
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.7.5
 License-File: LICENSE.txt
 
 # Odak
 Odak (pronounced "O-dac") is the fundamental library for scientific computing in optical sciences, computer graphics and visual perception.
 To learn more about what Odak can do to help your design, experimentation and development, consult to our [documentation](https://kaanaksit.github.io/odak/)!
+
+
```

### Comparing `odak-0.2.2/odak/catalog/data/plano_convex_lenses.json` & `odak-0.2.3/odak/catalog/data/plano_convex_lenses.json`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/catalog/detectors.py` & `odak-0.2.3/odak/catalog/detectors.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/catalog/diffusers.py` & `odak-0.2.3/odak/catalog/diffusers.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/catalog/lenses.py` & `odak-0.2.3/odak/catalog/lenses.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/fit/__init__.py` & `odak-0.2.3/odak/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/jones/__init__.py` & `odak-0.2.3/odak/jones/__init__.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/blur_loss.py` & `odak-0.2.3/odak/learn/perception/blur_loss.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/foveation.py` & `odak-0.2.3/odak/learn/perception/foveation.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/metamer_mse_loss.py` & `odak-0.2.3/odak/learn/perception/metamer_mse_loss.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/metameric_loss.py` & `odak-0.2.3/odak/learn/perception/metameric_loss.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/metameric_loss_uniform.py` & `odak-0.2.3/odak/learn/perception/metameric_loss_uniform.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/radially_varying_blur.py` & `odak-0.2.3/odak/learn/perception/radially_varying_blur.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/spatial_steerable_pyramid.py` & `odak-0.2.3/odak/learn/perception/spatial_steerable_pyramid.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/steerable_pyramid_filters.py` & `odak-0.2.3/odak/learn/perception/steerable_pyramid_filters.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/perception/util.py` & `odak-0.2.3/odak/learn/perception/util.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/raytracing/boundary.py` & `odak-0.2.3/odak/learn/raytracing/boundary.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/raytracing/primitives.py` & `odak-0.2.3/odak/learn/raytracing/primitives.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/raytracing/ray.py` & `odak-0.2.3/odak/learn/raytracing/ray.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/tools/file.py` & `odak-0.2.3/odak/learn/tools/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import odak.tools
 import torch
-import numpy as np_cpu
+import os
 
 
 def resize(image, multiplier = 0.5, mode = 'nearest'):
     """
     Definition to resize an image.
 
     Parameters
@@ -30,15 +30,15 @@
         new_cache = scale(cache).unsqueeze(0)
         new_image[:,:,i] = new_cache.unsqueeze(0)
     return new_image
 
 
 def load_image(fn, normalizeby = 0., torch_style = False):
     """
-    Definition to load an image from a given location as a Numpy array.
+    Definition to load an image from a given location as a torch tensor.
 
     Parameters
     ----------
     fn           : str
                    Filename.
     normalized   : float
                    Value to to normalize images with. Default value of zero will lead to no normalization.
@@ -55,15 +55,15 @@
     image = odak.tools.load_image(fn, normalizeby=normalizeby, torch_style=torch_style)
     image = torch.from_numpy(image).float()
     return image
 
 
 def save_image(fn, img, cmin=0, cmax=255, color_depth=8):
     """
-    Definition to save a Numpy array as an image.
+    Definition to save a torch tensor as an image.
 
     Parameters
     ----------
     fn           : str
                    Filename.
     img          : ndarray
                    A numpy array with NxMx3 or NxMx1 shapes.
@@ -77,14 +77,49 @@
 
     Returns
     ----------
     bool         :  bool
                     True if successful.
 
     """
+    if len(img.shape) ==  4:
+        img = img.squeeze(0)
     if len(img.shape) > 2 and torch.argmin(torch.tensor(img.shape)) == 0:
         new_img = torch.zeros(img.shape[1], img.shape[2], img.shape[0]).to(img.device)
         for i in range(img.shape[0]):
             new_img[:, :, i] = img[i].detach().clone()
         img = new_img.detach().clone()
     img = img.cpu().detach().numpy()
     return odak.tools.save_image(fn, img, cmin=cmin, cmax=cmax, color_depth=color_depth)
+
+
+def save_torch_tensor(fn, tensor):
+    """
+    Definition to save a torch tensor.
+
+
+    Parameters
+    ----------
+    fn           : str
+                   Filename.
+    tensor       : torch.tensor
+                   Torch tensor to be saved.
+    """ 
+    torch.save(tensor, os.path.expanduser(fn))
+
+
+def torch_load(fn):
+    """
+    Definition to load a torch files (*.pt).
+
+    Parameters
+    ----------
+    fn           : str
+                   Filename.
+    
+    Returns
+    -------
+    data         : any
+                   See torch.load() for more.
+    """  
+    data = torch.load(os.path.expanduser(fn))
+    return data
```

### Comparing `odak-0.2.2/odak/learn/tools/fitcurve.py` & `odak-0.2.3/odak/learn/tools/fitcurve.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,37 +45,37 @@
     def estimate(self, x):
         """
         Internal function representing the forward model w/o grad.
         """
         return self.forward(x).detach()
 
 
-    def fit(self, x_values, y_values, epochs=100, learning_rate=1e-5):
+    def fit(self, x_values, y_values, epochs = 100, learning_rate = 1e-5):
         """
         Function to train the weights of the multi layer perceptron.
 
         Parameters
         ----------
         x_values        : torch.tensor
                           Input values [mx1].
         y_values        : torch.tensor
                           Output values [nx1].
         epochs          : int
                           Number of epochs.
         learning_rate   : float
                           Learning rate of the optimizer.
         """
-        t = tqdm(range(epochs), leave=False)
+        t = tqdm(range(epochs), leave = False, dynamic_ncols = True)
         self.optimizer = torch.optim.Adam(self.parameters(), lr=learning_rate)
         self.loss_function = torch.nn.MSELoss()
         for i in t:
             self.optimizer.zero_grad()
             estimate = self.forward(x_values)
             loss = self.loss_function(estimate, y_values)
-            loss.backward(retain_graph=True)
+            loss.backward(retain_graph = True)
             self.optimizer.step()
             description = 'Loss:{:.4f}'.format(loss.item())
             t.set_description(description)
         print(description)
         return True
```

### Comparing `odak-0.2.2/odak/learn/tools/mask.py` & `odak-0.2.3/odak/learn/tools/mask.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/tools/matrix.py` & `odak-0.2.3/odak/learn/tools/matrix.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,74 +21,95 @@
     """
     divider = 2**(8-bits)
     new_field = image_field/divider
     new_field = new_field.int()
     return new_field
 
 
-def zero_pad(field, size=None, method='center'):
+def zero_pad(field, size = None, method = 'center'):
     """
     Definition to zero pad a MxN array to 2Mx2N array.
 
     Parameters
     ----------
     field             : ndarray
                         Input field MxN array.
     size              : list
-                        Size to be zeropadded.
+                        Size to be zeropadded (e.g., [1, 1, m, n] or [m, n] depending on the input field).
     method            : str
                         Zeropad either by placing the content to center or to the left.
 
     Returns
     ----------
     field_zero_padded : ndarray
                         Zeropadded version of the input field.
     """
+    squeeze = False
+    if len(field.shape) < 3:
+        field = field.unsqueeze(0)
+    if len(field.shape) < 4:
+        field = field.unsqueeze(0)
+        squeeze = True
     if type(size) == type(None):
-        hx = int(torch.ceil(torch.tensor([field.shape[0]/2])))
-        hy = int(torch.ceil(torch.tensor([field.shape[1]/2])))
+        resolution = [1, 1, 2 * field.shape[-2], 2 * field.shape[-1]]
     else:
-        hx = int(torch.ceil(torch.tensor([(size[0]-field.shape[0])/2])))
-        hy = int(torch.ceil(torch.tensor([(size[1]-field.shape[1])/2])))
+        resolution = size
+    field_zero_padded = torch.zeros(resolution, device = field.device, dtype = field.dtype)
     if method == 'center':
-        m = torch.nn.ZeroPad2d((hy, hy, hx, hx))
-    elif method == 'left aligned':
-        m = torch.nn.ZeroPad2d((0, hy*2, 0, hx*2))
-    field_zero_padded = m(field)
-    if type(size) != type(None):
-        field_zero_padded = field_zero_padded[0:size[0], 0:size[1]]
+       field_zero_padded[
+                         :, :,
+                         resolution[-2] // 4: resolution[-2] // 4 + field.shape[-2],
+                         resolution[-1] // 4: resolution[-1] // 4 + field.shape[-1]
+                         ] = field
+    elif method == 'left':
+       field_zero_padded[
+                         :, :,
+                         0: field.shape[-2],
+                         0: field.shape[-1]
+                        ] = field
+    if squeeze == True:
+        field_zero_padded = field_zero_padded.squeeze(0).squeeze(0)
     return field_zero_padded
 
 
-def crop_center(field, size=None):
+def crop_center(field, size = None):
     """
     Definition to crop the center of a field with 2Mx2N size. The outcome is a MxN array.
 
     Parameters
     ----------
     field       : ndarray
-                  Input field 2Mx2N array.
+                  Input field 2M x 2N or K x L x 2M x 2N array.
     size        : list
-                  Dimensions to crop with respect to center of the image.
+                  Dimensions to crop with respect to center of the image (e.g., M x N or 1 x 1 x M x N).
 
     Returns
     ----------
     cropped     : ndarray
                   Cropped version of the input field.
     """
+    squeeze = False
+    if len(field.shape) < 3:
+        field = field.unsqueeze(0)
+    if len(field.shape) < 4:
+        field = field.unsqueeze(0)
+        squeeze = True
     if type(size) == type(None):
-        qx = int(torch.ceil(torch.tensor(field.shape[0])/4))
-        qy = int(torch.ceil(torch.tensor(field.shape[1])/4))
-        cropped = field[qx:3*qx, qy:3*qy]
+        qx = int(field.shape[-2] // 4)
+        qy = int(field.shape[-1] // 4)
+        cropped_padded = field[:, :, qx: qx + field.shape[-2] // 2, qy:qy + field.shape[-1] // 2]
     else:
-        cx = int(torch.ceil(torch.tensor(field.shape[0]/2)))
-        cy = int(torch.ceil(torch.tensor(field.shape[1]/2)))
-        hx = int(torch.ceil(torch.tensor(size[0]/2)))
-        hy = int(torch.ceil(torch.tensor(size[1]/2)))
-        cropped = field[cx-hx:cx+hx, cy-hy:cy+hy]
+        cx = int(field.shape[-2] // 2)
+        cy = int(field.shape[-1] // 2)
+        hx = int(size[-2] // 2)
+        hy = int(size[-1] // 2)
+        cropped_padded = field[:, :, cx-hx:cx+hx, cy-hy:cy+hy]
+    cropped = cropped_padded
+    if squeeze == True:
+        cropped = cropped_padded.squeeze(0).squeeze(0)
     return cropped
 
 
 def convolve2d(field, kernel):
     """
     Definition to convolve a field with a kernel by multiplying in frequency space.
```

### Comparing `odak-0.2.2/odak/learn/tools/sample.py` & `odak-0.2.3/odak/learn/tools/sample.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/tools/transformation.py` & `odak-0.2.3/odak/learn/tools/transformation.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/tools/vector.py` & `odak-0.2.3/odak/learn/tools/vector.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/learn/wave/classical.py` & `odak-0.2.3/odak/learn/wave/classical.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,15 @@
     device = torch.device("cuda" if cuda else "cpu")
     field = field.to(device)
     phase = torch.rand(resolution[0], resolution[1])
     amplitude = torch.ones(
         resolution[0], resolution[1], requires_grad=False).to(device)
     k = wavenumber(wavelength)
     loss_function = torch.nn.MSELoss(reduction='none').to(device)
-    t = tqdm(range(n_iteration), leave=False)
+    t = tqdm(range(n_iteration), leave = False, dynamic_ncols = True)
     hologram = generate_complex_field(amplitude, phase)
     for i in t:
         hologram_padded = zero_pad(hologram)
         reconstruction_padded = propagate_beam(
             hologram_padded, k, distance, dx, wavelength, propagation_type)
         reconstruction = crop_center(reconstruction_padded)
         reconstruction_intensity = calculate_amplitude(reconstruction)**2
@@ -414,15 +414,15 @@
         device).requires_grad_()
     amplitude = torch.ones(
         resolution[0], resolution[1], requires_grad=False).to(device)
     k = wavenumber(wavelength)
     optimizer = torch.optim.Adam([{'params': [phase]}], lr=learning_rate)
     if type(loss_function) == type(None):
         loss_function = torch.nn.MSELoss().to(device)
-    t = tqdm(range(n_iteration), leave=False)
+    t = tqdm(range(n_iteration), leave = False, dynamic_ncols = True)
     for i in t:
         optimizer.zero_grad()
         hologram = generate_complex_field(amplitude, phase)
         hologram_padded = zero_pad(hologram)
         reconstruction_padded = propagate_beam(
             hologram_padded, k, distance, dx, wavelength, propogation_type)
         reconstruction = crop_center(reconstruction_padded)
```

### Comparing `odak-0.2.2/odak/learn/wave/lens.py` & `odak-0.2.3/odak/wave/lens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,39 @@
-import torch
 import numpy as np
-from .util import wavenumber
-from ..tools import zero_pad, crop_center
+
+
+def double_convergence(nx, ny, k, r, dx):
+    """
+    A definition to generate initial phase for a Gerchberg-Saxton method. For more details consult Sun, Peng, et al. "Holographic near-eye display system based on double-convergence light Gerchberg-Saxton algorithm." Optics express 26.8 (2018): 10140-10151.
+
+    Parameters
+    ----------
+    nx         : int
+                 Size of the output along X.
+    ny         : int
+                 Size of the output along Y.
+    k          : odak.wave.wavenumber
+                 See odak.wave.wavenumber for more.
+    r          : float
+                 The distance between location of a light source and an image plane.
+    dx         : float
+                 Pixel pitch.
+
+    Returns
+    -------
+    function   : ndarray
+                 Generated phase pattern for a Gerchberg-Saxton method.
+    """
+    size = [ny, nx]
+    x = np.linspace(-size[0]*dx/2, size[0]*dx/2, size[0])
+    y = np.linspace(-size[1]*dx/2, size[1]*dx/2, size[1])
+    X, Y = np.meshgrid(x, y)
+    Z = X**2+Y**2
+    w = np.exp(1j*k*Z/r)
+    return w
 
 
 def quadratic_phase_function(nx, ny, k, focal=0.4, dx=0.001, offset=[0, 0]):
     """ 
     A definition to generate 2D quadratic phase function, which is typically use to represent lenses.
 
     Parameters
@@ -21,23 +49,23 @@
     dx         : float
                  Pixel pitch.
     offset     : list
                  Deviation from the center along X and Y axes.
 
     Returns
     -------
-    function   : torch.tensor
+    function   : ndarray
                  Generated quadratic phase function.
     """
     size = [nx, ny]
-    x = torch.linspace(-size[0] * dx / 2, size[0] * dx / 2, size[0]) - offset[1] * dx
-    y = torch.linspace(-size[1] * dx / 2, size[1] * dx / 2, size[1]) - offset[0] * dx
-    X, Y = torch.meshgrid(x, y, indexing='ij')
-    Z = X**2 + Y**2
-    qwf = torch.exp(-0.5j * k / focal * Z)
+    x = np.linspace(-size[0]*dx/2, size[0]*dx/2, size[0])-offset[1]*dx
+    y = np.linspace(-size[1]*dx/2, size[1]*dx/2, size[1])-offset[0]*dx
+    X, Y = np.meshgrid(x, y)
+    Z = X**2+Y**2
+    qwf = np.exp(1j*k*0.5*np.sin(Z/focal))
     return qwf
 
 
 def prism_phase_function(nx, ny, k, angle, dx=0.001, axis='x'):
     """
     A definition to generate 2D phase function that represents a prism. See Goodman's Introduction to Fourier Optics book for more.
 
@@ -53,31 +81,31 @@
                  Tilt angle of the prism in degrees.
     dx         : float
                  Pixel pitch.
     axis       : str
                  Axis of the prism.
 
     Returns
-    ----------
-    prism      : torch.tensor
+    -------
+    prism      : ndarray
                  Generated phase function for a prism.
     """
-    angle = torch.deg2rad(torch.tensor([angle]))
-    size = [nx, ny]
-    x = torch.linspace(-size[0]*dx/2, size[0]*dx/2, size[0])
-    y = torch.linspace(-size[1]*dx/2, size[1]*dx/2, size[1])
-    X, Y = torch.meshgrid(x, y, indexing='ij')
+    angle = np.radians(angle)
+    size = [ny, nx]
+    x = np.linspace(-size[0]*dx/2, size[0]*dx/2, size[0])
+    y = np.linspace(-size[1]*dx/2, size[1]*dx/2, size[1])
+    X, Y = np.meshgrid(x, y)
     if axis == 'y':
-        prism = torch.exp(-1j*k*torch.sin(angle)*Y)
+        prism = np.exp(-1j*k*np.sin(angle)*Y)
     elif axis == 'x':
-        prism = torch.exp(-1j*k*torch.sin(angle)*X)
+        prism = np.exp(-1j*k*np.sin(angle)*X)
     return prism
 
 
-def linear_grating(nx, ny, every=2, add=None, axis='x'):
+def linear_grating(nx, ny, every=2, add=3.14, axis='x'):
     """
     A definition to generate a linear grating.
 
     Parameters
     ----------
     nx         : int
                  Size of the output along X.
@@ -87,25 +115,22 @@
                  Add the add value at every given number.
     add        : float
                  Angle to be added.
     axis       : string
                  Axis eiter X,Y or both.
 
     Returns
-    ----------
-    field      : torch.tensor
+    -------
+    field      : ndarray
                  Linear grating term.
     """
-    if isinstance(add, type(None)):
-        add = np.pi
-    grating = torch.zeros((nx, ny), dtype=torch.complex64)
+    grating = np.zeros((nx, ny), dtype=np.complex64)
     if axis == 'x':
-        grating[::every, :] = torch.exp(torch.tensor(1j*add))
+        grating[::every, :] = np.exp(1j*add)
     if axis == 'y':
-        grating[:, ::every] = torch.exp(torch.tensor(1j*add))
+        grating[:, ::every] = np.exp(1j*add)
     if axis == 'xy':
         checker = np.indices((nx, ny)).sum(axis=0) % every
-        checker = torch.from_numpy(checker)
         checker += 1
         checker = checker % 2
-        grating = torch.exp(1j*checker*add)
+        grating = np.exp(1j*checker*add)
     return grating
```

### Comparing `odak-0.2.2/odak/learn/wave/loss.py` & `odak-0.2.3/odak/learn/wave/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
     This implements a convolution of the phase with a kernel.
 
     The kernel is a simple 3 by 3 Laplacian kernel here, but you can also try other edge detection methods.
     """
     
 
-    def __init__(self, kernel = None, loss = nn.MSELoss(), device=torch.device("cpu")):
+    def __init__(self, kernel = None, loss = nn.MSELoss(), device = torch.device("cpu")):
         """
         Parameters
         ----------
         kernel                  : torch.tensor
                                     Convolution filter kernel, 3 by 3 Laplacian kernel by default.
         loss                    : torch.nn.Module
                                     loss function, L2 Loss by default.
         """
         super(phase_gradient, self).__init__()
         self.device = device
         self.loss = loss
         if kernel == None:
-            self.kernel = torch.tensor([[[[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]]]], dtype=torch.float32)/8
+            self.kernel = torch.tensor([[[[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]]]], dtype=torch.float32) / 8
         else:
             if len(kernel.shape) == 4:
                 self.kernel = kernel
             else:
                 self.kernel = kernel.reshape((1, 1, kernel.shape[0], kernel.shape[1]))
         self.kernel = Variable(self.kernel.to(self.device))
         
@@ -72,15 +72,15 @@
 
         Returns
         -------
 
         edge_detect              : torch.tensor
                                     The computed phase gradient.
         """
-        edge_detect = F.conv2d(phase, self.kernel, padding=self.kernel.shape[-1]//2)
+        edge_detect = F.conv2d(phase, self.kernel, padding = self.kernel.shape[-1] // 2)
         return edge_detect
 
 
 
 class speckle_contrast(nn.Module):
 
     """
@@ -104,15 +104,15 @@
                                     loss function, L2 Loss by default.
         """
         super(speckle_contrast, self).__init__()
         self.device = device
         self.loss = loss
         self.step_size = step_size
         self.kernel_size = kernel_size
-        self.kernel = torch.ones((1, 1, self.kernel_size, self.kernel_size))/(self.kernel_size**2)
+        self.kernel = torch.ones((1, 1, self.kernel_size, self.kernel_size)) / (self.kernel_size ** 2)
         self.kernel = Variable(self.kernel.type(torch.FloatTensor).to(self.device))
 
 
     def forward(self, intensity):
         """
         Calculates the speckle contrast Loss.
 
@@ -148,30 +148,32 @@
         -------
 
         Speckle_C               : torch.tensor
                                     The computed speckle contrast.
         """
         mean = F.conv2d(intensity, self.kernel, stride = self.step_size)
         var = torch.sqrt(F.conv2d(torch.pow(intensity, 2), self.kernel, stride = self.step_size) - torch.pow(mean, 2))
-        Speckle_C = var/mean
+        Speckle_C = var / mean
         return Speckle_C
 
 
 class multiplane_loss():
     """
     Loss function for computing loss in multiplanar images. Unlike, previous methods, this loss function accounts for defocused parts of an image.
     """
 
 
-    def __init__(self, target_image, target_depth, blur_ratio=0.25, target_blur_size=10, number_of_planes=4, weights=[1., 2.1, 0.6], multiplier=1., scheme='defocus', reduction='mean', device=None):
+    def __init__(self, target_image, target_depth, blur_ratio = 0.25, 
+                 target_blur_size = 10, number_of_planes = 4, weights = [1., 2.1, 0.6, 0.], 
+                 multiplier = 1., scheme = 'defocus', reduction = 'sum', device = torch.device('cpu')):
         """
         Parameters
         ----------
         target_image      : torch.tensor
-                            Monochrome target image (mxn resolution).
+                            Color target image [3 x m x n].
         target_depth      : torch.tensor
                             Monochrome target depth, same resolution as target_image.
         target_blur_size  : int
                             Maximum target blur size.
         blur_ratio        : float
                             Blur ratio, a value between zero and one.
         number_of_planes  : int
@@ -184,30 +186,28 @@
                             The type of the loss, `naive` without defocus or `defocus` with defocus.
         reduction         : str
                             Reduction can either be 'mean', 'none' or 'sum'. For more see: https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html#torch.nn.MSELoss
         device            : torch.device
                             Device to be used (e.g., cuda, cpu, opencl).
         """
         self.device = device
-        if isinstance(device, type(None)):
-            self.device = torch.device("cpu")
         self.target_image     = target_image.float().to(self.device)
         self.target_depth     = target_depth.float().to(self.device)
         self.target_blur_size = target_blur_size
         if self.target_blur_size % 2 == 0:
             self.target_blur_size += 1
         self.number_of_planes = number_of_planes
         self.multiplier       = multiplier
         self.weights          = weights
         self.reduction        = reduction
         self.blur_ratio       = blur_ratio
         self.set_targets()
         if scheme == 'defocus':
             self.add_defocus_blur()
-        self.loss_function = torch.nn.MSELoss(reduction=self.reduction)
+        self.loss_function = torch.nn.MSELoss(reduction = self.reduction)
 
 
     def get_targets(self):
         """
         Returns
         -------
         targets           : torch.tensor
@@ -220,88 +220,84 @@
 
 
     def set_targets(self):
         """
         Internal function for slicing the depth into planes without considering defocus. Users can query the results with get_targets() within the same class.
         """
         self.target_depth = self.target_depth * (self.number_of_planes - 1)
-        self.target_depth = torch.round(self.target_depth, decimals=0)
+        self.target_depth = torch.round(self.target_depth, decimals = 0)
         self.targets      = torch.zeros(
                                         self.number_of_planes,
                                         self.target_image.shape[0],
                                         self.target_image.shape[1],
-                                        requires_grad=False
+                                        self.target_image.shape[2],
+                                        requires_grad = False
                                        ).to(self.device)
         self.focus_target = torch.zeros_like(self.target_image,
-                                             requires_grad=False).to(self.device)
+                                             requires_grad = False).to(self.device)
         self.masks        = torch.zeros_like(self.targets).to(self.device)
         for i in range(self.number_of_planes):
-            mask_zeros = torch.zeros_like(self.target_image, dtype=torch.int)
-            mask_ones = torch.ones_like(self.target_image, dtype=torch.int)
-            mask = torch.where(self.target_depth==i, mask_ones, mask_zeros)
-            new_target = self.target_image * mask
-            self.focus_target = self.focus_target + new_target.squeeze(0).squeeze(0).detach().clone()
-            self.targets[i] = new_target.squeeze(0).squeeze(0)
-            self.masks[i] = mask.detach().clone() 
+            for ch in range(self.target_image.shape[0]):
+                mask_zeros = torch.zeros_like(self.target_image[ch], dtype = torch.int)
+                mask_ones = torch.ones_like(self.target_image[ch], dtype = torch.int)
+                mask = torch.where(self.target_depth == i, mask_ones, mask_zeros)
+                new_target = self.target_image[ch] * mask
+                self.focus_target = self.focus_target + new_target.squeeze(0).squeeze(0).detach().clone()
+                self.targets[i, ch] = new_target.squeeze(0).squeeze(0)
+                self.masks[i, ch] = mask.detach().clone() 
 
 
     def add_defocus_blur(self):
         """
         Internal function for adding defocus blur to the multiplane targets. Users can query the results with get_targets() within the same class.
         """
-        targets_cache = self.targets.detach().clone()
-        target = torch.sum(targets_cache, axis=0)
         kernel_length = [self.target_blur_size, self.target_blur_size ]
-        for i in range(self.number_of_planes):
-            sigmas = torch.linspace(start=0,end=self.target_blur_size,steps=self.number_of_planes)
-            sigmas = sigmas-i*self.target_blur_size/(self.number_of_planes-1+1e-10)
-            defocus = torch.zeros_like(targets_cache[i])
-            for j in range(self.number_of_planes):
-                nsigma = [int(abs(i - j) * self.blur_ratio), int(abs(i -j) * self.blur_ratio)]
-                if torch.sum(targets_cache[j]) > 0:
-                    if i == j:
-                        nsigma = [0., 0.]
-                    kernel = generate_2d_gaussian(kernel_length, nsigma).to(self.device)
-                    kernel = kernel / torch.sum(kernel)
-                    kernel = kernel.unsqueeze(0).unsqueeze(0)
-                    target_current = target.detach().clone().unsqueeze(0).unsqueeze(0)
-                    defocus_plane = torch.nn.functional.conv2d(target_current, kernel, padding='same')
-                    defocus_plane = defocus_plane.view(defocus_plane.shape[-2], defocus_plane.shape[-1])
-                    defocus = defocus + defocus_plane * torch.abs(self.masks[j])
-            self.targets[i] = defocus
+        for ch in range(self.target_image.shape[0]):
+            targets_cache = self.targets[:, ch].detach().clone()
+            target = torch.sum(targets_cache, axis = 0)
+            for i in range(self.number_of_planes):
+                sigmas = torch.linspace(start = 0, end = self.target_blur_size, steps = self.number_of_planes)
+                sigmas = sigmas - i * self.target_blur_size / (self.number_of_planes - 1 + 1e-10)
+                defocus = torch.zeros_like(targets_cache[i])
+                for j in range(self.number_of_planes):
+                    nsigma = [int(abs(i - j) * self.blur_ratio), int(abs(i -j) * self.blur_ratio)]
+                    if torch.sum(targets_cache[j]) > 0:
+                        if i == j:
+                            nsigma = [0., 0.]
+                        kernel = generate_2d_gaussian(kernel_length, nsigma).to(self.device)
+                        kernel = kernel / torch.sum(kernel)
+                        kernel = kernel.unsqueeze(0).unsqueeze(0)
+                        target_current = target.detach().clone().unsqueeze(0).unsqueeze(0)
+                        defocus_plane = torch.nn.functional.conv2d(target_current, kernel, padding = 'same')
+                        defocus_plane = defocus_plane.view(defocus_plane.shape[-2], defocus_plane.shape[-1])
+                        defocus = defocus + defocus_plane * torch.abs(self.masks[j, ch])
+                self.targets[i, ch] = defocus
         self.targets = self.targets.detach().clone() * self.multiplier
     
 
-    def __call__(self, image, target, plane_id=None):
+    def __call__(self, image, target, plane_id = None):
         """
         Calculates the multiplane loss against a given target.
         
         Parameters
         ----------
         image         : torch.tensor
-                        Image to compare with a target.
+                        Image to compare with a target [3 x m x n].
         target        : torch.tensor
-                        Target image for comparison.
+                        Target image for comparison [3 x m x n].
         plane_id      : int
                         Number of the plane under test.
         
         Returns
         -------
         loss          : torch.tensor
-                        Computer loss.
+                        Computed loss.
         """
         l2 = self.weights[0] * self.loss_function(image, target)
         if isinstance(plane_id, type(None)):
             mask = self.masks
-        mask = self.masks[plane_id]
+        else:
+            mask= self.masks[plane_id, :]
         l2_mask = self.weights[1] * self.loss_function(image * mask, target * mask)
         l2_cor = self.weights[2] * self.loss_function(image * target, target * target)
         loss = l2 + l2_mask + l2_cor
         return loss
-
-
-    def to(self, device):
-        """
-        Utilization function for setting the device.
-        """
-        self.device = device
-        return self
```

### Comparing `odak-0.2.2/odak/learn/wave/util.py` & `odak-0.2.3/odak/learn/wave/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                    Wavelength of a wave in mm.
 
     Returns
     -------
     k            : float
                    Wave number for a given wavelength.
     """
-    k = 2*np.pi/wavelength
+    k = 2 * np.pi / wavelength
     return k
 
 
 def calculate_phase(field, deg=False):
     """ 
     Definition to calculate phase of a single or multiple given electric field(s).
 
@@ -34,15 +34,15 @@
     Returns
     -------
     phase        : torch.float
                    Phase or phases of electric field(s) in radians.
     """
     phase = field.imag.atan2(field.real)
     if deg == True:
-        phase *= 180./3.14
+        phase *= 180. / np.pi
     return phase
 
 
 def calculate_amplitude(field):
     """ 
     Definition to calculate amplitude of a single or multiple given electric field(s).
 
@@ -84,28 +84,24 @@
 
 def generate_complex_field(amplitude, phase):
     """
     Definition to generate a complex field with a given amplitude and phase.
 
     Parameters
     ----------
-    amplitude         : ndarray or float
+    amplitude         : torch.tensor
                         Amplitude of the field.
-    phase             : ndarray or float
+    phase             : torch.tensor
                         Phase of the field.
 
     Returns
     -------
     field             : ndarray
                         Complex field.
     """
-    if isinstance(type(phase), type(1.)):
-        phase = torch.tensor([phase], requires_grad = True)
-    if isinstance(type(amplitude), type(1.)):
-        amplitude = torch.tensor([amplitude], requires_grad =True)
     field = amplitude * torch.cos(phase) + 1j * amplitude * torch.sin(phase)
     return field
 
 
 def adjust_phase_only_slm_range(native_range, working_wavelength, native_wavelength):
     """
     Definition for calculating the phase range of the Spatial Light Modulator (SLM) for a given wavelength. Here you prove maximum angle as the lower bound is typically zero. If the lower bound isn't zero in angles, you can use this very same definition for calculating lower angular bound as well.
```

### Comparing `odak-0.2.2/odak/manager/__init__.py` & `odak-0.2.3/odak/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/measurement/image_quality.py` & `odak-0.2.3/odak/measurement/image_quality.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/raytracing/boundary.py` & `odak-0.2.3/odak/raytracing/boundary.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/raytracing/primitives.py` & `odak-0.2.3/odak/raytracing/primitives.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/raytracing/ray.py` & `odak-0.2.3/odak/raytracing/ray.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/asset.py` & `odak-0.2.3/odak/tools/asset.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/conversions.py` & `odak-0.2.3/odak/tools/conversions.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/file.py` & `odak-0.2.3/odak/tools/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     Resized image.
 
     """
     img = cv2.resize(img, dsize=(target_size[0], target_size[1]), interpolation=cv2.INTER_AREA)
     return img
 
 
-def save_image(fn, img, cmin=0, cmax=255, color_depth=8):
+def save_image(fn, img, cmin = 0, cmax = 255, color_depth = 8):
     """
     Definition to save a Numpy array as an image.
 
     Parameters
     ----------
     fn           : str
                    Filename.
@@ -66,19 +66,19 @@
         input_img = input_img.astype(np.uint16)
     if len(input_img.shape) > 2:
         if input_img.shape[2] > 1:
             cache_img = np.copy(input_img)
             cache_img[:, :, 0] = input_img[:, :, 2]
             cache_img[:, :, 2] = input_img[:, :, 0]
             input_img = cache_img
-    cv2.imwrite(fn, input_img)
+    cv2.imwrite(os.path.expanduser(fn), input_img)
     return True
 
 
-def load_image(fn, normalizeby=0., torch_style=False):
+def load_image(fn, normalizeby = 0., torch_style = False):
     """ 
     Definition to load an image from a given location as a Numpy array.
 
     Parameters
     ----------
     fn           : str
                    Filename.
@@ -89,28 +89,28 @@
 
     Returns
     ----------
     image        :  ndarray
                     Image loaded as a Numpy array.
 
     """
-    image = cv2.imread(fn, cv2.IMREAD_UNCHANGED)
+    image = cv2.imread(os.path.expanduser(fn), cv2.IMREAD_UNCHANGED)
     if len(image.shape) > 2:
         new_image = np.copy(image)
         new_image[:, :, 0] = image[:, :, 2]
         new_image[:, :, 2] = image[:, :, 0]
         image = new_image
     if normalizeby != 0.:
         image = image * 1. / normalizeby
     if torch_style == True and len(image.shape) > 2:
         image = np.moveaxis(image, -1, 0)
     return image.astype(float)
 
 
-def shell_command(cmd, cwd='.', timeout=None, check=True):
+def shell_command(cmd, cwd = '.', timeout = None, check = True):
     """
     Definition to initiate shell commands.
 
     Parameters
     ----------
     cmd          : list
                    Command to be executed. 
@@ -151,16 +151,16 @@
     Definition to check if a directory exist. If it doesn't exist, this definition will create one.
 
     Parameters
     ----------
     directory     : str
                     Full directory path.
     """
-    if not os.path.exists(directory):
-        os.makedirs(directory)
+    if not os.path.exists(os.path.expanduser(directory)):
+        os.makedirs(os.path.expanduser(directory))
         return False
     return True
 
 
 def save_dictionary(settings, filename):
     """
     Definition to load a dictionary (JSON) file.
@@ -169,15 +169,15 @@
     Parameters
     ----------
     settings      : dict
                     Dictionary read from the file.
     filename      : str
                     Filename.
     """
-    with open(filename, 'w', encoding='utf-8') as f:
+    with open(os.path.expanduser(filename), 'w', encoding='utf-8') as f:
         json.dump(settings, f, ensure_ascii=False, indent=4)
     return settings
 
 
 def load_dictionary(filename):
     """
     Definition to load a dictionary (JSON) file.
@@ -194,15 +194,15 @@
                     Dictionary read from the file.
 
     """
     settings = json.load(open(filename))
     return settings
 
 
-def list_files(path, key='*.*', recursive=True):
+def list_files(path, key = '*.*', recursive = True):
     """
     Definition to list files in a given path with a given key.
 
     Parameters
     ----------
     path        : str
                   Path to a folder.
@@ -213,17 +213,17 @@
 
     Returns
     ----------
     files_list  : ndarray
                   list of files found in a given path.
     """
     if recursive == True:
-        search_result = pathlib.Path(path).rglob(key)
+        search_result = pathlib.Path(os.path.expanduser(path)).rglob(key)
     elif recursive == False:
-        search_result = pathlib.Path(path).glob(key)
+        search_result = pathlib.Path(os.path.expanduser(path)).glob(key)
     files_list = []
     for item in search_result:
         files_list.append(str(item))
     files_list = sorted(files_list)
     return files_list
```

### Comparing `odak-0.2.2/odak/tools/matrix.py` & `odak-0.2.3/odak/tools/matrix.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/sample.py` & `odak-0.2.3/odak/tools/sample.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/transformation.py` & `odak-0.2.3/odak/tools/transformation.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/tools/vector.py` & `odak-0.2.3/odak/tools/vector.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/blender/__init__.py` & `odak-0.2.3/odak/visualize/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/blender/libblend.py` & `odak-0.2.3/odak/visualize/blender/libblend.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/blender/server.py` & `odak-0.2.3/odak/visualize/blender/server.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/blender/wrapper.py` & `odak-0.2.3/odak/visualize/blender/wrapper.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/export.py` & `odak-0.2.3/odak/visualize/export.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/visualize/plotly.py` & `odak-0.2.3/odak/visualize/plotly.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/wave/__init__.py` & `odak-0.2.3/odak/wave/__init__.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/wave/classical.py` & `odak-0.2.3/odak/wave/classical.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/wave/utils.py` & `odak-0.2.3/odak/wave/utils.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak/wave/vector.py` & `odak-0.2.3/odak/wave/vector.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/odak.egg-info/PKG-INFO` & `odak-0.2.3/odak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odak
-Version: 0.2.2
+Version: 0.2.3
 Summary: Odak, the fundamental Python library for scientific computing in optical sciences.
 Home-page: https://github.com/kaanaksit/odak
 Author: Kaan Akşit
 Author-email: kaanaksit@kaanaksit.com
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -376,19 +376,22 @@
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
 Keywords: optics,holography,perception,graphics
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.7.5
 License-File: LICENSE.txt
 
 # Odak
 Odak (pronounced "O-dac") is the fundamental library for scientific computing in optical sciences, computer graphics and visual perception.
 To learn more about what Odak can do to help your design, experimentation and development, consult to our [documentation](https://kaanaksit.github.io/odak/)!
+
+
```

### Comparing `odak-0.2.2/odak.egg-info/SOURCES.txt` & `odak-0.2.3/odak.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 odak/catalog/lenses.py
 odak/catalog/data/plano_convex_lenses.json
 odak/fit/__init__.py
 odak/jones/__init__.py
 odak/learn/__init__.py
 odak/learn/models/__init__.py
 odak/learn/models/components.py
+odak/learn/models/models.py
 odak/learn/perception/__init__.py
 odak/learn/perception/blur_loss.py
 odak/learn/perception/color_conversion.py
 odak/learn/perception/foveation.py
 odak/learn/perception/metamer_mse_loss.py
 odak/learn/perception/metameric_loss.py
 odak/learn/perception/metameric_loss_uniform.py
@@ -44,15 +45,16 @@
 odak/learn/tools/sample.py
 odak/learn/tools/transformation.py
 odak/learn/tools/vector.py
 odak/learn/wave/__init__.py
 odak/learn/wave/classical.py
 odak/learn/wave/lens.py
 odak/learn/wave/loss.py
-odak/learn/wave/optimizer.py
+odak/learn/wave/optimizers.py
+odak/learn/wave/propagators.py
 odak/learn/wave/util.py
 odak/manager/__init__.py
 odak/measurement/__init__.py
 odak/measurement/image_quality.py
 odak/raytracing/__init__.py
 odak/raytracing/boundary.py
 odak/raytracing/primitives.py
@@ -76,29 +78,32 @@
 odak/wave/classical.py
 odak/wave/lens.py
 odak/wave/utils.py
 odak/wave/vector.py
 test/test_3d_gerchberg_saxton.py
 test/test_PLY.py
 test/test_beam_propagation.py
+test/test_color_conversion.py
 test/test_curve_fit.py
 test/test_cylinder_intersection.py
 test/test_detector.py
 test/test_diffuser.py
 test/test_export_import_PLY.py
 test/test_gerchberg_saxton.py
 test/test_gradient_descent_1d.py
 test/test_import.py
 test/test_intersect_reflect.py
 test/test_jones.py
 test/test_learn_beam_propagation.py
+test/test_learn_components.py
 test/test_learn_gerchberg_saxton.py
 test/test_learn_gradient_descent.py
 test/test_learn_lenses.py
 test/test_learn_loss.py
+test/test_learn_multiplane_optimizer.py
 test/test_learn_point_wise.py
 test/test_learn_ray_intersect_w_a_triangle.py
 test/test_learn_sgd.py
 test/test_least_square.py
 test/test_lenses.py
 test/test_mtf.py
 test/test_perceptron.py
```

### Comparing `odak-0.2.2/setup.py` & `odak-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 install_requires = []
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 setup(
     name="odak",
-    version="0.2.2",
+    version="0.2.3",
     author="Kaan Akşit",
     author_email="kaanaksit@kaanaksit.com",
     description="Odak, the fundamental Python library for scientific computing in optical sciences.",
     license=read('LICENSE.txt'),
     keywords="optics, holography, perception, graphics",
     url="https://github.com/kaanaksit/odak",
     install_requires=install_requires,
```

### Comparing `odak-0.2.2/test/test_3d_gerchberg_saxton.py` & `odak-0.2.3/test/test_3d_gerchberg_saxton.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_PLY.py` & `odak-0.2.3/test/test_PLY.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_beam_propagation.py` & `odak-0.2.3/test/test_beam_propagation.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_curve_fit.py` & `odak-0.2.3/test/test_curve_fit.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_cylinder_intersection.py` & `odak-0.2.3/test/test_cylinder_intersection.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_detector.py` & `odak-0.2.3/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_diffuser.py` & `odak-0.2.3/test/test_diffuser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import odak.raytracing as raytracer
 import odak.catalog as catalog
 import sys
 from odak.tools.sample import grid_sample, batch_of_rays
 
-
 def test():
     sample_entry_points = grid_sample(
         no=[2, 2],
         size=[100., 100.],
         center=[0., 0., 0.],
         angles=[0., 0., 0.]
     )
```

### Comparing `odak-0.2.2/test/test_gerchberg_saxton.py` & `odak-0.2.3/test/test_gerchberg_saxton.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_gradient_descent_1d.py` & `odak-0.2.3/test/test_gradient_descent_1d.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_intersect_reflect.py` & `odak-0.2.3/test/test_intersect_reflect.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_beam_propagation.py` & `odak-0.2.3/test/test_learn_beam_propagation.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_gerchberg_saxton.py` & `odak-0.2.3/test/test_learn_gerchberg_saxton.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_gradient_descent.py` & `odak-0.2.3/test/test_learn_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_lenses.py` & `odak-0.2.3/test/test_learn_lenses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import os
 import odak
-from odak.learn.wave import wavenumber, linear_grating, prism_phase_function, quadratic_phase_function
+from odak.learn.wave import wavenumber, linear_grating, prism_grating, quadratic_phase_function
 
 
 def test():
     wavelength = 0.5*pow(10, -6)
     pixeltom = 6*pow(10, -6)
     distance = 10.0
     resolution = [1080, 1920]
@@ -20,15 +20,15 @@
     lens_field = quadratic_phase_function(
         resolution[0],
         resolution[1],
         k,
         focal=0.3,
         dx=pixeltom
     )
-    prism_field = prism_phase_function(
+    prism_field = prism_grating(
         resolution[0],
         resolution[1],
         k,
         angle=0.1,
         dx=pixeltom,
         axis='x'
     )
```

### Comparing `odak-0.2.2/test/test_learn_loss.py` & `odak-0.2.3/test/test_learn_loss.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_point_wise.py` & `odak-0.2.3/test/test_learn_point_wise.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_ray_intersect_w_a_triangle.py` & `odak-0.2.3/test/test_learn_ray_intersect_w_a_triangle.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_learn_sgd.py` & `odak-0.2.3/test/test_learn_sgd.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_lenses.py` & `odak-0.2.3/test/test_lenses.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_mtf.py` & `odak-0.2.3/test/test_mtf.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_perceptron.py` & `odak-0.2.3/test/test_perceptron.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_perceptual_losses.py` & `odak-0.2.3/test/test_perceptual_losses.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_plano_convex_lens.py` & `odak-0.2.3/test/test_plano_convex_lens.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_propagate_field.py` & `odak-0.2.3/test/test_propagate_field.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_ray_intersect_w_a_surface.py` & `odak-0.2.3/test/test_ray_intersect_w_a_surface.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_ray_intersect_w_a_triangle.py` & `odak-0.2.3/test/test_ray_intersect_w_a_triangle.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_rayleigh.py` & `odak-0.2.3/test/test_rayleigh.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_sample_ray.py` & `odak-0.2.3/test/test_sample_ray.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_save_load.py` & `odak-0.2.3/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_sphere_intersection.py` & `odak-0.2.3/test/test_sphere_intersection.py`

 * *Files identical despite different names*

### Comparing `odak-0.2.2/test/test_two_rays_closest_point.py` & `odak-0.2.3/test/test_two_rays_closest_point.py`

 * *Files identical despite different names*

