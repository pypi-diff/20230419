# Comparing `tmp/tuned-lens-0.0.4.tar.gz` & `tmp/tuned-lens-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuned-lens-0.0.4.tar", last modified: Tue Apr 18 03:12:02 2023, max compression
+gzip compressed data, was "tuned-lens-0.0.5.tar", last modified: Wed Apr 19 16:10:28 2023, max compression
```

## Comparing `tuned-lens-0.0.4.tar` & `tuned-lens-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_load_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tests/test_subspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tuned_lens/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/ablation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/causal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/model_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/_model_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/downstream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/nn/lenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/plotting/plot_lens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/residual_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/argparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/cbe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/downstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/eval_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/scripts/train_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.796734 tuned-lens-0.0.4/tuned_lens/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/logit_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/stats/residual_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-18 03:11:53.000000 tuned-lens-0.0.4/tuned_lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:12:02.792734 tuned-lens-0.0.4/tuned_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 03:12:02.000000 tuned-lens-0.0.4/tuned_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:27.999213 tuned-lens-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_load_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tests/test_subspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/ablation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/causal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/model_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/_model_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/downstream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/nn/lenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/plotting/plot_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/residual_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/argparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/cbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/eval_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/scripts/train_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.007212 tuned-lens-0.0.5/tuned_lens/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/logit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/stats/residual_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-19 16:10:18.000000 tuned-lens-0.0.5/tuned_lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:10:28.003213 tuned-lens-0.0.5/tuned_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 16:10:27.000000 tuned-lens-0.0.5/tuned_lens.egg-info/top_level.txt
```

### Comparing `tuned-lens-0.0.4/LICENSE` & `tuned-lens-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/PKG-INFO` & `tuned-lens-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `tuned-lens-0.0.4/README.md` & `tuned-lens-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/pyproject.toml` & `tuned-lens-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "plotly>=5.13.1",
     "scikit-learn",
     "zstandard",
     "torch>=1.13.0",
     "transformers",
     "huggingface_hub>=0.12.1",
 ]
-version = "0.0.4"
+version = "0.0.5"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "bump2version",
     "pytest-skip-slow",
     "pytest",
```

### Comparing `tuned-lens-0.0.4/tests/test_decoder.py` & `tuned-lens-0.0.5/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_distance.py` & `tuned-lens-0.0.5/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_feature_extraction.py` & `tuned-lens-0.0.5/tests/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_lenses.py` & `tuned-lens-0.0.5/tests/test_lenses.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_plotting.py` & `tuned-lens-0.0.5/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_stats.py` & `tuned-lens-0.0.5/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tests/test_subspaces.py` & `tuned-lens-0.0.5/tests/test_subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/__main__.py` & `tuned-lens-0.0.5/tuned_lens/__main__.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/causal/ablation.py` & `tuned-lens-0.0.5/tuned_lens/causal/ablation.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/causal/subspaces.py` & `tuned-lens-0.0.5/tuned_lens/causal/subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/causal/utils.py` & `tuned-lens-0.0.5/tuned_lens/causal/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/data.py` & `tuned-lens-0.0.5/tuned_lens/data.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/load_artifacts.py` & `tuned-lens-0.0.5/tuned_lens/load_artifacts.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/model_surgery.py` & `tuned-lens-0.0.5/tuned_lens/model_surgery.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/nn/_model_specific.py` & `tuned-lens-0.0.5/tuned_lens/nn/_model_specific.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/nn/decoder.py` & `tuned-lens-0.0.5/tuned_lens/nn/decoder.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/nn/downstream_wrapper.py` & `tuned-lens-0.0.5/tuned_lens/nn/downstream_wrapper.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/nn/lenses.py` & `tuned-lens-0.0.5/tuned_lens/nn/lenses.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,26 +204,27 @@
         """Get iterator over the translators within the lens."""
         if isinstance(self.input_translator, th.nn.Module):
             yield self.input_translator
 
         yield from self.layer_translators
 
     @classmethod
-    def load(cls, resource_id: str, **kwargs) -> "TunedLens":
+    def load(cls, resource_id: str, revision: str = "v0.0.5", **kwargs) -> "TunedLens":
         """Load a tuned lens from a or hugging face hub.
 
         Args:
             resource_id : The path to the directory containing the config and checkpoint
                 or the name of the model on the hugging face hub.
+            revision : The git revision of the lens to load from the hub.
             **kwargs : Additional arguments to pass to torch.load.
 
         Returns:
             A TunedLens instance.
         """
-        config_path, ckpt_path = load_lens_artifacts(resource_id)
+        config_path, ckpt_path = load_lens_artifacts(resource_id, revision=revision)
         # Load config
         with open(config_path, "r") as f:
             config = json.load(f)
 
         # Load parameters
         state = th.load(ckpt_path, **kwargs)
```

### Comparing `tuned-lens-0.0.4/tuned_lens/plotting/plot_lens.py` & `tuned-lens-0.0.5/tuned_lens/plotting/plot_lens.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/residual_stream.py` & `tuned-lens-0.0.5/tuned_lens/residual_stream.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/argparsers.py` & `tuned-lens-0.0.5/tuned_lens/scripts/argparsers.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/cbe.py` & `tuned-lens-0.0.5/tuned_lens/scripts/cbe.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/downstream.py` & `tuned-lens-0.0.5/tuned_lens/scripts/downstream.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/eval_loop.py` & `tuned-lens-0.0.5/tuned_lens/scripts/eval_loop.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/lens.py` & `tuned-lens-0.0.5/tuned_lens/scripts/lens.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/scripts/train_loop.py` & `tuned-lens-0.0.5/tuned_lens/scripts/train_loop.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/anomaly.py` & `tuned-lens-0.0.5/tuned_lens/stats/anomaly.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/dimensionality.py` & `tuned-lens-0.0.5/tuned_lens/stats/dimensionality.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/distance.py` & `tuned-lens-0.0.5/tuned_lens/stats/distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/logit_stats.py` & `tuned-lens-0.0.5/tuned_lens/stats/logit_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/rank.py` & `tuned-lens-0.0.5/tuned_lens/stats/rank.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/stats/residual_stats.py` & `tuned-lens-0.0.5/tuned_lens/stats/residual_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens/utils.py` & `tuned-lens-0.0.5/tuned_lens/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.0.4/tuned_lens.egg-info/PKG-INFO` & `tuned-lens-0.0.5/tuned_lens.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `tuned-lens-0.0.4/tuned_lens.egg-info/SOURCES.txt` & `tuned-lens-0.0.5/tuned_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

