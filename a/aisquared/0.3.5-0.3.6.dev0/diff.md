# Comparing `tmp/aisquared-0.3.5.tar.gz` & `tmp/aisquared-0.3.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisquared-0.3.5.tar", last modified: Fri Mar 24 17:21:28 2023, max compression
+gzip compressed data, was "aisquared-0.3.6.dev0.tar", last modified: Wed Apr 19 16:49:30 2023, max compression
```

## Comparing `aisquared-0.3.5.tar` & `aisquared-0.3.6.dev0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.522411 aisquared-0.3.5/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19124 2023-03-24 17:21:28.522195 aisquared-0.3.5/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)    18805 2023-03-24 17:10:38.000000 aisquared-0.3.5/README.md
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.508255 aisquared-0.3.5/aisquared/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      478 2023-03-24 17:10:38.000000 aisquared-0.3.5/aisquared/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.510738 aisquared-0.3.5/aisquared/base/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/base/BaseObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      756 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/base/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4473 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/base/css.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/base/endpoints.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.5/aisquared/base/harvesting.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/base/platform.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.5/aisquared/base/preprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/base/rendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/base/stages.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.511447 aisquared-0.3.5/aisquared/config/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/CustomObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8938 2023-03-24 17:10:38.000000 aisquared-0.3.5/aisquared/config/GraphConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    21223 2023-03-24 17:10:38.000000 aisquared-0.3.5/aisquared/config/ModelConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.512294 aisquared-0.3.5/aisquared/config/analytic/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2189 2023-02-20 17:59:37.000000 aisquared-0.3.5/aisquared/config/analytic/DeployedAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/analytic/DeployedModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.5/aisquared/config/analytic/LocalAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/analytic/LocalModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3519 2023-03-24 17:10:38.000000 aisquared-0.3.5/aisquared/config/analytic/ReverseMLWorkflow.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.5/aisquared/config/analytic/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.513189 aisquared-0.3.5/aisquared/config/feedback/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/BinaryFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/ModelFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/MulticlassFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/QualitativeFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/RegressionFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/SimpleFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/feedback/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.513817 aisquared-0.3.5/aisquared/config/harvesting/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/harvesting/ImageHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/harvesting/InputHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/harvesting/QueryParameterHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/harvesting/TextHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/harvesting/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.514446 aisquared-0.3.5/aisquared/config/postprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/postprocessing/BinaryClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/postprocessing/MulticlassClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/postprocessing/ObjectDetection.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/postprocessing/Regression.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/postprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.514599 aisquared-0.3.5/aisquared/config/preprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.515029 aisquared-0.3.5/aisquared/config/preprocessing/image/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/image/ImagePreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/image/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/image/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.515471 aisquared-0.3.5/aisquared/config/preprocessing/tabular/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/tabular/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/tabular/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.515858 aisquared-0.3.5/aisquared/config/preprocessing/text/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/preprocessing/text/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/text/TextPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/preprocessing/text/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.518274 aisquared-0.3.5/aisquared/config/rendering/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4554 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/BarChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/rendering/ContainerRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/DashboardRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/rendering/DashboardReplacementRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/rendering/DocumentRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4524 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/DoughnutChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/rendering/FilterRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/rendering/HTMLTagRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/ImageRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4506 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/LineChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/ObjectRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4539 2023-02-10 15:11:26.000000 aisquared-0.3.5/aisquared/config/rendering/PieChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/rendering/SOSRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/rendering/TableRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4377 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/config/rendering/WordRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/rendering/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      562 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/config/rendering/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.518401 aisquared-0.3.5/aisquared/logging/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/logging/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.519764 aisquared-0.3.5/aisquared/platform/
--rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/AISquaredAPIException.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/AISquaredPlatformClient.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/NoResultsFoundError.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/platform/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/additional_utils.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/crudl.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/metrics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/sharing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/platform/user_group.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.520160 aisquared-0.3.5/aisquared/serving/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/serving/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-02-24 19:53:35.000000 aisquared-0.3.5/aisquared/serving/deploy_model.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/serving/get_remote_prediction.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.520458 aisquared-0.3.5/aisquared/utils/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.5/aisquared/utils/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.5/aisquared/utils/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.508991 aisquared-0.3.5/aisquared.egg-info/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19124 2023-03-24 17:21:28.000000 aisquared-0.3.5/aisquared.egg-info/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-03-24 17:21:28.000000 aisquared-0.3.5/aisquared.egg-info/SOURCES.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-03-24 17:21:28.000000 aisquared-0.3.5/aisquared.egg-info/dependency_links.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)      109 2023-03-24 17:21:28.000000 aisquared-0.3.5/aisquared.egg-info/requires.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-03-24 17:21:28.000000 aisquared-0.3.5/aisquared.egg-info/top_level.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-03-24 17:21:28.522454 aisquared-0.3.5/setup.cfg
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.5/setup.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-03-24 17:21:28.521976 aisquared-0.3.5/tests/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_air.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      853 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_analytics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_base.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.5/tests/test_custom.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_harvesters.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_postprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_preprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    21527 2023-03-09 19:06:33.000000 aisquared-0.3.5/tests/test_renderers.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.5/tests/test_simple.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.488554 aisquared-0.3.6.dev0/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19223 2023-04-19 16:49:30.488266 aisquared-0.3.6.dev0/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    18899 2023-04-19 16:47:20.000000 aisquared-0.3.6.dev0/README.md
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.456450 aisquared-0.3.6.dev0/aisquared/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-04-19 16:46:40.000000 aisquared-0.3.6.dev0/aisquared/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.461121 aisquared-0.3.6.dev0/aisquared/base/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/base/BaseObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      756 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4473 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/css.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/endpoints.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/aisquared/base/harvesting.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/platform.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/aisquared/base/preprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/base/rendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/base/stages.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.462615 aisquared-0.3.6.dev0/aisquared/config/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/CustomObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8935 2023-04-19 16:44:10.000000 aisquared-0.3.6.dev0/aisquared/config/GraphConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    21226 2023-04-19 16:46:21.000000 aisquared-0.3.6.dev0/aisquared/config/ModelConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.464625 aisquared-0.3.6.dev0/aisquared/config/analytic/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2189 2023-02-20 17:59:37.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/LocalAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/LocalModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3519 2023-03-24 17:10:38.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/ReverseMLWorkflow.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.466691 aisquared-0.3.6.dev0/aisquared/config/feedback/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/BinaryFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/ModelFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/MulticlassFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/QualitativeFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/RegressionFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/SimpleFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.468124 aisquared-0.3.6.dev0/aisquared/config/harvesting/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/ImageHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/InputHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/QueryParameterHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/TextHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.469628 aisquared-0.3.6.dev0/aisquared/config/postprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/BinaryClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/MulticlassClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/ObjectDetection.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/Regression.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.469923 aisquared-0.3.6.dev0/aisquared/config/preprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.470930 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.471869 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.472916 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.478709 aisquared-0.3.6.dev0/aisquared/config/rendering/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4554 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/BarChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ContainerRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardReplacementRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DocumentRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4524 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DoughnutChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/FilterRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/HTMLTagRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ImageRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4506 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/LineChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ObjectRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4539 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/PieChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/SOSRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/TableRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4377 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/WordRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      562 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.479072 aisquared-0.3.6.dev0/aisquared/logging/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/logging/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.482609 aisquared-0.3.6.dev0/aisquared/platform/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/AISquaredAPIException.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/AISquaredPlatformClient.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/NoResultsFoundError.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/platform/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/additional_utils.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/crudl.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/metrics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/sharing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/user_group.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.483668 aisquared-0.3.6.dev0/aisquared/serving/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/serving/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.6.dev0/aisquared/serving/deploy_model.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/serving/get_remote_prediction.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.484337 aisquared-0.3.6.dev0/aisquared/utils/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/utils/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/utils/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.457567 aisquared-0.3.6.dev0/aisquared.egg-info/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19223 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/SOURCES.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/dependency_links.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      109 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/requires.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/top_level.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-04-19 16:49:30.488643 aisquared-0.3.6.dev0/setup.cfg
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/setup.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.487880 aisquared-0.3.6.dev0/tests/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_air.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      853 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_analytics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_base.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/tests/test_custom.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_harvesters.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_postprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_preprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    21527 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/tests/test_renderers.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_simple.py
```

### Comparing `aisquared-0.3.5/PKG-INFO` & `aisquared-0.3.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.5
+Version: 0.3.6.dev0
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -324,7 +324,10 @@
 - Moved `CustomObject` to `aisquared.config` from `aisquared.base`
 - Changed endpoint used to list platform users
 - Fixed response behaviors where no data was returned from `AISquaredPlatformClient`
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
+
+## Version 0.3.6
+- Fixed issue with type checking for `ModelConfiguration` Rendering classes
```

### Comparing `aisquared-0.3.5/README.md` & `aisquared-0.3.6.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -313,7 +313,10 @@
 - Moved `CustomObject` to `aisquared.config` from `aisquared.base`
 - Changed endpoint used to list platform users
 - Fixed response behaviors where no data was returned from `AISquaredPlatformClient`
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
+
+## Version 0.3.6
+- Fixed issue with type checking for `ModelConfiguration` Rendering classes
```

### Comparing `aisquared-0.3.5/aisquared/base/BaseObject.py` & `aisquared-0.3.6.dev0/aisquared/base/BaseObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/base/__init__.py` & `aisquared-0.3.6.dev0/aisquared/base/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/base/css.py` & `aisquared-0.3.6.dev0/aisquared/base/css.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/base/endpoints.py` & `aisquared-0.3.6.dev0/aisquared/base/endpoints.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/base/rendering.py` & `aisquared-0.3.6.dev0/aisquared/base/rendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/CustomObject.py` & `aisquared-0.3.6.dev0/aisquared/config/CustomObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/GraphConfiguration.py` & `aisquared-0.3.6.dev0/aisquared/config/GraphConfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 from aisquared.base import BaseObject, ALLOWED_STAGES
-from aisquared.config import CustomObject
+from .CustomObject import CustomObject
 import tensorflowjs as tfjs
 import tensorflow as tf
 import shutil
 import json
 import os
 
 LOCAL_CLASSES = ['LocalModel', 'LocalAnalytic', 'CustomObject']
