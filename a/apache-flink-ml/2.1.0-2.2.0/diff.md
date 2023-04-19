# Comparing `tmp/apache-flink-ml-2.1.0.tar.gz` & `tmp/apache-flink-ml-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-flink-ml-2.1.0.tar", last modified: Fri Jul  1 02:14:42 2022, max compression
+gzip compressed data, was "dist/apache-flink-ml-2.2.0.tar", last modified: Wed Apr 12 05:42:26 2023, max compression
```

## Comparing `apache-flink-ml-2.1.0.tar` & `apache-flink-ml-2.2.0.tar`

### file list

```diff
@@ -1,84 +1,162 @@
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/
--rw-r--r--   0 zhangzp    (502) staff       (20)     1061 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/MANIFEST.in
--rw-r--r--   0 zhangzp    (502) staff       (20)     1694 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/PKG-INFO
--rw-r--r--   0 zhangzp    (502) staff       (20)      916 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/README.md
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/
--rw-r--r--   0 zhangzp    (502) staff       (20)     1694 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/PKG-INFO
--rw-r--r--   0 zhangzp    (502) staff       (20)     2404 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/SOURCES.txt
--rw-r--r--   0 zhangzp    (502) staff       (20)        1 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/dependency_links.txt
--rw-r--r--   0 zhangzp    (502) staff       (20)       97 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/requires.txt
--rw-r--r--   0 zhangzp    (502) staff       (20)        8 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/apache_flink_ml.egg-info/top_level.txt
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/deps/examples/ml/__init__.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3873 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/knn_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3438 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/linearsvc_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3554 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/logisticregression_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3247 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/classification/naivebayes_example.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/clustering/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/clustering/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2764 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/clustering/kmeans_example.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/evaluation/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/evaluation/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3283 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/evaluation/binaryclassificationevaluator_example.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3028 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/bucketizer_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3166 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/indextostringmodel_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3110 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/minmaxscaler_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2800 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/onehotencoder_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2741 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/standardscaler_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3431 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/stringindexer_example.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3160 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/feature/vectorassembler_example.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/regression/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/regression/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3196 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/regression/linearregression_example.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/deps/examples/ml/tests/
--rw-r--r--   0 zhangzp    (502) staff       (20)     1410 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/tests/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     1788 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/deps/examples/ml/tests/test_examples.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/
--rw-r--r--   0 zhangzp    (502) staff       (20)     4297 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/pyflink/ml/__init__.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/core/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/pyflink/ml/core/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3874 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/core/api.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     5274 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/core/builder.py
--rw-r--r--   0 zhangzp    (502) staff       (20)    24750 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/pyflink/ml/core/linalg.py
--rw-r--r--   0 zhangzp    (502) staff       (20)    12783 2022-06-06 03:27:13.000000 apache-flink-ml-2.1.0/pyflink/ml/core/param.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     9485 2022-06-06 03:27:13.000000 apache-flink-ml-2.1.0/pyflink/ml/core/wrapper.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/__init__.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2388 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/common.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3107 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/knn.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3709 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/linearsvc.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     6583 2022-06-07 11:43:41.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/logisticregression.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3775 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/classification/naivebayes.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2348 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/common.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     6024 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/kmeans.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-06-06 03:27:13.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3077 2022-06-06 03:27:13.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/binaryclassificationevaluator.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     1797 2022-06-06 03:27:13.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/common.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2766 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/bucketizer.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3002 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/common.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3635 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/minmaxscaler.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3338 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/onehotencoder.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     3696 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/standardscaler.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     5120 2022-07-01 02:12:07.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/stringindexer.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     2096 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/feature/vectorassembler.py
--rw-r--r--   0 zhangzp    (502) staff       (20)    12921 2022-05-31 01:13:53.000000 apache-flink-ml-2.1.0/pyflink/ml/lib/param.py
-drwxr-xr-x   0 zhangzp    (502) staff       (20)        0 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/pyflink/ml/util/
--rw-r--r--   0 zhangzp    (502) staff       (20)      958 2022-03-24 03:06:15.000000 apache-flink-ml-2.1.0/pyflink/ml/util/__init__.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     6470 2022-05-18 02:24:30.000000 apache-flink-ml-2.1.0/pyflink/ml/util/read_write_utils.py
--rw-r--r--   0 zhangzp    (502) staff       (20)     1123 2022-07-01 02:14:21.000000 apache-flink-ml-2.1.0/pyflink/ml/version.py
--rw-r--r--   0 zhangzp    (502) staff       (20)      246 2022-07-01 02:14:42.000000 apache-flink-ml-2.1.0/setup.cfg
--rw-r--r--   0 zhangzp    (502) staff       (20)     4657 2022-06-28 02:40:04.000000 apache-flink-ml-2.1.0/setup.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/
+-rw-r--r--   0 lindong    (502) staff       (20)     1084 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/MANIFEST.in
+-rw-r--r--   0 lindong    (502) staff       (20)     1503 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/PKG-INFO
+-rw-r--r--   0 lindong    (502) staff       (20)      896 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/README.md
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/
+-rw-r--r--   0 lindong    (502) staff       (20)     1503 2023-04-12 05:42:25.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/PKG-INFO
+-rw-r--r--   0 lindong    (502) staff       (20)     5314 2023-04-12 05:42:25.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 lindong    (502) staff       (20)        1 2023-04-12 05:42:25.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 lindong    (502) staff       (20)       97 2023-04-12 05:42:25.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/requires.txt
+-rw-r--r--   0 lindong    (502) staff       (20)        8 2023-04-12 05:42:25.000000 apache-flink-ml-2.2.0/apache_flink_ml.egg-info/top_level.txt
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-01 02:29:24.000000 apache-flink-ml-2.2.0/deps/examples/ml/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2346 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/arraytovector_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3594 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/knn_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3159 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/linearsvc_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3275 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/logisticregression_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2968 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/classification/naivebayes_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/clustering/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/clustering/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3414 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/clustering/agglomerativeclustering_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2485 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/clustering/kmeans_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/evaluation/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/evaluation/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2995 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/evaluation/binaryclassificationevaluator_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2914 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/binarizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2754 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/bucketizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2549 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/countvectorizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2261 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/dct_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2548 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/elementwiseproduct_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2614 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/featurehasher_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2379 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/hashingtf_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2407 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/idf_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2648 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/imputer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2885 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/indextostringmodel_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2661 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/interaction_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2812 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/kbinsdiscreteizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2828 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/maxabsscaler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3606 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/minhashlsh_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2831 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/minmaxscaler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2266 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/ngram_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2463 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/normalizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2526 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/onehotencoder_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4139 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/online_standardscaler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2558 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/polynomialexpansion_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2344 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/randomsplitter_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2295 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/regextokenizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2894 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/robustscaler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2014 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/sqltransformer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2462 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/standardscaler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2412 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/stopwordsremover_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3157 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/stringindexer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2246 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/tokenizer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3020 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/univariatefeatureselector_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2988 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/variancethresholdselector_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2907 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/vectorassembler_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2883 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/vectorindexer_example.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2484 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/feature/vectorslicer_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/recommendation/
+-rw-r--r--   0 lindong    (502) staff       (20)     2421 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/recommendation/swing_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/regression/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/regression/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2917 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/regression/linearregression_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/stats/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/stats/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2827 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/stats/chisqtest_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/examples/ml/tests/
+-rw-r--r--   0 lindong    (502) staff       (20)     1410 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/tests/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1852 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/tests/test_examples.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2402 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/deps/examples/ml/vectortoarray_example.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/deps/lib/
+-rw-r--r--   0 lindong    (502) staff       (20)   102754 2020-01-22 15:10:15.000000 apache-flink-ml-2.2.0/deps/lib/flink-ml-examples-2.2.0.jar
+-rw-r--r--   0 lindong    (502) staff       (20)    12311 2020-01-22 15:10:15.000000 apache-flink-ml-2.2.0/deps/lib/flink-ml-python-2.2.0.jar
+-rw-r--r--   0 lindong    (502) staff       (20)  2858387 2020-01-22 15:10:15.000000 apache-flink-ml-2.2.0/deps/lib/flink-ml-uber-2.2.0.jar
+-rw-r--r--   0 lindong    (502) staff       (20)   667137 2020-01-22 15:10:15.000000 apache-flink-ml-2.2.0/deps/lib/statefun-flink-core-3.2.0.jar
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/
+-rw-r--r--   0 lindong    (502) staff       (20)     4297 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3869 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/api.py
+-rw-r--r--   0 lindong    (502) staff       (20)     5264 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/builder.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2383 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/common.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3092 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/knn.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3700 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/linearsvc.py
+-rw-r--r--   0 lindong    (502) staff       (20)     6577 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/logisticregression.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3760 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/classification/naivebayes.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/clustering/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/clustering/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     5702 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/clustering/agglomerativeclustering.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3049 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/clustering/common.py
+-rw-r--r--   0 lindong    (502) staff       (20)     6019 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/clustering/kmeans.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/common/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/common/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)    17519 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/common/param.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4456 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/common/window.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/evaluation/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/evaluation/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3066 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/evaluation/binaryclassification.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1792 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/evaluation/common.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2671 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/binarizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2737 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/bucketizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2997 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/common.py
+-rw-r--r--   0 lindong    (502) staff       (20)     6550 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/countvectorizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2562 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/dct.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2621 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/elementwiseproduct.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2585 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/featurehasher.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3068 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/hashingtf.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3352 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/idf.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4383 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/imputer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2249 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/interaction.py
+-rw-r--r--   0 lindong    (502) staff       (20)     6473 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/kbinsdiscretizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     9186 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/lsh.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2542 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/maxabsscaler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3605 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/minmaxscaler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2412 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/ngram.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2250 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/normalizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3327 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/onehotencoder.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4016 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/onlinestandardscaler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2620 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/polynomialexpansion.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2953 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/randomsplitter.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4132 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/regextokenizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     5460 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/robustscaler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3228 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/sqltransformer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3686 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/standardscaler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     5084 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/stopwordsremover.py
+-rw-r--r--   0 lindong    (502) staff       (20)     5905 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/stringindexer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1821 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/tokenizer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     7998 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/univariatefeatureselector.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3807 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/variancethresholdselector.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3895 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/vectorassembler.py
+-rw-r--r--   0 lindong    (502) staff       (20)     4709 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/vectorindexer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3264 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/feature/vectorslicer.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1526 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/functions.py
+-rw-r--r--   0 lindong    (502) staff       (20)    25845 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/linalg.py
+-rw-r--r--   0 lindong    (502) staff       (20)    13709 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/param.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/recommendation/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/recommendation/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1820 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/recommendation/common.py
+-rw-r--r--   0 lindong    (502) staff       (20)     7813 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/recommendation/swing.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/regression/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/regression/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     2343 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/regression/common.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3142 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/regression/linearregression.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/stats/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/stats/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     3130 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/stats/chisqtest.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1766 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/stats/common.py
+drwxr-xr-x   0 lindong    (502) staff       (20)        0 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/pyflink/ml/util/
+-rw-r--r--   0 lindong    (502) staff       (20)      958 2023-04-01 02:29:24.000000 apache-flink-ml-2.2.0/pyflink/ml/util/__init__.py
+-rw-r--r--   0 lindong    (502) staff       (20)     6465 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/util/read_write_utils.py
+-rw-r--r--   0 lindong    (502) staff       (20)     1123 2023-04-12 05:34:23.000000 apache-flink-ml-2.2.0/pyflink/ml/version.py
+-rw-r--r--   0 lindong    (502) staff       (20)    15167 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/pyflink/ml/wrapper.py
+-rw-r--r--   0 lindong    (502) staff       (20)      246 2023-04-12 05:42:26.000000 apache-flink-ml-2.2.0/setup.cfg
+-rw-r--r--   0 lindong    (502) staff       (20)     5152 2023-04-12 03:25:08.000000 apache-flink-ml-2.2.0/setup.py
```

### Comparing `apache-flink-ml-2.1.0/MANIFEST.in` & `apache-flink-ml-2.2.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 global-exclude *.py[cod] __pycache__ .DS_Store
+include deps/lib/*.jar
 recursive-include deps/examples *.py
 include README.md
```

### Comparing `apache-flink-ml-2.1.0/README.md` & `apache-flink-ml-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Flink ML is a library which provides machine learning (ML) APIs and infrastructures that simplify the building of ML pipelines. Users can implement ML algorithms with the standard ML APIs and further use these infrastructures to build ML pipelines for both training and inference jobs.
 
 Flink ML is developed under the umbrella of [Apache Flink](https://flink.apache.org/).
 
-## <a name="build"></a>Python Packaging
+## Python Packaging
 
 Prerequisites for building apache-flink-ml:
 
 * Unix-like environment (we use Linux, Mac OS X)
 * Python version(3.6, 3.7 or 3.8) is required
 
 Then go to the root directory of flink-ml-python source code and run this command to build the sdist package of apache-flink-ml:
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/classification/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/classification/knn_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/classification/knn_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a Knn model and uses it for classification.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.classification.knn import KNN
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.classification.knn import KNN
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/classification/linearsvc_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/classification/linearsvc_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a LinearSVC model and uses it for classification.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.classification.linearsvc import LinearSVC
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.classification.linearsvc import LinearSVC
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/classification/logisticregression_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/classification/logisticregression_example.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a LogisticRegression model and uses it for
 # classification.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.classification.logisticregression import LogisticRegression
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.classification.logisticregression import LogisticRegression
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/classification/naivebayes_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/vectorindexer_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,69 +12,63 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
-# Simple program that trains a NaiveBayes model and uses it for classification.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
+# Simple program that trains a VectorIndexer model and uses it for feature
+# engineering.
 
 from pyflink.common import Types
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.classification.naivebayes import NaiveBayes
+from pyflink.ml.feature.vectorindexer import VectorIndexer
 from pyflink.table import StreamTableEnvironment
 
-# create a new StreamExecutionEnvironment
+# Creates a new StreamExecutionEnvironment.
 env = StreamExecutionEnvironment.get_execution_environment()
 
-# create a StreamTableEnvironment
+# Creates a StreamTableEnvironment.
 t_env = StreamTableEnvironment.create(env)
 
-# generate input training and prediction data
+# Generates input training and prediction data.
 train_table = t_env.from_data_stream(
     env.from_collection([
-        (Vectors.dense([0, 0.]), 11.),
-        (Vectors.dense([1, 0]), 10.),
-        (Vectors.dense([1, 1.]), 10.),
+        (Vectors.dense(1, 1),),
+        (Vectors.dense(2, -1),),
+        (Vectors.dense(3, 1),),
+        (Vectors.dense(4, 0),),
+        (Vectors.dense(5, 0),)
     ],
         type_info=Types.ROW_NAMED(
-            ['features', 'label'],
-            [DenseVectorTypeInfo(), Types.DOUBLE()])))
+            ['input', ],
+            [DenseVectorTypeInfo(), ])))
 
 predict_table = t_env.from_data_stream(
     env.from_collection([
-        (Vectors.dense([0, 1.]),),
-        (Vectors.dense([0, 0.]),),
-        (Vectors.dense([1, 0]),),
-        (Vectors.dense([1, 1.]),),
+        (Vectors.dense(0, 2),),
+        (Vectors.dense(0, 0),),
+        (Vectors.dense(0, -1),),
     ],
         type_info=Types.ROW_NAMED(
-            ['features'],
-            [DenseVectorTypeInfo()])))
+            ['input', ],
+            [DenseVectorTypeInfo(), ])))
 
-# create a naive bayes object and initialize its parameters
-naive_bayes = NaiveBayes() \
-    .set_smoothing(1.0) \
-    .set_features_col('features') \
-    .set_label_col('label') \
-    .set_prediction_col('prediction') \
-    .set_model_type('multinomial')
+# Creates a VectorIndexer object and initializes its parameters.
+vector_indexer = VectorIndexer() \
+    .set_input_col('input') \
+    .set_output_col('output') \
+    .set_handle_invalid('keep') \
+    .set_max_categories(3)
 
-# train the naive bayes model
-model = naive_bayes.fit(train_table)
+# Trains the VectorIndexer Model.
+model = vector_indexer.fit(train_table)
 
-# use the naive bayes model for predictions
+# Uses the VectorIndexer Model for predictions.
 output = model.transform(predict_table)[0]
 
-# extract and display the results
+# Extracts and displays the results.
 field_names = output.get_schema().get_field_names()
 for result in t_env.to_data_stream(output).execute_and_collect():
-    features = result[field_names.index(naive_bayes.get_features_col())]
-    prediction_result = result[field_names.index(naive_bayes.get_prediction_col())]
-    print('Features: ' + str(features) + ' \tPrediction Result: ' + str(prediction_result))
+    print('Input Value: ' + str(result[field_names.index(vector_indexer.get_input_col())])
+          + '\tOutput Value: ' + str(result[field_names.index(vector_indexer.get_output_col())]))
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/clustering/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/clustering/kmeans_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/idf_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,56 +12,49 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
-# Simple program that trains a KMeans model and uses it for clustering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
+# Simple program that trains an IDF model and uses it for feature
+# engineering.
 
 from pyflink.common import Types
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.clustering.kmeans import KMeans
+from pyflink.ml.feature.idf import IDF
 from pyflink.table import StreamTableEnvironment
 
-# create a new StreamExecutionEnvironment
+# Creates a new StreamExecutionEnvironment.
 env = StreamExecutionEnvironment.get_execution_environment()
 
-# create a StreamTableEnvironment
+# Creates a StreamTableEnvironment.
 t_env = StreamTableEnvironment.create(env)
 
-# generate input data
-input_data = t_env.from_data_stream(
+# Generates input for training and prediction.
+input_table = t_env.from_data_stream(
     env.from_collection([
-        (Vectors.dense([0.0, 0.0]),),
-        (Vectors.dense([0.0, 0.3]),),
-        (Vectors.dense([0.3, 3.0]),),
-        (Vectors.dense([9.0, 0.0]),),
-        (Vectors.dense([9.0, 0.6]),),
-        (Vectors.dense([9.6, 0.0]),),
+        (Vectors.dense(0, 1, 0, 2),),
+        (Vectors.dense(0, 1, 2, 3),),
+        (Vectors.dense(0, 1, 0, 0),),
     ],
         type_info=Types.ROW_NAMED(
-            ['features'],
-            [DenseVectorTypeInfo()])))
+            ['input', ],
+            [DenseVectorTypeInfo(), ])))
 
-# create a kmeans object and initialize its parameters
-kmeans = KMeans().set_k(2).set_seed(1)
+# Creates an IDF object and initializes its parameters.
+idf = IDF().set_min_doc_freq(2)
 
-# train the kmeans model
-model = kmeans.fit(input_data)
+# Trains the IDF Model.
+model = idf.fit(input_table)
 
-# use the kmeans model for predictions
-output = model.transform(input_data)[0]
+# Uses the IDF Model for predictions.
+output = model.transform(input_table)[0]
 
-# extract and display the results
+# Extracts and displays the results.
 field_names = output.get_schema().get_field_names()
 for result in t_env.to_data_stream(output).execute_and_collect():
-    features = result[field_names.index(kmeans.get_features_col())]
-    cluster_id = result[field_names.index(kmeans.get_prediction_col())]
-    print('Features: ' + str(features) + ' \tCluster Id: ' + str(cluster_id))
+    input_index = field_names.index(idf.get_input_col())
+    output_index = field_names.index(idf.get_output_col())
+    print('Input Value: ' + str(result[input_index]) +
+          '\tOutput Value: ' + str(result[output_index]))
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/evaluation/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/evaluation/binaryclassificationevaluator_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/evaluation/binaryclassificationevaluator_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that creates a BinaryClassificationEvaluator instance and uses
 # it for evaluation.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.evaluation.binaryclassificationevaluator import BinaryClassificationEvaluator
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.evaluation.binaryclassification import BinaryClassificationEvaluator
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/bucketizer_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/bucketizer_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that creates a Bucketizer instance and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.lib.feature.bucketizer import Bucketizer
+from pyflink.ml.feature.bucketizer import Bucketizer
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/indextostringmodel_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/indextostringmodel_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,20 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
-# Simple program that creates an IndexToStringModelExample instance and uses it
+# Simple program that creates an IndexToStringModel instance and uses it
 # for feature engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.lib.feature.stringindexer import IndexToStringModel
+from pyflink.ml.feature.stringindexer import IndexToStringModel
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/minmaxscaler_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/robustscaler_example.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,68 +12,63 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
-# Simple program that trains a MinMaxScaler model and uses it for feature
+# Simple program that creates a RobustScaler instance and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.feature.minmaxscaler import MinMaxScaler
 from pyflink.table import StreamTableEnvironment
 
-# create a new StreamExecutionEnvironment
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+
+from pyflink.ml.feature.robustscaler import RobustScaler
+
+# Creates a new StreamExecutionEnvironment.
 env = StreamExecutionEnvironment.get_execution_environment()
 
-# create a StreamTableEnvironment
+# Creates a StreamTableEnvironment.
 t_env = StreamTableEnvironment.create(env)
 
-# generate input training and prediction data
+# Generates input training and prediction data.
 train_data = t_env.from_data_stream(
     env.from_collection([
-        (Vectors.dense(0.0, 3.0),),
-        (Vectors.dense(2.1, 0.0),),
-        (Vectors.dense(4.1, 5.1),),
-        (Vectors.dense(6.1, 8.1),),
-        (Vectors.dense(200, 400),),
-    ],
-        type_info=Types.ROW_NAMED(
-            ['input'],
-            [DenseVectorTypeInfo()])
-    ))
-
-predict_data = t_env.from_data_stream(
-    env.from_collection([
-        (Vectors.dense(150.0, 90.0),),
-        (Vectors.dense(50.0, 40.0),),
-        (Vectors.dense(100.0, 50.0),),
+        (1, Vectors.dense(0.0, 0.0),),
+        (2, Vectors.dense(1.0, -1.0),),
+        (3, Vectors.dense(2.0, -2.0),),
+        (4, Vectors.dense(3.0, -3.0),),
+        (5, Vectors.dense(4.0, -4.0),),
+        (6, Vectors.dense(5.0, -5.0),),
+        (7, Vectors.dense(6.0, -6.0),),
+        (8, Vectors.dense(7.0, -7.0),),
+        (9, Vectors.dense(8.0, -8.0),),
     ],
         type_info=Types.ROW_NAMED(
-            ['input'],
-            [DenseVectorTypeInfo()])
+            ['id', 'input'],
+            [Types.INT(), DenseVectorTypeInfo()])
     ))
 
-# create a min-max-scaler object and initialize its parameters
-min_max_scaler = MinMaxScaler()
+# Creates an RobustScaler object and initializes its parameters.
+robust_scaler = RobustScaler()\
+    .set_lower(0.25)\
+    .set_upper(0.75)\
+    .set_relative_error(0.001)\
+    .set_with_scaling(True)\
+    .set_with_centering(True)
 
-# train the min-max-scaler model
-model = min_max_scaler.fit(train_data)
+# Trains the RobustScaler Model.
+model = robust_scaler.fit(train_data)
 
-# use the min-max-scaler model for predictions
-output = model.transform(predict_data)[0]
+# Uses the RobustScaler Model for predictions.
+output = model.transform(train_data)[0]
 
-# extract and display the results
+# Extracts and displays the results.
 field_names = output.get_schema().get_field_names()
 for result in t_env.to_data_stream(output).execute_and_collect():
-    input_value = result[field_names.index(min_max_scaler.get_input_col())]
-    output_value = result[field_names.index(min_max_scaler.get_output_col())]
-    print('Input Value: ' + str(input_value) + ' \tOutput Value: ' + str(output_value))
+    input_index = field_names.index(robust_scaler.get_input_col())
+    output_index = field_names.index(robust_scaler.get_output_col())
+    print('Input Value: ' + str(result[input_index]) +
+          '\tOutput Value: ' + str(result[output_index]))
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/onehotencoder_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/onehotencoder_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a OneHotEncoder model and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Row
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.lib.feature.onehotencoder import OneHotEncoder
+from pyflink.ml.feature.onehotencoder import OneHotEncoder
 from pyflink.table import StreamTableEnvironment, DataTypes
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/standardscaler_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/standardscaler_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a StandardScaler model and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.feature.standardscaler import StandardScaler
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.feature.standardscaler import StandardScaler
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/stringindexer_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/stringindexer_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a StringIndexer model and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.lib.feature.stringindexer import StringIndexer
+from pyflink.ml.feature.stringindexer import StringIndexer
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/feature/vectorassembler_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/feature/vectorassembler_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that creates a VectorAssembler instance and uses it for feature
 # engineering.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo, SparseVectorTypeInfo
-from pyflink.ml.lib.feature.vectorassembler import VectorAssembler
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo, SparseVectorTypeInfo
+from pyflink.ml.feature.vectorassembler import VectorAssembler
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
@@ -52,17 +46,18 @@
             ['vec', 'num', 'sparse_vec'],
             [DenseVectorTypeInfo(), Types.DOUBLE(), SparseVectorTypeInfo()])))
 
 # create a vector assembler object and initialize its parameters
 vector_assembler = VectorAssembler() \
     .set_input_cols('vec', 'num', 'sparse_vec') \
     .set_output_col('assembled_vec') \
+    .set_input_sizes(2, 1, 5) \
     .set_handle_invalid('keep')
 
-# use the vector assembler model for feature engineering
+# use the vector assembler for feature engineering
 output = vector_assembler.transform(input_data_table)[0]
 
 # extract and display the results
 field_names = output.get_schema().get_field_names()
 input_values = [None for _ in vector_assembler.get_input_cols()]
 for result in t_env.to_data_stream(output).execute_and_collect():
     for i in range(len(vector_assembler.get_input_cols())):
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/regression/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/regression/linearregression_example.py` & `apache-flink-ml-2.2.0/deps/examples/ml/regression/linearregression_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 # Simple program that trains a LinearRegression model and uses it for
 # regression.
-#
-# Before executing this program, please make sure you have followed Flink ML's
-# quick start guideline to set up Flink ML and Flink environment. The guideline
-# can be found at
-#
-# https://nightlies.apache.org/flink/flink-ml-docs-master/docs/try-flink-ml/quick-start/
 
 from pyflink.common import Types
 from pyflink.datastream import StreamExecutionEnvironment
-from pyflink.ml.core.linalg import Vectors, DenseVectorTypeInfo
-from pyflink.ml.lib.regression.linearregression import LinearRegression
+from pyflink.ml.linalg import Vectors, DenseVectorTypeInfo
+from pyflink.ml.regression.linearregression import LinearRegression
 from pyflink.table import StreamTableEnvironment
 
 # create a new StreamExecutionEnvironment
 env = StreamExecutionEnvironment.get_execution_environment()
 
 # create a StreamTableEnvironment
 t_env = StreamTableEnvironment.create(env)
```

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/tests/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/deps/examples/ml/tests/test_examples.py` & `apache-flink-ml-2.2.0/deps/examples/ml/tests/test_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 class ExamplesTest(PyFlinkMLTestCase):
     def test_examples(self):
         self.execute_all_in_module('pyflink.examples.ml.classification')
         self.execute_all_in_module('pyflink.examples.ml.clustering')
         self.execute_all_in_module('pyflink.examples.ml.evaluation')
         self.execute_all_in_module('pyflink.examples.ml.feature')
         self.execute_all_in_module('pyflink.examples.ml.regression')
+        self.execute_all_in_module('pyflink.examples.ml.stats')
 
     def execute_all_in_module(self, module):
         module = importlib.import_module(module)
         for importer, sub_modname, ispkg in pkgutil.iter_modules(module.__path__):
             # importing an example module means executing the example.
             importlib.import_module(module.__name__ + "." + sub_modname)
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/core/__init__.py` & `apache-flink-ml-2.2.0/deps/examples/ml/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/core/api.py` & `apache-flink-ml-2.2.0/pyflink/ml/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ################################################################################
 
 from abc import ABC, abstractmethod
 from typing import TypeVar, List, Generic
 
 from pyflink.table import Table, StreamTableEnvironment
 
-from pyflink.ml.core.param import WithParams
+from pyflink.ml.param import WithParams
 
 T = TypeVar('T')
 E = TypeVar('E')
 M = TypeVar('M')
 
 
 class Stage(WithParams[T], ABC):
@@ -68,15 +68,15 @@
         :return: A list of tables.
         """
         pass
 
 
 class Transformer(AlgoOperator[T], ABC):
     """
-    A Transformer is an AlgoOperator with the semantic difference that it encodes the Transformation
+    A Transformer is an AlgoOperator with the semantic difference that it encodes the transformation
     logic, such that a record in the output typically corresponds to one record in the input. In
     contrast, an AlgoOperator is a better fit to express aggregation logic where a record in the
     output could be computed from an arbitrary number of records in the input.
     """
     pass
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/core/builder.py` & `apache-flink-ml-2.2.0/pyflink/ml/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # limitations under the License.
 ################################################################################
 
 from typing import List, TypeVar, Dict, Any
 
 from pyflink.table import Table, StreamTableEnvironment
 
-from pyflink.ml.core.api import Estimator, Model, AlgoOperator, Stage
-from pyflink.ml.core.param import Param
+from pyflink.ml.api import Estimator, Model, AlgoOperator, Stage
+from pyflink.ml.param import Param
 
 E = TypeVar('E')
 
 
 class PipelineModel(Model):
     """
     A PipelineModel acts as a Model. It consists of an ordered list of stages, each of which could
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/core/linalg.py` & `apache-flink-ml-2.2.0/pyflink/ml/linalg.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,14 +219,21 @@
     def size(self) -> int:
         """
         Gets the size of the vector.
         """
         pass
 
     @abstractmethod
+    def set(self, i: int, value: np.float64):
+        """
+        Sets the value of the ith element.
+        """
+        pass
+
+    @abstractmethod
     def get(self, i: int):
         """
         Gets the value of the ith element.
         """
         pass
 
     @abstractmethod
@@ -301,14 +308,17 @@
 
     def size(self) -> int:
         return len(self._values)
 
     def get(self, i: int):
         return self._values[i]
 
+    def set(self, i: int, value: np.float64):
+        self._values[i] = value
+
     def to_array(self) -> np.ndarray:
         return self._values
 
     def dot(self, other: Union[Vector, np.ndarray, Sized]) -> np.ndarray:
         """
         Dot product of two Vectors.
 
@@ -477,15 +487,37 @@
                         "Indices {0} and {1} are not strictly increasing".format(
                             self._indices[i], self._indices[i + 1]))
 
     def size(self) -> int:
         return self._size
 
     def get(self, i: int):
-        return self._values[self._indices.searchsorted(i)]
+        idx = self._indices.searchsorted(i)
+        if idx < len(self._indices) and self._indices[idx] == i:
+            return self._values[idx]
+        else:
+            return 0.0
+
+    def set(self, i: int, value: np.float64):
+        idx = self._indices.searchsorted(i)
+        if idx < len(self._indices) and self._indices[idx] == i:
+            self._values[idx] = value
+        elif value != 0:
+            assert i < self._size
+            cur_len = len(self._indices)
+            indices = np.zeros(cur_len + 1, dtype=np.int32)
+            values = np.zeros(cur_len + 1, dtype=np.float64)
+            indices[0:idx] = self._indices[0:idx]
+            values[0:idx] = self._values[0:idx]
+            indices[idx] = i
+            values[idx] = value
+            indices[idx + 1:] = self._indices[idx:]
+            values[idx + 1:] = self._values[idx]
+            self._indices = indices
+            self._values = values
 
     def to_array(self) -> np.ndarray:
         """
         Returns a copy of this SparseVector as a 1-dimensional NumPy array.
         """
         arr = np.zeros((self._size,), dtype=np.float64)
         arr[self._indices] = self._values
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/core/param.py` & `apache-flink-ml-2.2.0/pyflink/ml/param.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from abc import ABC, abstractmethod
 from typing import TypeVar, Generic, List, Dict, Any, Optional, Tuple, Union
+from pyflink.ml.linalg import Vector
+from pyflink.ml.common.window import Windows
 
 import jsonpickle
 
 T = TypeVar('T')
 V = TypeVar('V')
 
 
@@ -82,15 +84,15 @@
         Returns a map which maps parameter definition to parameter value.
         """
         pass
 
     @staticmethod
     def _is_compatible_type(param: 'Param[V]', value: V) -> bool:
         if value is not None and param.type != type(value):
-            return False
+            return issubclass(type(value), param.type)
         if isinstance(value, list):
             for item in value:
                 if param.type_name != f'list[{type(item).__name__}]':
                     return False
             return True
         return True
 
@@ -374,7 +376,29 @@
     Class for the string array parameter.
     """
 
     def __init__(self, name: str, description: str, default_value: Optional[Tuple[str, ...]],
                  validator: ParamValidator[Tuple[str, ...]] = ParamValidators.always_true()):
         super(StringArrayParam, self).__init__(name, tuple, "Tuple[str]", description,
                                                default_value, validator)
+
+
+class VectorParam(Param[Vector]):
+    """
+    Class for the vector parameter.
+    """
+
+    def __init__(self, name: str, description: str, default_value: Optional[Vector],
+                 validator: ParamValidator[Vector] = ParamValidators.always_true()):
+        super(VectorParam, self).__init__(name, Vector, "str", description, default_value,
+                                          validator)
+
+
+class WindowsParam(Param[Windows]):
+    """
+    Class for the Windows parameter.
+    """
+
+    def __init__(self, name: str, description: str, default_value: Optional[Windows],
+                 validator: ParamValidator[Windows] = ParamValidators.always_true()):
+        super(WindowsParam, self).__init__(name, Windows, "str", description, default_value,
+                                           validator)
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/common.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC, abstractmethod
 
-from pyflink.ml.core.wrapper import JavaModel, JavaEstimator
+from pyflink.ml.wrapper import JavaModel, JavaEstimator
 
 JAVA_CLASSIFICATION_PACKAGE_NAME = "org.apache.flink.ml.classification"
 
 
 class JavaClassificationModel(JavaModel, ABC):
     """
     Wrapper class for a Java Classification Model.
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/knn.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/knn.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC
 
 import typing
 
-from pyflink.ml.core.param import Param, IntParam, ParamValidators
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.classification.common import (JavaClassificationModel,
-                                                  JavaClassificationEstimator)
-from pyflink.ml.lib.param import HasFeaturesCol, HasPredictionCol, HasLabelCol
+from pyflink.ml.param import Param, IntParam, ParamValidators
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.classification.common import (JavaClassificationModel,
+                                              JavaClassificationEstimator)
+from pyflink.ml.common.param import HasFeaturesCol, HasPredictionCol, HasLabelCol
 
 
 class _KNNModelParams(
     JavaWithParams,
     HasFeaturesCol,
     HasPredictionCol,
     ABC
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/linearsvc.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/linearsvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 from abc import ABC
 
-from pyflink.ml.core.param import Param, ParamValidators, FloatParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.classification.common import (JavaClassificationModel,
-                                                  JavaClassificationEstimator)
-from pyflink.ml.lib.param import (HasFeaturesCol, HasPredictionCol, HasLabelCol,
-                                  HasRawPredictionCol, HasWeightCol, HasMaxIter, HasReg,
-                                  HasElasticNet, HasLearningRate, HasGlobalBatchSize, HasTol)
+from pyflink.ml.param import Param, ParamValidators, FloatParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.classification.common import (JavaClassificationModel,
+                                              JavaClassificationEstimator)
+from pyflink.ml.common.param import (HasFeaturesCol, HasPredictionCol, HasLabelCol,
+                                     HasRawPredictionCol, HasWeightCol, HasMaxIter, HasReg,
+                                     HasElasticNet, HasLearningRate, HasGlobalBatchSize, HasTol)
 
 
 class _LinearSVCModelParams(
     JavaWithParams,
     HasFeaturesCol,
     HasPredictionCol,
     HasRawPredictionCol,
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/logisticregression.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/logisticregression.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC
 
-from pyflink.ml.core.param import (ParamValidators, Param, StringParam, FloatParam)
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.classification.common import (JavaClassificationModel,
-                                                  JavaClassificationEstimator)
-from pyflink.ml.lib.param import (HasWeightCol, HasMaxIter, HasReg, HasLearningRate,
-                                  HasGlobalBatchSize, HasTol, HasMultiClass, HasFeaturesCol,
-                                  HasPredictionCol, HasRawPredictionCol, HasLabelCol,
-                                  HasBatchStrategy, HasElasticNet)
+from pyflink.ml.param import (ParamValidators, Param, StringParam, FloatParam)
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.classification.common import (JavaClassificationModel,
+                                              JavaClassificationEstimator)
+from pyflink.ml.common.param import (HasWeightCol, HasMaxIter, HasReg, HasLearningRate,
+                                     HasGlobalBatchSize, HasTol, HasMultiClass, HasFeaturesCol,
+                                     HasPredictionCol, HasRawPredictionCol, HasLabelCol,
+                                     HasBatchStrategy, HasElasticNet)
 
 
 class _LogisticRegressionModelParams(
     JavaWithParams,
     HasFeaturesCol,
     HasPredictionCol,
     HasRawPredictionCol,
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/classification/naivebayes.py` & `apache-flink-ml-2.2.0/pyflink/ml/classification/naivebayes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC
 
 import typing
 
-from pyflink.ml.core.param import Param, StringParam, ParamValidators, FloatParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.classification.common import (JavaClassificationModel,
-                                                  JavaClassificationEstimator)
-from pyflink.ml.lib.param import HasFeaturesCol, HasPredictionCol, HasLabelCol
+from pyflink.ml.param import Param, StringParam, ParamValidators, FloatParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.classification.common import (JavaClassificationModel,
+                                              JavaClassificationEstimator)
+from pyflink.ml.common.param import HasFeaturesCol, HasPredictionCol, HasLabelCol
 
 
 class _NaiveBayesModelParams(
     JavaWithParams,
     HasFeaturesCol,
     HasPredictionCol,
     ABC
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/common/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/common.py` & `apache-flink-ml-2.2.0/pyflink/ml/regression/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC, abstractmethod
 
-from pyflink.ml.core.wrapper import JavaModel, JavaEstimator
+from pyflink.ml.wrapper import JavaModel, JavaEstimator
 
-JAVA_CLUSTERING_PACKAGE_NAME = "org.apache.flink.ml.clustering"
+JAVA_REGRESSION_PACKAGE_NAME = "org.apache.flink.ml.regression"
 
 
-class JavaClusteringModel(JavaModel, ABC):
+class JavaRegressionModel(JavaModel, ABC):
     """
-    Wrapper class for a Java Clustering Model.
+    Wrapper class for a Java Regression Model.
     """
 
     def __init__(self, java_model):
-        super(JavaClusteringModel, self).__init__(java_model)
+        super(JavaRegressionModel, self).__init__(java_model)
 
     @classmethod
     def _java_stage_path(cls) -> str:
         return ".".join(
-            [JAVA_CLUSTERING_PACKAGE_NAME,
+            [JAVA_REGRESSION_PACKAGE_NAME,
              cls._java_model_package_name(),
              cls._java_model_class_name()])
 
     @classmethod
     @abstractmethod
     def _java_model_package_name(cls) -> str:
         pass
 
     @classmethod
     @abstractmethod
     def _java_model_class_name(cls) -> str:
         pass
 
 
-class JavaClusteringEstimator(JavaEstimator, ABC):
+class JavaRegressionEstimator(JavaEstimator, ABC):
     """
-    Wrapper class for a Java Clustering Estimator.
+    Wrapper class for a Java Regression Estimator.
     """
 
     def __init__(self):
-        super(JavaClusteringEstimator, self).__init__()
+        super(JavaRegressionEstimator, self).__init__()
 
     @classmethod
     def _java_stage_path(cls):
         return ".".join(
-            [JAVA_CLUSTERING_PACKAGE_NAME,
+            [JAVA_REGRESSION_PACKAGE_NAME,
              cls._java_estimator_package_name(),
              cls._java_estimator_class_name()])
 
     @classmethod
     @abstractmethod
     def _java_estimator_package_name(cls) -> str:
         pass
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/clustering/kmeans.py` & `apache-flink-ml-2.2.0/pyflink/ml/clustering/kmeans.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC
 
 import typing
 
-from pyflink.ml.core.param import ParamValidators, Param, IntParam, StringParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.clustering.common import JavaClusteringModel, JavaClusteringEstimator
-from pyflink.ml.lib.param import (HasDistanceMeasure, HasFeaturesCol, HasPredictionCol,
-                                  HasBatchStrategy, HasGlobalBatchSize, HasDecayFactor, HasSeed,
-                                  HasMaxIter)
+from pyflink.ml.param import ParamValidators, Param, IntParam, StringParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.clustering.common import JavaClusteringModel, JavaClusteringEstimator
+from pyflink.ml.common.param import (HasDistanceMeasure, HasFeaturesCol, HasPredictionCol,
+                                     HasBatchStrategy, HasGlobalBatchSize, HasDecayFactor, HasSeed,
+                                     HasMaxIter)
 
 
 class _KMeansModelParams(
     JavaWithParams,
     HasDistanceMeasure,
     HasFeaturesCol,
     HasPredictionCol,
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/binaryclassificationevaluator.py` & `apache-flink-ml-2.2.0/pyflink/ml/evaluation/binaryclassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 from typing import Tuple
 
-from pyflink.ml.core.param import Param, StringArrayParam, ParamValidators
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.evaluation.common import JavaEvaluationAlgoOperator
-from pyflink.ml.lib.param import HasLabelCol, HasRawPredictionCol, HasWeightCol
+from pyflink.ml.param import Param, StringArrayParam, ParamValidators
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.evaluation.common import JavaEvaluationAlgoOperator
+from pyflink.ml.common.param import HasLabelCol, HasRawPredictionCol, HasWeightCol
 
 
 class _BinaryClassificationEvaluatorParams(
     JavaWithParams,
     HasLabelCol,
     HasRawPredictionCol,
     HasWeightCol
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/evaluation/common.py` & `apache-flink-ml-2.2.0/pyflink/ml/evaluation/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC, abstractmethod
 
-from pyflink.ml.core.wrapper import JavaAlgoOperator
+from pyflink.ml.wrapper import JavaAlgoOperator
 
 JAVA_EVALUATION_PACKAGE_NAME = "org.apache.flink.ml.evaluation"
 
 
 class JavaEvaluationAlgoOperator(JavaAlgoOperator, ABC):
     """
     Wrapper class for a Java Feature Transformer.
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/bucketizer.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/bucketizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 from typing import Tuple
 
-from pyflink.ml.core.param import Param, FloatArrayArrayParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureTransformer
-from pyflink.ml.lib.param import HasInputCols, HasOutputCols, HasHandleInvalid
+from pyflink.ml.param import Param, FloatArrayArrayParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.feature.common import JavaFeatureTransformer
+from pyflink.ml.common.param import HasInputCols, HasOutputCols, HasHandleInvalid
 
 
 class _BucketizerParams(
     JavaWithParams,
     HasInputCols,
     HasOutputCols,
     HasHandleInvalid
 ):
     """
-    Params for :class:`StandardScaler`.
+    Params for :class:`Bucketizer`.
     """
 
     SPLITS_ARRAY: Param[Tuple[float, ...]] = FloatArrayArrayParam(
         "splits_array",
         "Array of split points for mapping continuous features into buckets.",
         None)
 
@@ -51,15 +51,15 @@
     @property
     def split_array(self):
         return self.get_split_array()
 
 
 class Bucketizer(JavaFeatureTransformer, _BucketizerParams):
     """
-    Bucketizer is a transformer that maps multiple columns of continuous features to multiple
+    A Transformer that maps multiple columns of continuous features to multiple
     columns of discrete features, i.e., buckets indices. The indices are in
     [0, numSplitsInThisColumn - 1].
 
     The `keep` option of HasHandleInvalid means that we put the invalid data in the last
     bucket of the splits, whose index is the number of the buckets.
     """
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/common.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC, abstractmethod
 
-from pyflink.ml.core.wrapper import JavaModel, JavaEstimator, JavaTransformer
+from pyflink.ml.wrapper import JavaModel, JavaEstimator, JavaTransformer
 
 JAVA_FEATURE_PACKAGE_NAME = "org.apache.flink.ml.feature"
 
 
 class JavaFeatureTransformer(JavaTransformer, ABC):
     """
     Wrapper class for a Java Feature Transformer.
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/minmaxscaler.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/minmaxscaler.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 
-from pyflink.ml.core.param import Param, FloatParam, ParamValidators
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureModel, JavaFeatureEstimator
-from pyflink.ml.lib.param import HasInputCol, HasOutputCol
+from pyflink.ml.param import Param, FloatParam, ParamValidators
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.feature.common import JavaFeatureModel, JavaFeatureEstimator
+from pyflink.ml.common.param import HasInputCol, HasOutputCol
 
 
 class _MinMaxScalerParams(
     JavaWithParams,
     HasInputCol,
     HasOutputCol
 ):
@@ -66,16 +66,15 @@
     @property
     def max(self):
         return self.get_max()
 
 
 class MinMaxScalerModel(JavaFeatureModel, _MinMaxScalerParams):
     """
-    * A Model which do a minMax scaler operation using the model data computed
-    by :class:`MinMaxScaler`.
+    A Model which transforms data using the model data computed by :class:`MinMaxScaler`.
     """
 
     def __init__(self, java_model=None):
         super(MinMaxScalerModel, self).__init__(java_model)
 
     @classmethod
     def _java_model_package_name(cls) -> str:
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/onehotencoder.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/onehotencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 
-from pyflink.ml.core.param import Param, BooleanParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureEstimator, JavaFeatureModel
-from pyflink.ml.lib.param import (HasInputCols, HasOutputCols, HasHandleInvalid)
+from pyflink.ml.param import Param, BooleanParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.feature.common import JavaFeatureEstimator, JavaFeatureModel
+from pyflink.ml.common.param import (HasInputCols, HasOutputCols, HasHandleInvalid)
 
 
 class _OneHotEncoderParams(
     JavaWithParams,
     HasInputCols,
     HasOutputCols,
     HasHandleInvalid
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/standardscaler.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/standardscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 
-from pyflink.ml.core.param import Param, BooleanParam
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureEstimator, JavaFeatureModel
-from pyflink.ml.lib.param import HasInputCol, HasOutputCol
+from pyflink.ml.param import Param, BooleanParam
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.feature.common import JavaFeatureEstimator, JavaFeatureModel
+from pyflink.ml.common.param import HasInputCol, HasOutputCol
 
 
 class _StandardScalerParams(
     JavaWithParams,
     HasInputCol,
     HasOutputCol
 ):
@@ -84,15 +84,15 @@
 
 
 class StandardScaler(JavaFeatureEstimator, _StandardScalerParams):
     """
     An Estimator which implements the standard scaling algorithm.
 
     Standardization is a common requirement for machine learning training because they may behave
-    badly if the individual features of a input do not look like standard normally distributed data
+    badly if the individual features of an input do not look like standard normally distributed data
     (e.g. Gaussian with 0 mean and unit variance).
 
     This estimator standardizes the input features by removing the mean and scaling each dimension
     to unit variance.
     """
 
     def __init__(self):
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/stringindexer.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/stringindexer.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 import typing
 
-from pyflink.ml.core.param import Param, StringParam, ParamValidators
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureModel, JavaFeatureEstimator
-from pyflink.ml.lib.param import HasInputCols, HasOutputCols, HasHandleInvalid
+from pyflink.ml.param import Param, IntParam, StringParam, ParamValidators
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.feature.common import JavaFeatureModel, JavaFeatureEstimator
+from pyflink.ml.common.param import HasInputCols, HasOutputCols, HasHandleInvalid
 
 
 class _IndexToStringModelParams(
     JavaWithParams,
     HasInputCols,
     HasOutputCols
 ):
@@ -58,27 +58,44 @@
     STRING_ORDER_TYPE: Param[str] = StringParam(
         "string_order_type",
         "How to order strings of each column.",
         "arbitrary",
         ParamValidators.in_array(
             ['arbitrary', 'frequencyDesc', 'frequencyAsc', 'alphabetDesc', 'alphabetAsc']))
 
+    MAX_INDEX_NUM: Param[int] = IntParam(
+        "max_index_num",
+        "The max number of indices for each column. It only works when "
+        + "'stringOrderType' is set as 'frequencyDesc'.",
+        2 ** 31 - 1,
+        ParamValidators.gt(1))
+
     def __init__(self, java_params):
         super(_StringIndexerParams, self).__init__(java_params)
 
     def set_string_order_type(self, value: str):
         return typing.cast(_StringIndexerParams, self.set(self.STRING_ORDER_TYPE, value))
 
     def get_string_order_type(self) -> str:
         return self.get(self.STRING_ORDER_TYPE)
 
+    def set_max_index_num(self, value: int):
+        return typing.cast(_StringIndexerParams, self.set(self.MAX_INDEX_NUM, value))
+
+    def get_max_index_num(self) -> int:
+        return self.get(self.MAX_INDEX_NUM)
+
     @property
     def string_order_type(self):
         return self.get_string_order_type()
 
+    @property
+    def max_index_num(self):
+        return self.get_max_index_num()
+
 
 class IndexToStringModel(JavaFeatureModel, _IndexToStringModelParams):
     """
     A Model which transforms input index column(s) to string column(s) using the model data computed
     by :class:StringIndexer. It is a reverse operation of :class:StringIndexerModel.
     """
 
@@ -95,16 +112,16 @@
 
 
 class StringIndexerModel(JavaFeatureModel, _StringIndexerModelParams):
     """
     A Model which transforms input string/numeric column(s) to integer column(s) using the model
     data computed by :class:StringIndexer.
 
-    The `keep` option of {@link HasHandleInvalid} means that we put the invalid entries in a
-    special bucket, whose index is the number of distinct values in this column.
+    The `keep` option of {@link HasHandleInvalid} means that we transform the invalid input
+    into a special index, whose value is the number of distinct values in this column.
     """
 
     def __init__(self, java_model=None):
         super(StringIndexerModel, self).__init__(java_model)
 
     @classmethod
     def _java_model_package_name(cls) -> str:
@@ -124,16 +141,20 @@
     their corresponding input columns are the same. The indices are in [0,
     numDistinctValuesInThisColumn].
 
     The input columns are cast to string if they are numeric values. By default, the output model
     is arbitrarily ordered. Users can control this by setting {@link
     StringIndexerParams#STRING_ORDER_TYPE}.
 
-    The `keep` option of {@link HasHandleInvalid} means that we put the invalid entries in a
-    special bucket, whose index is the number of distinct values in this column.
+    User can also control the max number of output indices by setting {@link
+    StringIndexerParams#MAX_INDEX_NUM}. This parameter only works if {@link
+    StringIndexerParams#STRING_ORDER_TYPE} is set as 'frequencyDesc'.
+
+    The `keep` option of {@link HasHandleInvalid} means that we transform the invalid input
+    into a special index, whose value is the number of distinct values in this column.
     """
 
     def __init__(self):
         super(StringIndexer, self).__init__()
 
     @classmethod
     def _create_model(cls, java_model) -> StringIndexerModel:
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/feature/vectorassembler.py` & `apache-flink-ml-2.2.0/pyflink/ml/feature/normalizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,46 +11,59 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
+import typing
 
-from pyflink.ml.core.wrapper import JavaWithParams
-from pyflink.ml.lib.feature.common import JavaFeatureTransformer
-from pyflink.ml.lib.param import HasInputCols, HasOutputCol, HasHandleInvalid
+from pyflink.ml.wrapper import JavaWithParams
+from pyflink.ml.param import FloatParam, ParamValidators
+from pyflink.ml.feature.common import JavaFeatureTransformer
+from pyflink.ml.common.param import HasInputCol, HasOutputCol, Param
 
 
-class _VectorAssemblerParams(
+class _NormalizerParams(
     JavaWithParams,
-    HasInputCols,
-    HasOutputCol,
-    HasHandleInvalid
+    HasInputCol,
+    HasOutputCol
 ):
     """
-    Params for :class:`VectorAssembler`.
+    Params for :class:`Normalizer`.
     """
 
+    P: Param[float] = FloatParam(
+        "p",
+        "The p norm value.",
+        2.0,
+        ParamValidators.gt_eq(1.0))
+
     def __init__(self, java_params):
-        super(_VectorAssemblerParams, self).__init__(java_params)
+        super(_NormalizerParams, self).__init__(java_params)
 
+    def set_p(self, value: float):
+        return typing.cast(_NormalizerParams, self.set(self.P, value))
 
-class VectorAssembler(JavaFeatureTransformer, _VectorAssemblerParams):
-    """
-    A feature transformer that combines a given list of input columns into a vector column. Types of
-    input columns must be either vector or numerical value.
+    def get_p(self) -> float:
+        return self.get(self.P)
+
+    @property
+    def p(self):
+        return self.get_p()
 
-    The `keep` option of :class:HasHandleInvalid means that we output bad rows with output column
-    set to null.
+
+class Normalizer(JavaFeatureTransformer, _NormalizerParams):
+    """
+    A Transformer that normalizes a vector to have unit norm using the given p-norm.
     """
 
     def __init__(self, java_model=None):
-        super(VectorAssembler, self).__init__(java_model)
+        super(Normalizer, self).__init__(java_model)
 
     @classmethod
     def _java_transformer_package_name(cls) -> str:
-        return "vectorassembler"
+        return "normalizer"
 
     @classmethod
     def _java_transformer_class_name(cls) -> str:
-        return "VectorAssembler"
+        return "Normalizer"
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/lib/param.py` & `apache-flink-ml-2.2.0/pyflink/ml/common/param.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 from abc import ABC
 from typing import Tuple
 
-from pyflink.ml.core.param import WithParams, Param, ParamValidators, StringParam, IntParam, \
-    StringArrayParam, FloatParam
+from pyflink.ml.param import WithParams, Param, ParamValidators, StringParam, IntParam, \
+    StringArrayParam, FloatParam, WindowsParam, BooleanParam
+from pyflink.ml.common.window import Windows, GlobalWindows
 
 
 class HasDistanceMeasure(WithParams, ABC):
     """
     Base class for the shared distance_measure param.
     """
     DISTANCE_MEASURE: Param[str] = StringParam(
         "distance_measure",
-        "Distance measure. Supported options: 'euclidean' and 'cosine'.",
+        "Distance measure. Supported options: 'euclidean', 'manhattan' and 'cosine'.",
         "euclidean",
-        ParamValidators.in_array(['euclidean', 'cosine']))
+        ParamValidators.in_array(['euclidean', 'manhattan', 'cosine']))
 
     def set_distance_measure(self, distance_measure: str):
         return self.set(self.DISTANCE_MEASURE, distance_measure)
 
     def get_distance_measure(self) -> str:
         return self.get(self.DISTANCE_MEASURE)
 
@@ -42,14 +43,17 @@
     def distance_measure(self) -> str:
         return self.get_distance_measure()
 
 
 class HasFeaturesCol(WithParams, ABC):
     """
     Base class for the shared feature_col param.
+
+    `HasFeaturesCol` is typically used for `Stage`s that implement `HasLabelCol`. It is preferred
+    to use `HasInputCol` for other cases.
     """
     FEATURES_COL: Param[str] = StringParam(
         "features_col",
         "Features column name.",
         "features",
         ParamValidators.not_null())
 
@@ -151,14 +155,56 @@
         return self.get(self.INPUT_COLS)
 
     @property
     def input_cols(self) -> Tuple[str, ...]:
         return self.get_input_cols()
 
 
+class HasCategoricalCols(WithParams, ABC):
+    """
+    Base class for the shared categorical cols param.
+    """
+    CATEGORICAL_COLS: Param[Tuple[str, ...]] = StringArrayParam(
+        "categorical_cols",
+        "Categorical column names.",
+        [],
+        ParamValidators.not_null())
+
+    def set_categorical_cols(self, *cols: str):
+        return self.set(self.CATEGORICAL_COLS, cols)
+
+    def get_categorical_cols(self) -> Tuple[str, ...]:
+        return self.get(self.CATEGORICAL_COLS)
+
+    @property
+    def categorical_cols(self) -> Tuple[str, ...]:
+        return self.get_categorical_cols()
+
+
+class HasNumFeatures(WithParams, ABC):
+    """
+    Base class for the shared numFeatures param.
+    """
+    NUM_FEATURES: Param[int] = IntParam(
+        "num_features",
+        "Number of features.",
+        262144,
+        ParamValidators.gt(0))
+
+    def set_num_features(self, num_features: int):
+        return self.set(self.NUM_FEATURES, num_features)
+
+    def get_num_features(self) -> int:
+        return self.get(self.NUM_FEATURES)
+
+    @property
+    def num_features(self) -> int:
+        return self.get_num_features()
+
+
 class HasLabelCol(WithParams, ABC):
     """
     Base class for the shared label column param.
     """
     LABEL_COL: Param[str] = StringParam(
         "label_col",
         "Label column name.",
@@ -467,7 +513,117 @@
 
     def get_elastic_net(self) -> float:
         return self.get(self.ELASTIC_NET)
 
     @property
     def elastic_net(self):
         return self.get(self.ELASTIC_NET)
+
+
+class HasWindows(WithParams, ABC):
+    """
+    Base class for the shared windows param.
+    """
+    WINDOWS: Param[Windows] = WindowsParam(
+        "windows",
+        "Windowing strategy that determines how to create mini-batches from input data.",
+        GlobalWindows(),
+        ParamValidators.not_null())
+
+    def set_windows(self, value: Windows):
+        self.set(self.WINDOWS, value)
+        return self
+
+    def get_windows(self) -> Windows:
+        return self.get(self.WINDOWS)
+
+    @property
+    def windows(self):
+        return self.get(self.WINDOWS)
+
+
+class HasRelativeError(WithParams, ABC):
+    """
+    Interface for shared param relativeError.
+    """
+    RELATIVE_ERROR: Param[float] = FloatParam(
+        "relative_error",
+        "The relative target precision for the approximate quantile algorithm.",
+        0.001,
+        ParamValidators.in_range(0.0, 1.0))
+
+    def set_relative_error(self, value: float):
+        return self.set(self.RELATIVE_ERROR, value)
+
+    def get_relative_error(self) -> float:
+        return self.get(self.RELATIVE_ERROR)
+
+    @property
+    def relative_error(self):
+        return self.get(self.RELATIVE_ERROR)
+
+
+class HasFlatten(WithParams, ABC):
+    """
+    Interface for shared flatten param.
+    """
+    FLATTEN: Param[bool] = BooleanParam(
+        "flatten",
+        "If false, the returned table contains only a single row, otherwise, one row per feature.",
+        False
+    )
+
+    def set_flatten(self, value: bool):
+        return self.set(self.FLATTEN, value)
+
+    def get_flatten(self) -> bool:
+        return self.get(self.FLATTEN)
+
+    @property
+    def flatten(self):
+        return self.get(self.FLATTEN)
+
+
+class HasModelVersionCol(WithParams, ABC):
+    """
+    Interface for the shared model version column param.
+    """
+    MODEL_VERSION_COL: Param[str] = StringParam(
+        "model_version_col",
+        "The name of the column which contains the version of the model data that "
+        "the input data is predicted with. The version should be a 64-bit integer.",
+        "version"
+    )
+
+    def set_model_version_col(self, value: str):
+        return self.set(self.MODEL_VERSION_COL, value)
+
+    def get_model_version_col(self) -> str:
+        return self.get(self.MODEL_VERSION_COL)
+
+    @property
+    def model_version_col(self):
+        return self.get_model_version_col()
+
+
+class HasMaxAllowedModelDelayMs(WithParams, ABC):
+    """
+    Interface for the shared max allowed model delay in milliseconds param.
+    """
+    MAX_ALLOWED_MODEL_DELAY_MS: Param[int] = IntParam(
+        "max_allowed_model_delay_ms",
+        "The maximum difference allowed between the timestamps of the input record "
+        "and the model data that is used to predict that input record. "
+        "This param only works when the input contains event time.",
+        0,
+        ParamValidators.gt_eq(0)
+    )
+
+    def set_max_allowed_model_delay_ms(self, value: int):
+        return self.set(self.MAX_ALLOWED_MODEL_DELAY_MS, value)
+
+    def get_max_allowed_model_delay_ms(self) -> int:
+        return self.get(self.MAX_ALLOWED_MODEL_DELAY_MS)
+
+    @property
+    def max_allowed_model_delay_ms(self):
+        return self.get_max_allowed_model_delay_ms()
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/util/__init__.py` & `apache-flink-ml-2.2.0/pyflink/ml/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/util/read_write_utils.py` & `apache-flink-ml-2.2.0/pyflink/ml/util/read_write_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import time
 from importlib import import_module
 from typing import List, Dict, Any
 
 import cloudpickle
 from pyflink.table import StreamTableEnvironment
 
-from pyflink.ml.core.api import Stage
+from pyflink.ml.api import Stage
 
 
 def save_pipeline(pipeline: Stage, stages: List[Stage], path: str) -> None:
     """
     Saves a Pipeline or PipelineModel with the given list of stages to the given path.
 
     :param pipeline: A Pipeline or PipelineModel instance.
```

### Comparing `apache-flink-ml-2.1.0/pyflink/ml/version.py` & `apache-flink-ml-2.2.0/pyflink/ml/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # limitations under the License.
 ################################################################################
 
 """
 The version will be consistent with the flink ml version and follow the PEP440.
 .. seealso:: https://www.python.org/dev/peps/pep-0440
 """
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

### Comparing `apache-flink-ml-2.1.0/setup.py` & `apache-flink-ml-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 from platform import python_version
 from shutil import copytree, rmtree
 
 from setuptools import setup
 
-if sys.version_info < (3, 6) or sys.version_info > (3, 8):
+if sys.version_info < (3, 6) or sys.version_info >= (3, 9):
     print("Only Python versions between 3.6 and 3.8 (inclusive) are supported for Flink ML. "
           "The current Python version is %s." % python_version(), file=sys.stderr)
     sys.exit(-1)
 
 
 def remove_if_exists(file_path):
     if os.path.exists(file_path):
@@ -51,68 +51,79 @@
 VERSION = __version__  # noqa
 
 with io.open(os.path.join(this_directory, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 TEMP_PATH = "deps"
 
+LIB_TEMP_PATH = os.path.join(TEMP_PATH, "lib")
 EXAMPLES_TEMP_PATH = os.path.join(TEMP_PATH, "examples")
 
 in_flink_ml_source = os.path.isfile("../flink-ml-core/src/main/java/org/apache/flink/ml/api/"
                                     "Stage.java")
 try:
     if in_flink_ml_source:
 
         try:
             os.mkdir(TEMP_PATH)
         except:
             print("Temp path for symlink to parent already exists {0}".format(TEMP_PATH),
                   file=sys.stderr)
             sys.exit(-1)
         flink_ml_version = VERSION.replace(".dev0", "-SNAPSHOT")
+        FLINK_ML_HOME = os.path.abspath(
+            "../flink-ml-dist/target/flink-ml-%s-bin/flink-ml-%s"
+            % (flink_ml_version, flink_ml_version))
         FLINK_ML_ROOT = os.path.abspath("..")
 
+        LIB_PATH = os.path.join(FLINK_ML_HOME, "lib")
         EXAMPLES_PATH = os.path.join(this_directory, "pyflink/examples")
 
-        try:
+        if getattr(os, "symlink", None) is not None:
+            os.symlink(LIB_PATH, LIB_TEMP_PATH)
             os.symlink(EXAMPLES_PATH, EXAMPLES_TEMP_PATH)
-        except BaseException:  # pylint: disable=broad-except
+        else:
+            copytree(LIB_PATH, LIB_TEMP_PATH)
             copytree(EXAMPLES_PATH, EXAMPLES_TEMP_PATH)
 
     PACKAGES = ['pyflink',
                 'pyflink.ml',
-                'pyflink.ml.core',
-                'pyflink.ml.lib',
-                'pyflink.ml.lib.classification',
-                'pyflink.ml.lib.clustering',
-                'pyflink.ml.lib.evaluation',
-                'pyflink.ml.lib.feature',
-                'pyflink.ml.lib',
+                'pyflink.ml.classification',
+                'pyflink.ml.clustering',
+                'pyflink.ml.evaluation',
+                'pyflink.ml.feature',
+                'pyflink.ml.recommendation',
+                'pyflink.ml.regression',
+                'pyflink.ml.stats',
                 'pyflink.ml.util',
+                'pyflink.ml.common',
+                'pyflink.lib',
                 'pyflink.examples']
 
     PACKAGE_DIR = {
+        'pyflink.lib': TEMP_PATH + '/lib',
         'pyflink.examples': TEMP_PATH + '/examples'}
 
     PACKAGE_DATA = {
+        'pyflink.lib': ['*.jar'],
         'pyflink.examples': ['*.py', '*/*.py']}
 
     setup(
         name='apache-flink-ml',
         version=VERSION,
         packages=PACKAGES,
         include_package_data=True,
         package_dir=PACKAGE_DIR,
         package_data=PACKAGE_DATA,
         url='https://flink.apache.org',
         license='https://www.apache.org/licenses/LICENSE-2.0',
         author='Apache Software Foundation',
         author_email='dev@flink.apache.org',
         python_requires='>=3.6',
-        install_requires=['apache-flink==1.15.0', 'pandas>=1.0,<1.2.0', 'jsonpickle==2.0.0',
+        install_requires=['apache-flink==1.15.1', 'pandas>=1.0,<1.2.0', 'jsonpickle==2.0.0',
                           'cloudpickle==1.2.2', 'numpy>=1.14.3,<1.20'],
         tests_require=['pytest==4.4.1'],
         description='Apache Flink ML Python API',
         long_description=long_description,
         long_description_content_type='text/markdown',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

