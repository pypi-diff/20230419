# Comparing `tmp/rubicon-ml-0.4.3.tar.gz` & `tmp/rubicon-ml-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-ml-0.4.3.tar", last modified: Wed Dec 14 16:11:45 2022, max compression
+gzip compressed data, was "rubicon-ml-0.4.4.tar", last modified: Wed Apr 19 18:45:21 2023, max compression
```

## Comparing `rubicon-ml-0.4.3.tar` & `rubicon-ml-0.4.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2022-12-14 16:11:45.844027 rubicon-ml-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.844027 rubicon-ml-0.4.3/rubicon_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-14 16:11:45.844027 rubicon-ml-0.4.3/rubicon_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.836027 rubicon-ml-0.4.3/rubicon_ml/client/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/rubicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.836027 rubicon-ml-0.4.3/rubicon_ml/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/utils/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/client/utils/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.836027 rubicon-ml-0.4.3/rubicon_ml/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.836027 rubicon-ml-0.4.3/rubicon_ml/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/utils/training_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/domain/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38793 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/repository/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/repository/utils/slugify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/sklearn/estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/sklearn/filter_estimator_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/sklearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.832027 rubicon-ml-0.4.3/rubicon_ml/viz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/dropdown-header.css
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/experiments-table.css
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/frame.css
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/metric-correlation-plot.css
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/metric-lists-comparison.css
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/css/plots-comparison.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/viz/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/viz/common/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/common/dropdown_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/dataframe_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/experiments_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/metric_correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/viz/metric_lists_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/rubicon_ml/workflow/prefect/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/workflow/prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/rubicon_ml/workflow/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.836027 rubicon-ml-0.4.3/rubicon_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-14 16:11:45.000000 rubicon-ml-0.4.3/rubicon_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2022-12-14 16:11:45.844027 rubicon-ml-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:45.840027 rubicon-ml-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2022-12-14 16:11:36.000000 rubicon-ml-0.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/rubicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/client/utils/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/training_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/domain/utils/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/repository/utils/slugify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/filter_estimator_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/sklearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/dropdown-header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/experiments-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/frame.css
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/metric-correlation-plot.css
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/metric-lists-comparison.css
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/css/plots-comparison.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/rubicon-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.213481 rubicon-ml-0.4.4/rubicon_ml/viz/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/common/dropdown_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/dataframe_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/experiments_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/metric_correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/viz/metric_lists_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.209481 rubicon-ml-0.4.4/rubicon_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 18:45:21.000000 rubicon-ml-0.4.4/rubicon_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:21.217481 rubicon-ml-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-19 18:45:10.000000 rubicon-ml-0.4.4/versioneer.py
```

### Comparing `rubicon-ml-0.4.3/LICENSE` & `rubicon-ml-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/PKG-INFO` & `rubicon-ml-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.3
+Version: 0.4.4
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.3/README.md` & `rubicon-ml-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/__init__.py` & `rubicon-ml-0.4.4/rubicon_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/cli.py` & `rubicon-ml-0.4.4/rubicon_ml/cli.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/__init__.py` & `rubicon-ml-0.4.4/rubicon_ml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/artifact.py` & `rubicon-ml-0.4.4/rubicon_ml/client/artifact.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/base.py` & `rubicon-ml-0.4.4/rubicon_ml/client/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/config.py` & `rubicon-ml-0.4.4/rubicon_ml/client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def _load_config(self, persistence, root_dir, is_auto_git_enabled):
         """Get the configuration values."""
         persistence = os.environ.get("PERSISTENCE", persistence)
         if persistence not in self.PERSISTENCE_TYPES:
             raise ValueError(f"PERSISTENCE must be one of {self.PERSISTENCE_TYPES}.")
 
         root_dir = os.environ.get("ROOT_DIR", root_dir)
-        if root_dir is None and persistence != "memory":
+        if root_dir is None and persistence == "filesystem":
             raise ValueError("root_dir cannot be None.")
 
         if is_auto_git_enabled:
             self._check_is_in_git_repo()
 
         return (persistence, root_dir, is_auto_git_enabled)
 
