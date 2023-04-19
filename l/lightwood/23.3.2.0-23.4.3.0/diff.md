# Comparing `tmp/lightwood-23.3.2.0.tar.gz` & `tmp/lightwood-23.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightwood-23.3.2.0.tar", last modified: Tue Mar 14 23:07:29 2023, max compression
+gzip compressed data, was "dist/lightwood-23.4.3.0.tar", last modified: Wed Apr 19 01:28:40 2023, max compression
```

## Comparing `lightwood-23.3.2.0.tar` & `lightwood-23.4.3.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    18289 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-14 23:07:28.000000 lightwood-23.3.2.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 23:07:28.000000 lightwood-23.3.2.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-14 23:07:28.000000 lightwood-23.3.2.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 23:07:28.000000 lightwood-23.3.2.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 23:07:29.000000 lightwood-23.3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-14 23:07:19.000000 lightwood-23.3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/categorical/onehot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 01:28:39.000000 lightwood-23.4.3.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 01:28:40.000000 lightwood-23.4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 01:28:29.000000 lightwood-23.4.3.0/setup.py
```

### Comparing `lightwood-23.3.2.0/PKG-INFO` & `lightwood-23.4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.3.2.0
+Version: 23.4.3.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -217,14 +217,14 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: image
-Provides-Extra: xai
-Provides-Extra: extra
-Provides-Extra: quantum
 Provides-Extra: extra_ts
+Provides-Extra: quantum
 Provides-Extra: audio
+Provides-Extra: extra
+Provides-Extra: image
+Provides-Extra: xai
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.3.2.0/README.md` & `lightwood-23.4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/__init__.py` & `lightwood-23.4.3.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/analyze.py` & `lightwood-23.4.3.0/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/base.py` & `lightwood-23.4.3.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/explain.py` & `lightwood-23.4.3.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.4.3.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.4.3.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.4.3.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.4.3.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.4.3.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/base.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/icp.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/nc.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/norm.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nc/util.py` & `lightwood-23.4.3.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.4.3.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/api/__init__.py` & `lightwood-23.4.3.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/api/high_level.py` & `lightwood-23.4.3.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/api/json_ai.py` & `lightwood-23.4.3.0/lightwood/api/json_ai.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/api/predictor.py` & `lightwood-23.4.3.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/api/types.py` & `lightwood-23.4.3.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/data/encoded_ds.py` & `lightwood-23.4.3.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/data/timeseries_analyzer.py` & `lightwood-23.4.3.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/data/timeseries_transform.py` & `lightwood-23.4.3.0/lightwood/data/timeseries_transform.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/__init__.py` & `lightwood-23.4.3.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/array/array.py` & `lightwood-23.4.3.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.4.3.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.4.3.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.4.3.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/base.py` & `lightwood-23.4.3.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.4.3.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.4.3.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.4.3.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.4.3.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.4.3.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.4.3.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.4.3.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/helpers.py` & `lightwood-23.4.3.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/identity/identity.py` & `lightwood-23.4.3.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.4.3.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.4.3.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.4.3.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.4.3.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.4.3.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.4.3.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.4.3.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/rnn.py` & `lightwood-23.4.3.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/short.py` & `lightwood-23.4.3.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.4.3.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/text/vocab.py` & `lightwood-23.4.3.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.4.3.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.4.3.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.4.3.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/__init__.py` & `lightwood-23.4.3.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/base.py` & `lightwood-23.4.3.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/best_of.py` & `lightwood-23.4.3.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.4.3.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.4.3.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.4.3.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.4.3.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.4.3.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/__init__.py` & `lightwood-23.4.3.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/device.py` & `lightwood-23.4.3.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/general.py` & `lightwood-23.4.3.0/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/io.py` & `lightwood-23.4.3.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/log.py` & `lightwood-23.4.3.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/parallelism.py` & `lightwood-23.4.3.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/templating.py` & `lightwood-23.4.3.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/text.py` & `lightwood-23.4.3.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/torch.py` & `lightwood-23.4.3.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/helpers/ts.py` & `lightwood-23.4.3.0/lightwood/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/__init__.py` & `lightwood-23.4.3.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/arima.py` & `lightwood-23.4.3.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/base.py` & `lightwood-23.4.3.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/ets.py` & `lightwood-23.4.3.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/gluonts.py` & `lightwood-23.4.3.0/lightwood/mixer/gluonts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/helpers/ts.py` & `lightwood-23.4.3.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/lightgbm.py` & `lightwood-23.4.3.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.4.3.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/neural.py` & `lightwood-23.4.3.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/neural_ts.py` & `lightwood-23.4.3.0/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/nhits.py` & `lightwood-23.4.3.0/lightwood/mixer/nhits.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/prophet.py` & `lightwood-23.4.3.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/qclassic.py` & `lightwood-23.4.3.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/random_forest.py` & `lightwood-23.4.3.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/regression.py` & `lightwood-23.4.3.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/sktime.py` & `lightwood-23.4.3.0/lightwood/mixer/sktime.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,20 @@
             series = series_data[self.target]
             if series_data.size > self.ts_analysis['tss'].window:
                 series = series.sort_index(ascending=True)
                 series = series.reset_index(drop=True)
                 series = series.loc[~pd.isnull(series.values)]  # remove NaN  # @TODO: benchmark imputation vs this?
 
                 if self.model_path == 'fbprophet.Prophet':
