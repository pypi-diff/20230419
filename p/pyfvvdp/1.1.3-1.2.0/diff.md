# Comparing `tmp/pyfvvdp-1.1.3.tar.gz` & `tmp/pyfvvdp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfvvdp-1.1.3.tar", last modified: Tue Oct 18 07:45:13 2022, max compression
+gzip compressed data, was "pyfvvdp-1.2.0.tar", last modified: Wed Apr 19 17:44:45 2023, max compression
```

## Comparing `pyfvvdp-1.1.3.tar` & `pyfvvdp-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.868189 pyfvvdp-1.1.3/
--rw-rw-rw-   0        0        0    13319 2021-11-10 13:54:36.000000 pyfvvdp-1.1.3/LICENSE
--rw-rw-rw-   0        0        0    14543 2022-10-18 07:45:13.868189 pyfvvdp-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    13580 2022-10-18 07:32:19.000000 pyfvvdp-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.824546 pyfvvdp-1.1.3/pyfvvdp/
--rw-rw-rw-   0        0        0      233 2022-10-18 07:32:19.000000 pyfvvdp-1.1.3/pyfvvdp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.851968 pyfvvdp-1.1.3/pyfvvdp/csf_cache/
--rw-rw-rw-   0        0        0    97539 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/csf_cache/o0_sn1_5_cm0_604562_gpu0.mat
--rw-rw-rw-   0        0        0    99527 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/csf_cache/o5_sn1_5_cm0_604562_gpu0.mat
--rw-rw-rw-   0        0        0    39636 2022-09-23 10:25:07.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp.py
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.866187 pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/
--rw-rw-rw-   0        0        0     5225 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/color_spaces.json
--rw-rw-rw-   0        0        0     4181 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/display_models.json
--rw-rw-rw-   0        0        0      779 2022-10-18 07:41:33.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/fvvdp_parameters.json
--rw-rw-rw-   0        0        0      785 2022-08-28 12:53:50.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/fvvdp_parameters_1_0.json
--rw-rw-rw-   0        0        0    16997 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_display_model.py
--rw-rw-rw-   0        0        0     3947 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/fvvdp_test.py
--rw-rw-rw-   0        0        0    10444 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/hdrvdp_lpyr_dec.py
--rw-rw-rw-   0        0        0     3420 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/interp.py
--rw-rw-rw-   0        0        0     7336 2022-10-18 07:32:19.000000 pyfvvdp-1.1.3/pyfvvdp/run_fvvdp.py
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.842563 pyfvvdp-1.1.3/pyfvvdp/third_party/
--rw-rw-rw-   0        0        0        0 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/third_party/__init__.py
--rw-rw-rw-   0        0        0    25185 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/third_party/cpuinfo.py
--rw-rw-rw-   0        0        0     1159 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/third_party/loadmat.py
--rw-rw-rw-   0        0        0     4240 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/utils.py
--rw-rw-rw-   0        0        0     8110 2022-10-18 07:32:19.000000 pyfvvdp-1.1.3/pyfvvdp/video_source_file.py
--rw-rw-rw-   0        0        0     3090 2022-08-28 12:20:13.000000 pyfvvdp-1.1.3/pyfvvdp/visualize_diff_map.py
-drwxrwxrwx   0        0        0        0 2022-10-18 07:45:13.839560 pyfvvdp-1.1.3/pyfvvdp.egg-info/
--rw-rw-rw-   0        0        0    14543 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      890 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-10-18 07:45:13.000000 pyfvvdp-1.1.3/pyfvvdp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-18 07:45:13.869191 pyfvvdp-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1486 2022-10-18 07:42:16.000000 pyfvvdp-1.1.3/setup.py
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.615345 pyfvvdp-1.2.0/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    13319 2021-11-15 18:16:16.000000 pyfvvdp-1.2.0/LICENSE
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    16898 2023-04-19 17:44:45.613345 pyfvvdp-1.2.0/PKG-INFO
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    16146 2023-04-19 17:44:39.000000 pyfvvdp-1.2.0/README.md
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.307348 pyfvvdp-1.2.0/pyfvvdp/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)      269 2022-11-13 12:50:26.000000 pyfvvdp-1.2.0/pyfvvdp/__init__.py
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.438347 pyfvvdp-1.2.0/pyfvvdp/csf_cache/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    97539 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/csf_cache/o0_sn1_5_cm0_604562_gpu0.mat
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    99527 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/csf_cache/o5_sn1_5_cm0_604562_gpu0.mat
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    35022 2023-04-19 17:07:26.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp.py
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.531347 pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     5224 2022-11-08 19:00:05.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/color_spaces.json
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     4608 2022-12-14 18:07:19.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/display_models.json
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)      779 2022-11-25 22:34:41.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/fvvdp_parameters.json
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)      785 2022-09-02 13:08:22.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/fvvdp_parameters_1_0.json
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    22128 2023-04-19 17:32:23.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_display_model.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    11503 2022-11-20 13:24:58.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_lpyr_dec.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     3947 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/fvvdp_test.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     3420 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/interp.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     3617 2022-11-14 09:18:14.000000 pyfvvdp-1.2.0/pyfvvdp/pupsnr.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    11454 2022-11-25 22:34:41.000000 pyfvvdp-1.2.0/pyfvvdp/run_fvvdp.py
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.588349 pyfvvdp-1.2.0/pyfvvdp/third_party/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)        0 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/third_party/__init__.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    25185 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/third_party/cpuinfo.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     1159 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/third_party/loadmat.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     7359 2022-11-25 22:34:41.000000 pyfvvdp-1.2.0/pyfvvdp/utils.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    13363 2023-04-19 17:07:26.000000 pyfvvdp-1.2.0/pyfvvdp/video_source.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    20279 2023-04-19 17:07:26.000000 pyfvvdp-1.2.0/pyfvvdp/video_source_file.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    11796 2023-04-19 17:07:26.000000 pyfvvdp-1.2.0/pyfvvdp/video_source_yuv.py
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     3090 2022-08-28 14:00:19.000000 pyfvvdp-1.2.0/pyfvvdp/visualize_diff_map.py
+drwxrwsr-x   0 rkm38     (3596) rkm38     (3596)        0 2023-04-19 17:44:45.406347 pyfvvdp-1.2.0/pyfvvdp.egg-info/
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)    16898 2023-04-19 17:44:44.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/PKG-INFO
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)      865 2023-04-19 17:44:45.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/SOURCES.txt
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)        1 2023-04-19 17:44:44.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/dependency_links.txt
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)       49 2023-04-19 17:44:44.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/entry_points.txt
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)       89 2023-04-19 17:44:44.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/requires.txt
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)       28 2023-04-19 17:44:44.000000 pyfvvdp-1.2.0/pyfvvdp.egg-info/top_level.txt
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)       38 2023-04-19 17:44:45.616350 pyfvvdp-1.2.0/setup.cfg
+-rw-rw-r--   0 rkm38     (3596) rkm38     (3596)     1486 2022-11-25 22:34:41.000000 pyfvvdp-1.2.0/setup.py
```

### Comparing `pyfvvdp-1.1.3/LICENSE` & `pyfvvdp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/PKG-INFO` & `pyfvvdp-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,191 +1,214 @@
-Metadata-Version: 2.1
-Name: pyfvvdp
-Version: 1.1.3
-Summary: PyTorch code for 'FovVideoVDP': a full-referencevisual quality metric that predicts the perceptualdifference between pairs of images or videos.
-Home-page: https://github.com/gfxdisp/FovVideoVDP
-Author: Rafał K. Mantiuk
-Author-email: mantiuk@gmail.com
-License: Creative Commons Attribution-NonCommercial 4.0 International Public License
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FovVideoVDP: A visible difference predictor for wide field-of-view video
-
-<img src="https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/teaser.png"></img>
-
-FovVideoVDP is a full-reference visual quality metric that predicts the perceptual difference between pairs of images and videos. Similar to popular metrics like PSNR and SSIM, it is aimed at comparing a ground truth reference video against a distorted (e.g. compressed, lower framerate) version.
-
-However, unlike traditional quality metrics, FovVideoVDP works for videos in addition to images, accounts for peripheral acuity, works with SDR and HDR content. We model the response of the human visual system to changes over time as well as across the visual field, so we can predict temporal artifacts like flicker and judder, as well as spatiotemporal artifacts as perceived at different degrees of peripheral vision. Such a metric is important for head-mounted displays as it accounts for both the dynamic content, as well as the large field of view.
-
-FovVideoVDP has both a PyTorch and MATLAB implementations. The usage is described below.
-
-The details of the metric can be found in:
-
-Mantiuk, Rafał K., Gyorgy Denes, Alexandre Chapiro, Anton Kaplanyan, Gizem Rufo, Romain Bachy, Trisha Lian, and Anjul Patney. “FovVideoVDP : A Visible Difference Predictor for Wide Field-of-View Video.” ACM Transaction on Graphics 40, no. 4 (2021): 49. https://doi.org/10.1145/3450626.3459831.
-
-The paper, videos and additional results can be found at the project web page: https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/
-
-If you use the metric in your research, please cite the paper above. 
-
-## PyTorch quickstart
-
-Install with PyPI `pip install pyfvvdp` and run directly from the command line:
-
-```bash
-fvvdp --test test_file --ref ref_file --gpu 0 --display standard_fhd
-```
-The test and reference files can be images or videos. The option `--display` specifies a display on which the content is viewed. See [fvvdp_data/display_models.json](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/fvvdp_data/display_models.json) for the available displays.
-
-Note that the default installation skips the [PyEXR](https://pypi.org/project/PyEXR/) package and uses ImageIO instead. It is recommended to separately install this package since ImageIO's handling of OpenEXR files is unreliable as evidenced [here](https://github.com/imageio/imageio/issues/517). PyEXR is not automatically installed because it depends on the [OpenEXR](https://www.openexr.com/) library, whose installation is operating system specific.
-
-See [Command line interface](#command-line-interface) for further details. FovVideoVDP can be also run directly from Python - see [Low-level Python interface](#low-level-python-interface). 
-
-**Table of contents**
-- [Display specification](#display-specification)
-    - [Custom specification](#custom-specification)
-    - [Reporting metric results](#reporting-metric-results)
-    - [Predicting quality scores](#predicted-quality-scores)
-- [PyTorch](#pytorch)
-    - [Command line interface](#command-line-interface)
-    - [Low-level Python interface](#low-level-python-interface)
-- [MATLAB](#matlab)
-    - [Low-level MATLAB interface](#low-level-matlab-interface)
-- [Differences between MATLAB and PyTorch versions](#differences-between-matlab-and-pytorch-versions)
-- [Release notes](#release-notes)
-
-## Display specification
-
-Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, however, it is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
-
-You specify the display by passing `--display` argument to the PyTorch code, or `display_name` parameter to the MATLAB code. 
-
-Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_hdr` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). 
-
-
-### Custom specification
-
-The display photometry and geometry is typically specified by passing `display_name` parameter to the metric. Alternatively, if you need more flexibility in specifying display geometry (size, fov, viewing distance) and its colorimetry, you can instead pass objects of the classes `fvvdp_display_geometry`, `fvvdp_display_photo_gog` for most SDR displays, and `fvvdp_display_photo_absolute` for HDR displays. You can also create your own subclasses of those classes for custom display specification. 
-
-### Reporting metric results
-
-When reporting the results of the metric, please include the string returned by the metric, such as:
-`"FovVideoVDP v1.1, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
-This is to ensure that you provide enough details to reproduce your results. 
-
-### Predicted quality scores
-
-FovVideoVDP reports image/video quality in the JOD (Just-Objectionable-Difference) units. The highest quality (no difference) is reported as 10 and lower values are reported for distorted content. In case of very strong distortion, or when comparing two unrelated images, the quality value can drop below 0. 
-
-The main advantage of JODs is that they (a) should be linearly related to the perceived magnitude of the distortion and (b) the difference of JODs can be interpreted as the preference prediction across the population. For example, if method A produces a video with the quality score of 8 JOD and method B gives the quality score of 9 JOD, it means that 75% of the population will choose method B over A. The plots below show the mapping from the difference between two conditions in JOD units to the probability of selecting the condition with the higher JOD score (black numbers on the left) and the percentage increase in preference (blue numbers on the right). For more explanation, please refer to Section 3.9 and Fig. 9 in the main paper.
-
-The differences in JOD scores can be converted to the percentage increase in preference (or the probability selecting A over B) using the MATLAB function `fvvdp_preference`.
-
-<table>
-  <tr>
-    <td>Fine JOD scale</td>
-    <td>Coarse JOD scale</td>
-  </tr>
-  <tr>
-    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/fine_jod_scale.png"></img></td>
-    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/coarse_jod_scale.png"></img></td>
-  </tr>
-</table>
-
-## PyTorch
-
-### Command line interface
-The main script to run the model on a set of images or videos is [run_fvvdp.py](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/run_fvvdp.py), from which the binary `fvvdp` is created . Run `fvvdp --help` for detailed usage information.
-
-For the first example, a video was downsampled (4x4) and upsampled (4x4) by different combinations of Bicubic and Nearest filters. To predict quality, you can run:
-
-```bash
-fvvdp --test example_media/aliasing/ferris-*-*.mp4 --ref example_media/aliasing/ferris-ref.mp4 --gpu 0 --display standard_fhd --heatmap supra-threshold
-```
-
-|Original | ![ferris wheel](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-ref.gif) | Quality | Difference map |
-| :---: | :---: | :---: | :---: |
-| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.6277 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
-| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.4803 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
-| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 6.0446 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
-| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.9450 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
-
-### Low-level Python interface
-FovVideoVDP can also be run through the Python interface by instatiating the `pyfvvdp.fvvdp.fvvdp` class. This example shows how to predict the quality of images degraded by Gaussian noise and blur.
-
-```python
-import pyfvvdp
-import ex_utils as utils
-
-I_ref = pyfvvdp.load_image_as_array(os.path.join('example_media', 'wavy_facade.png'))
-fv = pyfvvdp.fvvdp(display_name='standard_4k', heatmap='threshold')
-
-# Gaussian noise with variance 0.003
-I_test_noise = utils.imnoise(I_ref, np.sqrt(0.003))
-Q_JOD_noise, stats_noise = fv.predict( I_test_noise, I_ref, dim_order="HWC" )
-
-# Gaussian blur with sigma=2
-I_test_blur = utils.imgaussblur(I_ref, 2)
-Q_JOD_blur, stats_blur = fv.predict( I_test_blur, I_ref, dim_order="HWC" )
-```
-
-|Original | ![wavy-facade](https://github.com/gfxdisp/FovVideoVDP/raw/main/example_media/wavy_facade.png) | Quality | Difference map |
-| :---: | :---: | :---: | :---: |
-| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.532 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
-| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.674 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
-
-More examples can be found in these [example scripts](https://github.com/gfxdisp/FovVideoVDP/blob/main/pytorch_examples).
-
-
-## MATLAB
-
-MATLAB code for the metric can be found in `matlab/fvvdp.m`. The full documentation of the metric can be shown by typing `doc fvvdp`.
-
-The best starting point is the examples, which can be found in `matlab/examples`. For example, to measure the quality of a noisy image and display the difference map, you can use the code:
-
-```
-I_ref = imread( 'wavy_facade.png' );
-I_test_noise = imnoise( I_ref, 'gaussian', 0, 0.001 );
-
-[Q_JOD_noise, diff_map_noise] = fvvdp( I_test_noise, I_ref, 'display_name', 'standard_phone', 'heatmap', 'threshold' );
-
-clf
-imshow( diff_map_noise );
-
-```
-
-By default, FovVideoVDP will run the code on a GPU using `gpuArray`s, which require functioning CUDA on your computer. If you do not have GPU with CUDA support (e.g. you are on Mac), the code will automatically fallback to the CPU, which will be much slower. 
- 
-### Low-level MATLAB interface
-
-`fvvdp` function is the suitable choice for most cases. But if you need to run metric on large datasets, you can use a low-level function `fvvdp_core`. It requires as input an object of the class `fvvdp_video_source`, which supplies the metric with the frames. Refer to the documentation of that class for further details. 
-
-## Differences between MATLAB and Pytorch versions
-
-* Both versions are implementation of the same metric, but due to differences in the video loaders, you can expect to see small differences in their predictions - typically up to 0.05 JOD.
-* PyTorch version is a bit faster when running on a GPU. 
-
-## Release notes
-
-* v1.1.2 - 23 September 2022
- * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
-
-* v1.1.1 - 28 August 2022
-  * We found a small inconsistency in eccentricity calculations. After fixing this, the metric has been retrained on the same datasets as described in the paper. FovVideoVDP v1.1 will return JOD values that are different than v1.0. For that reason, it is important to mention the version number when reporting the results. 
-  * Python interface has been thoroughly redesigned and make more consistent with Matlab's conterpart. Now it should be much easier to call the metric from Python. 
-  * All Matlab examples have been ported to Python. 
-  * Python version is now faster. 
-  * Published as a PIP repository. 
-
-* v1.0 - 21 April 2021
-  * The original FovVideoVDP release, released with the paper.
-
-The detailed list of changes can be found in [ChangeLog.md](https://github.com/gfxdisp/FovVideoVDP/blob/main/ChangeLog.md).
-
-
+Metadata-Version: 2.1
+Name: pyfvvdp
+Version: 1.2.0
+Summary: PyTorch code for 'FovVideoVDP': a full-referencevisual quality metric that predicts the perceptualdifference between pairs of images or videos.
+Home-page: https://github.com/gfxdisp/FovVideoVDP
+Author: Rafał K. Mantiuk
+Author-email: mantiuk@gmail.com
+License: Creative Commons Attribution-NonCommercial 4.0 International Public License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FovVideoVDP: A visible difference predictor for wide field-of-view video
+
+<img src="https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/teaser.png"></img>
+
+FovVideoVDP is a full-reference visual quality metric that predicts the perceptual difference between pairs of images and videos. Similar to popular metrics like PSNR and SSIM, it is aimed at comparing a ground truth reference video against a distorted (e.g. compressed, lower framerate) version.
+
+However, unlike traditional quality metrics, FovVideoVDP works for videos in addition to images, accounts for peripheral acuity, works with SDR and HDR content. We model the response of the human visual system to changes over time as well as across the visual field, so we can predict temporal artifacts like flicker and judder, as well as spatiotemporal artifacts as perceived at different degrees of peripheral vision. Such a metric is important for head-mounted displays as it accounts for both the dynamic content, as well as the large field of view.
+
+FovVideoVDP has both a PyTorch and MATLAB implementations. The usage is described below.
+
+The details of the metric can be found in:
+
+Mantiuk, Rafał K., Gyorgy Denes, Alexandre Chapiro, Anton Kaplanyan, Gizem Rufo, Romain Bachy, Trisha Lian, and Anjul Patney. “FovVideoVDP : A Visible Difference Predictor for Wide Field-of-View Video.” ACM Transaction on Graphics 40, no. 4 (2021): 49. https://doi.org/10.1145/3450626.3459831.
+
+The paper, videos and additional results can be found at the project web page: https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/
+
+If you use the metric in your research, please cite the paper above. 
+
+## PyTorch quickstart
+
+Start by installing the right version of PyTorch (with CUDA if supported) by following [these instructions](https://pytorch.org/get-started/locally/). Then, install pyfvvdp with PyPI `pip install pyfvvdp` or Anaconda `conda install -c gfxdisp -c conda-forge pyfvvdp`. You can run `fvvdp` directly from the command line:
+
+```bash
+fvvdp --test test_file --ref ref_file --display standard_fhd
+```
+The test and reference files can be images or videos. The option `--display` specifies a display on which the content is viewed. See [fvvdp_data/display_models.json](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/fvvdp_data/display_models.json) for the available displays.
+
+Note that the default installation skips the [PyEXR](https://pypi.org/project/PyEXR/) package and uses ImageIO instead. It is recommended to separately install this package since ImageIO's handling of OpenEXR files is unreliable as evidenced [here](https://github.com/imageio/imageio/issues/517). PyEXR is not automatically installed because it depends on the [OpenEXR](https://www.openexr.com/) library, whose installation is operating system specific.
+
+See [Command line interface](#command-line-interface) for further details. FovVideoVDP can be also run directly from Python - see [Low-level Python interface](#low-level-python-interface). 
+
+**Table of contents**
+- [Display specification](#display-specification)
+    - [Custom specification](#custom-specification)
+    - [HDR content](#HDR-content)
+    - [Reporting metric results](#reporting-metric-results)
+    - [Predicting quality scores](#predicted-quality-scores)
+- [PyTorch](#pytorch)
+    - [Command line interface](#command-line-interface)
+    - [Low-level Python interface](#low-level-python-interface)
+- [MATLAB](#matlab)
+    - [Low-level MATLAB interface](#low-level-matlab-interface)
+- [Differences between MATLAB and PyTorch versions](#differences-between-matlab-and-pytorch-versions)
+- [Release notes](#release-notes)
+
+## Display specification
+
+Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, or create a new JSON file and pass the directory it is located in as `--config-dir` parameter (`fvvdp` command). If the display specification is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
+
+You specify the display by passing `--display` argument to the PyTorch code, or `display_name` parameter to the MATLAB code. 
+
+Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_4k` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). If you want to enlarge the image to the full resolution of the display, pass `--full-screen-resize {fast_bilinear,bilinear,bicubic,lanczos}` option (now works with video only). 
+
+The command line version of FovVideoVDP can take as input HDR video streams encoded using the PQ transfer function (from version 1.1.4). To correctly model HDR content, it is necessary to pass a display model with `EOTF="PQ"`, for example `standard_hdr`.
+
+### Custom specification
+
+The display photometry and geometry is typically specified by passing `display_name` parameter to the metric. Alternatively, if you need more flexibility in specifying display geometry (size, fov, viewing distance) and its colorimetry, you can instead pass objects of the classes `fvvdp_display_geometry`, `fvvdp_display_photo_gog` for most SDR displays, and `fvvdp_display_photo_absolute` for HDR displays. You can also create your own subclasses of those classes for custom display specification. 
+
+### HDR content
+
+(Python command line only) You can use the metric to compare: 
+
+* HDR video files encoded using PQ EOTF function (SMPTE ST 2084). Pass the video files as `--test` and `--ref` arguments and specify `--display standard_hdr_pq`.
+
+* OpenEXR images. The images *MUST* contain absolute linear colour values (colour graded values, emitted from the display). That is, if the disply peak luminance is 1000, RGB=(1000,1000,1000) corresponds to the maximum value emitted from the display. If you pass images with the maximum value of 1, the metric will assume that the images are very dark (the peak of 1 nit) and result in incorerect predictrions. You need to specify `--display standard_hdr_linear` to use correct EOTF.
+
+### Reporting metric results
+
+When reporting the results of the metric, please include the string returned by the metric, such as:
+`"FovVideoVDP v1.2.0, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
+This is to ensure that you provide enough details to reproduce your results. 
+
+### Predicted quality scores
+
+FovVideoVDP reports image/video quality in the JOD (Just-Objectionable-Difference) units. The highest quality (no difference) is reported as 10 and lower values are reported for distorted content. In case of very strong distortion, or when comparing two unrelated images, the quality value can drop below 0. 
+
+The main advantage of JODs is that they (a) should be linearly related to the perceived magnitude of the distortion and (b) the difference of JODs can be interpreted as the preference prediction across the population. For example, if method A produces a video with the quality score of 8 JOD and method B gives the quality score of 9 JOD, it means that 75% of the population will choose method B over A. The plots below show the mapping from the difference between two conditions in JOD units to the probability of selecting the condition with the higher JOD score (black numbers on the left) and the percentage increase in preference (blue numbers on the right). For more explanation, please refer to Section 3.9 and Fig. 9 in the main paper.
+
+The differences in JOD scores can be converted to the percentage increase in preference (or the probability selecting A over B) using the MATLAB function `fvvdp_preference`.
+
+<table>
+  <tr>
+    <td>Fine JOD scale</td>
+    <td>Coarse JOD scale</td>
+  </tr>
+  <tr>
+    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/fine_jod_scale.png"></img></td>
+    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/coarse_jod_scale.png"></img></td>
+  </tr>
+</table>
+
+## PyTorch
+
+### Command line interface
+The main script to run the model on a set of images or videos is [run_fvvdp.py](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/run_fvvdp.py), from which the binary `fvvdp` is created . Run `fvvdp --help` for detailed usage information.
+
+For the first example, a video was downsampled (4x4) and upsampled (4x4) by different combinations of Bicubic and Nearest filters. To predict quality, you can run:
+
+```bash
+fvvdp --test example_media/aliasing/ferris-*-*.mp4 --ref example_media/aliasing/ferris-ref.mp4 --gpu 0 --display standard_fhd --heatmap supra-threshold
+```
+
+|Original | ![ferris wheel](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-ref.gif) | Quality | Difference map |
+| :---: | :---: | :---: | :---: |
+| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.469 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
+| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.328 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
+| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 5.923 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
+| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.821 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
+
+
+### Low-level Python interface
+FovVideoVDP can also be run through the Python interface by instatiating the `pyfvvdp.fvvdp.fvvdp` class. This example shows how to predict the quality of images degraded by Gaussian noise and blur.
+
+```python
+import os
+import numpy as np
+import pyfvvdp
+import ex_utils as utils
+
+I_ref = pyfvvdp.load_image_as_array(os.path.join('example_media', 'wavy_facade.png'))
+fv = pyfvvdp.fvvdp(display_name='standard_4k', heatmap='threshold')
+
+# Gaussian noise with variance 0.003
+I_test_noise = utils.imnoise(I_ref, np.sqrt(0.003))
+Q_JOD_noise, stats_noise = fv.predict( I_test_noise, I_ref, dim_order="HWC" )
+
+# Gaussian blur with sigma=2
+I_test_blur = utils.imgaussblur(I_ref, 2)
+Q_JOD_blur, stats_blur = fv.predict( I_test_blur, I_ref, dim_order="HWC" )
+```
+
+|Original | ![wavy-facade](https://github.com/gfxdisp/FovVideoVDP/raw/main/example_media/wavy_facade.png) | Quality | Difference map |
+| :---: | :---: | :---: | :---: |
+| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.537 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
+| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.693 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
+
+More examples can be found in these [example scripts](https://github.com/gfxdisp/FovVideoVDP/blob/main/pytorch_examples).
+
+
+## MATLAB
+
+MATLAB code for the metric can be found in `matlab/fvvdp.m`. The full documentation of the metric can be shown by typing `doc fvvdp`.
+
+The best starting point is the examples, which can be found in `matlab/examples`. For example, to measure the quality of a noisy image and display the difference map, you can use the code:
+
+```
+I_ref = imread( 'wavy_facade.png' );
+I_test_noise = imnoise( I_ref, 'gaussian', 0, 0.001 );
+
+[Q_JOD_noise, diff_map_noise] = fvvdp( I_test_noise, I_ref, 'display_name', 'standard_phone', 'heatmap', 'threshold' );
+
+clf
+imshow( diff_map_noise );
+
+```
+
+By default, FovVideoVDP will run the code on a GPU using `gpuArray`s, which require functioning CUDA on your computer. If you do not have GPU with CUDA support (e.g. you are on Mac), the code will automatically fallback to the CPU, which will be much slower. 
+ 
+### Low-level MATLAB interface
+
+`fvvdp` function is the suitable choice for most cases. But if you need to run metric on large datasets, you can use a low-level function `fvvdp_core`. It requires as input an object of the class `fvvdp_video_source`, which supplies the metric with the frames. Refer to the documentation of that class for further details. 
+
+## Differences between MATLAB and Pytorch versions
+
+* Both versions are implementation of the same metric, but due to differences in the video loaders, you can expect to see small differences in their predictions - typically up to 0.05 JOD.
+* PyTorch version is a bit faster when running on a GPU. 
+
+## Release notes
+
+* v1.2.0 - 19 April 2023
+  * The python command line interface can now accept HDR video files and OpenEXR images. 
+  * [PU21-PSNR](https://github.com/gfxdisp/pu21) can be run in addition to FovVideoVDP
+  * Added new command line options: `--full-screen-resize`, `--metrics`, `--temp-padding`, `--feature`, `--output-dir`
+  * Faster decoding for large (4k) videos when run on CUDA (python, the command line interface `fvvdp`). 
+  * The prediction may differ slightly because of the way video files are handled and processed. There are no changes in the metric.
+  * Fixed issue when reading video frames in python freezed on some platforms (issue with python's `/dev/null` redirection)
+
+* v1.1.3 - 18 October 2022
+  * Added "raw" heatmap type to the command line. 
+  * Changed the way pyfvvdp classes are imported  to avoid clash between the file and class names (see updated pytortch_examples)
+  * Installation of PyEXR is now optional (caused problems on some operating systems).
+
+* v1.1.2 - 23 September 2022
+  * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
+
+* v1.1.1 - 28 August 2022
+  * We found a small inconsistency in eccentricity calculations. After fixing this, the metric has been retrained on the same datasets as described in the paper. FovVideoVDP v1.1 will return JOD values that are different than v1.0. For that reason, it is important to mention the version number when reporting the results. 
+  * Python interface has been thoroughly redesigned and make more consistent with Matlab's conterpart. Now it should be much easier to call the metric from Python. 
+  * All Matlab examples have been ported to Python. 
+  * Python version is now faster. 
+  * Published as a PIP repository. 
+
+* v1.0 - 21 April 2021
+  * The original FovVideoVDP release, released with the paper.
+
+The detailed list of changes can be found in [ChangeLog.md](https://github.com/gfxdisp/FovVideoVDP/blob/main/ChangeLog.md).
```

### Comparing `pyfvvdp-1.1.3/README.md` & `pyfvvdp-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,55 +14,65 @@
 
 The paper, videos and additional results can be found at the project web page: https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/
 
 If you use the metric in your research, please cite the paper above. 
 
 ## PyTorch quickstart
 
-Install with PyPI `pip install pyfvvdp` and run directly from the command line:
+Start by installing the right version of PyTorch (with CUDA if supported) by following [these instructions](https://pytorch.org/get-started/locally/). Then, install pyfvvdp with PyPI `pip install pyfvvdp` or Anaconda `conda install -c gfxdisp -c conda-forge pyfvvdp`. You can run `fvvdp` directly from the command line:
 
 ```bash
-fvvdp --test test_file --ref ref_file --gpu 0 --display standard_fhd
+fvvdp --test test_file --ref ref_file --display standard_fhd
 ```
 The test and reference files can be images or videos. The option `--display` specifies a display on which the content is viewed. See [fvvdp_data/display_models.json](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/fvvdp_data/display_models.json) for the available displays.
 
 Note that the default installation skips the [PyEXR](https://pypi.org/project/PyEXR/) package and uses ImageIO instead. It is recommended to separately install this package since ImageIO's handling of OpenEXR files is unreliable as evidenced [here](https://github.com/imageio/imageio/issues/517). PyEXR is not automatically installed because it depends on the [OpenEXR](https://www.openexr.com/) library, whose installation is operating system specific.
 
 See [Command line interface](#command-line-interface) for further details. FovVideoVDP can be also run directly from Python - see [Low-level Python interface](#low-level-python-interface). 
 
 **Table of contents**
 - [Display specification](#display-specification)
     - [Custom specification](#custom-specification)
+    - [HDR content](#HDR-content)
     - [Reporting metric results](#reporting-metric-results)
     - [Predicting quality scores](#predicted-quality-scores)
 - [PyTorch](#pytorch)
     - [Command line interface](#command-line-interface)
     - [Low-level Python interface](#low-level-python-interface)
 - [MATLAB](#matlab)
     - [Low-level MATLAB interface](#low-level-matlab-interface)
 - [Differences between MATLAB and PyTorch versions](#differences-between-matlab-and-pytorch-versions)
 - [Release notes](#release-notes)
 
 ## Display specification
 
-Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, however, it is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
+Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, or create a new JSON file and pass the directory it is located in as `--config-dir` parameter (`fvvdp` command). If the display specification is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
 
 You specify the display by passing `--display` argument to the PyTorch code, or `display_name` parameter to the MATLAB code. 
 
-Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_hdr` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). 
+Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_4k` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). If you want to enlarge the image to the full resolution of the display, pass `--full-screen-resize {fast_bilinear,bilinear,bicubic,lanczos}` option (now works with video only). 
 
+The command line version of FovVideoVDP can take as input HDR video streams encoded using the PQ transfer function (from version 1.1.4). To correctly model HDR content, it is necessary to pass a display model with `EOTF="PQ"`, for example `standard_hdr`.
 
 ### Custom specification
 
 The display photometry and geometry is typically specified by passing `display_name` parameter to the metric. Alternatively, if you need more flexibility in specifying display geometry (size, fov, viewing distance) and its colorimetry, you can instead pass objects of the classes `fvvdp_display_geometry`, `fvvdp_display_photo_gog` for most SDR displays, and `fvvdp_display_photo_absolute` for HDR displays. You can also create your own subclasses of those classes for custom display specification. 
 
+### HDR content
+
+(Python command line only) You can use the metric to compare: 
+
+* HDR video files encoded using PQ EOTF function (SMPTE ST 2084). Pass the video files as `--test` and `--ref` arguments and specify `--display standard_hdr_pq`.
+
+* OpenEXR images. The images *MUST* contain absolute linear colour values (colour graded values, emitted from the display). That is, if the disply peak luminance is 1000, RGB=(1000,1000,1000) corresponds to the maximum value emitted from the display. If you pass images with the maximum value of 1, the metric will assume that the images are very dark (the peak of 1 nit) and result in incorerect predictrions. You need to specify `--display standard_hdr_linear` to use correct EOTF.
+
 ### Reporting metric results
 
 When reporting the results of the metric, please include the string returned by the metric, such as:
-`"FovVideoVDP v1.1, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
+`"FovVideoVDP v1.2.0, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
 This is to ensure that you provide enough details to reproduce your results. 
 
 ### Predicted quality scores
 
 FovVideoVDP reports image/video quality in the JOD (Just-Objectionable-Difference) units. The highest quality (no difference) is reported as 10 and lower values are reported for distorted content. In case of very strong distortion, or when comparing two unrelated images, the quality value can drop below 0. 
 
 The main advantage of JODs is that they (a) should be linearly related to the perceived magnitude of the distortion and (b) the difference of JODs can be interpreted as the preference prediction across the population. For example, if method A produces a video with the quality score of 8 JOD and method B gives the quality score of 9 JOD, it means that 75% of the population will choose method B over A. The plots below show the mapping from the difference between two conditions in JOD units to the probability of selecting the condition with the higher JOD score (black numbers on the left) and the percentage increase in preference (blue numbers on the right). For more explanation, please refer to Section 3.9 and Fig. 9 in the main paper.
@@ -89,23 +99,26 @@
 
 ```bash
 fvvdp --test example_media/aliasing/ferris-*-*.mp4 --ref example_media/aliasing/ferris-ref.mp4 --gpu 0 --display standard_fhd --heatmap supra-threshold
 ```
 
 |Original | ![ferris wheel](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-ref.gif) | Quality | Difference map |
 | :---: | :---: | :---: | :---: |
-| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.6277 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
-| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.4803 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
-| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 6.0446 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
-| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.9450 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
+| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.469 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
+| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.328 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
+| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 5.923 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
+| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.821 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
+
 
 ### Low-level Python interface
 FovVideoVDP can also be run through the Python interface by instatiating the `pyfvvdp.fvvdp.fvvdp` class. This example shows how to predict the quality of images degraded by Gaussian noise and blur.
 
 ```python
+import os
+import numpy as np
 import pyfvvdp
 import ex_utils as utils
 
 I_ref = pyfvvdp.load_image_as_array(os.path.join('example_media', 'wavy_facade.png'))
 fv = pyfvvdp.fvvdp(display_name='standard_4k', heatmap='threshold')
 
 # Gaussian noise with variance 0.003
@@ -115,16 +128,16 @@
 # Gaussian blur with sigma=2
 I_test_blur = utils.imgaussblur(I_ref, 2)
 Q_JOD_blur, stats_blur = fv.predict( I_test_blur, I_ref, dim_order="HWC" )
 ```
 
 |Original | ![wavy-facade](https://github.com/gfxdisp/FovVideoVDP/raw/main/example_media/wavy_facade.png) | Quality | Difference map |
 | :---: | :---: | :---: | :---: |
-| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.532 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
-| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.674 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
+| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.537 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
+| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.693 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
 
 More examples can be found in these [example scripts](https://github.com/gfxdisp/FovVideoVDP/blob/main/pytorch_examples).
 
 
 ## MATLAB
 
 MATLAB code for the metric can be found in `matlab/fvvdp.m`. The full documentation of the metric can be shown by typing `doc fvvdp`.
@@ -151,16 +164,29 @@
 ## Differences between MATLAB and Pytorch versions
 
 * Both versions are implementation of the same metric, but due to differences in the video loaders, you can expect to see small differences in their predictions - typically up to 0.05 JOD.
 * PyTorch version is a bit faster when running on a GPU. 
 
 ## Release notes
 
+* v1.2.0 - 19 April 2023
+  * The python command line interface can now accept HDR video files and OpenEXR images. 
+  * [PU21-PSNR](https://github.com/gfxdisp/pu21) can be run in addition to FovVideoVDP
+  * Added new command line options: `--full-screen-resize`, `--metrics`, `--temp-padding`, `--feature`, `--output-dir`
+  * Faster decoding for large (4k) videos when run on CUDA (python, the command line interface `fvvdp`). 
+  * The prediction may differ slightly because of the way video files are handled and processed. There are no changes in the metric.
+  * Fixed issue when reading video frames in python freezed on some platforms (issue with python's `/dev/null` redirection)
+
+* v1.1.3 - 18 October 2022
+  * Added "raw" heatmap type to the command line. 
+  * Changed the way pyfvvdp classes are imported  to avoid clash between the file and class names (see updated pytortch_examples)
+  * Installation of PyEXR is now optional (caused problems on some operating systems).
+
 * v1.1.2 - 23 September 2022
- * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
+  * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
 
 * v1.1.1 - 28 August 2022
   * We found a small inconsistency in eccentricity calculations. After fixing this, the metric has been retrained on the same datasets as described in the paper. FovVideoVDP v1.1 will return JOD values that are different than v1.0. For that reason, it is important to mention the version number when reporting the results. 
   * Python interface has been thoroughly redesigned and make more consistent with Matlab's conterpart. Now it should be much easier to call the metric from Python. 
   * All Matlab examples have been ported to Python. 
   * Python version is now faster. 
   * Published as a PIP repository.
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/csf_cache/o0_sn1_5_cm0_604562_gpu0.mat` & `pyfvvdp-1.2.0/pyfvvdp/csf_cache/o0_sn1_5_cm0_604562_gpu0.mat`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/csf_cache/o5_sn1_5_cm0_604562_gpu0.mat` & `pyfvvdp-1.2.0/pyfvvdp/csf_cache/o5_sn1_5_cm0_604562_gpu0.mat`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp.py` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,273 +1,68 @@
 from abc import abstractmethod
 from urllib.parse import ParseResultBytes
 from numpy.lib.shape_base import expand_dims
 import torch
+from torch.utils import checkpoint
 from torch.functional import Tensor
 import torch.nn.functional as Func
 import numpy as np 
 import os
 import sys
-import argparse
-import time
-import math
+import json
+#import argparse
+#import time
+#import math
 import torch.utils.benchmark as torchbench
 import logging
 
 from pyfvvdp.visualize_diff_map import visualize_diff_map
+from pyfvvdp.video_source import *
 
 # For debugging only
 # from gfxdisp.pfs.pfs_torch import pfs_torch
 
 sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 
 from third_party.cpuinfo import cpuinfo
-from hdrvdp_lpyr_dec import hdrvdp_lpyr_dec
+from pyfvvdp.fvvdp_lpyr_dec import fvvdp_lpyr_dec, fvvdp_contrast_pyr
 from interp import interp1, interp3
-from utils import *
-from fvvdp_test import FovVideoVDP_Testbench
-
-from pyfvvdp.fvvdp_display_model import fvvdp_display_photometry, fvvdp_display_geometry
-
-
-"""
-fvvdp_video_source_* objects are used to supply test/reference frames to FovVideoVDP. 
-Those could be comming from memory or files. The subclasses of this abstract class implement
-reading the frames and converting them to the approprtate format. 
-"""
-class fvvdp_video_source:
-   
-    # Return (height, width, frames) touple with the resolution and
-    # the length of the video clip.
-    @abstractmethod
-    def get_video_size(self):
-        pass
-
-    # Return the frame rate of the video
-    @abstractmethod
-    def get_frames_per_second(self) -> int:
-        pass
-    
-    # Get a pair of test and reference video frames as a single-precision luminance map
-    # scaled in absolute inits of cd/m^2. 'frame' is the frame index,
-    # starting from 0. 
-    @abstractmethod
-    def get_test_frame( self, frame, device ) -> Tensor:
-        pass
-
-    @abstractmethod
-    def get_reference_frame( self, frame, device ) -> Tensor:
-        pass
-
-
-"""
-Function for changing the order of dimensions, for example, from "WHC" (width, height, colour) to "BCHW" (batch, colour, height, width)
-If a dimension is missing in in_dims, it will be added as a singleton dimension
-"""
-def reshuffle_dims( T: Tensor, in_dims: str, out_dims: str ) -> Tensor:
-    in_dims = in_dims.upper()
-    out_dims = out_dims.upper()    
-
-    # Find intersection of two strings    
-    inter_dims = ""
-    for kk in range(len(out_dims)):
-        if in_dims.find(out_dims[kk]) != -1:
-            inter_dims += out_dims[kk]
-
-    # First, permute into the right order
-    perm = [0] * len(inter_dims)
-    for kk in range(len(inter_dims)):
-        ind = in_dims.find(inter_dims[kk])
-        if ind == -1:
-            raise RuntimeError( 'Dimension "{}" missing in the target dimensions: "{}"'.format(in_dims[kk],out_dims) )
-        perm[kk] = ind                    
-    T_p = T.permute(perm)
-
-    # Add missing dimensions
-    out_sh = [1] * len(out_dims)
-    for kk in range(len(out_dims)):        
-        ind = inter_dims.find(out_dims[kk])
-        if ind != -1:
-            out_sh[kk] = T_p.shape[ind]
-
-    return T_p.reshape( out_sh )
-
-
-"""
-This video_source uses a photometric display model to convert input content (e.g. sRGB) to luminance maps. 
-"""
-class fvvdp_video_source_dm( fvvdp_video_source ):
-
-    def __init__( self,  display_photometry='sdr_4k_30', color_space_name='sRGB' ):
-        colorspaces_file = os.path.join(os.path.dirname(__file__), "fvvdp_data/color_spaces.json")
-        colorspaces = json2dict(colorspaces_file)
-
-        if not color_space_name in colorspaces:
-            raise RuntimeError( "Unknown color space: \"" + color_space_name + "\"" )
-
-        self.color_to_luminance = colorspaces[color_space_name]['RGB2Y']
-
-        if isinstance( display_photometry, str ):
-            display_models_file = os.path.join(os.path.dirname(__file__), "fvvdp_data/display_models.json")
-            display_models = json2dict(display_models_file)
-
-            self.dm_photometry = fvvdp_display_photometry.load(display_photometry)
-        elif isinstance( display_photometry, fvvdp_display_photometry ):
-            self.dm_photometry = display_photometry
-        else:
-            raise RuntimeError( "display_model must be a string or fvvdp_display_photometry subclass" )
-
-
-"""
-This video source supplies frames from either Pytorch tensors and Numpy arrays. It also applies a photometric display model.
-
-A batch of videos should be stored as a tensor or numpy array. Ideally, the tensor should have the dimensions BCFHW (batch, colour, frame, height, width).If tensor is stored in another formay, you can pass the order of dimsions as "dim_order" parameter. If any dimension is missing, it will
-be added as a singleton dimension. 
-
-This class is for display-encoded (gamma-encoded) content that will be processed by a display model to produce linear  absolute luminance emitted from a display.
-"""
-class fvvdp_video_source_array( fvvdp_video_source_dm ):
-               
-    # test_video, reference video - tensor with test and reference video frames. See the class description above for the explanation of dimensions of those tensors.
-    # fps - frames per second. Must be 0 for images
-    # dim_order - a string with the order of the dimensions. 'BCFHW' is the default.
-    # display_model - object that implements fvvdp_display_photometry
-    #   class
-    # color_space_name - name of the colour space (see
-    #   fvvdp_data/color_spaces.json)
-    def __init__( self, test_video, reference_video, fps, dim_order='BCFHW', display_photometry='sdr_4k_30', color_space_name='sRGB' ):
-
-        super().__init__(display_photometry=display_photometry, color_space_name=color_space_name)        
-
-        if test_video.shape != reference_video.shape:
-            raise RuntimeError( 'Test and reference image/video tensors must be exactly the same shape' )
-        
-        if len(dim_order) != len(test_video.shape):
-            raise RuntimeError( 'Input tensor much have exactly as many dimensions as there are characters in the "dims" parameter' )
 
-        # Convert numpy arrays to tensors. Note that we do not upload to device or change dtype at this point (to save GPU memory)
-        if isinstance( test_video, np.ndarray ):
-            if test_video.dtype == np.uint16:
-                # Torch does not natively support uint16. A workaround is to pack uint16 values into int16.
-                # This will be efficiently transferred and unpacked on the GPU.
-                # logging.info('Test has datatype uint16, packing into int16')
-                test_video = test_video.astype(np.int16)
-            test_video = torch.tensor(test_video)
-        if isinstance( reference_video, np.ndarray ):
-            if reference_video.dtype == np.uint16:
-                # Torch does not natively support uint16. A workaround is to pack uint16 values into int16.
-                # This will be efficiently transferred and unpacked on the GPU.
-                # logging.info('Reference has datatype uint16, packing into int16')
-                reference_video = reference_video.astype(np.int16)
-            reference_video = torch.tensor(reference_video)
-
-        # Change the order of dimension to match BFCHW - batch, frame, colour, height, width
-        test_video = reshuffle_dims( test_video, in_dims=dim_order, out_dims="BCFHW" )
-        reference_video = reshuffle_dims( reference_video, in_dims=dim_order, out_dims="BCFHW" )
+import pyfvvdp.utils as utils
 
-        B, C, F, H, W = test_video.shape
-        
-        if fps==0 and F>1:
-            raise RuntimeError( 'When passing video sequences, you must set ''frames_per_second'' parameter' )
-
-        if C!=3 and C!=1:
-            raise RuntimeError( 'The content must have either 1 or 3 colour channels.' )
-
-        self.fps = fps
-        self.is_video = (fps>0)
-        self.is_color = (C==3)
-        self.test_video = test_video
-        self.reference_video = reference_video
-
-
-    def get_frames_per_second(self):
-        return self.fps
-            
-    # Return a [height width frames] vector with the resolution and
-    # the number of frames in the video clip. [height width 1] is
-    # returned for an image. 
-    def get_video_size(self):
-
-        sh = self.test_video.shape
-        return (sh[3], sh[4], sh[2])
-    
-    # % Get a test video frame as a single-precision luminance map
-    # % scaled in absolute inits of cd/m^2. 'frame' is the frame index,
-    # % starting from 0. If use_gpu==true, the function should return a
-    # % gpuArray.
-
-    def get_test_frame( self, frame, device=torch.device('cpu') ):
-        return self._get_frame(self.test_video, frame, device )
-
-    def get_reference_frame( self, frame, device=torch.device('cpu') ):
-        return self._get_frame(self.reference_video, frame, device )
-
-    def _get_frame( self, from_array, frame, device ):        
-        # Determine the maximum value of the data type storing the
-        # image/video
-
-        if from_array.dtype is torch.float32:
-            frame = from_array[:,:,frame:(frame+1),:,:].to(device)
-        elif from_array.dtype is torch.int16:
-            # Use int16 to losslessly pack uint16 values
-            # Unpack from int16 by bit masking as described in this thread:
-            # https://stackoverflow.com/a/20766900
-            # logging.info('Found int16 datatype, unpack into uint16')
-            max_value = 2**16 - 1
-            # Cast to int32 to store values >= 2**15
-            frame_int32 = from_array[:,:,frame:(frame+1),:,:].to(device).to(torch.int32)
-            frame_uint16 = frame_int32 & max_value
-            # Finally convert to float in the range [0,1]
-            frame = frame_uint16.to(torch.float32) / max_value
-        elif from_array.dtype is torch.uint8:
-            frame = from_array[:,:,frame:(frame+1),:,:].to(device).to(torch.float32)/255
-        else:
-            raise RuntimeError( "Only uint8, uint16 and float32 is currently supported" )
+#from utils import *
+from fvvdp_test import FovVideoVDP_Testbench
 
-        L = self.dm_photometry.forward( frame )
-        
-        if self.is_color:
-            # Convert to grayscale
-            L = L[:,0:1,:,:,:]*self.color_to_luminance[0] + L[:,1:2,:,:,:]*self.color_to_luminance[1] + L[:,2:3,:,:,:]*self.color_to_luminance[2]
+from pyfvvdp.fvvdp_display_model import fvvdp_display_photometry, fvvdp_display_geometry
 
-        return L
 
 """
 FovVideoVDP metric. Refer to pytorch_examples for examples on how to use this class. 
 """
 class fvvdp:
-    def __init__(self, display_name="standard_4k", display_photometry=None, display_geometry=None, color_space="sRGB", foveated=False, heatmap=None, quiet=False, device=None):
+    def __init__(self, display_name="standard_4k", display_photometry=None, display_geometry=None, color_space="sRGB", foveated=False, heatmap=None, quiet=False, device=None, temp_padding="replicate", use_checkpoints=False):
         self.quiet = quiet
         self.foveated = foveated
         self.heatmap = heatmap
         self.color_space = color_space
+        self.temp_padding = temp_padding
+        self.use_checkpoints = use_checkpoints # Used for training
 
-        if display_photometry is None:
-            self.display_photometry = fvvdp_display_photometry.load(display_name)
-        else:
-            self.display_photometry = display_photometry
-        
         self.do_heatmap = (not self.heatmap is None) and (self.heatmap != "none")
 
-        if display_geometry is None:
-            self.display_geometry = fvvdp_display_geometry.load(display_name)
-        else:
-            self.display_geometry = display_geometry
-
-        self.pix_per_deg = self.display_geometry.get_ppd()
-
         # Use GPU if available
         if device is None:
             if torch.cuda.is_available() and torch.cuda.device_count()>0:
                 self.device = torch.device('cuda:0')
             else:
                 self.device = torch.device('cpu')
         else:
             self.device = device
-
+        
+        self.set_display_model(display_name, display_photometry=display_photometry, display_geometry=display_geometry)
         self.load_config()
 
         # if self.mask_s > 0.0:
         #     self.mask_p = self.mask_q + self.mask_s
 
         self.csf_cache              = {}
         self.csf_cache_dirs         = [
@@ -276,21 +71,34 @@
                                       ]
 
         self.omega = torch.tensor([0,5], device=self.device, requires_grad=False)
         for oo in self.omega:
             self.preload_cache(oo, self.csf_sigma)
 
         self.lpyr = None
-        self.imgaussfilt = ImGaussFilt(0.5 * self.pix_per_deg, self.device)
+        self.imgaussfilt = utils.ImGaussFilt(0.5 * self.pix_per_deg, self.device)
+        self.heatmap_pyr = None
 
+    def update_device( self, device ):
+        self.device = device
+        self.omega = torch.tensor([0,5], device=self.device, requires_grad=False)
+        for oo in self.omega:
+            self.preload_cache(oo, self.csf_sigma)
+
+        self.lpyr = None
+        self.imgaussfilt = utils.ImGaussFilt(0.5 * self.pix_per_deg, self.device)
+        # self.quality_band_freq_log = self.quality_band_freq_log.to(device)
+        # self.quality_band_w_log = self.quality_band_w_log.to(device)
 
     def load_config( self ):
 
-        parameters_file = os.path.join(os.path.dirname(__file__), "fvvdp_data/fvvdp_parameters.json")
-        parameters = json2dict(parameters_file)
+        #parameters_file = os.path.join(os.path.dirname(__file__), "fvvdp_data/fvvdp_parameters.json")
+        self.parameters_file = utils.config_files.find( "fvvdp_parameters.json" )
+        logging.debug( f"Loading FovVideoVDP parameters from '{self.parameters_file}'" )
+        parameters = utils.json2dict(self.parameters_file)
 
         #all common parameters between Matlab and Pytorch, loaded from the .json file
         self.mask_p = parameters['mask_p']
         self.mask_c = parameters['mask_c'] # content masking adjustment
         self.pu_dilate = parameters['pu_dilate']
         self.w_transient = parameters['w_transient'] # The weight of the transient temporal channel
         self.beta = parameters['beta'] # The exponent of the spatial summation (p-norm)
@@ -311,14 +119,30 @@
         self.k_cm = parameters['k_cm']  # new parameter controlling cortical magnification
         self.filter_len = parameters['filter_len']
         self.version = parameters['version']
 
         # other parameters
         self.debug = False
 
+    def set_display_model(self, display_name="standard_4k", display_photometry=None, display_geometry=None):
+        if display_photometry is None:
+            self.display_photometry = fvvdp_display_photometry.load(display_name)
+            self.display_name = display_name
+        else:
+            self.display_photometry = display_photometry
+            self.display_name = "unspecified"
+        
+        if display_geometry is None:
+            self.display_geometry = fvvdp_display_geometry.load(display_name)
+        else:
+            self.display_geometry = display_geometry
+
+        self.pix_per_deg = self.display_geometry.get_ppd()
+        self.imgaussfilt = utils.ImGaussFilt(0.5 * self.pix_per_deg, self.device)
+
     '''
     Predict image/video quality using FovVideoVDP.
 
     test_cont and reference_cont can be either numpy arrays or PyTorch tensors with images or video frames. 
         Depending on the display model (display_photometry), the pixel values should be either display encoded, or absolute linear.
         The two supported datatypes are float16 and uint8.
     dim_order - a string with the order of dimensions of test_cont and reference_cont. The individual characters denote
@@ -331,24 +155,24 @@
         The default order is "BCFHW". The processing can be a bit faster if data is provided in that order. 
     frame_padding - the metric requires at least 250ms of video for temporal processing. Because no previous frames exist in the
         first 250ms of video, the metric must pad those first frames. This options specifies the type of padding to use:
           'replicate' - replicate the first frame
           'circular'  - tile the video in the front, so that the last frame is used for frame 0.
           'pingpong'  - the video frames are mirrored so that frames -1, -2, ... correspond to frames 0, 1, ...
     '''
-    def predict(self, test_cont, reference_cont, dim_order="BCFHW", frames_per_second=0, fixation_point=None, frame_padding="replicate"):
+    def predict(self, test_cont, reference_cont, dim_order="BCFHW", frames_per_second=0, fixation_point=None):
 
         test_vs = fvvdp_video_source_array( test_cont, reference_cont, frames_per_second, dim_order=dim_order, display_photometry=self.display_photometry, color_space_name=self.color_space )
 
-        return self.predict_video_source(test_vs, fixation_point=fixation_point, frame_padding=frame_padding)
+        return self.predict_video_source(test_vs, fixation_point=fixation_point)
 
     '''
     The same as `predict` but takes as input fvvdp_video_source_* object instead of Numpy/Pytorch arrays.
     '''
-    def predict_video_source(self, vid_source, fixation_point=None, frame_padding="replicate"):
+    def predict_video_source(self, vid_source, fixation_point=None):
 
         # T_vid and R_vid are the tensors of the size (1,1,N,H,W)
         # where:
         # N - the number of frames
         # H - height in pixels
         # W - width in pixels
         # Both images must contain linear absolute luminance values in cd/m^2
@@ -360,15 +184,22 @@
 
         if fixation_point is None:
             fixation_point = torch.tensor([width//2, height//2])
         elif isinstance(fixation_point, np.ndarray):
             fixation_point = torch.tensor(fixation_point)
 
         if self.lpyr is None or self.lpyr.W!=width or self.lpyr.H!=height:
-            self.lpyr = hdrvdp_lpyr_dec(width, height, self.pix_per_deg, self.device)
+            if self.local_adapt=="gpyr":
+                self.lpyr = fvvdp_contrast_pyr(width, height, self.pix_per_deg, self.device)
+            else:
+                self.lpyr = fvvdp_lpyr_dec(width, height, self.pix_per_deg, self.device)
+
+            if self.do_heatmap:
+                self.heatmap_pyr = fvvdp_lpyr_dec(width, height, self.pix_per_deg, self.device)
+
 
         #assert self.W == R_vid.shape[-1] and self.H == R_vid.shape[-2]
         #assert len(R_vid.shape)==5
 
         is_image = (N_frames==1)  # Can run faster on images
 
         if is_image:
@@ -380,15 +211,15 @@
             self.F, self.omega = self.get_temporal_filters(vid_source.get_frames_per_second())
             # if self.debug: self.tb.verify_against_matlab(self.F,     'F_pod', self.device)
             # if self.debug: self.tb.verify_against_matlab(self.omega, 'omega', self.device)
 
 
         if self.do_heatmap:
             dmap_channels = 1 if self.heatmap == "raw" else 3
-            heatmap = torch.zeros([1,dmap_channels,N_frames,height,width], dtype=torch.float, device=self.device) 
+            heatmap = torch.zeros([1,dmap_channels,N_frames,height,width], dtype=torch.float16, device=torch.device('cpu')) # Store heatmap in the CPU memory
         else:
             heatmap = None
 
         N_nCSF = []
         sw_buf = [None, None]
         Q_per_ch = None
         w_temp_ch = [1.0, self.w_transient]
@@ -402,41 +233,41 @@
                 R[:,0, :, :, :] = vid_source.get_test_frame(0, device=self.device)
                 R[:,1, :, :, :] = vid_source.get_reference_frame(0, device=self.device)
 
             else: # This is video
                 if self.debug: print("Frame %d:\n----" % ff)
 
                 if ff == 0: # First frame
-                    if frame_padding == "replicate":
+                    if self.temp_padding == "replicate":
                         # TODO: proper handling of batches
                         sw_buf[0] = vid_source.get_test_frame(0, device=self.device).expand([1, 1, fl, height, width])
                         sw_buf[1] = vid_source.get_reference_frame(0, device=self.device).expand([1, 1, fl, height, width])
-                    elif frame_padding == "circular":
+                    elif self.temp_padding == "circular":
                         sw_buf[0] = torch.zeros([1, 1, fl, height, width], device=self.device)
                         sw_buf[1] = torch.zeros([1, 1, fl, height, width], device=self.device)
                         for kk in range(fl):
                             fidx = (N_frames - 1 - fl + kk) % N_frames
                             sw_buf[0][:,:,kk,...] = vid_source.get_test_frame(fidx, device=self.device)
                             sw_buf[1][:,:,kk,...] = vid_source.get_reference_frame(fidx, device=self.device)
-                    elif frame_padding == "pingpong":
+                    elif self.temp_padding == "pingpong":
                         sw_buf[0] = torch.zeros([1, 1, fl, height, width], device=self.device)
                         sw_buf[1] = torch.zeros([1, 1, fl, height, width], device=self.device)
 
                         pingpong = list(range(0,N_frames)) + list(range(N_frames-2,0,-1))
                         indices = []
                         while(len(indices) < (fl-1)):
                             indices = indices + pingpong
                         indices = indices[-(fl-1):] + [0]
 
                         for kk in range(fl):
                             fidx = indices[kk]
                             sw_buf[0][:,:,kk,...] = vid_source.get_test_frame(fidx,device=self.device)
                             sw_buf[1][:,:,kk,...] = vid_source.get_reference_frame(fidx,device=self.device)
                     else:
-                        raise RuntimeError( 'Unknown padding method "{}"'.format(frame_padding) )
+                        raise RuntimeError( 'Unknown padding method "{}"'.format(self.temp_padding) )
                 else:
                     cur_tframe = vid_source.get_test_frame(ff, device=self.device)
                     cur_rframe = vid_source.get_reference_frame(ff, device=self.device)
 
                     sw_buf[0] = torch.cat((sw_buf[0][:, :, 1:, :, :], cur_tframe), 2)
                     sw_buf[1] = torch.cat((sw_buf[1][:, :, 1:, :, :], cur_rframe), 2)
 
@@ -445,151 +276,186 @@
 
                 for cc in range(temp_ch):
                     # 1D filter over time (over frames)
                     corr_filter = self.F[cc].flip(0).view([1,1,self.F[cc].shape[0],1,1]) 
                     R[:,cc*2+0, :, :, :] = (sw_buf[0] * corr_filter).sum(dim=-3,keepdim=True)
                     R[:,cc*2+1, :, :, :] = (sw_buf[1] * corr_filter).sum(dim=-3,keepdim=True)
 
-            if self.debug: self.tb.verify_against_matlab(R.permute(0,2,3,4,1), 'Rdata', self.device, file='R_%d' % (ff+1), tolerance = 0.01)
+            if self.use_checkpoints:
+                # Used for training
+                Q_per_ch_block = checkpoint.checkpoint(self.process_block_of_frames, ff, R, vid_sz, temp_ch, fixation_point, heatmap, use_reentrant=False)
+            else:
+                Q_per_ch_block = self.process_block_of_frames(ff, R, vid_sz, temp_ch, fixation_point, heatmap)
 
-            # Perform Laplacian decomposition
-            # B = [None] * R.shape[1]
-            # for rr in range(R.shape[1]):
-            #     B[rr] = hdrvdp_lpyr_dec( R[0,rr:(rr+1),0:1,:,:], self.pix_per_deg, self.device)
+            if Q_per_ch is None:
+                Q_per_ch = torch.zeros((Q_per_ch_block.shape[0], Q_per_ch_block.shape[1], N_frames), device=self.device)
+            
+            Q_per_ch[:,:,ff:(ff+Q_per_ch_block.shape[2])] = Q_per_ch_block  
 
-            B_bands, B_gbands = self.lpyr.decompose(R[0,...])
+        rho_band = self.lpyr.get_freqs()
+        Q_jod = self.do_pooling_and_jods(Q_per_ch, rho_band[0:-1])
 
-            if self.debug: assert len(B_bands) == self.lpyr.get_band_count()
+        stats = {}
+        stats['Q_per_ch'] = Q_per_ch.detach().cpu().numpy() # the quality per channel and per frame
+        stats['rho_band'] = rho_band # Thespatial frequency per band
+        stats['frames_per_second'] = vid_source.get_frames_per_second()
+        stats['width'] = width
+        stats['height'] = height
+        stats['N_frames'] = N_frames
 
-            # CSF
-            N_nCSF = [[None, None] for i in range(self.lpyr.get_band_count()-1)]
+        if self.do_heatmap:            
+            stats['heatmap'] = heatmap
 
-            if self.do_heatmap:
-                Dmap_pyr_bands, Dmap_pyr_gbands = self.lpyr.decompose( torch.zeros([1,1,height,width], dtype=torch.float, device=self.device))
+        # if self.debug: self.tb.verify_against_matlab(Q_per_ch, 'Q_per_ch_data', self.device, file='Q_per_ch', tolerance = 0.1, relative=True, verbose=True)
+        # if self.debug: self.tb.verify_against_matlab(Q_sc,     'Q_sc_data',     self.device, file='Q_sc',     tolerance = 0.1, relative=True, verbose=True)
+        # if self.debug: self.tb.verify_against_matlab(Q_tc,     'Q_tc_data',     self.device, file='Q_tc',     tolerance = 0.1, relative=True, verbose=True)
+        # if self.debug: self.tb.verify_against_matlab(Q,        'Q_data',        self.device, file='Q',        tolerance = 0.1, relative=True, verbose=True)
+        # if self.debug: self.tb.verify_against_matlab(Q_jod,    'Q_jod_data',    self.device, file='Q_jod',    tolerance = 0.1, relative=True, verbose=True)
+        # if self.debug: self.tb.print_summary()    
 
-            # L_bkg_bb = [None for i in range(self.lpyr.get_band_count()-1)]
+        return (Q_jod.squeeze(), stats)
 
-            rho_band = self.lpyr.get_freqs()
+    # Perform pooling with per-band weights and map to JODs
+    def do_pooling_and_jods(self, Q_per_ch, rho_band):
 
-            # Adaptation
-            L_adapt = None
+        # Weights for the two temporal channels
+        if Q_per_ch.shape[1]==2: # If video
+            per_tband_w = torch.stack( (torch.ones(1, device=self.device), torch.as_tensor(self.w_transient, device=self.device)[None] ), dim=1)[:,:,None]
+        else: # If image
+            per_tband_w = 1
+
+        # Weights for the spatial bands
+        #per_sband_w = torch.exp(interp1( self.quality_band_freq_log, self.quality_band_w_log, torch.log(torch.as_tensor(rho_band, device=self.device)) ))[:,None,None]
+
+        #Q_sc = self.lp_norm(Q_per_ch*per_tband_w*per_sband_w, self.beta_sch, 0, False)  # Sum across spatial channels
+        Q_sc = self.lp_norm(Q_per_ch*per_tband_w, self.beta_sch, 0, False)  # Sum across spatial channels
+        Q_tc = self.lp_norm(Q_sc,     self.beta_tch, 1, False)  # Sum across temporal channels
+        Q    = self.lp_norm(Q_tc,     self.beta_t,   2, True)   # Sum across frames
+        Q = Q.squeeze()
 
-            if self.local_adapt == "simple":
-                L_adapt = R[0,1,0,...] # reference, sustained
-                if self.contrast == "log":
-                    L_adapt = torch.pow(10.0, L_adapt)
-                L_adapt = self.imgaussfilt.run(L_adapt)
-            elif self.local_adapt == "global":
-                print("ERROR: global adapt not supported")
-                return
+        sign = lambda x: (1, -1)[x<0]
+        beta_jod = 10.0**self.log_jod_exp
+        Q_jod = sign(self.jod_a) * ((abs(self.jod_a)**(1.0/beta_jod))* Q)**beta_jod + 10.0 # This one can help with very large numbers
+        return Q_jod.squeeze()
 
-            for cc in range(temp_ch):
-                for bb in range(self.lpyr.get_band_count()-1):
+    def process_block_of_frames(self, ff, R, vid_sz, temp_ch, fixation_point, heatmap):
+        # TODO: process multiple frames at a time. Right now, we process one frame at a time
 
-                    T_f = self.lpyr.get_band(B_bands, bb)[cc*2+0,0,...]
-                    R_f = self.lpyr.get_band(B_bands, bb)[cc*2+1,0,...]
+        height, width, N_frames = vid_sz
 
-                    L_bkg, R_f, T_f = self.compute_local_contrast(R_f, T_f, 
-                        self.lpyr.get_gband(B_gbands, bb+1)[1:2,...], L_adapt)
+        if self.debug: self.tb.verify_against_matlab(R.permute(0,2,3,4,1), 'Rdata', self.device, file='R_%d' % (ff+1), tolerance = 0.01)
 
-                    # temp_errs[ff] += torch.mean(torch.abs(R_f - T_f))
-                    # continue
+        # Perform Laplacian pyramid decomposition
+        B_bands, B_gbands = self.lpyr.decompose(R[0,...])
 
-                    # if self.debug: self.tb.verify_against_matlab(L_bkg, 'L_bkg_data', self.device, file='L_bkg_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01)
+        if self.debug: assert len(B_bands) == self.lpyr.get_band_count()
 
-                    # #  TODO: check cc = 1
-                    # if self.debug:
-                    #     print("%d, %d" % (cc, bb))
-                    #     h, w = T_f.shape[-2], T_f.shape[-1]
-                    #     np2img(stack_horizontal([
-                    #         (T_f * 100.0).squeeze().unsqueeze(-1).expand(h,w,3).cpu().numpy(), 
-                    #         (R_f * 100.0).squeeze().unsqueeze(-1).expand(h,w,3).cpu().numpy()])).show()
-                    if self.debug: self.tb.verify_against_matlab(T_f, 'T_f_data', self.device, file='T_f_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.001) 
-                    if self.debug: self.tb.verify_against_matlab(R_f, 'R_f_data', self.device, file='R_f_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.001)
+        # CSF
+        N_nCSF = [[None, None] for i in range(self.lpyr.get_band_count()-1)]
 
-                    if N_nCSF[bb][cc] is None:
+        if self.do_heatmap:
+            Dmap_pyr_bands, Dmap_pyr_gbands = self.heatmap_pyr.decompose( torch.zeros([1,1,height,width], dtype=torch.float, device=self.device))
 
-                        if self.foveated:   # Fixation, parafoveal sensitivity
-                            if fixation_point.dim() == 2:
-                                current_fixation_point = fixation_point[ff,:].squeeze()
-                            else:
-                                current_fixation_point = fixation_point
+        # L_bkg_bb = [None for i in range(self.lpyr.get_band_count()-1)]
 
-                            xv = torch.linspace( 0.5, vid_sz[1]-0.5, T_f.shape[-1], device=self.device )
-                            yv = torch.linspace( 0.5, vid_sz[0]-0.5, T_f.shape[-2], device=self.device )
-                            [xx, yy] = torch.meshgrid( xv, yv, indexing='xy' )
+        rho_band = self.lpyr.get_freqs()
 
-                            ecc = self.display_geometry.pix2eccentricity( torch.tensor((vid_sz[1], vid_sz[0])), xx, yy, current_fixation_point+0.5 )
+        # Adaptation
+        L_adapt = None
 
-                            # The same shape as bands
-                            ecc = ecc.reshape( [1, 1, ecc.shape[-2], ecc.shape[-1]] )
+        # if self.local_adapt == "simple":
+        #     L_adapt = R[0,1,0,...] # reference, sustained
+        #     if self.contrast == "log":
+        #         L_adapt = torch.pow(10.0, L_adapt)
+        #     L_adapt = self.imgaussfilt.run(L_adapt)
 
-                            res_mag = self.display_geometry.get_resolution_magnification(ecc)
-                        else:   # No fixation, foveal sensitivity everywhere
-                            res_mag = torch.ones(R_f.shape[-2:], device=self.device)
-                            ecc = torch.zeros(R_f.shape[-2:], device=self.device)
+        Q_per_ch_block = None
 
-                        rho = rho_band[bb] * res_mag
+        for cc in range(temp_ch):
+            for bb in range(self.lpyr.get_band_count()-1):
 
-                        # if self.debug: self.tb.verify_against_matlab(ecc, 'ecc_data', self.device, file='ecc_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01)  
-                        # if self.debug: self.tb.verify_against_matlab(rho, 'rho_data', self.device, file='rho_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.05)  
+                T_f = self.lpyr.get_band(B_bands, bb)[cc*2+0,0,...]
+                R_f = self.lpyr.get_band(B_bands, bb)[cc*2+1,0,...]
 
-                        S = self.cached_sensitivity(rho, self.omega[cc], L_bkg, ecc, self.csf_sigma) * np.power(10.0, self.sensitivity_correction/20.0)
-                        # if self.debug: self.tb.verify_against_matlab(S, 'S_data', self.device, file='S_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01, verbose=False)
+                if self.local_adapt=="gpyr":
+                    L_bkg = self.lpyr.get_gband(B_gbands, bb)
+                else:
+                    # 1:2 below is passing reference sustained
+                    L_bkg, R_f, T_f = self.compute_local_contrast(R_f, T_f, 
+                        self.lpyr.get_gband(B_gbands, bb+1)[1:2,...], L_adapt)
 
-                        if self.contrast == "log": N_nCSF[bb][cc] = self.weber2log(torch.min(1./S, self.torch_scalar(0.9999999)))
-                        else:                      N_nCSF[bb][cc] = torch.reciprocal(S)
-                        # if self.debug: self.tb.verify_against_matlab(N_nCSF[bb][cc], 'N_nCSF_data', self.device, file='N_nCSF_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01, relative = True)
+                # temp_errs[ff] += torch.mean(torch.abs(R_f - T_f))
+                # continue
 
-                    D = self.apply_masking_model(T_f, R_f, N_nCSF[bb][cc], cc)
-                    if self.debug: self.tb.verify_against_matlab(D, 'D_data', self.device, file='D_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.1, relative = True, verbose=False)
+                # if self.debug: self.tb.verify_against_matlab(L_bkg, 'L_bkg_data', self.device, file='L_bkg_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01)
 
-                    if self.do_heatmap:
-                        if cc == 0: self.lpyr.set_band(Dmap_pyr_bands, bb, D)
-                        else:       self.lpyr.set_band(Dmap_pyr_bands, bb, self.lpyr.get_band(Dmap_pyr_bands, bb) + w_temp_ch[cc] * D)
+                if self.debug: self.tb.verify_against_matlab(T_f, 'T_f_data', self.device, file='T_f_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.001) 
+                if self.debug: self.tb.verify_against_matlab(R_f, 'R_f_data', self.device, file='R_f_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.001)
 
-                    if Q_per_ch is None:
-                        Q_per_ch = torch.zeros((len(B_bands)-1, 2, N_frames), device=self.device)
+                # Pre-compute the inverse of the CSF (contrast thresholds)
+                if N_nCSF[bb][cc] is None:
 
-                    Q_per_ch[bb,cc,ff] = w_temp_ch[cc] * self.lp_norm(D.flatten(), self.beta, 0, True)
+                    if self.foveated:   # Fixation, parafoveal sensitivity
+                        if fixation_point.dim() == 2:
+                            current_fixation_point = fixation_point[ff,:].squeeze()
+                        else:
+                            current_fixation_point = fixation_point
 
-                    if self.debug: self.tb.verify_against_matlab(Q_per_ch[bb,cc,ff], 'Q_per_ch_data', self.device, file='Q_per_ch_%d_%d_%d' % (bb+1,cc+1,ff+1), tolerance = 0.1, relative=True, verbose=False)
-            # break
-            if self.do_heatmap:
-                beta_jod = np.power(10.0, self.log_jod_exp)
-                dmap = torch.pow(self.lpyr.reconstruct(Dmap_pyr_bands), beta_jod) * abs(self.jod_a)         
-                if self.heatmap == "raw":
-                    heatmap[:,:,ff,...] = dmap 
-                else:
-                    ref_frame = R[:,0, :, :, :]
-                    heatmap[:,:,ff,...] = visualize_diff_map(dmap, context_image=ref_frame, colormap_type=self.heatmap)
+                        xv = torch.linspace( 0.5, vid_sz[1]-0.5, T_f.shape[-1], device=self.device )
+                        yv = torch.linspace( 0.5, vid_sz[0]-0.5, T_f.shape[-2], device=self.device )
+                        [xx, yy] = torch.meshgrid( xv, yv, indexing='xy' )
 
+                        ecc = self.display_geometry.pix2eccentricity( torch.tensor((vid_sz[1], vid_sz[0])), xx, yy, current_fixation_point+0.5 )
 
-        Q_sc = self.lp_norm(Q_per_ch, self.beta_sch, 0, False)
-        Q_tc = self.lp_norm(Q_sc,     self.beta_tch, 1, False)
-        Q    = self.lp_norm(Q_tc,     self.beta_t,   2, True)
+                        # The same shape as bands
+                        ecc = ecc.reshape( [1, 1, ecc.shape[-2], ecc.shape[-1]] )
 
-        Q = Q.squeeze()
+                        res_mag = self.display_geometry.get_resolution_magnification(ecc)
+                    else:   # No fixation, foveal sensitivity everywhere
+                        res_mag = torch.ones(R_f.shape[-2:], device=self.device)
+                        ecc = torch.zeros(R_f.shape[-2:], device=self.device)
 
-        beta_jod = np.power(10.0, self.log_jod_exp)
-        Q_jod = np.sign(self.jod_a) * torch.pow(torch.tensor(np.power(np.abs(self.jod_a),(1.0/beta_jod)), device=self.device)* Q, beta_jod) + 10.0 # This one can help with very large numbers
+                    rho = rho_band[bb] * res_mag
 
-        stats = {}
+                    # if self.debug: self.tb.verify_against_matlab(ecc, 'ecc_data', self.device, file='ecc_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01)  
+                    # if self.debug: self.tb.verify_against_matlab(rho, 'rho_data', self.device, file='rho_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.05)  
 
-        if self.do_heatmap:            
-            stats['heatmap'] = heatmap
+                    S = self.cached_sensitivity(rho, self.omega[cc], L_bkg, ecc, self.csf_sigma) * 10.0**(self.sensitivity_correction/20.0)
+                    # if self.debug: self.tb.verify_against_matlab(S, 'S_data', self.device, file='S_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01, verbose=False)
 
-        if self.debug: self.tb.verify_against_matlab(Q_per_ch, 'Q_per_ch_data', self.device, file='Q_per_ch', tolerance = 0.1, relative=True, verbose=True)
-        if self.debug: self.tb.verify_against_matlab(Q_sc,     'Q_sc_data',     self.device, file='Q_sc',     tolerance = 0.1, relative=True, verbose=True)
-        if self.debug: self.tb.verify_against_matlab(Q_tc,     'Q_tc_data',     self.device, file='Q_tc',     tolerance = 0.1, relative=True, verbose=True)
-        if self.debug: self.tb.verify_against_matlab(Q,        'Q_data',        self.device, file='Q',        tolerance = 0.1, relative=True, verbose=True)
-        if self.debug: self.tb.verify_against_matlab(Q_jod,    'Q_jod_data',    self.device, file='Q_jod',    tolerance = 0.1, relative=True, verbose=True)
-        if self.debug: self.tb.print_summary()    
+                    if self.contrast == "log": N_nCSF[bb][cc] = self.weber2log(torch.min(1./S, self.torch_scalar(0.9999999)))
+                    else:                      N_nCSF[bb][cc] = torch.reciprocal(S)
+                    # if self.debug: self.tb.verify_against_matlab(N_nCSF[bb][cc], 'N_nCSF_data', self.device, file='N_nCSF_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.01, relative = True)
+
+                D = self.apply_masking_model(T_f, R_f, N_nCSF[bb][cc], cc)
+
+                if self.debug: self.tb.verify_against_matlab(D, 'D_data', self.device, file='D_%d_%d_%d' % (ff+1,bb+1,cc+1), tolerance = 0.1, relative = True, verbose=False)
+
+                if self.do_heatmap:
+                    if cc == 0: self.heatmap_pyr.set_band(Dmap_pyr_bands, bb, D)
+                    else:       
+                        w_temp_ch = [1.0, self.w_transient]
+                        self.heatmap_pyr.set_band(Dmap_pyr_bands, bb, self.heatmap_pyr.get_band(Dmap_pyr_bands, bb) + w_temp_ch[cc] * D)
+
+                if Q_per_ch_block is None:
+                    Q_per_ch_block = torch.zeros((self.lpyr.height, 2, 1), device=self.device)
+
+                Q_per_ch_block[bb,cc,0] = self.lp_norm(D.flatten(), self.beta, 0, True)
+
+        if self.do_heatmap:
+            beta_jod = np.power(10.0, self.log_jod_exp)
+            dmap = torch.pow(self.heatmap_pyr.reconstruct(Dmap_pyr_bands), beta_jod) * abs(self.jod_a)         
+            if self.heatmap == "raw":
+                heatmap[:,:,ff,...] = dmap.detach().type(torch.float16).cpu()
+            else:
+                ref_frame = R[:,0, :, :, :]
+                heatmap[:,:,ff,...] = visualize_diff_map(dmap, context_image=ref_frame, colormap_type=self.heatmap).detach().type(torch.float16).cpu()
+        
+        return Q_per_ch_block
 
-        return (Q_jod.squeeze(), stats)
 
     def compute_local_contrast(self, R, T, next_gauss_band, L_adapt):
         if self.local_adapt=="simple":
             L_bkg = Func.interpolate(L_adapt.unsqueeze(0).unsqueeze(0), R.shape, mode='bicubic', align_corners=True)
             # L_bkg = torch.ones_like(R) * torch.mean(R)
             # np2img(l2rgb(L_adapt.unsqueeze(-1).cpu().data.numpy())/200.0).show()
             # np2img(l2rgb(L_bkg[0,0].unsqueeze(-1).cpu().data.numpy())/200.0).show()
@@ -614,15 +480,15 @@
     def preload_cache(self, omega, sigma):
         key = self.get_cache_key(omega, sigma, self.k_cm)
         for csf_cache_dir in self.csf_cache_dirs:
             #fname = os.path.join(csf_cache_dir, key + '_cpu.mat')
             fname = os.path.join(csf_cache_dir, key + '_gpu0.mat')
             if os.path.isfile(fname):
                 #lut = load_mat_dict(fname, "lut_cpu", self.device)
-                lut = load_mat_dict(fname, "lut", self.device)
+                lut = utils.load_mat_dict(fname, "lut", self.device)
                 for k in lut:
                     lut[k] = torch.tensor(lut[k], device=self.device, requires_grad=False)
                 self.csf_cache[key] = {"lut" : lut}
                 break
         if key not in self.csf_cache:
             raise RuntimeError("Error: cache file for %s not found" % key)
 
@@ -654,56 +520,56 @@
         #
         # G = log10( B/A );
         #
         return torch.log10(1.0 + W)
 
     def phase_uncertainty(self, M):
         if self.pu_dilate != 0:
-            M_pu = imgaussfilt( M, self.pu_dilate ) * torch.pow(10.0, self.mask_c)
+            M_pu = utils.imgaussfilt( M, self.pu_dilate ) * torch.pow(10.0, self.mask_c)
         else:
+            #M_pu = M * (10**self.mask_c); # * torch.pow(self.torch_scalar(10.0), self.torch_scalar(self.mask_c))
             M_pu = M * torch.pow(self.torch_scalar(10.0), self.torch_scalar(self.mask_c))
         return M_pu
 
-    def mask_func_perc_norm(self, G, G_mask):
-        # Masking on perceptually normalized quantities (as in Daly's VDP)
+    # def mask_func_perc_norm(self, G, G_mask):
+    #     # Masking on perceptually normalized quantities (as in Daly's VDP)
         
-        p = self.mask_p
-        #q = self.mask_q
-        #k = self.k_mask_self
+    #     p = self.mask_p
+    #     #q = self.mask_q
+    #     #k = self.k_mask_self
         
-        R = torch.div(torch.pow(G,p), torch.sqrt( 1. + torch.pow(k * G_mask, 2*q)))
+    #     R = torch.div(torch.pow(G,p), torch.sqrt( 1. + torch.pow(k * G_mask, 2*q)))
 
-        return R
+    #     return R
 
     def mask_func_perc_norm2(self, G, G_mask, p, q ):
         # Masking on perceptually normalized quantities (as in Daly's VDP)        
         R = torch.div(torch.pow(G,p), 1. + torch.pow(G_mask, q))
         return R
 
     def apply_masking_model(self, T, R, N, cc):
         # cc - temporal channel: 0 - sustained, 1 - transient
-        if self.masking_model == "joint_mutual_masking_perc_norm":
-            T = torch.div(T, N)
-            R = torch.div(R, N)
-            M = self.phase_uncertainty( torch.min( torch.abs(T), torch.abs(R) ) )
-            d = torch.abs(T-R)
-            M = M + d
-            D = self.mask_func_perc_norm( d, M )
-        elif self.masking_model == 'min_mutual_masking_perc_norm2':
-            p = self.mask_p
-            if cc==0:
-                q = self.mask_q_sust
-            else:
-                q = self.mask_q_trans     
-            T = torch.div(T, N)
-            R = torch.div(R, N)
-            M = self.phase_uncertainty( torch.min( torch.abs(T), torch.abs(R) ) )
-            D = self.mask_func_perc_norm2( torch.abs(T-R), M, p, q )
-        else:
-            print("Error: Masking model" + self.masking_model + "not implemented")
+        # if self.masking_model == "joint_mutual_masking_perc_norm":
+        #     T = torch.div(T, N)
+        #     R = torch.div(R, N)
+        #     M = self.phase_uncertainty( torch.min( torch.abs(T), torch.abs(R) ) )
+        #     d = torch.abs(T-R)
+        #     M = M + d
+        #     D = self.mask_func_perc_norm( d, M )
+        # elif self.masking_model == 'min_mutual_masking_perc_norm2':
+
+        p = self.mask_p
+        q = self.mask_q_sust if cc==0 else self.mask_q_trans            
+        T = torch.div(T, N)
+        R = torch.div(R, N)
+        M = self.phase_uncertainty( torch.min( torch.abs(T), torch.abs(R) ) )
+        D = self.mask_func_perc_norm2( torch.abs(T-R), M, p, q )
+
+        # else:
+        #     print("Error: Masking model" + self.masking_model + "not implemented")
 
         D = torch.clamp( D, max=1e4)
         return D
 
     def lp_norm(self, x, p, dim=0, normalize=True):
         if dim is None:
             dim = 0
@@ -736,15 +602,48 @@
         F[0].requires_grad = False
         F[1].requires_grad = False
 
         return F, omega
 
     def torch_scalar(self, val, dtype=torch.float32):
         return torch.tensor(val, dtype=dtype, device=self.device)
-        
+
+    def short_name(self):
+        return "FovVideoVDP"
+
+    def quality_unit(self):
+        return "JOD"
+
+    def get_info_string(self):
+        if self.display_name.startswith('standard_'):
+            #append this if are using one of the standard displays
+            standard_str = ', (' + self.display_name + ')'
+        else:
+            standard_str = ''
+        fv_mode = 'foveated' if self.foveated else 'non-foveated'
+        return '"FovVideoVDP v{}, {:.4g} [pix/deg], Lpeak={:.5g}, Lblack={:.4g} [cd/m^2], {}{}"'.format(self.version, self.pix_per_deg, self.display_photometry.get_peak_luminance(), self.display_photometry.get_black_level(), fv_mode, standard_str)
+
+    def write_features_to_json(self, stats, dest_fname):
+        Q_per_ch = stats['Q_per_ch'] # quality per channel [bb,cc,ff]
+        fmap = {}
+        for key, value in stats.items():
+            if not key in ["Q_per_ch", "heatmap"]:
+                if isinstance(value, np.ndarray):
+                    fmap[key] = value.tolist()
+                else:
+                    fmap[key] = value
+
+        for cc in range(Q_per_ch.shape[1]): # for each temporal channel
+            for bb in range(Q_per_ch.shape[0]): # for each band
+                fmap[f"t{cc}_b{bb}"] = Q_per_ch[bb,cc,:].tolist()
+
+        with open(dest_fname, 'w', encoding='utf-8') as f:
+            json.dump(fmap, f, ensure_ascii=False, indent=4)
+
+
 
 # def parse_args():
 #     parser = argparse.ArgumentParser(description="Video-VDP metric test app")
 #     parser.add_argument("--gpu",      type=int,  default=-1, help="use GPU")
 #     group = parser.add_mutually_exclusive_group(required = True)
 #     group.add_argument("--benchmark", type=str, default=None, required=False, help="benchmark performance for chosen resolution: e.g. 1920x1080x60")
 #     group.add_argument("--test", action='store_true', default=False, required=False, help="test against FovDots MATLAB dataset (must be present on disk)")
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/color_spaces.json` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/color_spaces.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8947368421052632%*

 * *Differences: {"'BT.2020'": "OrderedDict([('gamma', '2.4'), ('whitepoint', 'D65'), ('RGB2Y', [0.29203, 0.79652, "*

 * *              '0.04588])])',*

 * * 'delete': "['Rec.2020']"}*

```diff
@@ -63,14 +63,23 @@
             2.9515373,
             -1.2894116,
             -0.4738445
         ],
         "gamma": "1.8",
         "whitepoint": "D65"
     },
+    "BT.2020": {
+        "RGB2Y": [
+            0.29203,
+            0.79652,
+            0.04588
+        ],
+        "gamma": "2.4",
+        "whitepoint": "D65"
+    },
     "Best RGB": {
         "RGB2X": [
             0.6326696,
             0.2045558,
             0.1269946
         ],
         "RGB2Y": [
@@ -413,23 +422,14 @@
             1.3459433,
             -0.2556075,
             -0.0511118
         ],
         "gamma": "1.8",
         "whitepoint": "D50"
     },
-    "Rec.2020": {
-        "RGB2Y": [
-            0.29203,
-            0.79652,
-            0.04588
-        ],
-        "gamma": "2.4",
-        "whitepoint": "D65"
-    },
     "SMPTE-C RGB": {
         "RGB2X": [
             0.3935891,
             0.3652497,
             0.1916313
         ],
         "RGB2Y": [
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/display_models.json` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/display_models.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'standard_hdr_linear'": "OrderedDict([('name', '30-inch 4K HDR, monitor, peak luminance 1500 "*

 * *                          'cd/m^2, viewed under low light levels (10 lux), seen from 2 x display '*

 * *                          "height'), ('EOTF', 'linear'), ('resolution', [3840, 2160]), "*

 * *                          "('viewing_distance_meters', 0.7472), ('diagonal_size_inches', 30), "*

 * *                          "('max_luminance', 1500), ('contrast', 1000000), ('E_ambient', 10), "*

 * *                          "('source […]*

```diff
@@ -124,15 +124,30 @@
         "resolution": [
             1920,
             1080
         ],
         "source": "none",
         "viewing_distance_meters": 0.6
     },
-    "standard_hdr": {
+    "standard_hdr_linear": {
+        "EOTF": "linear",
+        "E_ambient": 10,
+        "contrast": 1000000,
+        "diagonal_size_inches": 30,
+        "max_luminance": 1500,
+        "name": "30-inch 4K HDR, monitor, peak luminance 1500 cd/m^2, viewed under low light levels (10 lux), seen from 2 x display height",
+        "resolution": [
+            3840,
+            2160
+        ],
+        "source": "none",
+        "viewing_distance_meters": 0.7472
+    },
+    "standard_hdr_pq": {
+        "EOTF": "PQ",
         "E_ambient": 10,
         "contrast": 1000000,
         "diagonal_size_inches": 30,
         "max_luminance": 1500,
         "name": "30-inch 4K HDR, monitor, peak luminance 1500 cd/m^2, viewed under low light levels (10 lux), seen from 2 x display height",
         "resolution": [
             3840,
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/fvvdp_parameters.json` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/fvvdp_parameters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.94%*

 * *Differences: {"'__comment'": "'Calibration parameters of FovVideoVDP 1.2. See the source of fvvdp_core.m for "*

 * *                "their description.'",*

 * * "'internal_model_name'": "'fvvdp_1_20'",*

 * * "'version'": "'1.2.0'"}*

```diff
@@ -1,27 +1,27 @@
 {
-    "__comment": "Calibration parameters of FovVideoVDP 1.1. See the source of fvvdp_core.m for their description.",
+    "__comment": "Calibration parameters of FovVideoVDP 1.2. See the source of fvvdp_core.m for their description.",
     "beta": 1.52134,
     "beta_sch": 1,
     "beta_t": 1,
     "beta_tch": 0.666092,
     "calibration_date": "20/11/2021",
     "contrast": "weber",
     "csf_sigma": -1.5,
     "filter_len": -1,
-    "internal_model_name": "fvvdp_1_12",
+    "internal_model_name": "fvvdp_1_20",
     "jod_a": -0.0161713,
     "k_cm": 0.604562,
     "local_adapt": "gpyr",
     "log_jod_exp": -0.228,
     "mask_c": -0.973838,
     "mask_p": 2.4,
     "mask_q_sust": 2.43685,
     "mask_q_trans": 4.946,
     "masking_model": "min_mutual_masking_perc_norm2",
     "pu_dilate": 0,
     "sensitivity_correction": 16.2596,
     "sustained_beta": 0.06,
     "sustained_sigma": 0.5,
-    "version": "1.1.3",
+    "version": "1.2.0",
     "w_transient": 0.25
 }
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_data/fvvdp_parameters_1_0.json` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_data/fvvdp_parameters_1_0.json`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_display_model.py` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_display_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 import torch.nn.functional as Func
 import numpy as np 
 import math
 import logging
 import os
 
-from utils import json2dict
+import pyfvvdp.utils as utils
 
 # Convert pixel values to linear RGB using sRGB non-linearity
 # 
 # L = srgb2lin( p )
 #
 # p - pixel values (between 0 and 1)
 # L - relative linear RGB (or luminance), normalized to the range 0-1
@@ -28,27 +28,48 @@
         pass
 
     # Print the display specification    
     @abstractmethod
     def print( self ):
         pass
 
+    # @classmethod
+    # def default_model_file( cls ):
+    #     return os.path.join(os.path.dirname(__file__), "fvvdp_data/display_models.json")
+
+    @classmethod
+    def list_displays( cls ):
+        models_file = utils.config_files.find( "display_models.json" )
+
+        logging.info( f"JSON file with display models: {models_file}" )
+
+        models = utils.json2dict(models_file)
+
+        for display_name in models:
+            dm = fvvdp_display_photometry.load(display_name)
+            dm.print()
+
     @classmethod
     def load( cls, display_name ):
-        models_file      = os.path.join(os.path.dirname(__file__), "fvvdp_data/display_models.json")
+        models_file = utils.config_files.find( "display_models.json" )
 
-        models = json2dict(models_file)
+        models = utils.json2dict(models_file)
 
         if not display_name in models:
             raise RuntimeError( "Unknown display model: \"" + display_name + "\"" )
 
         model = models[display_name]
 
         Y_peak = model["max_luminance"]
 
+        if "EOTF" in model:
+            EOTF = model["EOTF"]
+        else:
+            EOTF = 'sRGB'
+
         if "min_luminance" in model:
             contrast = Y_peak/model["min_luminance"]
         elif "contrast" in model:
             contrast = model["contrast"]
         else:
             contrast = 500
 
@@ -66,38 +87,156 @@
 
         # Reflectivity of the display panel
         if "gamma" in model: 
             gamma = model["gamma"]
         else:
             gamma = 2.2
 
-        obj = fvvdp_display_photo_gog( Y_peak, contrast, gamma, E_ambient, k_refl)
+        obj = fvvdp_display_photo_eotf( Y_peak, contrast=contrast, gamma=gamma, EOTF=EOTF, E_ambient=E_ambient, k_refl=k_refl, name=display_name)
         obj.full_name = model["name"]
         obj.short_name = display_name
 
         return obj
 
+def pq2lin( V ):
+    """ Convert from PQ-encoded values V (between 0 and 1) to absolute linear values (between 0.005 and 10000)
+    """
+    Lmax = 10000
+    n    = 0.15930175781250000
+    m    = 78.843750000000000
+    c1   = 0.83593750000000000
+    c2   = 18.851562500000000
+    c3   = 18.687500000000000
 
+    im_t = torch.pow(V,1/m)
+    L = Lmax * torch.pow((im_t-c1).clamp(min=0)/(c2-c3*im_t), 1/n)
+    return L
 
+class fvvdp_display_photo_eotf(fvvdp_display_photometry): 
+    # Display model with several EOTF, to simulate both SDR and HDR displays
+    #
+    # dm = fvvdp_display_photo_eotf( Y_peak, contrast, EOTF, gamma, E_ambient, k_refl )
+    #
+    # Parameters (default value shown in []):
+    # Y_peak - display peak luminance in cd/m^2 (nit), e.g. 200 for a typical
+    #          office monitor, 1000 for an HDR display, ...
+    # contrast - [1000] the contrast of the display. The value 1000 means
+    #          1000:1
+    # EOTF - 'sRGB', 'gamma' or 'PQ'
+    # gamma - gamma of the display, typically 2.2. Used only if EOTF=='gamma'       
+    # E_ambient - [0] ambient light illuminance in lux, e.g. 600 for bright
+    #         office
+    # k_refl - [0.005] reflectivity of the display screen
+    #
+    # For more details on the GOG display model, see:
+    # https://www.cl.cam.ac.uk/~rkm38/pdfs/mantiuk2016perceptual_display.pdf
+    #
+    # Copyright (c) 2010-2022, Rafal Mantiuk
+    def __init__( self, Y_peak, contrast = 1000, EOTF='sRGB', gamma = 2.2, E_ambient = 0, k_refl = 0.005, name=None ):
+            
+        self.Y_peak = Y_peak            
+        self.contrast = contrast
+        self.EOTF = EOTF
+        self.gamma = gamma
+        self.E_ambient = E_ambient
+        self.k_refl = k_refl
+        self.name = name    
+        
+    # Transforms display-encoded pixel values V, which must be in the range
+    # 0-1 into absolute linear colorimetric values emitted from
+    # the display.
+    def forward( self, V ):
+        
+        if self.EOTF != 'linear' and (torch.any(V>1).bool() or torch.any(V<0).bool()):
+            logging.warning("Pixel outside the valid range 0-1")
+            V = V.clamp( 0., 1. )
+            
+        Y_black = self.get_black_level()
+                
+        if self.EOTF=='sRGB':
+            L = (self.Y_peak-Y_black)*srgb2lin(V) + Y_black
+        elif self.EOTF=='gamma':
+            L = (self.Y_peak-Y_black)*torch.pow(V, self.gamma) + Y_black
+        elif self.EOTF=='PQ':
+            L = pq2lin( V ).clip(0.005, self.Y_peak) + Y_black #TODO: soft clipping
+        elif self.EOTF=='linear':
+            L = V.clip(0.005, self.Y_peak) + Y_black #TODO: soft clipping
+        else:
+            raise RuntimeError( f"Unknown EOTF '{self.EOTF}'" )        
+        return L
+        
 
-class fvvdp_display_photo_gog(fvvdp_display_photometry): 
-    # Gain-gamma-offset display model to simulate SDR displays
-    # Object variables:
-    #  Y_peak - display peak luminance in cd/m^2
-    #  contrast - display contrast 
-    #  gamma
-    #  E_ambient
-    #  k_refl
+    def get_peak_luminance( self ):
+        return self.Y_peak
+
+    # Get the effective black level, accounting for screen reflections
+    def get_black_level( self ):
+        Y_refl = self.E_ambient/math.pi*self.k_refl  # Reflected ambient light            
+        Y_black = Y_refl + self.Y_peak/self.contrast
+
+        return Y_black
+
+    # Print the display specification    
+    def print( self ):
+        Y_black = self.get_black_level()
+        
+        logging.info( 'Photometric display model: {}'.format(self.name) )
+        logging.info( '  Peak luminance: {} cd/m^2'.format(self.Y_peak) )
+        logging.info( '  EOTF: {}'.format(self.EOTF) )
+        logging.info( '  Contrast - theoretical: {}:1'.format( round(self.contrast) ) )
+        logging.info( '  Contrast - effective: {}:1'.format( round(self.Y_peak/Y_black) ) )
+        logging.info( '  Ambient light: {} lux'.format( self.E_ambient ) )
+        logging.info( '  Display reflectivity: {}%'.format( self.k_refl*100 ) )
     
+
+class fvvdp_display_photo_absolute(fvvdp_display_photometry):
+    # Use this photometric model when passing absolute colorimetric of
+    # photometric values, scaled in cd/m^2
+    # Object variables:
+    #  L_max - display peak luminance in cd/m^2
+    #  L_min - display black level
+    def __init__(self, L_max=10000, L_min=0.005):
+
+        self.L_max = L_max
+        self.L_min = L_min
+
+
+    def forward( self, V ):
+
+        # Clamp the values that are outside the (L_min, L_max) range.
+        L = V.clamp(self.L_min, self.L_max)
+
+        if V.max() < 1:
+            logging.warning('Pixel values are very low. Perhaps images are' \
+                            ' not scaled in the absolute units of cd/m^2.')
+
+        return L
+
+
+    def  get_peak_luminance( self ):
+        return self.L_max
+
+
+    def get_black_level( self ):
+        return self.L_min
+
+    # Print the display specification
+    def print( self ):
+        Y_black = self.get_black_level()
+
+        logging.info('Photometric display model:')
+        logging.info('  Absolute photometric/colorimetric values')
+
+
+
+class fvvdp_display_photo_gog(fvvdp_display_photometry): 
     # Gain-gamma-offset display model to simulate SDR displays
     #
-    # dm = fvvdp_display_photo_gog( Y_peak )
-    # dm = fvvdp_display_photo_gog( Y_peak, contrast )
-    # dm = fvvdp_display_photo_gog( Y_peak, contrast, gamma )
-    # dm = fvvdp_display_photo_gog( Y_peak, contrast, gamma, E_ambient )
+    # Depreciated, included for compatibility. Use fvvdp_display_photo_eotf instead
+    #
     # dm = fvvdp_display_photo_gog( Y_peak, contrast, gamma, E_ambient, k_refl )
     #
     # Parameters (default value shown in []):
     # Y_peak - display peak luminance in cd/m^2 (nit), e.g. 200 for a typical
     #          office monitor
     # contrast - [1000] the contrast of the display. The value 1000 means
     #          1000:1
@@ -107,21 +246,22 @@
     #         office
     # k_refl - [0.005] reflectivity of the display screen
     #
     # For more details on the GOG display model, see:
     # https://www.cl.cam.ac.uk/~rkm38/pdfs/mantiuk2016perceptual_display.pdf
     #
     # Copyright (c) 2010-2021, Rafal Mantiuk
-    def __init__( self, Y_peak, contrast = 1000, gamma = 2.2, E_ambient = 0, k_refl = 0.005 ):
+    def __init__( self, Y_peak, contrast = 1000, gamma = 2.2, E_ambient = 0, k_refl = 0.005, name=None ):
             
         self.Y_peak = Y_peak            
         self.contrast = contrast
         self.gamma = gamma
         self.E_ambient = E_ambient
         self.k_refl = k_refl
+        self.name = name
     
         
     # Transforms gamma-encoded pixel values V, which must be in the range
     # 0-into absolute linear colorimetric values emitted from
     # the display.
     def forward( self, V ):
         
@@ -150,18 +290,18 @@
 
         return Y_black
 
     # Print the display specification    
     def print( self ):
         Y_black = self.get_black_level()
         
-        logging.info( 'Photometric display model:' )
+        logging.info( 'Photometric display model: {}'.format(self.name) )
         logging.info( '  Peak luminance: {} cd/m^2'.format(self.Y_peak) )
-        logging.info( '  Contrast - theoretical: {}:1'.format( math.round(self.contrast) ) )
-        logging.info( '  Contrast - effective: {}:1'.format, math.round(self.Y_peak/Y_black) )
+        logging.info( '  Contrast - theoretical: {}:1'.format( round(self.contrast) ) )
+        logging.info( '  Contrast - effective: {}:1'.format( round(self.Y_peak/Y_black) ) )
         logging.info( '  Ambient light: {} lux'.format( self.E_ambient ) )
         logging.info( '  Display reflectivity: {}%'.format( self.k_refl*100 ) )
     
 
 class fvvdp_display_photo_absolute(fvvdp_display_photometry):
     # Use this photometric model when passing absolute colorimetric of
     # photometric values, scaled in cd/m^2
@@ -385,16 +525,17 @@
             logging.info( '  Display size: {w:.1f} x {h:.1f} cm'.format( w=self.display_size_m[0]*100, h=self.display_size_m[1]*100) )
             logging.info( '  Display size: {w:.2f} x {h:.2f} deg'.format( w=self.display_size_deg[0], h=self.display_size_deg[1] ) )
             logging.info( '  Viewing distance: {d:.3f} m'.format(d=self.distance_m) )
             logging.info( '  Pixels-per-degree (center): {ppd:.2f}'.format(ppd=self.get_ppd()) )
 
     @classmethod
     def load( cls, display_name ):
-        models_file      = os.path.join(os.path.dirname(__file__), "fvvdp_data/display_models.json")
-        models = json2dict(models_file)
+
+        models_file = utils.config_files.find( "display_models.json" )
+        models = utils.json2dict(models_file)
 
         for mk in models:
             if mk == display_name:
                 model = models[mk]
                 assert "resolution" in model
 
                 inches_to_meters = 0.0254
@@ -411,10 +552,10 @@
                 if   "diagonal_size_meters" in model: diag_size_inch = model["diagonal_size_meters"] / inches_to_meters
                 elif "diagonal_size_inches" in model: diag_size_inch = model["diagonal_size_inches"] 
                 else:                                 diag_size_inch = None
 
                 obj = fvvdp_display_geometry( (W, H), distance_m=distance_m, fov_diagonal=fov_diagonal, diagonal_size_inches=diag_size_inch)
                 return obj
 
-        logging.error("Error: Display model '%s' not found in display_models.json" % display_name)
-        return None
+        raise RuntimeError("Error: Display model '%s' not found in display_models.json" % display_name)
+        #return None
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/fvvdp_test.py` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_test.py`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/hdrvdp_lpyr_dec.py` & `pyfvvdp-1.2.0/pyfvvdp/fvvdp_lpyr_dec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+# Decimated Laplacian Pyramid
 import torch
 import torch.nn.functional as Func
 import numpy as np 
 #import scipy.io as spio
 import os
 import sys
 #import torch.autograd.profiler as profiler
 
 def ceildiv(a, b):
     return -(-a // b)
 
-class hdrvdp_lpyr_dec():
+class fvvdp_lpyr_dec():
 
     def __init__(self, W, H, ppd, device):
         self.device = device
         self.ppd = ppd
         self.min_freq = 0.5
         self.W = W
         self.H = H
@@ -236,14 +237,47 @@
     def interleave_zeros(self, x, dim):
         z = torch.zeros_like(x, device=self.device)
         if dim==2:
             return torch.cat([x,z],dim=3).view(x.shape[0], x.shape[1], 2*x.shape[2],x.shape[3])
         elif dim==3:
             return torch.cat([x.permute(0,1,3,2),z.permute(0,1,3,2)],dim=3).view(x.shape[0], x.shape[1], 2*x.shape[3],x.shape[2]).permute(0,1,3,2)
 
+
+# This pyramid computes and stores contrast during decomposition, improving performance and reducing memory consumption
+class fvvdp_contrast_pyr(fvvdp_lpyr_dec):
+
+    def decompose(self, image):
+        levels = self.height+1
+        kernel_a = 0.4
+        gpyr = self.gaussian_pyramid_dec(image, levels, kernel_a)
+
+        height = len(gpyr)
+        if height == 0:
+            return []
+
+        lpyr = []
+        L_bkg_pyr = []
+        for i in range(height-1):
+            glayer_ex = self.gausspyr_expand(gpyr[i+1], [gpyr[i].shape[-2], gpyr[i].shape[-1]], kernel_a)
+            layer = gpyr[i] - glayer_ex 
+
+            # Order: test-sustained, ref-sustained, test-transient, ref-transient
+            # L_bkg is set to ref-sustained 
+            L_bkg = torch.clamp(glayer_ex[...,1:2,:,:,:], min=0.1)
+            contrast = torch.clamp(torch.div(layer, L_bkg), max=1000.0)
+
+            lpyr.append(contrast)
+            L_bkg_pyr.append(L_bkg)
+
+        lpyr.append(gpyr[height-1]) 
+        
+        return lpyr, L_bkg_pyr
+
+
+
     # def gausspyr_expand(self, x, sz = None, kernel_a = 0.4):
     #     if sz is None:
     #         sz = [x.shape[-2]*2, x.shape[-1]*2]
 
     #     K_vert, K_horiz = self.get_kernels( x, kernel_a )
 
     #     y_a = self.interleave_zeros(x, dim=2)[...,0:sz[0],:]
@@ -279,16 +313,16 @@
 #     # image = torch.cat((image, image, image), axis = -1)
 #     # image = torch.cat((image, image, image), axis = -2)
 
 #     ppd = 50
 
 #     im_tensor = image.view(1, 1, image.shape[-2], image.shape[-1])
 
-#     lp = hdrvdp_lpyr_dec_fast(im_tensor.shape[-2], im_tensor.shape[-1], ppd, device)
-#     lp_old = hdrvdp_lpyr_dec(im_tensor.shape[-2], im_tensor.shape[-1], ppd, device)
+#     lp = fvvdp_lpyr_dec_fast(im_tensor.shape[-2], im_tensor.shape[-1], ppd, device)
+#     lp_old = fvvdp_lpyr_dec(im_tensor.shape[-2], im_tensor.shape[-1], ppd, device)
 
 #     lpyr, gpyr = lp.decompose( im_tensor )
 #     lpyr_2, gpyr_2 = lp_old.decompose( im_tensor )
 
 #     for li in range(lp.get_band_count()):
 #         E = Func.mse_loss(lp.get_band(lpyr, li), lp_old.get_band(lpyr_2, li))
 #         print( "Level {}, MSE={}".format(li, E))
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp/interp.py` & `pyfvvdp-1.2.0/pyfvvdp/interp.py`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/third_party/cpuinfo.py` & `pyfvvdp-1.2.0/pyfvvdp/third_party/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/third_party/loadmat.py` & `pyfvvdp-1.2.0/pyfvvdp/third_party/loadmat.py`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp/visualize_diff_map.py` & `pyfvvdp-1.2.0/pyfvvdp/visualize_diff_map.py`

 * *Files identical despite different names*

### Comparing `pyfvvdp-1.1.3/pyfvvdp.egg-info/PKG-INFO` & `pyfvvdp-1.2.0/pyfvvdp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,191 +1,214 @@
-Metadata-Version: 2.1
-Name: pyfvvdp
-Version: 1.1.3
-Summary: PyTorch code for 'FovVideoVDP': a full-referencevisual quality metric that predicts the perceptualdifference between pairs of images or videos.
-Home-page: https://github.com/gfxdisp/FovVideoVDP
-Author: Rafał K. Mantiuk
-Author-email: mantiuk@gmail.com
-License: Creative Commons Attribution-NonCommercial 4.0 International Public License
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FovVideoVDP: A visible difference predictor for wide field-of-view video
-
-<img src="https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/teaser.png"></img>
-
-FovVideoVDP is a full-reference visual quality metric that predicts the perceptual difference between pairs of images and videos. Similar to popular metrics like PSNR and SSIM, it is aimed at comparing a ground truth reference video against a distorted (e.g. compressed, lower framerate) version.
-
-However, unlike traditional quality metrics, FovVideoVDP works for videos in addition to images, accounts for peripheral acuity, works with SDR and HDR content. We model the response of the human visual system to changes over time as well as across the visual field, so we can predict temporal artifacts like flicker and judder, as well as spatiotemporal artifacts as perceived at different degrees of peripheral vision. Such a metric is important for head-mounted displays as it accounts for both the dynamic content, as well as the large field of view.
-
-FovVideoVDP has both a PyTorch and MATLAB implementations. The usage is described below.
-
-The details of the metric can be found in:
-
-Mantiuk, Rafał K., Gyorgy Denes, Alexandre Chapiro, Anton Kaplanyan, Gizem Rufo, Romain Bachy, Trisha Lian, and Anjul Patney. “FovVideoVDP : A Visible Difference Predictor for Wide Field-of-View Video.” ACM Transaction on Graphics 40, no. 4 (2021): 49. https://doi.org/10.1145/3450626.3459831.
-
-The paper, videos and additional results can be found at the project web page: https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/
-
-If you use the metric in your research, please cite the paper above. 
-
-## PyTorch quickstart
-
-Install with PyPI `pip install pyfvvdp` and run directly from the command line:
-
-```bash
-fvvdp --test test_file --ref ref_file --gpu 0 --display standard_fhd
-```
-The test and reference files can be images or videos. The option `--display` specifies a display on which the content is viewed. See [fvvdp_data/display_models.json](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/fvvdp_data/display_models.json) for the available displays.
-
-Note that the default installation skips the [PyEXR](https://pypi.org/project/PyEXR/) package and uses ImageIO instead. It is recommended to separately install this package since ImageIO's handling of OpenEXR files is unreliable as evidenced [here](https://github.com/imageio/imageio/issues/517). PyEXR is not automatically installed because it depends on the [OpenEXR](https://www.openexr.com/) library, whose installation is operating system specific.
-
-See [Command line interface](#command-line-interface) for further details. FovVideoVDP can be also run directly from Python - see [Low-level Python interface](#low-level-python-interface). 
-
-**Table of contents**
-- [Display specification](#display-specification)
-    - [Custom specification](#custom-specification)
-    - [Reporting metric results](#reporting-metric-results)
-    - [Predicting quality scores](#predicted-quality-scores)
-- [PyTorch](#pytorch)
-    - [Command line interface](#command-line-interface)
-    - [Low-level Python interface](#low-level-python-interface)
-- [MATLAB](#matlab)
-    - [Low-level MATLAB interface](#low-level-matlab-interface)
-- [Differences between MATLAB and PyTorch versions](#differences-between-matlab-and-pytorch-versions)
-- [Release notes](#release-notes)
-
-## Display specification
-
-Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, however, it is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
-
-You specify the display by passing `--display` argument to the PyTorch code, or `display_name` parameter to the MATLAB code. 
-
-Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_hdr` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). 
-
-
-### Custom specification
-
-The display photometry and geometry is typically specified by passing `display_name` parameter to the metric. Alternatively, if you need more flexibility in specifying display geometry (size, fov, viewing distance) and its colorimetry, you can instead pass objects of the classes `fvvdp_display_geometry`, `fvvdp_display_photo_gog` for most SDR displays, and `fvvdp_display_photo_absolute` for HDR displays. You can also create your own subclasses of those classes for custom display specification. 
-
-### Reporting metric results
-
-When reporting the results of the metric, please include the string returned by the metric, such as:
-`"FovVideoVDP v1.1, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
-This is to ensure that you provide enough details to reproduce your results. 
-
-### Predicted quality scores
-
-FovVideoVDP reports image/video quality in the JOD (Just-Objectionable-Difference) units. The highest quality (no difference) is reported as 10 and lower values are reported for distorted content. In case of very strong distortion, or when comparing two unrelated images, the quality value can drop below 0. 
-
-The main advantage of JODs is that they (a) should be linearly related to the perceived magnitude of the distortion and (b) the difference of JODs can be interpreted as the preference prediction across the population. For example, if method A produces a video with the quality score of 8 JOD and method B gives the quality score of 9 JOD, it means that 75% of the population will choose method B over A. The plots below show the mapping from the difference between two conditions in JOD units to the probability of selecting the condition with the higher JOD score (black numbers on the left) and the percentage increase in preference (blue numbers on the right). For more explanation, please refer to Section 3.9 and Fig. 9 in the main paper.
-
-The differences in JOD scores can be converted to the percentage increase in preference (or the probability selecting A over B) using the MATLAB function `fvvdp_preference`.
-
-<table>
-  <tr>
-    <td>Fine JOD scale</td>
-    <td>Coarse JOD scale</td>
-  </tr>
-  <tr>
-    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/fine_jod_scale.png"></img></td>
-    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/coarse_jod_scale.png"></img></td>
-  </tr>
-</table>
-
-## PyTorch
-
-### Command line interface
-The main script to run the model on a set of images or videos is [run_fvvdp.py](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/run_fvvdp.py), from which the binary `fvvdp` is created . Run `fvvdp --help` for detailed usage information.
-
-For the first example, a video was downsampled (4x4) and upsampled (4x4) by different combinations of Bicubic and Nearest filters. To predict quality, you can run:
-
-```bash
-fvvdp --test example_media/aliasing/ferris-*-*.mp4 --ref example_media/aliasing/ferris-ref.mp4 --gpu 0 --display standard_fhd --heatmap supra-threshold
-```
-
-|Original | ![ferris wheel](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-ref.gif) | Quality | Difference map |
-| :---: | :---: | :---: | :---: |
-| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.6277 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
-| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.4803 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
-| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 6.0446 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
-| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.9450 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
-
-### Low-level Python interface
-FovVideoVDP can also be run through the Python interface by instatiating the `pyfvvdp.fvvdp.fvvdp` class. This example shows how to predict the quality of images degraded by Gaussian noise and blur.
-
-```python
-import pyfvvdp
-import ex_utils as utils
-
-I_ref = pyfvvdp.load_image_as_array(os.path.join('example_media', 'wavy_facade.png'))
-fv = pyfvvdp.fvvdp(display_name='standard_4k', heatmap='threshold')
-
-# Gaussian noise with variance 0.003
-I_test_noise = utils.imnoise(I_ref, np.sqrt(0.003))
-Q_JOD_noise, stats_noise = fv.predict( I_test_noise, I_ref, dim_order="HWC" )
-
-# Gaussian blur with sigma=2
-I_test_blur = utils.imgaussblur(I_ref, 2)
-Q_JOD_blur, stats_blur = fv.predict( I_test_blur, I_ref, dim_order="HWC" )
-```
-
-|Original | ![wavy-facade](https://github.com/gfxdisp/FovVideoVDP/raw/main/example_media/wavy_facade.png) | Quality | Difference map |
-| :---: | :---: | :---: | :---: |
-| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.532 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
-| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.674 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
-
-More examples can be found in these [example scripts](https://github.com/gfxdisp/FovVideoVDP/blob/main/pytorch_examples).
-
-
-## MATLAB
-
-MATLAB code for the metric can be found in `matlab/fvvdp.m`. The full documentation of the metric can be shown by typing `doc fvvdp`.
-
-The best starting point is the examples, which can be found in `matlab/examples`. For example, to measure the quality of a noisy image and display the difference map, you can use the code:
-
-```
-I_ref = imread( 'wavy_facade.png' );
-I_test_noise = imnoise( I_ref, 'gaussian', 0, 0.001 );
-
-[Q_JOD_noise, diff_map_noise] = fvvdp( I_test_noise, I_ref, 'display_name', 'standard_phone', 'heatmap', 'threshold' );
-
-clf
-imshow( diff_map_noise );
-
-```
-
-By default, FovVideoVDP will run the code on a GPU using `gpuArray`s, which require functioning CUDA on your computer. If you do not have GPU with CUDA support (e.g. you are on Mac), the code will automatically fallback to the CPU, which will be much slower. 
- 
-### Low-level MATLAB interface
-
-`fvvdp` function is the suitable choice for most cases. But if you need to run metric on large datasets, you can use a low-level function `fvvdp_core`. It requires as input an object of the class `fvvdp_video_source`, which supplies the metric with the frames. Refer to the documentation of that class for further details. 
-
-## Differences between MATLAB and Pytorch versions
-
-* Both versions are implementation of the same metric, but due to differences in the video loaders, you can expect to see small differences in their predictions - typically up to 0.05 JOD.
-* PyTorch version is a bit faster when running on a GPU. 
-
-## Release notes
-
-* v1.1.2 - 23 September 2022
- * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
-
-* v1.1.1 - 28 August 2022
-  * We found a small inconsistency in eccentricity calculations. After fixing this, the metric has been retrained on the same datasets as described in the paper. FovVideoVDP v1.1 will return JOD values that are different than v1.0. For that reason, it is important to mention the version number when reporting the results. 
-  * Python interface has been thoroughly redesigned and make more consistent with Matlab's conterpart. Now it should be much easier to call the metric from Python. 
-  * All Matlab examples have been ported to Python. 
-  * Python version is now faster. 
-  * Published as a PIP repository. 
-
-* v1.0 - 21 April 2021
-  * The original FovVideoVDP release, released with the paper.
-
-The detailed list of changes can be found in [ChangeLog.md](https://github.com/gfxdisp/FovVideoVDP/blob/main/ChangeLog.md).
-
-
+Metadata-Version: 2.1
+Name: pyfvvdp
+Version: 1.2.0
+Summary: PyTorch code for 'FovVideoVDP': a full-referencevisual quality metric that predicts the perceptualdifference between pairs of images or videos.
+Home-page: https://github.com/gfxdisp/FovVideoVDP
+Author: Rafał K. Mantiuk
+Author-email: mantiuk@gmail.com
+License: Creative Commons Attribution-NonCommercial 4.0 International Public License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FovVideoVDP: A visible difference predictor for wide field-of-view video
+
+<img src="https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/teaser.png"></img>
+
+FovVideoVDP is a full-reference visual quality metric that predicts the perceptual difference between pairs of images and videos. Similar to popular metrics like PSNR and SSIM, it is aimed at comparing a ground truth reference video against a distorted (e.g. compressed, lower framerate) version.
+
+However, unlike traditional quality metrics, FovVideoVDP works for videos in addition to images, accounts for peripheral acuity, works with SDR and HDR content. We model the response of the human visual system to changes over time as well as across the visual field, so we can predict temporal artifacts like flicker and judder, as well as spatiotemporal artifacts as perceived at different degrees of peripheral vision. Such a metric is important for head-mounted displays as it accounts for both the dynamic content, as well as the large field of view.
+
+FovVideoVDP has both a PyTorch and MATLAB implementations. The usage is described below.
+
+The details of the metric can be found in:
+
+Mantiuk, Rafał K., Gyorgy Denes, Alexandre Chapiro, Anton Kaplanyan, Gizem Rufo, Romain Bachy, Trisha Lian, and Anjul Patney. “FovVideoVDP : A Visible Difference Predictor for Wide Field-of-View Video.” ACM Transaction on Graphics 40, no. 4 (2021): 49. https://doi.org/10.1145/3450626.3459831.
+
+The paper, videos and additional results can be found at the project web page: https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/
+
+If you use the metric in your research, please cite the paper above. 
+
+## PyTorch quickstart
+
+Start by installing the right version of PyTorch (with CUDA if supported) by following [these instructions](https://pytorch.org/get-started/locally/). Then, install pyfvvdp with PyPI `pip install pyfvvdp` or Anaconda `conda install -c gfxdisp -c conda-forge pyfvvdp`. You can run `fvvdp` directly from the command line:
+
+```bash
+fvvdp --test test_file --ref ref_file --display standard_fhd
+```
+The test and reference files can be images or videos. The option `--display` specifies a display on which the content is viewed. See [fvvdp_data/display_models.json](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/fvvdp_data/display_models.json) for the available displays.
+
+Note that the default installation skips the [PyEXR](https://pypi.org/project/PyEXR/) package and uses ImageIO instead. It is recommended to separately install this package since ImageIO's handling of OpenEXR files is unreliable as evidenced [here](https://github.com/imageio/imageio/issues/517). PyEXR is not automatically installed because it depends on the [OpenEXR](https://www.openexr.com/) library, whose installation is operating system specific.
+
+See [Command line interface](#command-line-interface) for further details. FovVideoVDP can be also run directly from Python - see [Low-level Python interface](#low-level-python-interface). 
+
+**Table of contents**
+- [Display specification](#display-specification)
+    - [Custom specification](#custom-specification)
+    - [HDR content](#HDR-content)
+    - [Reporting metric results](#reporting-metric-results)
+    - [Predicting quality scores](#predicted-quality-scores)
+- [PyTorch](#pytorch)
+    - [Command line interface](#command-line-interface)
+    - [Low-level Python interface](#low-level-python-interface)
+- [MATLAB](#matlab)
+    - [Low-level MATLAB interface](#low-level-matlab-interface)
+- [Differences between MATLAB and PyTorch versions](#differences-between-matlab-and-pytorch-versions)
+- [Release notes](#release-notes)
+
+## Display specification
+
+Unlike most image quality metrics, FovVideoVDP needs physical specification of the display (e.g. its size, resolution, peak brightness) and viewing conditions (viewing distance, ambient light) to compute accurate predictions. The specifications of the displays are stored in `fvvdp_data/display_models.json`. You can add the exact specification of your display to this file, or create a new JSON file and pass the directory it is located in as `--config-dir` parameter (`fvvdp` command). If the display specification is unknown to you, you are encouraged to use one of the standard display specifications listed on the top of that file, for example `standard_4k`, or `standard_fhd`. If you use one of the standard displays, there is a better chance that your results will be comparable with other studies. 
+
+You specify the display by passing `--display` argument to the PyTorch code, or `display_name` parameter to the MATLAB code. 
+
+Note the the specification in `display_models.json` is for the display and not the image. If you select to use `standard_4k` with the resolution of 3840x2160 for your display and pass a 1920x1080 image, the metric will assume that the image occupies one quarter of that display (the central portion). If you want to enlarge the image to the full resolution of the display, pass `--full-screen-resize {fast_bilinear,bilinear,bicubic,lanczos}` option (now works with video only). 
+
+The command line version of FovVideoVDP can take as input HDR video streams encoded using the PQ transfer function (from version 1.1.4). To correctly model HDR content, it is necessary to pass a display model with `EOTF="PQ"`, for example `standard_hdr`.
+
+### Custom specification
+
+The display photometry and geometry is typically specified by passing `display_name` parameter to the metric. Alternatively, if you need more flexibility in specifying display geometry (size, fov, viewing distance) and its colorimetry, you can instead pass objects of the classes `fvvdp_display_geometry`, `fvvdp_display_photo_gog` for most SDR displays, and `fvvdp_display_photo_absolute` for HDR displays. You can also create your own subclasses of those classes for custom display specification. 
+
+### HDR content
+
+(Python command line only) You can use the metric to compare: 
+
+* HDR video files encoded using PQ EOTF function (SMPTE ST 2084). Pass the video files as `--test` and `--ref` arguments and specify `--display standard_hdr_pq`.
+
+* OpenEXR images. The images *MUST* contain absolute linear colour values (colour graded values, emitted from the display). That is, if the disply peak luminance is 1000, RGB=(1000,1000,1000) corresponds to the maximum value emitted from the display. If you pass images with the maximum value of 1, the metric will assume that the images are very dark (the peak of 1 nit) and result in incorerect predictrions. You need to specify `--display standard_hdr_linear` to use correct EOTF.
+
+### Reporting metric results
+
+When reporting the results of the metric, please include the string returned by the metric, such as:
+`"FovVideoVDP v1.2.0, 75.4 [pix/deg], Lpeak=200, Lblack=0.5979 [cd/m^2], non-foveated, (standard_4k)"`
+This is to ensure that you provide enough details to reproduce your results. 
+
+### Predicted quality scores
+
+FovVideoVDP reports image/video quality in the JOD (Just-Objectionable-Difference) units. The highest quality (no difference) is reported as 10 and lower values are reported for distorted content. In case of very strong distortion, or when comparing two unrelated images, the quality value can drop below 0. 
+
+The main advantage of JODs is that they (a) should be linearly related to the perceived magnitude of the distortion and (b) the difference of JODs can be interpreted as the preference prediction across the population. For example, if method A produces a video with the quality score of 8 JOD and method B gives the quality score of 9 JOD, it means that 75% of the population will choose method B over A. The plots below show the mapping from the difference between two conditions in JOD units to the probability of selecting the condition with the higher JOD score (black numbers on the left) and the percentage increase in preference (blue numbers on the right). For more explanation, please refer to Section 3.9 and Fig. 9 in the main paper.
+
+The differences in JOD scores can be converted to the percentage increase in preference (or the probability selecting A over B) using the MATLAB function `fvvdp_preference`.
+
+<table>
+  <tr>
+    <td>Fine JOD scale</td>
+    <td>Coarse JOD scale</td>
+  </tr>
+  <tr>
+    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/fine_jod_scale.png"></img></td>
+    <td><img width="512" src="https://github.com/gfxdisp/FovVideoVDP/raw/webpage/imgs/coarse_jod_scale.png"></img></td>
+  </tr>
+</table>
+
+## PyTorch
+
+### Command line interface
+The main script to run the model on a set of images or videos is [run_fvvdp.py](https://github.com/gfxdisp/FovVideoVDP/blob/main/pyfvvdp/run_fvvdp.py), from which the binary `fvvdp` is created . Run `fvvdp --help` for detailed usage information.
+
+For the first example, a video was downsampled (4x4) and upsampled (4x4) by different combinations of Bicubic and Nearest filters. To predict quality, you can run:
+
+```bash
+fvvdp --test example_media/aliasing/ferris-*-*.mp4 --ref example_media/aliasing/ferris-ref.mp4 --gpu 0 --display standard_fhd --heatmap supra-threshold
+```
+
+|Original | ![ferris wheel](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-ref.gif) | Quality | Difference map |
+| :---: | :---: | :---: | :---: |
+| Bicubic &#8595;<br />Bicubic &#8593;<br />(4x4) | ![bicubic-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-bicubic.gif) | 6.469 | ![bicubic-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-bicubic_diff_map_viz.gif) |
+| Bicubic &#8595;<br />Nearest &#8593;<br />(4x4) | ![bicubic-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-bicubic-nearest.gif) | 6.328 | ![bicubic-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-bicubic-nearest_diff_map_viz.gif) |
+| Nearest &#8595;<br />Bicubic &#8593;<br />(4x4) | ![nearest-bicubic](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-bicubic.gif) | 5.923 | ![nearest-bicubic-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-bicubic_diff_map_viz.gif) |
+| Nearest &#8595;<br />Nearest &#8593;<br />(4x4) | ![nearest-nearest](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/ferris-nearest-nearest.gif) | 5.821 | ![nearest-nearest-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/aliasing/diff_maps/ferris-nearest-nearest_diff_map_viz.gif) |
+
+
+### Low-level Python interface
+FovVideoVDP can also be run through the Python interface by instatiating the `pyfvvdp.fvvdp.fvvdp` class. This example shows how to predict the quality of images degraded by Gaussian noise and blur.
+
+```python
+import os
+import numpy as np
+import pyfvvdp
+import ex_utils as utils
+
+I_ref = pyfvvdp.load_image_as_array(os.path.join('example_media', 'wavy_facade.png'))
+fv = pyfvvdp.fvvdp(display_name='standard_4k', heatmap='threshold')
+
+# Gaussian noise with variance 0.003
+I_test_noise = utils.imnoise(I_ref, np.sqrt(0.003))
+Q_JOD_noise, stats_noise = fv.predict( I_test_noise, I_ref, dim_order="HWC" )
+
+# Gaussian blur with sigma=2
+I_test_blur = utils.imgaussblur(I_ref, 2)
+Q_JOD_blur, stats_blur = fv.predict( I_test_blur, I_ref, dim_order="HWC" )
+```
+
+|Original | ![wavy-facade](https://github.com/gfxdisp/FovVideoVDP/raw/main/example_media/wavy_facade.png) | Quality | Difference map |
+| :---: | :---: | :---: | :---: |
+| Gaussian noise (σ<sup>2</sup> = 0.003) | ![noise](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise.png) | 9.537 | ![noise-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_noise_diff_map_viz.png) |
+| Gaussian blur (σ = 2) | ![blur](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur.png) | 8.693 | ![blur-diff](https://www.cl.cam.ac.uk/research/rainbow/projects/fovvideovdp/html_reports/github_examples/simple_image/wavy_facade_blur_diff_map_viz.png) |
+
+More examples can be found in these [example scripts](https://github.com/gfxdisp/FovVideoVDP/blob/main/pytorch_examples).
+
+
+## MATLAB
+
+MATLAB code for the metric can be found in `matlab/fvvdp.m`. The full documentation of the metric can be shown by typing `doc fvvdp`.
+
+The best starting point is the examples, which can be found in `matlab/examples`. For example, to measure the quality of a noisy image and display the difference map, you can use the code:
+
+```
+I_ref = imread( 'wavy_facade.png' );
+I_test_noise = imnoise( I_ref, 'gaussian', 0, 0.001 );
+
+[Q_JOD_noise, diff_map_noise] = fvvdp( I_test_noise, I_ref, 'display_name', 'standard_phone', 'heatmap', 'threshold' );
+
+clf
+imshow( diff_map_noise );
+
+```
+
+By default, FovVideoVDP will run the code on a GPU using `gpuArray`s, which require functioning CUDA on your computer. If you do not have GPU with CUDA support (e.g. you are on Mac), the code will automatically fallback to the CPU, which will be much slower. 
+ 
+### Low-level MATLAB interface
+
+`fvvdp` function is the suitable choice for most cases. But if you need to run metric on large datasets, you can use a low-level function `fvvdp_core`. It requires as input an object of the class `fvvdp_video_source`, which supplies the metric with the frames. Refer to the documentation of that class for further details. 
+
+## Differences between MATLAB and Pytorch versions
+
+* Both versions are implementation of the same metric, but due to differences in the video loaders, you can expect to see small differences in their predictions - typically up to 0.05 JOD.
+* PyTorch version is a bit faster when running on a GPU. 
+
+## Release notes
+
+* v1.2.0 - 19 April 2023
+  * The python command line interface can now accept HDR video files and OpenEXR images. 
+  * [PU21-PSNR](https://github.com/gfxdisp/pu21) can be run in addition to FovVideoVDP
+  * Added new command line options: `--full-screen-resize`, `--metrics`, `--temp-padding`, `--feature`, `--output-dir`
+  * Faster decoding for large (4k) videos when run on CUDA (python, the command line interface `fvvdp`). 
+  * The prediction may differ slightly because of the way video files are handled and processed. There are no changes in the metric.
+  * Fixed issue when reading video frames in python freezed on some platforms (issue with python's `/dev/null` redirection)
+
+* v1.1.3 - 18 October 2022
+  * Added "raw" heatmap type to the command line. 
+  * Changed the way pyfvvdp classes are imported  to avoid clash between the file and class names (see updated pytortch_examples)
+  * Installation of PyEXR is now optional (caused problems on some operating systems).
+
+* v1.1.2 - 23 September 2022
+  * Updated Python dependencies - now works with earlier versions of PyTorch, Numpy and SciPy
+
+* v1.1.1 - 28 August 2022
+  * We found a small inconsistency in eccentricity calculations. After fixing this, the metric has been retrained on the same datasets as described in the paper. FovVideoVDP v1.1 will return JOD values that are different than v1.0. For that reason, it is important to mention the version number when reporting the results. 
+  * Python interface has been thoroughly redesigned and make more consistent with Matlab's conterpart. Now it should be much easier to call the metric from Python. 
+  * All Matlab examples have been ported to Python. 
+  * Python version is now faster. 
+  * Published as a PIP repository. 
+
+* v1.0 - 21 April 2021
+  * The original FovVideoVDP release, released with the paper.
+
+The detailed list of changes can be found in [ChangeLog.md](https://github.com/gfxdisp/FovVideoVDP/blob/main/ChangeLog.md).
```

### Comparing `pyfvvdp-1.1.3/pyfvvdp.egg-info/SOURCES.txt` & `pyfvvdp-1.2.0/pyfvvdp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 LICENSE
 README.md
 setup.py
 pyfvvdp/__init__.py
 pyfvvdp/fvvdp.py
 pyfvvdp/fvvdp_display_model.py
+pyfvvdp/fvvdp_lpyr_dec.py
 pyfvvdp/fvvdp_test.py
-pyfvvdp/hdrvdp_lpyr_dec.py
 pyfvvdp/interp.py
+pyfvvdp/pupsnr.py
 pyfvvdp/run_fvvdp.py
 pyfvvdp/utils.py
+pyfvvdp/video_source.py
 pyfvvdp/video_source_file.py
+pyfvvdp/video_source_yuv.py
 pyfvvdp/visualize_diff_map.py
 pyfvvdp.egg-info/PKG-INFO
 pyfvvdp.egg-info/SOURCES.txt
 pyfvvdp.egg-info/dependency_links.txt
 pyfvvdp.egg-info/entry_points.txt
 pyfvvdp.egg-info/requires.txt
 pyfvvdp.egg-info/top_level.txt
-pyfvvdp/third_party/__init__.py
-pyfvvdp/third_party/cpuinfo.py
-pyfvvdp/third_party/loadmat.py
 pyfvvdp/csf_cache/o0_sn1_5_cm0_604562_gpu0.mat
 pyfvvdp/csf_cache/o5_sn1_5_cm0_604562_gpu0.mat
 pyfvvdp/fvvdp_data/color_spaces.json
 pyfvvdp/fvvdp_data/display_models.json
 pyfvvdp/fvvdp_data/fvvdp_parameters.json
 pyfvvdp/fvvdp_data/fvvdp_parameters_1_0.json
 pyfvvdp/third_party/__init__.py
```

### Comparing `pyfvvdp-1.1.3/setup.py` & `pyfvvdp-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name='pyfvvdp',
-    version='1.1.3',
+    version='1.2.0',
     description='PyTorch code for \'FovVideoVDP\': a full-reference' \
                 'visual quality metric that predicts the perceptual' \
                 'difference between pairs of images or videos.',
     long_description=long_description,
     url='https://github.com/gfxdisp/FovVideoVDP',
     long_description_content_type='text/markdown',
     author='Rafał K. Mantiuk',
```