@@ -73,14 +73,16 @@
             return "memory"
         elif self.persistence == "filesystem":
             if self.root_dir.startswith("s3://"):
                 return "s3"
             else:
                 return "local"
 
+        return "custom"  # catch-all for external backends
+
     def _get_repository(self):
         """Get the repository for the configured persistence type."""
         protocol = self._get_protocol()
 
         repository_key = f"{self.persistence}-{protocol}"
         repository = self.REPOSITORIES.get(repository_key)
```

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/dataframe.py` & `rubicon-ml-0.4.4/rubicon_ml/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/experiment.py` & `rubicon-ml-0.4.4/rubicon_ml/client/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/feature.py` & `rubicon-ml-0.4.4/rubicon_ml/client/feature.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/metric.py` & `rubicon-ml-0.4.4/rubicon_ml/client/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/mixin.py` & `rubicon-ml-0.4.4/rubicon_ml/client/mixin.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/parameter.py` & `rubicon-ml-0.4.4/rubicon_ml/client/parameter.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/project.py` & `rubicon-ml-0.4.4/rubicon_ml/client/project.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/rubicon.py` & `rubicon-ml-0.4.4/rubicon_ml/client/rubicon.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/utils/exception_handling.py` & `rubicon-ml-0.4.4/rubicon_ml/client/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/client/utils/tags.py` & `rubicon-ml-0.4.4/rubicon_ml/client/utils/tags.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/domain/experiment.py` & `rubicon-ml-0.4.4/rubicon_ml/domain/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/domain/metric.py` & `rubicon-ml-0.4.4/rubicon_ml/domain/metric.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/domain/utils/training_metadata.py` & `rubicon-ml-0.4.4/rubicon_ml/domain/utils/training_metadata.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/base.py` & `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/experiment.py` & `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/experiment.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/intake_rubicon/publish.py` & `rubicon-ml-0.4.4/rubicon_ml/intake_rubicon/publish.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/repository/base.py` & `rubicon-ml-0.4.4/rubicon_ml/repository/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,19 @@
         the underlying filesystem class.
     """
 
     def __init__(self, root_dir, **storage_options):
         self.filesystem = fsspec.filesystem(self.PROTOCOL, **storage_options)
         self.root_dir = root_dir.rstrip("/")
 
-    def _ls_directories_only(self, path):
-        """Returns the names of all the directories at path `path`."""
-        directories = [
-            os.path.join(p.get("name"), "metadata.json")
-            for p in self.filesystem.ls(path, detail=True)
-            if p.get("type", p.get("StorageClass")).lower() == "directory"
-        ]
+    # --- Filesystem Helpers ---
 
-        return directories
+    def _cat(self, path):
+        """Returns the contents of the file at `path`."""
+        return self.filesystem.cat(path)
 
     def _cat_paths(self, metadata_paths):
         """Cat `metadata_paths` to get the list of files to include.
         Ignore FileNotFoundErrors to avoid misc file errors, like hidden
         dotfiles.
         """
         files = []
@@ -56,14 +52,72 @@
                 warning = f"{path} not found. Was this file unintentionally created?"
                 warnings.warn(warning)
             else:
                 files.append(metadata)
 
         return files
 
+    def _exists(self, path):
+        """Returns True if a file exists at `path`, False otherwise."""
+        return self.filesystem.exists(path)
+
+    def _glob(self, globstring):
+        """Returns the names of the files matching `globstring`."""
+        return self.filesystem.glob(globstring, detail=True)
+
+    def _ls_directories_only(self, path):
+        """Returns the names of all the directories at path `path`."""
+        directories = [
+            os.path.join(p.get("name"), "metadata.json")
+            for p in self.filesystem.ls(path, detail=True)
+            if p.get("type", p.get("StorageClass")).lower() == "directory"
+        ]
+
+        return directories
+
+    def _mkdir(self, dirpath):
+        """Creates a directory `dirpath` with parents."""
+        return self.filesystem.mkdir(dirpath, parents=True, exist_ok=True)
+
+    def _persist_bytes(self, bytes_data, path):
+        """Write bytes to the filesystem.
+
+        To be implemented by extensions of the base filesystem.
+        """
+        raise NotImplementedError()
+
+    def _persist_domain(self, domain, path):
+        """Write a domain object to the filesystem.
+
+        To be implemented by extensions of the base filesystem.
+        """
+        raise NotImplementedError()
+
+    def _read_bytes(self, path, err_msg=None):
+        """Read bytes from the file at `path`."""
+        try:
+            open_file = self.filesystem.open(path, "rb")
+        except FileNotFoundError:
+            raise RubiconException(err_msg)
+
+        return open_file.read()
+
+    def _read_domain(self, path, err_msg=None):
+        """Read a domain object from the file at `path`."""
+        try:
+            open_file = self.filesystem.open(path)
+        except FileNotFoundError:
+            raise RubiconException(err_msg)
+
+        return json.load(open_file)
+
+    def _rm(self, path):
+        """Recursively remove all files at `path`."""
+        return self.filesystem.rm(path, recursive=True)
+
     # -------- Projects --------
 
     def _get_project_metadata_path(self, project_name):
         """Returns the path of the project with name `project_name`'s
         metadata.
         """
         return f"{self.root_dir}/{slugify(project_name)}/metadata.json"
@@ -74,15 +128,15 @@
         Parameters
         ----------
         project : rubicon.domain.Project
             The project to persist.
         """
         project_metadata_path = self._get_project_metadata_path(project.name)
 
-        if self.filesystem.exists(project_metadata_path):
+        if self._exists(project_metadata_path):
             raise RubiconException(f"A project with name '{project.name}' already exists.")
 
         self._persist_domain(project, project_metadata_path)
 
     def get_project(self, project_name):
         """Retrieve a project from the configured filesystem.
 
@@ -95,15 +149,15 @@
         -------
         rubicon.domain.Project
             The project with name `project_name`.
         """
         project_metadata_path = self._get_project_metadata_path(project_name)
 
         try:
-            project = json.loads(self.filesystem.cat(project_metadata_path))
+            project = json.loads(self._cat(project_metadata_path))
         except FileNotFoundError:
             raise RubiconException(f"No project with name '{project_name}' found.")
 
         return domain.Project(**project)
 
     def get_projects(self):
         """Get the list of projects from the filesystem.
@@ -168,22 +222,18 @@
 
         Returns
         -------
         rubicon.domain.Experiment
             The experiment with ID `experiment_id`.
         """
         experiment_metadata_path = self._get_experiment_metadata_path(project_name, experiment_id)
-
-        try:
-            open_file = self.filesystem.open(experiment_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No experiment with id `{experiment_id}` found.")
-
-        with open_file as f:
-            experiment = json.load(f)
+        experiment = self._read_domain(
+            experiment_metadata_path,
+            f"No experiment with id `{experiment_id}` found.",
+        )
 
         return domain.Experiment(**experiment)
 
     def get_experiments(self, project_name):
         """Retrieve all experiments from the configured filesystem
         that belong to the project with name `project_name`.
 
@@ -284,22 +334,18 @@
         -------
         rubicon.domain.Artifact
             The artifact with ID `artifact_id`.
         """
         artifact_metadata_path = self._get_artifact_metadata_path(
             project_name, experiment_id, artifact_id
         )
-
-        try:
-            open_file = self.filesystem.open(artifact_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No artifact with id `{artifact_id}` found.")
-
-        with open_file as f:
-            artifact = json.load(f)
+        artifact = self._read_domain(
+            artifact_metadata_path,
+            f"No artifact with id `{artifact_id}` found.",
+        )
 
         return domain.Artifact(**artifact)
 
     def get_artifacts_metadata(self, project_name, experiment_id=None):
         """Retrieve all artifacts' metadata from the configured
         filesystem that belong to the specified object.
 
@@ -349,21 +395,20 @@
 
         Returns
         -------
         bytes
             The artifact with ID `artifact_id`'s raw data.
         """
         artifact_data_path = self._get_artifact_data_path(project_name, experiment_id, artifact_id)
+        artifact_data = self._read_bytes(
+            artifact_data_path,
+            f"No data for artifact with id `{artifact_id}` found.",
+        )
 
-        try:
-            open_file = self.filesystem.open(artifact_data_path, "rb")
-        except FileNotFoundError:
-            raise RubiconException(f"No data for artifact with id `{artifact_id}` found.")
-
-        return open_file.read()
+        return artifact_data
 
     def delete_artifact(self, project_name, artifact_id, experiment_id=None):
         """Delete an artifact from the configured filesystem.
 
         Parameters
         ----------
         project_name : str
@@ -375,15 +420,15 @@
             The ID of the experiment the artifact with ID
             `artifact_id` is logged to. Artifacts do not
             need to belong to an experiment.
         """
         artifact_metadata_root = self._get_artifact_metadata_root(project_name, experiment_id)
 
         try:
-            self.filesystem.rm(f"{artifact_metadata_root}/{artifact_id}", recursive=True)
+            self._rm(f"{artifact_metadata_root}/{artifact_id}")
         except FileNotFoundError:
             raise RubiconException(f"No artifact with id `{artifact_id}` found.")
 
     # ------- Dataframes -------
 
     def _get_dataframe_metadata_root(self, project_name, experiment_id=None):
         """Returns the dataframes directory of the project with name
@@ -418,15 +463,15 @@
         Note
         ----
         `dask` dataframes will automatically be split into chunks by `dask.dataframe.to_parquet`.
         `pandas` dataframes, however, will be saved as a single file with the hope that users
         would leverage dask for large dataframes.
         """
         if isinstance(df, pd.DataFrame):
-            self.filesystem.mkdir(path, parents=True, exist_ok=True)
+            self._mkdir(path)
             path = f"{path}/data.parquet"
 
         df.to_parquet(path, engine="pyarrow")
 
     def _read_dataframe(self, path, df_type="pandas"):
         """Reads the dataframe `df` from the configured filesystem."""
         df = None
@@ -496,22 +541,18 @@
         -------
         rubicon.domain.Dataframe
             The dataframe with ID `dataframe_id`.
         """
         dataframe_metadata_path = self._get_dataframe_metadata_path(
             project_name, experiment_id, dataframe_id
         )
-
-        try:
-            open_file = self.filesystem.open(dataframe_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No dataframe with id `{dataframe_id}` found.")
-
-        with open_file as f:
-            dataframe = json.load(f)
+        dataframe = self._read_domain(
+            dataframe_metadata_path,
+            f"No dataframe with id `{dataframe_id}` found.",
+        )
 
         return domain.Dataframe(**dataframe)
 
     def get_dataframes_metadata(self, project_name, experiment_id=None):
         """Retrieve all dataframes' metadata from the configured
         filesystem that belong to the specified object.
 
@@ -594,15 +635,15 @@
             The ID of the experiment the dataframe with ID
             `artifact_id` is logged to. Dataframes do not
             need to belong to an experiment.
         """
         dataframe_metadata_root = self._get_dataframe_metadata_root(project_name, experiment_id)
 
         try:
-            self.filesystem.rm(f"{dataframe_metadata_root}/{dataframe_id}", recursive=True)
+            self._rm(f"{dataframe_metadata_root}/{dataframe_id}")
         except FileNotFoundError:
             raise RubiconException(f"No dataframe with id `{dataframe_id}` found.")
 
     # -------- Features --------
 
     def _get_feature_metadata_root(self, project_name, experiment_id):
         """Returns the features directory of the experiment with
@@ -633,15 +674,15 @@
         experiment_id : str
             The ID of the experiment this feature belongs to.
         """
         feature_metadata_path = self._get_feature_metadata_path(
             project_name, experiment_id, feature.name
         )
 
-        if self.filesystem.exists(feature_metadata_path):
+        if self._exists(feature_metadata_path):
             raise RubiconException(f"A feature with name '{feature.name}' already exists.")
 
         self._persist_domain(feature, feature_metadata_path)
 
     def get_feature(self, project_name, experiment_id, feature_name):
         """Retrieve a feature from the configured filesystem.
 
@@ -660,22 +701,18 @@
         -------
         rubicon.domain.Feature
             The feature with name `feature_name`.
         """
         feature_metadata_path = self._get_feature_metadata_path(
             project_name, experiment_id, feature_name
         )
-
-        try:
-            open_file = self.filesystem.open(feature_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No feature with name '{feature_name}' found.")
-
-        with open_file as f:
-            feature = json.load(f)
+        feature = self._read_domain(
+            feature_metadata_path,
+            f"No feature with name '{feature_name}' found.",
+        )
 
         return domain.Feature(**feature)
 
     def get_features(self, project_name, experiment_id):
         """Retrieve all features from the configured filesystem
         that belong to the experiment with ID `experiment_id`.
 
@@ -739,15 +776,15 @@
         experiment_id : str
             The ID of the experiment this metric belongs to.
         """
         metric_metadata_path = self._get_metric_metadata_path(
             project_name, experiment_id, metric.name
         )
 
-        if self.filesystem.exists(metric_metadata_path):
+        if self._exists(metric_metadata_path):
             raise RubiconException(f"A metric with name '{metric.name}' already exists.")
 
         self._persist_domain(metric, metric_metadata_path)
 
     def get_metric(self, project_name, experiment_id, metric_name):
         """Retrieve a metric from the configured filesystem.
 
@@ -766,22 +803,18 @@
         -------
         rubicon.domain.Metric
             The metric with name `metric_name`.
         """
         metric_metadata_path = self._get_metric_metadata_path(
             project_name, experiment_id, metric_name
         )
-
-        try:
-            open_file = self.filesystem.open(metric_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No metric with name '{metric_name}' found.")
-
-        with open_file as f:
-            metric = json.load(f)
+        metric = self._read_domain(
+            metric_metadata_path,
+            f"No metric with name '{metric_name}' found.",
+        )
 
         return domain.Metric(**metric)
 
     def get_metrics(self, project_name, experiment_id):
         """Retrieve all metrics from the configured filesystem
         that belong to the experiment with ID `experiment_id`.
 
@@ -845,15 +878,15 @@
         experiment_id : str
             The ID of the experiment this parameter belongs to.
         """
         parameter_metadata_path = self._get_parameter_metadata_path(
             project_name, experiment_id, parameter.name
         )
 
-        if self.filesystem.exists(parameter_metadata_path):
+        if self._exists(parameter_metadata_path):
             raise RubiconException(f"A parameter with name '{parameter.name}' already exists.")
 
         self._persist_domain(parameter, parameter_metadata_path)
 
     def get_parameter(self, project_name, experiment_id, parameter_name):
         """Retrieve a parameter from the configured filesystem.
 
@@ -871,22 +904,18 @@
         -------
         rubicon.domain.Parameter
             The parameter with name `parameter_name`.
         """
         parameter_metadata_path = self._get_parameter_metadata_path(
             project_name, experiment_id, parameter_name
         )
-
-        try:
-            open_file = self.filesystem.open(parameter_metadata_path)
-        except FileNotFoundError:
-            raise RubiconException(f"No parameter with name '{parameter_name}' found.")
-
-        with open_file as f:
-            parameter = json.load(f)
+        parameter = self._read_domain(
+            parameter_metadata_path,
+            f"No parameter with name '{parameter_name}' found.",
+        )
 
         return domain.Parameter(**parameter)
 
     def get_parameters(self, project_name, experiment_id):
         """Retrieve all parameters from the configured filesystem
         that belong to the experiment with ID `experiment_id`.
 
@@ -1049,17 +1078,17 @@
             added to or removed from the specified object.
         """
         tag_metadata_root = self._get_tag_metadata_root(
             project_name, experiment_id, entity_identifier, entity_type
         )
         tag_metadata_glob = f"{tag_metadata_root}/tags_*.json"
 
-        tag_paths = self.filesystem.glob(tag_metadata_glob, detail=True)
+        tag_paths = self._glob(tag_metadata_glob)
         if len(tag_paths) == 0:
             return []
 
         sorted_tag_paths = self._sort_tag_paths(tag_paths)
 
-        tag_data = self.filesystem.cat([p for _, p in sorted_tag_paths])
+        tag_data = self._cat([p for _, p in sorted_tag_paths])
         sorted_tag_data = [json.loads(tag_data[p]) for _, p in sorted_tag_paths]
 
         return sorted_tag_data
```