```

### Comparing `aisquared-0.3.5/aisquared/config/ModelConfiguration.py` & `aisquared-0.3.6.dev0/aisquared/config/ModelConfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Union
 from aisquared.base import BaseObject, ALLOWED_STAGES
-from aisquared.config import CustomObject
+from .CustomObject import CustomObject
 from aisquared.config.harvesting import ImageHarvester, TextHarvester, InputHarvester, QueryParameterHarvester
 from aisquared.config.preprocessing.tabular import TabularPreprocessor
 from aisquared.config.preprocessing.image import ImagePreprocessor
 from aisquared.config.preprocessing.text import TextPreprocessor
 from aisquared.config.analytic import DeployedAnalytic, DeployedModel, LocalModel, LocalAnalytic, ReverseMLWorkflow
 from aisquared.config.postprocessing import BinaryClassification, MulticlassClassification, ObjectDetection, Regression
-from aisquared.config.rendering import ImageRendering, ObjectRendering, DocumentRendering, WordRendering, FilterRendering, ContainerRendering, HTMLTagRendering, DoughnutChartRendering, TableRendering, BarChartRendering, LineChartRendering, DashboardReplacementRendering, PieChartRendering, SOSRendering, DashboardRendering
+from aisquared.config.rendering import ImageRendering, ObjectRendering, DocumentRendering, WordRendering, FilterRendering, ContainerRendering, HTMLTagRendering, DoughnutChartRendering, TableRendering, BarChartRendering, LineChartRendering, DashboardReplacementRendering, PieChartRendering, SOSRendering  # , DashboardRendering
 from aisquared.config.feedback import SimpleFeedback, BinaryFeedback, MulticlassFeedback, RegressionFeedback, ModelFeedback, QualitativeFeedback
 
 import tensorflowjs as tfjs
 import tensorflow as tf
 import shutil
 import json
 import os