-                    series = self._transform_index_to_datetime(series, series_oby, options['freq'])
+                    try:
+                        series = self._transform_index_to_datetime(series, series_oby, options['freq'])
+                    except Exception:
+                        if group == '__default':
+                            # out of bounds with true freq in __default group is fine, we skip it
+                            continue
 
                 series = series.astype(float)
 
                 # if data is huge, filter out old records for quicker fitting
                 if self.auto_size:
                     cutoff = min(len(series), max(500, options['sp'] * self.cutoff_factor))
                     series = series.iloc[-cutoff:]
```

### Comparing `lightwood-23.3.2.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.4.3.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/unit.py` & `lightwood-23.4.3.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood/mixer/xgboost.py` & `lightwood-23.4.3.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.4.3.0/lightwood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.3.2.0
+Version: 23.4.3.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -217,14 +217,14 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: image
-Provides-Extra: xai
-Provides-Extra: extra
-Provides-Extra: quantum
 Provides-Extra: extra_ts
+Provides-Extra: quantum
 Provides-Extra: audio
+Provides-Extra: extra
+Provides-Extra: image
+Provides-Extra: xai
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.3.2.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.4.3.0/lightwood.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightwood-23.3.2.0/lightwood.egg-info/requires.txt` & `lightwood-23.4.3.0/lightwood.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 type_infer==0.0.9
 dataprep_ml==0.0.8
-mindsdb-evaluator==0.0.6
+mindsdb-evaluator>=0.0.7
 numpy
 nltk<3.6,>=3
 python-dateutil>=2.8.1
 pandas<1.5.0,>=1.1.5
 schema>=0.6.8
 torch<1.14.0,>=1.13.0
 requests>=2.0.0
@@ -30,29 +30,29 @@
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
-suod
-autopep8>=1.5.7
-pystan==2.19.1.1
-prophet==1.1
 gluonts<0.12.0,>=0.11.0
-mxnet<2.0.0,>=1.6.0
 neuralforecast==0.1.0
+qiskit==0.31.0
 pillow>8.3.1
-torchvision<0.11.0,>=0.10.0
+prophet==1.1
 lightgbm<=3.3.3,>=3.3.0
-shap>=0.40.0
-librosa==0.8.1
-qiskit==0.31.0
 pytorch-lightning<1.7.0,>=1.6.0
+autopep8>=1.5.7
+mxnet<2.0.0,>=1.6.0
 pyod==1.0.4
+suod
+torchvision<0.11.0,>=0.10.0
+pystan==2.19.1.1
+librosa==0.8.1
+shap>=0.40.0
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
```

### Comparing `lightwood-23.3.2.0/requirements.txt` & `lightwood-23.4.3.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 type_infer ==0.0.9
 dataprep_ml ==0.0.8
-mindsdb-evaluator ==0.0.6
+mindsdb-evaluator >=0.0.7
 numpy
 nltk >=3,<3.6
 python-dateutil >=2.8.1
 pandas >=1.1.5, <1.5.0
 schema >=0.6.8
 torch >=1.13.0, <1.14.0
 requests >=2.0.0
```

### Comparing `lightwood-23.3.2.0/setup.py` & `lightwood-23.4.3.0/setup.py`

 * *Files identical despite different names*