### Comparing `rubicon-ml-0.4.3/rubicon_ml/repository/local.py` & `rubicon-ml-0.4.4/rubicon_ml/repository/local.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/repository/memory.py` & `rubicon-ml-0.4.4/rubicon_ml/repository/memory.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/repository/s3.py` & `rubicon-ml-0.4.4/rubicon_ml/repository/s3.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/repository/utils/json.py` & `rubicon-ml-0.4.4/rubicon_ml/repository/utils/json.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/sklearn/estimator_logger.py` & `rubicon-ml-0.4.4/rubicon_ml/sklearn/estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/sklearn/filter_estimator_logger.py` & `rubicon-ml-0.4.4/rubicon_ml/sklearn/filter_estimator_logger.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/sklearn/pipeline.py` & `rubicon-ml-0.4.4/rubicon_ml/sklearn/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from sklearn.pipeline import Pipeline, _name_estimators
 
 from rubicon_ml.client.project import Project
 from rubicon_ml.sklearn.estimator_logger import EstimatorLogger
 from rubicon_ml.sklearn.utils import log_parameter_with_warning
 
 
@@ -37,14 +39,16 @@
         directly. Use the attribute ``named_steps`` or ``steps`` to
         inspect estimators within the pipeline. Caching the
         transformers is advantageous when fitting is time consuming.
         (docstring source: Scikit-Learn)
     verbose : bool, default=False
         If True, the time elapsed while fitting each step will be printed as
         it is completed. (docstring source: Scikit-Learn)