@@ -60,15 +60,15 @@
     TableRendering,
     BarChartRendering,
     LineChartRendering,
     DashboardReplacementRendering,
     PieChartRendering,
     SOSRendering,
     CustomObject,
-    DashboardRendering
+    # DashboardRendering
 )
 
 FEEDBACK_CLASSES = (
     ModelFeedback,
     SimpleFeedback,
     BinaryFeedback,
     MulticlassFeedback,
```

### Comparing `aisquared-0.3.5/aisquared/config/analytic/DeployedAnalytic.py` & `aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/analytic/DeployedModel.py` & `aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/analytic/LocalAnalytic.py` & `aisquared-0.3.6.dev0/aisquared/config/analytic/LocalAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/analytic/LocalModel.py` & `aisquared-0.3.6.dev0/aisquared/config/analytic/LocalModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/analytic/ReverseMLWorkflow.py` & `aisquared-0.3.6.dev0/aisquared/config/analytic/ReverseMLWorkflow.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/BinaryFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/BinaryFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/ModelFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/ModelFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/MulticlassFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/MulticlassFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/QualitativeFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/QualitativeFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/RegressionFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/RegressionFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/feedback/SimpleFeedback.py` & `aisquared-0.3.6.dev0/aisquared/config/feedback/SimpleFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/harvesting/ImageHarvester.py` & `aisquared-0.3.6.dev0/aisquared/config/harvesting/ImageHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/harvesting/InputHarvester.py` & `aisquared-0.3.6.dev0/aisquared/config/harvesting/InputHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/harvesting/QueryParameterHarvester.py` & `aisquared-0.3.6.dev0/aisquared/config/harvesting/QueryParameterHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/harvesting/TextHarvester.py` & `aisquared-0.3.6.dev0/aisquared/config/harvesting/TextHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/postprocessing/BinaryClassification.py` & `aisquared-0.3.6.dev0/aisquared/config/postprocessing/BinaryClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/postprocessing/MulticlassClassification.py` & `aisquared-0.3.6.dev0/aisquared/config/postprocessing/MulticlassClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/postprocessing/ObjectDetection.py` & `aisquared-0.3.6.dev0/aisquared/config/postprocessing/ObjectDetection.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/postprocessing/Regression.py` & `aisquared-0.3.6.dev0/aisquared/config/postprocessing/Regression.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/image/ImagePreprocessing.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/image/Steps.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/tabular/Steps.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/tabular/TabularPreprocessing.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/text/Steps.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/preprocessing/text/TextPreprocessing.py` & `aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/BarChartRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/BarChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/ContainerRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/ContainerRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/DashboardRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/DashboardReplacementRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardReplacementRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/DocumentRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/DocumentRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/DoughnutChartRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/DoughnutChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/FilterRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/FilterRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/HTMLTagRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/HTMLTagRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/ImageRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/ImageRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/LineChartRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/LineChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/ObjectRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/ObjectRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/PieChartRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/PieChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/SOSRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/SOSRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/TableRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/TableRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/WordRendering.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/WordRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/__init__.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/config/rendering/utils.py` & `aisquared-0.3.6.dev0/aisquared/config/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/AISquaredPlatformClient.py` & `aisquared-0.3.6.dev0/aisquared/platform/AISquaredPlatformClient.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/additional_utils.py` & `aisquared-0.3.6.dev0/aisquared/platform/additional_utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/crudl.py` & `aisquared-0.3.6.dev0/aisquared/platform/crudl.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/feedback.py` & `aisquared-0.3.6.dev0/aisquared/platform/feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/metrics.py` & `aisquared-0.3.6.dev0/aisquared/platform/metrics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/sharing.py` & `aisquared-0.3.6.dev0/aisquared/platform/sharing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/platform/user_group.py` & `aisquared-0.3.6.dev0/aisquared/platform/user_group.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/serving/__init__.py` & `aisquared-0.3.6.dev0/aisquared/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/serving/deploy_model.py` & `aisquared-0.3.6.dev0/aisquared/serving/deploy_model.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/serving/get_remote_prediction.py` & `aisquared-0.3.6.dev0/aisquared/serving/get_remote_prediction.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared/utils/utils.py` & `aisquared-0.3.6.dev0/aisquared/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/aisquared.egg-info/PKG-INFO` & `aisquared-0.3.6.dev0/aisquared.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.5
+Version: 0.3.6.dev0
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -324,7 +324,10 @@
 - Moved `CustomObject` to `aisquared.config` from `aisquared.base`
 - Changed endpoint used to list platform users
 - Fixed response behaviors where no data was returned from `AISquaredPlatformClient`
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
+
+## Version 0.3.6
+- Fixed issue with type checking for `ModelConfiguration` Rendering classes
```

### Comparing `aisquared-0.3.5/aisquared.egg-info/SOURCES.txt` & `aisquared-0.3.6.dev0/aisquared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/setup.py` & `aisquared-0.3.6.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_air.py` & `aisquared-0.3.6.dev0/tests/test_air.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_analytics.py` & `aisquared-0.3.6.dev0/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_base.py` & `aisquared-0.3.6.dev0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_feedback.py` & `aisquared-0.3.6.dev0/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_harvesters.py` & `aisquared-0.3.6.dev0/tests/test_harvesters.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_postprocessors.py` & `aisquared-0.3.6.dev0/tests/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_preprocessors.py` & `aisquared-0.3.6.dev0/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.5/tests/test_renderers.py` & `aisquared-0.3.6.dev0/tests/test_renderers.py`

 * *Files identical despite different names*