+    ignore_warnings : bool, default=False
+        If True, ignores warnings thrown by pipeline.
 
     Examples
     --------
     >>> pipeline = RubiconPipeline(
     ...     project,
     ...     [
     ...         ("vect", CountVectorizer()),
@@ -67,20 +71,22 @@
         self,
         project,
         steps,
         user_defined_loggers={},
         experiment_kwargs={"name": "RubiconPipeline experiment"},
         memory=None,
         verbose=False,
+        ignore_warnings=False,
     ):
         self.project = project
         self.user_defined_loggers = user_defined_loggers
         self.experiment_kwargs = experiment_kwargs
 
         self.experiment = None
+        self.ignore_warnings = ignore_warnings
 
         super().__init__(steps, memory=memory, verbose=verbose)
 
     def fit(self, X, y=None, tags=None, log_fit_params=True, experiment=None, **fit_params):
         """Fit the model and automatically log the `fit_params`
         to rubicon-ml. Optionally, pass `tags` to update the experiment's
         tags.
@@ -103,30 +109,33 @@
             logged to a new experiment with self.experiment_kwargs.
 
         Returns
         -------
         rubicon_ml.sklearn.Pipeline
             This `RubiconPipeline`.
         """
-        pipeline = super().fit(X, y, **fit_params)
+        with warnings.catch_warnings():
+            if self.ignore_warnings:
+                warnings.simplefilter("ignore")
+            pipeline = super().fit(X, y, **fit_params)
+
+            if experiment is None:
+                experiment = self.project.log_experiment(**self.experiment_kwargs)
+            self.experiment = experiment
 
-        if experiment is None:
-            experiment = self.project.log_experiment(**self.experiment_kwargs)
-        self.experiment = experiment
-
-        if tags is not None:
-            self.experiment.add_tags(tags)
-
-        for step_name, estimator in self.steps:
-            logger = self.get_estimator_logger(step_name, estimator)
-            logger.log_parameters()
-
-        if log_fit_params:
-            for name, value in fit_params.items():
-                log_parameter_with_warning(self.experiment, name, value)
+            if tags is not None:
+                self.experiment.add_tags(tags)
+
+            for step_name, estimator in self.steps:
+                logger = self.get_estimator_logger(step_name, estimator)
+                logger.log_parameters()
+
+            if log_fit_params:
+                for name, value in fit_params.items():
+                    log_parameter_with_warning(self.experiment, name, value)
         return pipeline
 
     def score(self, X, y=None, sample_weight=None, experiment=None):
         """Score with the final estimator and automatically
         log the results to rubicon-ml.
 
         Parameters
@@ -143,26 +152,29 @@
             to a new experiment with self.experiment_kwargs.
 
         Returns
         -------
         float
             Result of calling `score` on the final estimator.
         """
-        score = super().score(X, y, sample_weight)
+        with warnings.catch_warnings():
+            if self.ignore_warnings:
+                warnings.simplefilter("ignore")
+            score = super().score(X, y, sample_weight)
+
+            if experiment is not None:
+                self.experiment = experiment
+            elif self.experiment is None:
+                self.experiment = self.project.log_experiment(**self.experiment_kwargs)
 
-        if experiment is not None:
-            self.experiment = experiment
-        elif self.experiment is None:
-            self.experiment = self.project.log_experiment(**self.experiment_kwargs)
+            logger = self.get_estimator_logger()
+            logger.log_metric("score", score)
 
-        logger = self.get_estimator_logger()
-        logger.log_metric("score", score)
-
-        # clear `self.experiment` to avoid duplicate metric logging errors
-        self.experiment = None
+            # clear `self.experiment` to avoid duplicate metric logging errors
+            self.experiment = None
 
         return score
 
     def score_samples(self, X, experiment=None):
         """Score samples with the final estimator and automatically
         log the results to rubicon-ml.
 
@@ -175,33 +187,36 @@
             to a new experiment with self.experiment_kwargs.
 
         Returns
         -------
         ndarray of shape (n_samples,)
             Result of calling `score_samples` on the final estimator.
         """
-        score_samples = super().score_samples(X)
-
-        if experiment is not None:
-            self.experiment = experiment
-        elif self.experiment is None:
-            self.experiment = self.project.log_experiment(**self.experiment_kwargs)
+        with warnings.catch_warnings():
+            if self.ignore_warnings:
+                warnings.simplefilter("ignore")
+            score_samples = super().score_samples(X)
+
+            if experiment is not None:
+                self.experiment = experiment
+            elif self.experiment is None:
+                self.experiment = self.project.log_experiment(**self.experiment_kwargs)
+
+            logger = self.get_estimator_logger()
+            try:
+                logger.log_metric("score_samples", score_samples)
+            except TypeError:
+                score_samples = score_samples.tolist()
 
-        logger = self.get_estimator_logger()
-        try:
-            logger.log_metric("score_samples", score_samples)
-        except TypeError:
-            score_samples = score_samples.tolist()
+                logger.log_metric("score_samples", score_samples)
 
-            logger.log_metric("score_samples", score_samples)
-
-        # clear `self.experiment` to avoid duplicate metric logging errors
-        self.experiment = None
+            # clear `self.experiment` to avoid duplicate metric logging errors
+            self.experiment = None
 
-        return score_samples
+            return score_samples
 
     def get_estimator_logger(self, step_name=None, estimator=None):
         """Get a logger for the estimator. By default, the logger will
         have the current experiment set.
         """
         logger = self.user_defined_loggers.get(step_name) or EstimatorLogger()
```

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/assets/images/rubicon-logo-dark.png` & `rubicon-ml-0.4.4/rubicon_ml/viz/assets/images/rubicon-logo-dark.png`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/base.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/base.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/common/dropdown_header.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/common/dropdown_header.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/dashboard.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/dataframe_plot.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/dataframe_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/experiments_table.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/experiments_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,20 +253,20 @@
             if experiment.name is not None:
                 show_columns.add("name")
 
             if len(experiment.tags) > 0:
                 show_columns.add("tags")
 
             for parameter in experiment.parameters():
-                experiment_record[parameter.name] = parameter.value
+                experiment_record[parameter.name] = str(parameter.value)
 
                 self.parameter_names.add(parameter.name)
 
             for metric in experiment.metrics():
-                experiment_record[metric.name] = metric.value
+                experiment_record[metric.name] = str(metric.value)
 
                 self.metric_names.add(metric.name)
 
             self.experiment_records.append(experiment_record)
 
         self.metric_names = list(self.metric_names)
         self.parameter_names = list(self.parameter_names)
```

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/metric_correlation_plot.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/metric_correlation_plot.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/viz/metric_lists_comparison.py` & `rubicon-ml-0.4.4/rubicon_ml/viz/metric_lists_comparison.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/workflow/prefect/__init__.py` & `rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml/workflow/prefect/tasks.py` & `rubicon-ml-0.4.4/rubicon_ml/workflow/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/rubicon_ml.egg-info/PKG-INFO` & `rubicon-ml-0.4.4/rubicon_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-ml
-Version: 0.4.3
+Version: 0.4.4
 Summary: "an ML library for model development and governance"
 Home-page: https://github.com/capitalone/rubicon-ml
 Author: "Joe Wolfe, Ryan Soley, Diane Lee, Mike McCarty, CapitalOne"
 License: "Apache License, Version 2.0"
 Project-URL: Documentation, https://capitalone.github.io/rubicon-ml/
 Project-URL: Bug Tracker, https://github.com/capitalone/rubicon-ml/issues
 Project-URL: Source Code, https://github.com/capitalone/rubicon-ml
```

### Comparing `rubicon-ml-0.4.3/rubicon_ml.egg-info/SOURCES.txt` & `rubicon-ml-0.4.4/rubicon_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/setup.cfg` & `rubicon-ml-0.4.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	click<=8.1.3,>=7.1
-	fsspec<=2022.11.0,>=2021.4.0
-	intake[dataframe]<=0.6.6,>=0.5.2
-	numpy<=1.23.5,>=1.22.0
-	pandas<=1.5.2,>=1.0.0
-	pyarrow<=10.0.1,>=0.18.0
+	fsspec<=2023.4.0,>=2021.4.0
+	intake[dataframe]<=0.6.8,>=0.5.2
+	numpy<=1.24.2,>=1.22.0
+	pandas<=2.0.0,>=1.0.0
+	pyarrow<=11.0.0,>=0.18.0
 	PyYAML<=6.0,>=5.4.0
-	scikit-learn<=1.2.0,>=0.22.0
+	scikit-learn<=1.2.2,>=0.22.0
 
 [options.extras_require]
 prefect = 
 	prefect<=1.2.4,>=0.12.0
 s3 = 
-	s3fs<=2022.11.0,>=0.4
+	s3fs<=2023.4.0,>=0.4
 ui = 
-	dash<=2.7.1,>=2.0.0
-	dash-bootstrap-components<=1.2.1,>=1.0.0
+	dash<=2.9.3,>=2.0.0
+	dash-bootstrap-components<=1.4.1,>=1.0.0
 viz = 
-	dash<=2.7.1,>=2.0.0
-	dash-bootstrap-components<=1.2.1,>=1.0.0
+	dash<=2.9.3,>=2.0.0
+	dash-bootstrap-components<=1.4.1,>=1.0.0
 all = 
-	dash<=2.7.1,>=2.0.0
-	dash-bootstrap-components<=1.2.1,>=1.0.0
+	dash<=2.9.3,>=2.0.0
+	dash-bootstrap-components<=1.4.1,>=1.0.0
 	prefect<=1.2.4,>=0.12.0
-	s3fs<=2022.11.0,>=0.4
+	s3fs<=2023.4.0,>=0.4
 
 [options.entry_points]
 console_scripts = 
 	rubicon_ml = rubicon_ml.cli:cli
 intake.drivers = 
 	rubicon_ml_experiment = rubicon_ml.intake_rubicon.experiment:ExperimentSource
 
@@ -95,19 +95,16 @@
 minversion = 3.2
 xfail_strict = True
 
 [edgetest.envs.core]
 python_version = 3.9
 deps = 
 	kaleido
-	matplotlib
-	numba>=0.56.2
 	palmerpenguins
 	Pillow
-	shap
 conda_install = 
 	dask
 	jupyterlab
 	nodejs
 	nbconvert
 	nbformat
 	pytest
```

### Comparing `rubicon-ml-0.4.3/tests/fixtures.py` & `rubicon-ml-0.4.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `rubicon-ml-0.4.3/versioneer.py` & `rubicon-ml-0.4.4/versioneer.py`

 * *Files identical despite different names*

