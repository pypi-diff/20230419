# Comparing `tmp/skyllh-23.0.0.tar.gz` & `tmp/skyllh-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyllh-23.0.0.tar", last modified: Mon Jan  9 17:05:35 2023, max compression
+gzip compressed data, was "skyllh-23.1.0.tar", last modified: Wed Apr 19 15:51:13 2023, max compression
```

## Comparing `skyllh-23.0.0.tar` & `skyllh-23.1.0.tar`

### file list

```diff
@@ -1,144 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-09 17:05:27.000000 skyllh-23.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-01-09 17:05:35.533358 skyllh-23.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-09 17:05:27.000000 skyllh-23.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-09 17:05:27.000000 skyllh-23.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-01-09 17:05:35.533358 skyllh-23.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-09 17:05:27.000000 skyllh-23.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/skyllh/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-09 17:05:35.533358 skyllh-23.0.0/skyllh/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.525358 skyllh-23.0.0/skyllh/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/cluster/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/cluster/compute_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/cluster/master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/cluster/srvclt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/core/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69209 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    55536 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/analysis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/background_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/background_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/backgroundpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    64697 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/detsigyield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/display.py
--rw-r--r--   0 runner    (1001) docker     (123)    18924 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/livetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/llhratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    33999 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/minimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/core/minimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/minimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/minimizers/iminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44046 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    94140 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    73499 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    38047 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/pdfratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20635 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/scrambling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/signal_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/signal_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/signalpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/source_hypo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/source_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    36717 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/test_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    30722 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/trialdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/utils/multidimgridpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/utils/ndphotosplinepdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/core/utils/trials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/i3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/background_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/backgroundpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/detsigyield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/livetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/pdfratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/scrambling.py
--rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/signal_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/signalpdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/i3/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/i3/utils/sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/physics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    55097 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/flux_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/physics/time_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/plotting/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/core/pdfratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/core/signalpdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.529358 skyllh-23.0.0/skyllh/plotting/i3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/i3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/i3/backgroundpdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/i3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/i3/pdfratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/skyllh/plotting/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/plotting/utils/trials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/skyllh/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-09 17:05:27.000000 skyllh-23.0.0/skyllh/utils/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.525358 skyllh-23.0.0/skyllh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-01-09 17:05:35.000000 skyllh-23.0.0/skyllh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-01-09 17:05:35.000000 skyllh-23.0.0/skyllh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 17:05:35.000000 skyllh-23.0.0/skyllh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-09 17:05:35.000000 skyllh-23.0.0/skyllh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-09 17:05:35.000000 skyllh-23.0.0/skyllh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31916 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    33818 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_signal_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/core/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/core/testdata/testdata_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/i3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/test_background_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/test_livetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/test_scrambling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/i3/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/i3/testdata/testdata_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:35.533358 skyllh-23.0.0/tests/physics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/physics/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/physics/test_flux_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/physics/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/physics/test_time_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-09 17:05:27.000000 skyllh-23.0.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-01-09 17:05:27.000000 skyllh-23.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 15:51:02.000000 skyllh-23.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-19 15:51:13.586627 skyllh-23.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 15:51:02.000000 skyllh-23.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 15:51:02.000000 skyllh-23.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-19 15:51:13.586627 skyllh-23.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 15:51:02.000000 skyllh-23.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.574627 skyllh-23.1.0/skyllh/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.574627 skyllh-23.1.0/skyllh/analyses/i3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.578627 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/aeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/backgroundpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/bkg_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/detsigyield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/mcbkg_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/pdfratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/signal_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/signalpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30526 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/smearing_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/time_dependent_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/time_integrated_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.578627 skyllh-23.1.0/skyllh/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/cluster/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/cluster/compute_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/cluster/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/cluster/srvclt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69120 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55665 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/analysis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/background_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/background_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/backgroundpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66267 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/detsigyield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/expectation_maximization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18924 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/livetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/llhratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/minimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/core/minimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/minimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/minimizers/iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44046 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94140 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74524 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38060 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/pdfratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/scrambling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/signal_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19833 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/signal_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30435 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/signalpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/source_hypo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/source_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45323 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/test_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30990 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/trialdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/utils/multidimgridpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/utils/ndphotosplinepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/core/utils/trials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/datasets/i3/
+-rw-r--r--   0 runner    (1001) docker     (123)    23450 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/datasets/i3/PublicData_10y_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/datasets/i3/PublicData_10y_ps_wMC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/datasets/i3/PublicData_10y_ps_wMCEq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/datasets/i3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/i3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/background_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/backgroundpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/detsigyield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/livetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/pdfratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/scrambling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/signal_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/signalpdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/i3/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/i3/utils/sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55097 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/flux_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/physics/time_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.582627 skyllh-23.1.0/skyllh/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/plotting/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/core/pdfratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/core/signalpdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/plotting/i3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/i3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/i3/backgroundpdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/i3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/i3/pdfratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/plotting/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/plotting/utils/trials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.586627 skyllh-23.1.0/skyllh/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 15:51:02.000000 skyllh-23.1.0/skyllh/utils/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:51:13.574627 skyllh-23.1.0/skyllh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-19 15:51:13.000000 skyllh-23.1.0/skyllh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-19 15:51:13.000000 skyllh-23.1.0/skyllh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:51:13.000000 skyllh-23.1.0/skyllh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 15:51:13.000000 skyllh-23.1.0/skyllh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 15:51:13.000000 skyllh-23.1.0/skyllh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 15:51:02.000000 skyllh-23.1.0/versioneer.py
```

### Comparing `skyllh-23.0.0/LICENSE.txt` & `skyllh-23.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/PKG-INFO` & `skyllh-23.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyllh
-Version: 23.0.0
+Version: 23.1.0
 Summary: The SkyLLH framework is an open-source Python3-based package licensed under the GPLv3 license. It provides a modular framework for implementing custom likelihood functions and executing log-likelihood ratio hypothesis tests. The idea is to provide a class structure tied to the mathematical objects of the likelihood functions.
 Home-page: https://github.com/icecube/skyllh
 Author: Martin Wolf
 Author-email: martin.wolf@icecube.wisc.edu
 License: GPL-3+
 Project-URL: Bug Tracker, https://github.com/icecube/skyllh/issues
 Project-URL: Documentation, https://icecube.github.io/skyllh
@@ -29,26 +29,31 @@
 
 The SkyLLH framework is an open-source Python3-based package licensed under the GPLv3 license. It provides a modular framework for implementing custom likelihood functions and executing log-likelihood ratio hypothesis tests. The idea is to provide a class structure tied to the mathematical objects of the likelihood functions, rather than to entire abstract likelihood models.
 
 # Installation
 
 ## Using pip
 
-The `skyllh` package can be installed using pip:
+The latest `skyllh` release can be installed from [PyPI](https://pypi.org/project/skyllh/) repository:
+```bash
+pip install skyllh
+```
+
+The current development version can be installed using pip:
 ```bash
 pip install git+https://github.com/icecube/skyllh.git#egg=skyllh 
 ```
 
 Optionally, the editable package version with a specified reference can be installed by:
 ```bash
-pip install -e git+https://github.com/icecube/skyllh.git@ref#egg=skyllh 
+pip install -e git+https://github.com/icecube/skyllh.git@[ref]#egg=skyllh 
 ```
 where
 - `-e` is an editable flag
-- `ref` in `@ref` is an optional argument containing a specific commit hash, branch name or tag
+- `[ref]` is an optional argument containing a specific commit hash, branch name or tag
 
 ## Cloning from GitHub
 
 The `skyllh` (and an optional private [i3skyllh](#i3skyllh)) package can be installed by cloning the GitHub repository and adding it to the Python path:
 
 ```python
 import sys
```

### Comparing `skyllh-23.0.0/README.md` & `skyllh-23.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 
 The SkyLLH framework is an open-source Python3-based package licensed under the GPLv3 license. It provides a modular framework for implementing custom likelihood functions and executing log-likelihood ratio hypothesis tests. The idea is to provide a class structure tied to the mathematical objects of the likelihood functions, rather than to entire abstract likelihood models.
 
 # Installation
 
 ## Using pip
 
-The `skyllh` package can be installed using pip:
+The latest `skyllh` release can be installed from [PyPI](https://pypi.org/project/skyllh/) repository:
+```bash
+pip install skyllh
+```
+
+The current development version can be installed using pip:
 ```bash
 pip install git+https://github.com/icecube/skyllh.git#egg=skyllh 
 ```
 
 Optionally, the editable package version with a specified reference can be installed by:
 ```bash
-pip install -e git+https://github.com/icecube/skyllh.git@ref#egg=skyllh 
+pip install -e git+https://github.com/icecube/skyllh.git@[ref]#egg=skyllh 
 ```
 where
 - `-e` is an editable flag
-- `ref` in `@ref` is an optional argument containing a specific commit hash, branch name or tag
+- `[ref]` is an optional argument containing a specific commit hash, branch name or tag
 
 ## Cloning from GitHub
 
 The `skyllh` (and an optional private [i3skyllh](#i3skyllh)) package can be installed by cloning the GitHub repository and adding it to the Python path:
 
 ```python
 import sys
```

### Comparing `skyllh-23.0.0/setup.cfg` & `skyllh-23.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/cluster/commands.py` & `skyllh-23.1.0/skyllh/cluster/commands.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/cluster/compute_node.py` & `skyllh-23.1.0/skyllh/cluster/compute_node.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/cluster/master_node.py` & `skyllh-23.1.0/skyllh/cluster/master_node.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/cluster/srvclt.py` & `skyllh-23.1.0/skyllh/cluster/srvclt.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/__init__.py` & `skyllh-23.1.0/skyllh/core/__init__.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/analysis.py` & `skyllh-23.1.0/skyllh/core/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # -*- coding: utf-8 -*-
 
 """The analysis module provides classes for pre-defined analyses.
 """
 
 import abc
 import numpy as np
-import pickle
 
 from skyllh.core.py import (
     classname,
     issequenceof
 )
 from skyllh.core.debugging import get_logger
 from skyllh.core.storage import DataFieldRecordArray
 from skyllh.core.dataset import (
     Dataset,
-    DatasetData
+    DatasetData,
 )
 from skyllh.core.parameters import (
     FitParameter,
     SourceFitParameterMapper,
-    SingleSourceFitParameterMapper
-)
-from skyllh.core.pdf import (
-    EnergyPDF,
-    SpatialPDF
+    SingleSourceFitParameterMapper,
 )
 from skyllh.core.pdfratio import PDFRatio
 from skyllh.core.progressbar import ProgressBar
 from skyllh.core.random import RandomStateService
 from skyllh.core.llhratio import (
     LLHRatio,
     MultiDatasetTCLLHRatio,
     SingleSourceDatasetSignalWeights,
     SingleSourceZeroSigH0SingleDatasetTCLLHRatio,
     MultiSourceZeroSigH0SingleDatasetTCLLHRatio,
-    MultiSourceDatasetSignalWeights
+    MultiSourceDatasetSignalWeights,
 )
-from skyllh.core.scrambling import DataScramblingMethod
 from skyllh.core.timing import TaskTimer
 from skyllh.core.trialdata import TrialDataManager
-from skyllh.core.optimize import (
-    EventSelectionMethod,
-    AllEventSelectionMethod
-)
+from skyllh.core.optimize import EventSelectionMethod
 from skyllh.core.source_hypothesis import SourceHypoGroupManager
 from skyllh.core.test_statistic import TestStatistic
 from skyllh.core.multiproc import get_ncpu, parallelize
 from skyllh.core.background_generation import BackgroundGenerationMethod
 from skyllh.core.background_generator import BackgroundGenerator
 from skyllh.core.signal_generator import (
     SignalGeneratorBase,
-    SignalGenerator
+    SignalGenerator,
 )
 from skyllh.physics.source import SourceModel
 
 
 logger = get_logger(__name__)
 
 
@@ -365,38 +356,40 @@
     @abc.abstractmethod
     def construct_llhratio(self):
         """This method is supposed to construct the log-likelihood ratio
         function and sets it as the _llhratio property.
         """
         pass
 
-    def construct_background_generator(self):
+    def construct_background_generator(self, **kwargs):
         """Constructs the background generator for all added datasets.
         This method must be called after all the datasets were added via the
         add_dataset method. It sets the `bkg_generator` property of this
         Analysis class instance.
         """
         if(self._bkg_gen_method is None):
             raise RuntimeError('No background generation method has been '
                 'defined for this analysis!')
 
         self._bkg_generator = BackgroundGenerator(
-            self._bkg_gen_method, self._dataset_list, self._data_list)
+            self._bkg_gen_method, self._dataset_list, self._data_list,
+            **kwargs)
 
-    def construct_signal_generator(self):
+    def construct_signal_generator(self, **kwargs):
         """Constructs the signal generator for all added datasets.
         This method must be called after all the datasets were added via the
         add_dataset method. It sets the `sig_generator` property of this
         Analysis class instance. The signal generation method has to be set
         through the source hypothesis group.
         """
         self._sig_generator = self.sig_generator_cls(
             src_hypo_group_manager=self._src_hypo_group_manager,
             dataset_list=self._dataset_list,
-            data_list=self._data_list)
+            data_list=self._data_list,
+            **kwargs)
 
     @abc.abstractmethod
     def initialize_trial(self, events_list, n_events_list=None):
         """This method is supposed to initialize the log-likelihood ratio
         function with a new set of given trial data. This is a low-level method.
         For convenient methods see the `unblind` and `do_trial` methods.
 
@@ -1028,15 +1021,15 @@
             }) for i in range(n)
         ]
         result_list = parallelize(
             self.do_trial, args_list, ncpu, rss=rss, tl=tl, ppbar=ppbar)
 
         result_dtype = result_list[0].dtype
         result = np.empty(n, dtype=result_dtype)
-        result[:] = result_list[:]
+        result[:] = np.array(result_list)[:,0]
         return result
 
 
 class TimeIntegratedMultiDatasetSingleSourceAnalysis(Analysis):
     """This is an analysis class that implements a time-integrated LLH ratio
     analysis for multiple datasets assuming a single source.
```

### Comparing `skyllh-23.0.0/skyllh/core/analysis_utils.py` & `skyllh-23.1.0/skyllh/core/analysis_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -851,25 +851,25 @@
         tl=tl,
         pathfilename=pathfilename)
 
     return (mu, mu_err)
 
 
 def estimate_discovery_potential(
-        ana, rss, h0_trials=None, h0_ts_quantile=5.733e-7, p=0.5, eps_p=0.005,
+        ana, rss, h0_trials=None, h0_ts_quantile=2.8665e-7, p=0.5, eps_p=0.005,
         mu_range=None, min_dmu=0.5, bkg_kwargs=None, sig_kwargs=None,
         ppbar=None, tl=None, pathfilename=None):
     """Estimates the mean number of signal events that whould have to be
     injected into the data such that the test-statistic value of p*100% of all
     trials are larger than the critical test-statistic value c, which
     corresponds to the test-statistic value where h0_ts_quantile*100% of all
     null hypothesis test-statistic values are larger than c.
 
     For the 5 sigma discovery potential `h0_ts_quantile`, and `p` are usually
-    set to 5.733e-7, and 0.5, respectively.
+    set to 2.8665e-7, and 0.5, respectively.
 
     Parameters
     ----------
     ana : Analysis
         The Analysis instance to use for discovery potential estimation.
     rss : RandomStateService
         The RandomStateService instance to use for generating random
@@ -1218,15 +1218,15 @@
 
     return (rss.seed, mean_n_sig, mean_n_sig_null, trial_data)
 
 
 def extend_trial_data_file(
         ana, rss, n_trials, trial_data, mean_n_sig=0, mean_n_sig_null=0,
         mean_n_bkg_list=None, bkg_kwargs=None, sig_kwargs=None,
-        pathfilename=None):
+        pathfilename=None, **kwargs):
     """Appends to the trial data file `n_trials` generated trials for each
     mean number of injected signal events up to `ns_max` for a given analysis.
 
     Parameters
     ----------
     ana : Analysis
         The Analysis instance to use for sensitivity estimation.
@@ -1262,31 +1262,45 @@
         `poisson`.
     sig_kwargs : dict | None
         Additional keyword arguments for the `generate_signal_events` method
         of the `SignalGenerator` class. An usual keyword argument is
         `poisson`.
     pathfilename : string | None
         Trial data file path including the filename.
+
+    Additional keyword arguments
+    ----------------------------
+    Additional keyword arguments are passed-on to the ``create_trial_data_file``
+    function.
+
     Returns
     -------
     trial_data :
         Trial data file extended by the required number of trials for each
         mean number of injected signal events..
     """
     # Use unique seed to generate non identical trials.
     if rss.seed in trial_data['seed']:
         seed = next(i for i, e in
                     enumerate(sorted(np.unique(trial_data['seed'])) +
                                 [None], 1) if i != e)
         rss.reseed(seed)
+
     (seed, mean_n_sig, mean_n_sig_null, trials) = create_trial_data_file(
-                                                    ana, rss, n_trials,
-                                                    mean_n_sig=mean_n_sig)
-    trial_data = np_rfn.stack_arrays([trial_data, trials], usemask=False,
-                                         asrecarray=True)
+        ana=ana,
+        rss=rss,
+        n_trials=n_trials,
+        mean_n_sig=mean_n_sig,
+        **kwargs
+    )
+    trial_data = np_rfn.stack_arrays(
+        [trial_data, trials],
+        usemask=False,
+        asrecarray=True)
+
     if(pathfilename is not None):
         # Save the trial data to file.
         makedirs(os.path.dirname(pathfilename), exist_ok=True)
         np.save(pathfilename, trial_data)
 
     return trial_data
```

### Comparing `skyllh-23.0.0/skyllh/core/background_generation.py` & `skyllh-23.1.0/skyllh/core/background_generation.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/background_generator.py` & `skyllh-23.1.0/skyllh/core/background_generator.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/backgroundpdf.py` & `skyllh-23.1.0/skyllh/core/backgroundpdf.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 """The ``backgroundpdf`` module contains possible background PDF models for the
 likelihood function.
 """
 
 from skyllh.core.pdf import (
     IsBackgroundPDF,
     MultiDimGridPDF,
-    NDPhotosplinePDF
+    NDPhotosplinePDF,
+    TimePDF,
 )
 
+import numpy as np
+
 
 class BackgroundMultiDimGridPDF(MultiDimGridPDF, IsBackgroundPDF):
     """This class provides a multi-dimensional background PDF. The PDF is
     created from pre-calculated PDF data on a grid. The grid data is
     interpolated using a :class:`scipy.interpolate.RegularGridInterpolator`
     instance.
     """
@@ -93,7 +96,96 @@
         """
         super(BackgroundNDPhotosplinePDF, self).__init__(
             axis_binnings=axis_binnings,
             param_set=param_set,
             path_to_pdf_splinefit=path_to_pdf_splinefit,
             norm_factor_func=norm_factor_func
         )
+
+
+class BackgroundUniformTimePDF(TimePDF, IsBackgroundPDF):
+
+    def __init__(self, grl):
+        """Creates a new background time PDF instance as uniform background
+
+        Parameters
+        ----------
+        grl : ndarray
+            Array of the detector good run list
+
+        """
+        super(BackgroundUniformTimePDF, self).__init__()
+        self.start = grl["start"][0]
+        self.end = grl["stop"][-1]
+        self.grl = grl
+
+
+    def cdf(self, t):
+        """Compute the cumulative density function for the box pdf. This is
+        needed for normalization.
+
+        Parameters
+        ----------
+        t : float, ndarray
+            MJD times
+
+        Returns
+        -------
+        cdf : float, ndarray
+            Values of cumulative density function evaluated at t
+        """
+        t_start = self.grl["start"][0]
+        t_end = self.grl["stop"][-1]
+        t = np.atleast_1d(t)
+
+        cdf = np.zeros(t.size, float)
+
+        # values between start and stop times
+        mask = (t_start <= t) & (t <= t_end)
+        cdf[mask] = (t[mask] - t_start) / [t_end - t_start]
+
+        # take care of values beyond stop time in sample
+
+        return cdf
+
+    def norm_uptime(self):
+        """Compute the normalization with the dataset uptime. Distributions like 
+        scipy.stats.norm are normalized (-inf, inf).
+        These must be re-normalized such that the function sums to 1 over the
+        finite good run list domain.
+
+        Returns
+        -------
+        norm : float
+            Normalization such that cdf sums to 1 over good run list domain
+        """
+
+        integral = (self.cdf(self.grl["stop"]) - self.cdf(self.grl["start"])).sum()
+
+        if np.isclose(integral, 0):
+            return 0
+
+        return 1. / integral
+
+    def get_prob(self, tdm, fitparams=None, tl=None):
+        """Calculates the background time probability density of each event.
+
+        tdm : TrialDataManager
+            Unused interface argument.
+        fitparams : None
+            Unused interface argument.
+        tl : instance of TimeLord | None
+            The optional instance of TimeLord that should be used to collect
+            timing information about this method.
+
+        Returns
+        -------
+        pd : array of float
+            The (N,)-shaped ndarray holding the probability density for each event.
+        grads : empty array of float
+            Does not depend on fit parameter, so no gradient.
+        """
+        livetime = self.grl["stop"][-1] - self.grl["start"][0]
+        pd = 1./livetime
+        grads = np.array([], dtype=np.double)
+
+        return (pd, grads)
```

### Comparing `skyllh-23.0.0/skyllh/core/config.py` & `skyllh-23.1.0/skyllh/core/config.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/coords.py` & `skyllh-23.1.0/skyllh/core/coords.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/dataset.py` & `skyllh-23.1.0/skyllh/core/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,17 @@
         Parameters
         ----------
         name : str
             The name of the dataset.
         exp_pathfilenames : str | sequence of str | None
             The file name(s), including paths, of the experimental data file(s).
             This can be None, if a MC-only study is performed.
-        mc_pathfilenames : str | sequence of str
+        mc_pathfilenames : str | sequence of str | None
             The file name(s), including paths, of the monte-carlo data file(s).
+            This can be None, if a MC-less analysis is performed.
         livetime : float | None
             The integrated live-time in days of the dataset. It can be None for
             cases where the live-time is retrieved directly from the data files
             uppon data loading.
         default_sub_path_fmt : str
             The default format of the sub path of the data set.
             This must be a string that can be formatted via the ``format``
@@ -219,14 +220,16 @@
         data for this dataset.
         If a file name is given with a relative path, it will be relative to the
         root_dir property of this Dataset instance.
         """
         return self._mc_pathfilename_list
     @mc_pathfilename_list.setter
     def mc_pathfilename_list(self, pathfilenames):
+        if(pathfilenames is None):
+            pathfilenames = []
         if(isinstance(pathfilenames, str)):
             pathfilenames = [pathfilenames]
         if(not issequenceof(pathfilenames, str)):
             raise TypeError('The mc_pathfilename_list property must be of '
                 'type str or a sequence of str!')
         self._mc_pathfilename_list = list(pathfilenames)
 
@@ -698,66 +701,73 @@
             return orig_field_names
 
         if(keep_fields is None):
             keep_fields = []
 
         # Load the experimental data if there is any.
         if(len(self._exp_pathfilename_list) > 0):
-            fileloader_exp = create_FileLoader(self.exp_abs_pathfilename_list)
             with TaskTimer(tl, 'Loading exp data from disk.'):
+                fileloader_exp = create_FileLoader(
+                    self.exp_abs_pathfilename_list)
                 # Create the list of field names that should get kept.
-                keep_fields = list(set(
+                keep_fields_exp = list(set(
                     _conv_new2orig_field_names(
                         CFG['dataset']['analysis_required_exp_field_names'] +
                         self._loading_extra_exp_field_name_list +
                         keep_fields,
                         self._exp_field_name_renaming_dict
                     )
                 ))
 
                 data_exp = fileloader_exp.load_data(
-                    keep_fields=keep_fields,
+                    keep_fields=keep_fields_exp,
                     dtype_convertions=dtc_dict,
                     dtype_convertion_except_fields=_conv_new2orig_field_names(
                         dtc_except_fields,
                         self._exp_field_name_renaming_dict),
                     efficiency_mode=efficiency_mode)
                 data_exp.rename_fields(self._exp_field_name_renaming_dict)
         else:
             data_exp = None
 
-        # Load the monte-carlo data.
-        with TaskTimer(tl, 'Loading mc data from disk.'):
-            fileloader_mc = create_FileLoader(self.mc_abs_pathfilename_list)
-            keep_fields = list(set(
-                _conv_new2orig_field_names(
-                    CFG['dataset']['analysis_required_exp_field_names'] +
-                    self._loading_extra_exp_field_name_list +
-                    keep_fields,
-                    self._exp_field_name_renaming_dict) +
-                _conv_new2orig_field_names(
-                    CFG['dataset']['analysis_required_mc_field_names'] +
-                    self._loading_extra_mc_field_name_list +
-                    keep_fields,
-                    self._mc_field_name_renaming_dict)
-            ))
-            data_mc = fileloader_mc.load_data(
-                keep_fields=keep_fields,
-                dtype_convertions=dtc_dict,
-                dtype_convertion_except_fields=_conv_new2orig_field_names(
-                    dtc_except_fields,
-                    self._mc_field_name_renaming_dict),
-                efficiency_mode=efficiency_mode)
-            data_mc.rename_fields(self._mc_field_name_renaming_dict)
+        # Load the monte-carlo data if there is any.
+        if(len(self._mc_pathfilename_list) > 0):
+            with TaskTimer(tl, 'Loading mc data from disk.'):
+                fileloader_mc = create_FileLoader(
+                    self.mc_abs_pathfilename_list)
+                # Determine `keep_fields_mc` for the generic case, where MC
+                # field names are an union of exp and mc field names.
+                # But the renaming dictionary can differ for exp and MC fields.
+                keep_fields_mc = list(set(
+                    _conv_new2orig_field_names(
+                        CFG['dataset']['analysis_required_exp_field_names'] +
+                        self._loading_extra_exp_field_name_list +
+                        keep_fields,
+                        self._exp_field_name_renaming_dict) +
+                    _conv_new2orig_field_names(
+                        CFG['dataset']['analysis_required_exp_field_names'] +
+                        self._loading_extra_exp_field_name_list +
+                        CFG['dataset']['analysis_required_mc_field_names'] +
+                        self._loading_extra_mc_field_name_list +
+                        keep_fields,
+                        self._mc_field_name_renaming_dict)
+                ))
+                data_mc = fileloader_mc.load_data(
+                    keep_fields=keep_fields_mc,
+                    dtype_convertions=dtc_dict,
+                    dtype_convertion_except_fields=_conv_new2orig_field_names(
+                        dtc_except_fields,
+                        self._mc_field_name_renaming_dict),
+                    efficiency_mode=efficiency_mode)
+                data_mc.rename_fields(self._mc_field_name_renaming_dict)
+        else:
+            data_mc = None
 
         if(livetime is None):
             livetime = self.livetime
-        if(livetime is None):
-            raise ValueError('No livetime was provided for dataset '
-                '"%s"!'%(self.name))
 
         data = DatasetData(data_exp, data_mc, livetime)
 
         return data
 
     def load_aux_data(self, name, tl=None):
         """Loads the auxiliary data for the given auxiliary data definition.
@@ -943,21 +953,23 @@
         if(data.exp is not None):
             with TaskTimer(tl, 'Cleaning exp data.'):
                 keep_fields_exp = (
                     CFG['dataset']['analysis_required_exp_field_names'] +
                     keep_fields
                 )
                 data.exp.tidy_up(keep_fields=keep_fields_exp)
-        with TaskTimer(tl, 'Cleaning MC data.'):
-            keep_fields_mc = (
-                CFG['dataset']['analysis_required_exp_field_names'] +
-                CFG['dataset']['analysis_required_mc_field_names'] +
-                keep_fields
-            )
-            data.mc.tidy_up(keep_fields=keep_fields_mc)
+
+        if(data.mc is not None):
+            with TaskTimer(tl, 'Cleaning MC data.'):
+                keep_fields_mc = (
+                    CFG['dataset']['analysis_required_exp_field_names'] +
+                    CFG['dataset']['analysis_required_mc_field_names'] +
+                    keep_fields
+                )
+                data.mc.tidy_up(keep_fields=keep_fields_mc)
 
         with TaskTimer(tl, 'Asserting data format.'):
             assert_data_format(self, data)
 
         return data
 
     def add_binning_definition(self, binning):
@@ -1357,16 +1369,19 @@
         Raises
         ------
         KeyError
             If the data set of the given name is not present in this data set
             collection.
         """
         if(name not in self._datasets):
+            ds_names = '", "'.join(self.dataset_names)
+            ds_names = '"'+ds_names+'"'
             raise KeyError('The dataset "%s" is not part of the dataset '
-                'collection "%s"!'%(name, self.name))
+                'collection "%s"! Possible dataset names are: %s!'%(
+                    name, self.name, ds_names))
         return self._datasets[name]
 
     def get_datasets(self, names):
         """Retrieves a list of Dataset objects from this dataset collection.
 
         Parameters
         ----------
@@ -1477,17 +1492,26 @@
 
     def remove_data_preparation(self, key=-1):
         """Removes data preparation function from all the datasets of this
         dataset collection.
 
         Parameters
         ----------
-        index : int, optional
-            Index of which data preparation function to remove. Default value
-            is the last added function.
+        key : str, int, optional
+            The name or the index of the data preparation function that should
+            be removed. Default value is ``-1``, i.e. the last added function.
+
+        Raises
+        ------
+        TypeError
+            If the type of the key argument is invalid.
+        IndexError
+            If the given key is out of range.
+        KeyError
+            If the data preparation function cannot be found.
         """
         for (dsname, dataset) in self._datasets.items():
             dataset.remove_data_preparation(key=key)
 
     def update_version_qualifiers(self, verqualifiers):
         """Updates the version qualifiers of all datasets of this dataset
         collection.
@@ -1577,32 +1601,36 @@
                 raise TypeError('The exp property must be an instance of '
                     'DataFieldRecordArray!')
         self._exp = data
 
     @property
     def mc(self):
         """The DataFieldRecordArray instance holding the monte-carlo data.
+        This is None, if there is no monte-carlo data available.
         """
         return self._mc
     @mc.setter
     def mc(self, data):
-        if(not isinstance(data, DataFieldRecordArray)):
-            raise TypeError('The mc property must be an instance of '
-                'DataFieldRecordArray!')
+        if(data is not None):
+            if(not isinstance(data, DataFieldRecordArray)):
+                raise TypeError('The mc property must be an instance of '
+                    'DataFieldRecordArray!')
         self._mc = data
 
     @property
     def livetime(self):
         """The integrated livetime in days of the data.
+        This is None, if there is no live-time provided.
         """
         return self._livetime
     @livetime.setter
     def livetime(self, lt):
-        lt = float_cast(lt,
-            'The livetime property must be castable to type float!')
+        if(lt is not None):
+            lt = float_cast(lt,
+                'The livetime property must be castable to type float!')
         self._livetime = lt
 
     @property
     def exp_field_names(self):
         """(read-only) The list of field names present in the experimental data.
         This is an empty list if there is no experimental data available.
         """
@@ -1638,21 +1666,28 @@
             data.exp.field_name_list,
             CFG['dataset']['analysis_required_exp_field_names'])
         if(len(missing_exp_keys) != 0):
             raise KeyError('The following data fields are missing for the '
                 'experimental data of dataset "%s": '%(dataset.name)+
                 ', '.join(missing_exp_keys))
 
-    # Check monte-carlo data keys.
-    missing_mc_keys = _get_missing_keys(
-        data.mc.field_name_list,
-        CFG['dataset']['analysis_required_exp_field_names'] +
-        CFG['dataset']['analysis_required_mc_field_names'])
-    if(len(missing_mc_keys) != 0):
-        raise KeyError('The following data fields are missing for the monte-carlo data of dataset "%s": '%(dataset.name)+', '.join(missing_mc_keys))
+    if(data.mc is not None):
+        # Check monte-carlo data keys.
+        missing_mc_keys = _get_missing_keys(
+            data.mc.field_name_list,
+            CFG['dataset']['analysis_required_exp_field_names'] +
+            CFG['dataset']['analysis_required_mc_field_names'])
+        if(len(missing_mc_keys) != 0):
+            raise KeyError('The following data fields are missing for the '
+                'monte-carlo data of dataset "%s": '%(dataset.name)+
+                ', '.join(missing_mc_keys))
+
+    if(data.livetime is None):
+        raise ValueError('No livetime was specified for dataset "{}"!'.format(
+            dataset.name))
 
 
 def remove_events(data_exp, mjds):
     """Utility function to remove events having the specified MJD time stamps.
 
     Parameters
     ----------
```

### Comparing `skyllh-23.0.0/skyllh/core/debugging.py` & `skyllh-23.1.0/skyllh/core/debugging.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/detsigyield.py` & `skyllh-23.1.0/skyllh/core/detsigyield.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/display.py` & `skyllh-23.1.0/skyllh/core/display.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/interpolate.py` & `skyllh-23.1.0/skyllh/core/interpolate.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/livetime.py` & `skyllh-23.1.0/skyllh/core/livetime.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/llhratio.py` & `skyllh-23.1.0/skyllh/core/llhratio.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/math.py` & `skyllh-23.1.0/skyllh/core/math.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/minimizer.py` & `skyllh-23.1.0/skyllh/core/minimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -923,12 +923,13 @@
             xmin = np.where(condmin, bounds[:, 0], xmin)
             xmin = np.where(condmax, bounds[:, 1], xmin)
             if(args is None):
                 args = tuple()
             (fmin, grads) = func(xmin, *args)
 
         logger.debug(
-            '%s (%s): Minimized function: %d iterations, %d repetitions' % (
+            '%s (%s): Minimized function: %d iterations, %d repetitions, '
+            'xmin=%s' % (
                 classname(self), classname(self._minimizer_impl),
-                self._minimizer_impl.get_niter(status), reps))
+                self._minimizer_impl.get_niter(status), reps, str(xmin)))
 
         return (xmin, fmin, status)
```

### Comparing `skyllh-23.0.0/skyllh/core/minimizers/iminuit.py` & `skyllh-23.1.0/skyllh/core/minimizers/iminuit.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/model.py` & `skyllh-23.1.0/skyllh/core/model.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/multiproc.py` & `skyllh-23.1.0/skyllh/core/multiproc.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/optimize.py` & `skyllh-23.1.0/skyllh/core/optimize.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/parameters.py` & `skyllh-23.1.0/skyllh/core/parameters.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/pdf.py` & `skyllh-23.1.0/skyllh/core/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,17 +396,18 @@
         """This method is supposed to check if this PDF is valid for
         all the given trial data. This means, it needs to check if there
         is a PDF value for each trial data event that will be used in the
         likelihood evaluation. This is just a seatbelt.
         The method must raise a ValueError if the PDF is not valid for the
         given trial data.
         """
-        raise NotImplementedError('The derived PDF class "%s" did not '
-                                  'implement the "assert_is_valid_for_trial_data" method!' % (
-                                      classname(self)))
+        raise NotImplementedError(
+            'The derived PDF class "%s" did not implement the '
+            '"assert_is_valid_for_trial_data" method!' % (
+                classname(self)))
 
     @abc.abstractmethod
     def get_prob(self, tdm, params=None, tl=None):
         """This abstract method is supposed to calculate the probability density
         for the specified events given the specified parameter values.
 
         Parameters
@@ -540,17 +541,25 @@
             The gradients of the PDF product w.r.t. the fit parameter of this
             PDFProduct instance.
 
         """
         pdf1 = self._pdf1
         pdf2 = self._pdf2
 
-        with TaskTimer(tl, 'Get signal prob from table.'):
-            (prob1, grads1) = pdf1.get_prob(tdm, params, tl=tl)
-            (prob2, grads2) = pdf2.get_prob(tdm, params, tl=tl)
+        with TaskTimer(tl, 'Get prob from individual PDFs.'):
+            p1 = pdf1.get_prob(tdm, params, tl=tl)
+            if isinstance(p1, tuple):
+                (prob1, grads1) = p1
+            else:
+                prob1 = p1
+            p2 = pdf2.get_prob(tdm, params, tl=tl)
+            if isinstance(p2, tuple):
+                (prob2, grads2) = p2
+            else:
+                prob2 = p2
 
         prob = prob1 * prob2
 
         pdf1_param_set = pdf1.param_set
         pdf2_param_set = pdf2.param_set
 
         N_events = prob.shape[0]
@@ -1383,26 +1392,63 @@
     def pdf_keys(self):
         """(read-only) The list of stored PDF object keys.
         """
         return list(self._gridfitparams_hash_pdf_dict.keys())
 
     @property
     def pdf_axes(self):
+        """DEPRECATED (read-only) The PDFAxes object of one of the PDFs of this
+        PDF set.
+        All PDFs of this set are supposed to have the same axes.
+        """
+        return self.axes
+
+    @property
+    def axes(self):
         """(read-only) The PDFAxes object of one of the PDFs of this PDF set.
         All PDFs of this set are supposed to have the same axes.
         """
         key = next(iter(self._gridfitparams_hash_pdf_dict.keys()))
         return self._gridfitparams_hash_pdf_dict[key].axes
 
+    def __getitem__(self, k):
+        """(read-only) Returns the PDF for the given PDF key.
+        """
+        return self._gridfitparams_hash_pdf_dict[k]
+
     def items(self):
         """Returns the list of 2-element tuples for the PDF stored in this
         PDFSet object.
         """
         return self._gridfitparams_hash_pdf_dict.items()
 
+    def make_pdf_key(self, gridfitparams):
+        """Creates the PDF key for the given grid fit parameter values.
+
+        Parameters
+        ----------
+        gridfitparams : dict | int
+            The dictionary with the grid fit parameters for which the PDF key
+            should get made. If an integer is given, it is assumed to be
+            the PDF key.
+
+        Returns
+        -------
+        pdf_key : int
+            The hash that represents the key for the PDF with the given grid
+            fit parameter values.
+        """
+        if(isinstance(gridfitparams, int)):
+            return gridfitparams
+        if(isinstance(gridfitparams, dict)):
+            return make_params_hash(gridfitparams)
+
+        raise TypeError(
+            'The gridfitparams argument must be of type dict or int!')
+
     def add_pdf(self, pdf, gridfitparams):
         """Adds the given PDF object for the given parameters to the internal
         registry. If this PDF set is not empty, the to-be-added PDF must have
         the same axes than the already added PDFs.
 
         Parameters
         ----------
@@ -1421,18 +1467,17 @@
         ValueError
             If the axes of the given PDFs are not the same as the axes of the
             already added PDFs.
         """
         if(not isinstance(pdf, self.pdf_type)):
             raise TypeError('The pdf argument must be an instance of %s!' % (
                 typename(self.pdf_type)))
-        if(not isinstance(gridfitparams, dict)):
-            raise TypeError('The fitparams argument must be of type dict!')
 
-        gridfitparams_hash = make_params_hash(gridfitparams)
+        gridfitparams_hash = self.make_pdf_key(gridfitparams)
+
         if(gridfitparams_hash in self._gridfitparams_hash_pdf_dict):
             raise KeyError('The PDF with grid fit parameters %s was already '
                            'added!' % (str(gridfitparams)))
 
         # Check that the new PDF has the same axes than the already added PDFs.
         if(len(self._gridfitparams_hash_pdf_dict) > 0):
             some_pdf = self._gridfitparams_hash_pdf_dict[
@@ -1464,25 +1509,20 @@
             The pdf_type object for the given parameters.
 
         Raises
         ------
         KeyError
             If no PDF object was created for the given set of parameters.
         """
-        if(isinstance(gridfitparams, int)):
-            gridfitparams_hash = gridfitparams
-        elif(isinstance(gridfitparams, dict)):
-            gridfitparams_hash = make_params_hash(gridfitparams)
-        else:
-            raise TypeError(
-                'The gridfitparams argument must be of type dict or int!')
+        gridfitparams_hash = self.make_pdf_key(gridfitparams)
 
         if(gridfitparams_hash not in self._gridfitparams_hash_pdf_dict):
             raise KeyError(
-                'No PDF was created for the parameter set "%s"!' % (str(gridfitparams)))
+                'No PDF was created for the parameter set "%s"!' %
+                (str(gridfitparams)))
 
         pdf = self._gridfitparams_hash_pdf_dict[gridfitparams_hash]
         return pdf
 
 
 class MultiDimGridPDFSet(PDF, PDFSet):
     def __init__(
```

### Comparing `skyllh-23.0.0/skyllh/core/pdfratio.py` & `skyllh-23.1.0/skyllh/core/pdfratio.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     Parabola1DGridManifoldInterpolationMethod
 )
 from skyllh.core.pdf import (
     PDF,
     PDFSet,
     IsBackgroundPDF,
     IsSignalPDF,
-    SpatialPDF
+    SpatialPDF,
+    TimePDF
 )
 from skyllh.core.timing import TaskTimer
 
 
 class PDFRatio(object, metaclass=abc.ABCMeta):
     """Abstract base class for a PDF ratio class. It defines the interface
     of a PDF ratio class.
```

### Comparing `skyllh-23.0.0/skyllh/core/progressbar.py` & `skyllh-23.1.0/skyllh/core/progressbar.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/py.py` & `skyllh-23.1.0/skyllh/core/py.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     return t.__name__
 
 def classname(obj):
     """Returns the name of the class of the class instance ``obj``.
     """
     return typename(type(obj))
 
+def module_classname(obj):
+    """Returns the module and class name of the class instance ``obj``.
+    """
+    return '{}.{}'.format(obj.__module__, classname(obj))
+
 def get_byte_size_prefix(size):
     """Determines the biggest size prefix for the given size in bytes such that
     the new size is still greater one.
 
     Parameters
     ----------
     size : int
```

### Comparing `skyllh-23.0.0/skyllh/core/random.py` & `skyllh-23.1.0/skyllh/core/random.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/scrambling.py` & `skyllh-23.1.0/skyllh/core/scrambling.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,21 +33,21 @@
         data : DataFieldRecordArray
             The given DataFieldRecordArray holding the scrambled data.
         """
         pass
 
 
 class UniformRAScramblingMethod(DataScramblingMethod):
-    """The UniformRAScramblingMethod method performs right-ascention scrambling
+    r"""The UniformRAScramblingMethod method performs right-ascention scrambling
     uniformly within a given RA range. By default it's (0, 2\pi).
 
     Note: This alters only the ``ra`` values of the data!
     """
     def __init__(self, ra_range=None):
-        """Initializes a new RAScramblingMethod instance.
+        r"""Initializes a new RAScramblingMethod instance.
 
         Parameters
         ----------
         ra_range : tuple | None
             The two-element tuple holding the range in radians within the RA
             values should get drawn from. If set to None, the default (0, 2\pi)
             will be used.
```

### Comparing `skyllh-23.0.0/skyllh/core/session.py` & `skyllh-23.1.0/skyllh/core/session.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/signal_generation.py` & `skyllh-23.1.0/skyllh/core/signal_generation.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/signal_generator.py` & `skyllh-23.1.0/skyllh/core/signal_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
             their spectra.
         dataset_list : list of Dataset instances
             The list of Dataset instances for which signal events should get
             generated for.
         data_list : list of DatasetData instances
             The list of DatasetData instances holding the actual data of each
             dataset. The order must match the order of ``dataset_list``.
+        kwargs
+            A typical keyword argument is the instance of MultiDatasetTCLLHRatio.
         """
         super().__init__(
             *args,
             src_hypo_group_manager=src_hypo_group_manager,
             dataset_list=dataset_list,
             data_list=data_list,
             **kwargs)
@@ -372,31 +374,34 @@
 
         return (n_signal, signal_events_dict)
 
 
 class MultiSourceSignalGenerator(SignalGenerator):
     """More optimal signal generator for multiple sources.
     """
-    def __init__(self, src_hypo_group_manager, dataset_list, data_list):
+    def __init__(self, src_hypo_group_manager, dataset_list, data_list,
+                **kwargs):
         """Constructs a new signal generator instance.
 
         Parameters
         ----------
         src_hypo_group_manager : SourceHypoGroupManager instance
             The SourceHypoGroupManager instance defining the source groups with
             their spectra.
         dataset_list : list of Dataset instances
             The list of Dataset instances for which signal events should get
             generated for.
         data_list : list of DatasetData instances
             The list of DatasetData instances holding the actual data of each
             dataset. The order must match the order of ``dataset_list``.
+        kwargs
+            A typical keyword argument is the instance of MultiDatasetTCLLHRatio.
         """
         super(MultiSourceSignalGenerator, self).__init__(
-            src_hypo_group_manager, dataset_list, data_list)
+            src_hypo_group_manager, dataset_list, data_list, **kwargs)
 
     def _construct_signal_candidates(self):
         """Constructs an array holding pointer information of signal candidate
         events pointing into the real MC dataset(s).
         """
         n_datasets = len(self._dataset_list)
         n_sources = self._src_hypo_group_manager.n_sources
```

### Comparing `skyllh-23.0.0/skyllh/core/signalpdf.py` & `skyllh-23.1.0/skyllh/analyses/i3/publicdata_ps/backgroundpdf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,506 +1,450 @@
 # -*- coding: utf-8 -*-
 
-"""The ``signalpdf`` module contains possible signal PDF models for the
-likelihood function.
-"""
-
 import numpy as np
-import scipy as scp
 
-from skyllh.core import display
-from skyllh.core.py import (
-    classname,
-    issequenceof
+from skyllh.core.binning import (
+    BinningDefinition,
+    UsesBinning,
 )
-from skyllh.core.livetime import Livetime
 from skyllh.core.pdf import (
-    PDFAxis,
-    IsSignalPDF,
-    MultiDimGridPDF,
-    MultiDimGridPDFSet,
-    MappedMultiDimGridPDFSet,
-    NDPhotosplinePDF,
-    SpatialPDF,
-    TimePDF
+    EnergyPDF,
+    IsBackgroundPDF,
+    PDFAxis
 )
-from skyllh.core.source_hypothesis import SourceHypoGroupManager
-from skyllh.physics.source import PointLikeSource
-from skyllh.physics.time_profile import TimeProfileModel
-
+from skyllh.core.storage import DataFieldRecordArray
+from skyllh.core.timing import TaskTimer
+from skyllh.core.smoothing import (
+    UNSMOOTH_AXIS,
+    SmoothingFilter,
+    HistSmoothingMethod,
+    NoHistSmoothingMethod,
+    NeighboringBinHistSmoothingMethod
+)
+from skyllh.core.timing import TaskTimer
 
-class GaussianPSFPointLikeSourceSignalSpatialPDF(SpatialPDF, IsSignalPDF):
-    """This spatial signal PDF model describes the spatial PDF for a point
-    source smeared with a 2D gaussian point-spread-function (PSF).
-    Mathematically, it's the convolution of a point in the sky, i.e. the source
-    location, with the PSF. The result of this convolution has the gaussian form
+from scipy.stats import gaussian_kde
 
-        1/(2*\pi*\sigma^2) * exp(-1/2*(r / \sigma)**2),
 
-    where \sigma is the spatial uncertainty of the event and r the distance on
-    the sphere between the source and the data event.
+class PDEnergyPDF(EnergyPDF, UsesBinning):
+    """This is the base class for IceCube specific energy PDF models.
+    IceCube energy PDFs depend solely on the energy and the
+    zenith angle, and hence, on the declination of the event.
 
-    This PDF requires the `src_array` data field, that is numpy record ndarray
-    with the data fields `ra` and `dec` holding the right-ascention and
-    declination of the point-like sources, respectively.
+    The IceCube energy PDF is modeled as a 1d histogram in energy,
+    but for different sin(declination) bins, hence, stored as a 2d histogram.
     """
 
-    def __init__(self, ra_range=None, dec_range=None, **kwargs):
-        """Creates a new spatial signal PDF for point-like sources with a
-        gaussian point-spread-function (PSF).
+    _KDE_BW_NORTH = 0.4
+    _KDE_BW_SOUTH = 0.32
 
-        Parameters
-        ----------
-        ra_range : 2-element tuple | None
-            The range in right-ascention this spatial PDF is valid for.
-            If set to None, the range (0, 2pi) is used.
-        dec_range : 2-element tuple | None
-            The range in declination this spatial PDF is valid for.
-            If set to None, the range (-pi/2, +pi/2) is used.
-        """
-        if(ra_range is None):
-            ra_range = (0, 2*np.pi)
-        if(dec_range is None):
-            dec_range = (-np.pi/2, np.pi/2)
-
-        super(GaussianPSFPointLikeSourceSignalSpatialPDF, self).__init__(
-            ra_range=ra_range,
-            dec_range=dec_range,
-            **kwargs)
-
-    def get_prob(self, tdm, fitparams=None, tl=None):
-        """Calculates the spatial signal probability of each event for all given
-        sources.
+    def __init__(self, data_logE, data_sinDec, data_mcweight, data_physicsweight,
+                 logE_binning, sinDec_binning, smoothing_filter, kde_smoothing=False):
+        """Creates a new IceCube energy PDF object.
 
         Parameters
         ----------
-        tdm : instance of TrialDataManager
-            The TrialDataManager instance holding the trial event data for which
-            to calculate the PDF values. The following data fields need to be
-            present:
-
-            'src_array' : numpy record ndarray
-                The numpy record ndarray with the following data fields:
-
-                `ra`: float
-                    The right-ascention of the point-like source.
-                `dec`: float
-                    The declination of the point-like source.
-
-            'ra' : float
-                The right-ascention in radian of the data event.
-            'dec' : float
-                The declination in radian of the data event.
-            'ang_err': float
-                The reconstruction uncertainty in radian of the data event.
-        fitparams : None
-            Unused interface argument.
-        tl : TimeLord instance | None
-            The optional TimeLord instance to use for measuring timing
-            information.
-
-        Returns
-        -------
-        prob : (N_sources,N_events) shaped 2D ndarray
-            The ndarray holding the spatial signal probability on the sphere for
-            each source and event.
-        """
-        get_data = tdm.get_data
-        src_ev_idxs = tdm.src_ev_idxs
-
-        ra = get_data('ra')
-        dec = get_data('dec')
-        sigma = get_data('ang_err')
-
-        if len(ra) == 1:
-            self.param_set = None
-
-        try:
-            # angular difference is pre calculated
-            prob = get_data('spatial_pdf_gauss')
-            src_ra = get_data('src_array')['ra']
-
-            if src_ev_idxs is None:
-                prob = prob.reshape((len(get_data('src_array')), len(ra)))
-            else:
-                (src_idxs, ev_idxs) = src_ev_idxs
-                sigma = np.take(sigma, src_ev_idxs[1])
-
-        except:
-            # psi is calculated here
-            if src_ev_idxs is None:
-                # Make the source position angles two-dimensional so the PDF value can
-                # be calculated via numpy broadcasting automatically for several
-                # sources. This is useful for stacking analyses.
-                src_ra = get_data('src_array')['ra'][:, np.newaxis]
-                src_dec = get_data('src_array')['dec'][:, np.newaxis]
-
-                delta_dec = np.abs(dec - src_dec)
-                delta_ra = np.abs(ra - src_ra)
-                x = (np.sin(delta_dec / 2.))**2. + np.cos(dec) *\
-                    np.cos(src_dec) * (np.sin(delta_ra / 2.))**2.
-            else:
-                # Calculate the angular difference only for events that are close
-                # to the respective source poisition. This is useful for stacking
-                # analyses.
-                (src_idxs, ev_idxs) = src_ev_idxs
-                src_ra = get_data('src_array')['ra'][src_idxs]
-                src_dec = get_data('src_array')['dec'][src_idxs]
-
-                delta_dec = np.abs(np.take(dec, ev_idxs) - src_dec)
-                delta_ra = np.abs(np.take(ra, ev_idxs) - src_ra)
-                x = (np.sin(delta_dec / 2.))**2. + np.cos(np.take(dec, ev_idxs)) *\
-                    np.cos(src_dec) * (np.sin(delta_ra / 2.))**2.
-
-                # also extend the sigma array to account for all relevant events
-                sigma = np.take(sigma, ev_idxs)
-
-                # Handle possible floating precision errors.
-            x[x < 0.] = 0.
-            x[x > 1.] = 1.
-
-            psi = (2.0*np.arcsin(np.sqrt(x)))
-
-            prob = 0.5/(np.pi*sigma**2)*np.exp(-0.5*(psi/sigma)**2)
-
-        # If the signal hypothesis contains single source
-        # return the output here.
-        if(len(get_data('src_array')['ra']) == 1):
-            grads = np.array([], dtype=np.float64)
-            # The new interface returns the pdf only for a single source.
-            return (prob[0], grads)
+        data_logE : 1d ndarray
+            The array holding the log10(E) values of the events.
+        data_sinDec : 1d ndarray
+            The array holding the sin(dec) values of the events.
+        data_mcweight : 1d ndarray
+            The array holding the monte-carlo weights of the events.
+            The final data weight will be the product of data_mcweight and
+            data_physicsweight.
+        data_physicsweight : 1d ndarray
+            The array holding the physics weights of the events.
+            The final data weight will be the product of data_mcweight and
+            data_physicsweight.
+        logE_binning : BinningDefinition
+            The binning definition for the log(E) axis.
+        sinDec_binning : BinningDefinition
+            The binning definition for the sin(declination) axis.
+        smoothing_filter : SmoothingFilter instance | None
+            The smoothing filter to use for smoothing the energy histogram.
+            If None, no smoothing will be applied.
+        kde_smoothing : bool
+            Apply a kde smoothing to the energy pdf for each bin in sin(dec).
+            This is useful for signal injections, because it ensures that the
+            background is not zero when injecting high energy events.
+            Default: False.
+        """
+        super(PDEnergyPDF, self).__init__()
+
+        # Define the PDF axes.
+        self.add_axis(PDFAxis(name='log_energy',
+                              vmin=logE_binning.lower_edge,
+                              vmax=logE_binning.upper_edge))
+        self.add_axis(PDFAxis(name='sin_dec',
+                              vmin=sinDec_binning.lower_edge,
+                              vmax=sinDec_binning.upper_edge))
+
+        self.add_binning(logE_binning, 'log_energy')
+        self.add_binning(sinDec_binning, 'sin_dec')
+
+        # Create the smoothing method instance tailored to the energy PDF.
+        # We will smooth only the first axis (logE).
+        if((smoothing_filter is not None) and
+           (not isinstance(smoothing_filter, SmoothingFilter))):
+            raise TypeError(
+                'The smoothing_filter argument must be None or an instance of SmoothingFilter!')
+        if(smoothing_filter is None):
+            self.hist_smoothing_method = NoHistSmoothingMethod()
         else:
-            # If the signal hypothesis contains multiple sources convolve
-            # the pdfs with the source weights.
-            src_w = get_data('src_array')['src_w'] * tdm.get_data('src_array')['src_w_W']
-            src_w_grads = get_data('src_array')['src_w_grad'] * tdm.get_data('src_array')['src_w_W']
-
-            norm = src_w.sum()
-            src_w /= norm
-            src_w_grads /= norm
-
-            if src_ev_idxs is not None:
-                prob = scp.sparse.csr_matrix((prob, (ev_idxs, src_idxs)))
-            else:
-                prob = prob.T
-            prob_res = prob.dot(src_w)
-            grads = (prob.dot(src_w_grads) -
-                     prob_res*src_w_grads.sum())
-
-            return (prob_res, np.atleast_2d(grads))
-
-
-class SignalTimePDF(TimePDF, IsSignalPDF):
-    """This class provides a time PDF class for a signal source. It consists of
-    a Livetime instance and a TimeProfileModel instance. Together they construct
-    the actual signal time PDF, which has detector down-time taking into
-    account.
-    """
-
-    def __init__(self, livetime, time_profile):
-        """Creates a new signal time PDF instance for a given time profile of
-        the source.
+            self.hist_smoothing_method = NeighboringBinHistSmoothingMethod(
+                (smoothing_filter.axis_kernel_array, UNSMOOTH_AXIS))
 
-        Parameters
-        ----------
-        livetime : Livetime instance
-            An instance of Livetime, which provides the detector live-time
-            information.
-        time_profile : TimeProfileModel instance
-            The time profile of the source.
-        """
-        super(SignalTimePDF, self).__init__()
+        # We have to figure out, which histogram bins are zero due to no
+        # monte-carlo coverage, and which due to zero physics model
+        # contribution.
+
+        # Create a 2D histogram with only the MC events to determine the MC
+        # coverage.
+        (h, bins_logE, bins_sinDec) = np.histogram2d(
+            data_logE, data_sinDec,
+            bins=[
+                logE_binning.binedges, sinDec_binning.binedges],
+            range=[
+                logE_binning.range, sinDec_binning.range],
+            density=False)
+        h = self._hist_smoothing_method.smooth(h)
+        self._hist_mask_mc_covered = h > 0
+
+        # Select the events which have MC coverage but zero physics
+        # contribution, i.e. the physics model predicts zero contribution.
+        mask = data_physicsweight == 0.
+
+        # Create a 2D histogram with only the MC events that have zero physics
+        # contribution. Note: By construction the zero physics contribution bins
+        # are a subset of the MC covered bins.
+        (h, bins_logE, bins_sinDec) = np.histogram2d(
+            data_logE[mask], data_sinDec[mask],
+            bins=[
+                logE_binning.binedges, sinDec_binning.binedges],
+            range=[
+                logE_binning.range, sinDec_binning.range],
+            density=False)
+        h = self._hist_smoothing_method.smooth(h)
+        self._hist_mask_mc_covered_zero_physics = h > 0
+
+        if kde_smoothing:
+            # If a bandwidth is passed, apply a KDE-based smoothing with the given
+            # bw parameter as bandwidth for the fit.
+            if not isinstance(kde_smoothing, bool):
+                raise ValueError(
+                    "The bandwidth parameter must be True or False!")
+            kde_pdf = np.empty(
+                (len(sinDec_binning.bincenters),), dtype=object)
+            data_logE_masked = data_logE[~mask]
+            data_sinDec_masked = data_sinDec[~mask]
+            for i in range(len(sinDec_binning.bincenters)):
+                sindec_mask = np.logical_and(
+                    data_sinDec_masked >= sinDec_binning.binedges[i],
+                    data_sinDec_masked < sinDec_binning.binedges[i+1]
+                )
+                this_energy = data_logE_masked[sindec_mask]
+                if sinDec_binning.binedges[i] >= 0:
+                    kde_pdf[i] = gaussian_kde(
+                        this_energy, bw_method=self._KDE_BW_NORTH)
+                else:
+                    kde_pdf[i] = gaussian_kde(
+                        this_energy, bw_method=self._KDE_BW_SOUTH)
+            h = np.vstack(
+                [kde_pdf[i].evaluate(logE_binning.bincenters)
+                 for i in range(len(sinDec_binning.bincenters))]).T
 
-        self.livetime = livetime
-        self.time_profile = time_profile
+        else:
+            # Create a 2D histogram with only the data which has physics
+            # contribution. We will do the normalization along the logE
+            # axis manually.
+            data_weights = data_mcweight[~mask] * data_physicsweight[~mask]
+            (h, bins_logE, bins_sinDec) = np.histogram2d(
+                data_logE[~mask], data_sinDec[~mask],
+                bins=[
+                    logE_binning.binedges, sinDec_binning.binedges],
+                weights=data_weights,
+                range=[
+                    logE_binning.range, sinDec_binning.range],
+                density=False)
+
+        # Calculate the normalization for each logE bin. Hence we need to sum
+        # over the logE bins (axis 0) for each sin(dec) bin and need to divide
+        # by the logE bin widths along the sin(dec) bins. The result array norm
+        # is a 2D array of the same shape as h.
+        norms = np.sum(h, axis=(0,))[np.newaxis, ...] * \
+            np.diff(logE_binning.binedges)[..., np.newaxis]
+        h /= norms
+        h = self._hist_smoothing_method.smooth(h)
 
-        # Define the time axis with the time boundaries of the live-time.
-        self.add_axis(PDFAxis(
-            name='time',
-            vmin=self._livetime.time_window[0],
-            vmax=self._livetime.time_window[1]))
-
-        # Get the total integral, I, of the time profile and the sum, S, of the
-        # integrals for each detector on-time interval during the time profile,
-        # in order to be able to rescale the time profile to unity with
-        # overlapping detector off-times removed.
-        (self._I, self._S) = self._calculate_time_profile_I_and_S()
+        self._hist_logE_sinDec = h
 
     @property
-    def livetime(self):
-        """The instance of Livetime, which provides the detector live-time
-        information.
-        """
-        return self._livetime
-
-    @livetime.setter
-    def livetime(self, lt):
-        if(not isinstance(lt, Livetime)):
+    def hist_smoothing_method(self):
+        """The HistSmoothingMethod instance defining the smoothing filter of the
+        energy PDF histogram.
+        """
+        return self._hist_smoothing_method
+
+    @hist_smoothing_method.setter
+    def hist_smoothing_method(self, method):
+        if(not isinstance(method, HistSmoothingMethod)):
             raise TypeError(
-                'The livetime property must be an instance of Livetime!')
-        self._livetime = lt
+                'The hist_smoothing_method property must be an instance of HistSmoothingMethod!')
+        self._hist_smoothing_method = method
 
     @property
-    def time_profile(self):
-        """The instance of TimeProfileModel providing the (assumed) physical
-        time profile of the source.
-        """
-        return self._time_profile
-
-    @time_profile.setter
-    def time_profile(self, tp):
-        if(not isinstance(tp, TimeProfileModel)):
-            raise TypeError(
-                'The time_profile property must be an instance of '
-                'TimeProfileModel!')
-        self._time_profile = tp
-
-    def __str__(self):
-        """Pretty string representation of the signal time PDF.
-        """
-        s = '%s(\n' % (classname(self))
-        s += ' '*display.INDENTATION_WIDTH + \
-            'livetime = %s,\n' % (str(self._livetime))
-        s += ' '*display.INDENTATION_WIDTH + \
-            'time_profile = %s\n' % (str(self._time_profile))
-        s += ')'
-        return s
-
-    def _calculate_time_profile_I_and_S(self):
-        """Calculates the total integral, I, of the time profile and the sum, A,
-        of the time-profile integrals during the detector on-time intervals.
-
-        Returns
-        -------
-        I : float
-            The total integral of the source time-profile.
-        S : float
-            The sum of the source time-profile integrals during the detector
-            on-time intervals.
-        """
-        ontime_intervals = self._livetime.get_ontime_intervals_between(
-            self._time_profile.t_start, self._time_profile.t_end)
-        I = self._time_profile.get_total_integral()
-        S = np.sum(self._time_profile.get_integral(
-            ontime_intervals[:, 0], ontime_intervals[:, 1]))
-        return (I, S)
-
-    def assert_is_valid_for_exp_data(self, data_exp):
-        """Checks if the time PDF is valid for all the given experimental data.
-        It checks if the time of all events is within the defined time axis of
-        the PDF.
+    def hist(self):
+        """(read-only) The 2D logE-sinDec histogram array.
+        """
+        return self._hist_logE_sinDec
 
-        Parameters
-        ----------
-        data_exp : numpy record ndarray
-            The array holding the experimental data. The following data fields
-            must exist:
+    @property
+    def hist_mask_mc_covered(self):
+        """(read-only) The boolean ndarray holding the mask of the 2D histogram
+        bins for which there is monte-carlo coverage.
+        """
+        return self._hist_mask_mc_covered
 
-            - 'time' : float
-                The MJD time of the data event.
+    @property
+    def hist_mask_mc_covered_zero_physics(self):
+        """(read-only) The boolean ndarray holding the mask of the 2D histogram
+        bins for which there is monte-carlo coverage but zero physics
+        contribution.
+        """
+        return self._hist_mask_mc_covered_zero_physics
 
-        Raises
-        ------
-        ValueError
-            If some of the data is outside the time range of the PDF.
+    @property
+    def hist_mask_mc_covered_with_physics(self):
+        """(read-only) The boolean ndarray holding the mask of the 2D histogram
+        bins for which there is monte-carlo coverage and has physics
+        contribution.
         """
-        time_axis = self.get_axis('time')
+        return self._hist_mask_mc_covered & ~self._hist_mask_mc_covered_zero_physics
 
-        if(np.any((data_exp['time'] < time_axis.vmin) |
-                  (data_exp['time'] > time_axis.vmax))):
-            raise ValueError('Some data is outside the time range (%.3f, %.3f)!' % (
-                time_axis.vmin, time_axis.vmax))
-
-    def get_prob(self, tdm, fitparams):
-        """Calculates the signal time probability of each event for the given
-        set of signal time fit parameter values.
+    def get_prob(self, tdm, fitparams=None, tl=None):
+        """Calculates the energy probability (in logE) of each event.
 
         Parameters
         ----------
         tdm : instance of TrialDataManager
-            The instance of TrialDataManager holding the trial event data for
-            which to calculate the PDF value. The following data fields must
+            The TrialDataManager instance holding the data events for which the
+            probability should be calculated for. The following data fields must
             exist:
 
-            - 'time' : float
-                The MJD time of the event.
-        fitparams : dict
-            The dictionary holding the signal time parameter values for which
-            the signal time probability should be calculated.
+            - 'log_energy' : float
+                The logarithm of the energy value of the event.
+            - 'sin_dec' : float
+                The sin(declination) value of the event.
+
+        fitparams : None
+            Unused interface parameter.
+        tl : TimeLord instance | None
+            The optional TimeLord instance that should be used to measure
+            timing information.
 
         Returns
         -------
-        prob : array of float
-            The (N,)-shaped ndarray holding the probability for each event.
+        prob : 1D (N_events,) shaped ndarray
+            The array with the energy probability for each event.
         """
-        # Update the time-profile if its fit-parameter values have changed and
-        # recalculate self._I and self._S if an updated was actually performed.
-        updated = self._time_profile.update(fitparams)
-        if(updated):
-            (self._I, self._S) = self._calculate_time_profile_I_and_S()
-
-        events_time = tdm.get_data('time')
-
-        # Get a mask of the event times which fall inside a detector on-time
-        # interval.
-        on = self._livetime.is_on(events_time)
-
-        # The sum of the on-time integrals of the time profile, A, will be zero
-        # if the time profile is entirly during detector off-time.
-        prob = np.zeros((tdm.n_selected_events,), dtype=np.float64)
-        if(self._S > 0):
-            prob[on] = self._time_profile.get_value(
-                events_time[on]) / (self._I * self._S)
+        get_data = tdm.get_data
+
+        logE_binning = self.get_binning('log_energy')
+        sinDec_binning = self.get_binning('sin_dec')
+
+        logE_idx = np.digitize(
+            get_data('log_energy'), logE_binning.binedges) - 1
+        sinDec_idx = np.digitize(
+            get_data('sin_dec'), sinDec_binning.binedges) - 1
+
+        with TaskTimer(tl, 'Evaluating logE-sinDec histogram.'):
+            prob = self._hist_logE_sinDec[(logE_idx, sinDec_idx)]
 
         return prob
 
 
-class SignalMultiDimGridPDF(MultiDimGridPDF, IsSignalPDF):
-    """This class provides a multi-dimensional signal PDF. The PDF is created
-    from pre-calculated PDF data on a grid. The grid data is interpolated using
-    a :class:`scipy.interpolate.RegularGridInterpolator` instance.
+class PDDataBackgroundI3EnergyPDF(PDEnergyPDF, IsBackgroundPDF):
+    """This is the IceCube energy background PDF, which gets constructed from
+    experimental data. This class is derived from I3EnergyPDF.
     """
 
-    def __init__(self, axis_binnings, path_to_pdf_splinetable=None,
-                 pdf_grid_data=None, norm_factor_func=None):
-        """Creates a new signal PDF instance for a multi-dimensional PDF given
-        as PDF values on a grid. The grid data is interpolated with a
-        :class:`scipy.interpolate.RegularGridInterpolator` instance. As grid
-        points the bin edges of the axis binning definitions are used.
+    def __init__(self, data_exp, logE_binning, sinDec_binning,
+                 smoothing_filter=None, kde_smoothing=False):
+        """Constructs a new IceCube energy background PDF from experimental
+        data.
 
         Parameters
         ----------
-        axis_binnings : sequence of BinningDefinition
-            The sequence of BinningDefinition instances defining the binning of
-            the PDF axes. The name of each BinningDefinition instance defines
-            the event field name that should be used for querying the PDF.
-        path_to_pdf_splinetable : str
-            The path to the file containing the spline table.
-            The spline table contains a  pre-computed fit to pdf_grid_data.
-        pdf_grid_data : n-dimensional numpy ndarray
-            The n-dimensional numpy ndarray holding the PDF values at given grid
-            points. The grid points must match the bin edges of the given
-            BinningDefinition instances of the `axis_binnings` argument.
-        norm_factor_func : callable | None
-            The function that calculates a possible required normalization
-            factor for the PDF value based on the event properties.
-            The call signature of this function
-            must be `__call__(pdf, events, fitparams)`, where `pdf` is this PDF
-            instance, `events` is a numpy record ndarray holding the events for
-            which to calculate the PDF values, and `fitparams` is a dictionary
-            with the current fit parameter names and values.
-        """
-        super(SignalMultiDimGridPDF, self).__init__(
-            axis_binnings=axis_binnings,
-            path_to_pdf_splinetable=path_to_pdf_splinetable,
-            pdf_grid_data=pdf_grid_data,
-            norm_factor_func=norm_factor_func)
-
-
-class SignalMultiDimGridPDFSet(MultiDimGridPDFSet, IsSignalPDF):
-    """This class extends the MultiDimGridPDFSet PDF class to be a signal PDF.
-    See the documentation of the :class:`skyllh.core.pdf.MultiDimGridPDFSet`
-    class for what this PDF provides.
+        data_exp : instance of DataFieldRecordArray
+            The array holding the experimental data. The following data fields
+            must exist:
+
+            - 'log_energy' : float
+                The logarithm of the reconstructed energy value of the data
+                event.
+            - 'sin_dec' : float
+                The sine of the reconstructed declination of the data event.
+
+        logE_binning : BinningDefinition
+            The binning definition for the binning in log10(E).
+        sinDec_binning : BinningDefinition
+            The binning definition for the sin(declination).
+        smoothing_filter : SmoothingFilter instance | None
+            The smoothing filter to use for smoothing the energy histogram.
+            If None, no smoothing will be applied.
+        """
+        if(not isinstance(data_exp, DataFieldRecordArray)):
+            raise TypeError('The data_exp argument must be an instance of '
+                            'DataFieldRecordArray!')
+
+        data_logE = data_exp['log_energy']
+        data_sinDec = data_exp['sin_dec']
+        # For experimental data, the MC and physics weight are unity.
+        data_mcweight = np.ones((len(data_exp),))
+        data_physicsweight = data_mcweight
+
+        # Create the PDF using the base class.
+        super(PDDataBackgroundI3EnergyPDF, self).__init__(
+            data_logE, data_sinDec, data_mcweight, data_physicsweight,
+            logE_binning, sinDec_binning, smoothing_filter, kde_smoothing
+        )
+
+
+class PDMCBackgroundI3EnergyPDF(EnergyPDF, IsBackgroundPDF, UsesBinning):
+    """This class provides a background energy PDF constructed from the public
+    data and a monte-carlo background flux model.
     """
 
-    def __init__(self, param_set, param_grid_set, gridparams_pdfs,
-                 interpolmethod=None, **kwargs):
-        """Creates a new SignalMultiDimGridPDFSet instance, which holds a set of
-        MultiDimGridPDF instances, one for each point of a parameter grid set.
+    def __init__(
+            self, pdf_log10emu_sindecmu, log10emu_binning, sindecmu_binning,
+            **kwargs):
+        """Constructs a new background energy PDF with the given PDF data and
+        binning.
 
         Parameters
         ----------
-        param_set : Parameter instance | sequence of Parameter instances |
-                    ParameterSet instance
-            The set of parameters defining the model parameters of this PDF.
-        param_grid_set : ParameterGrid instance | ParameterGridSet instance
-            The set of ParameterGrid instances, which define the grid values of
-            the model parameters, the given MultiDimGridPDF instances belong to.
-        gridparams_pdfs : sequence of (dict, MultiDimGridPDF) tuples
-            The sequence of 2-element tuples which define the mapping of grid
-            values to PDF instances.
-        interpolmethod : subclass of GridManifoldInterpolationMethod
-            The class specifying the interpolation method. This must be a
-            subclass of ``GridManifoldInterpolationMethod``.
-            If set to None, the default grid manifold interpolation method
-            ``Linear1DGridManifoldInterpolationMethod`` will be used.
-        """
-        super(SignalMultiDimGridPDFSet, self).__init__(
-            param_set=param_set,
-            param_grid_set=param_grid_set,
-            gridparams_pdfs=gridparams_pdfs,
-            interpolmethod=interpolmethod,
-            pdf_type=SignalMultiDimGridPDF,
-            **kwargs)
-
-
-class SignalMappedMultiDimGridPDFSet(MappedMultiDimGridPDFSet, IsSignalPDF):
-    """This class extends the MappedMultiDimGridPDFSet PDF class to be a signal
-    PDF. See the documentation of the
-    :class:`skyllh.core.pdf.MappedMultiDimGridPDFSet` class for what this PDF
-    provides.
-    """
+        pdf_log10emu_sindecmu : 2D numpy ndarray
+            The (n_log10emu, n_sindecmu)-shaped 2D numpy ndarray holding the
+            PDF values in unit 1/log10(E_mu/GeV).
+            A copy of this data will be created and held within this class
+            instance.
+        log10emu_binning : BinningDefinition
+            The binning definition for the binning in log10(E_mu/GeV).
+        sindecmu_binning : BinningDefinition
+            The binning definition for the binning in sin(dec_mu).
+        """
+        if not isinstance(pdf_log10emu_sindecmu, np.ndarray):
+            raise TypeError(
+                'The pdf_log10emu_sindecmu argument must be an instance of '
+                'numpy.ndarray!')
+        if not isinstance(sindecmu_binning, BinningDefinition):
+            raise TypeError(
+                'The sindecmu_binning argument must be an instance of '
+                'BinningDefinition!')
+        if not isinstance(log10emu_binning, BinningDefinition):
+            raise TypeError(
+                'The log10emu_binning argument must be an instance of '
+                'BinningDefinition!')
+
+        super().__init__(**kwargs)
+
+        self.add_axis(PDFAxis(
+            log10emu_binning.name,
+            log10emu_binning.lower_edge,
+            log10emu_binning.upper_edge,
+        ))
 
-    def __init__(self, param_grid_set, gridparams_pdfs,
-                 interpolmethod=None, **kwargs):
-        """Creates a new SignalMappedMultiDimGridPDFSet instance, which holds a
-        set of MultiDimGridPDF instances, one for each point of a parameter grid
-        set.
+        self.add_axis(PDFAxis(
+            sindecmu_binning.name,
+            sindecmu_binning.lower_edge,
+            sindecmu_binning.upper_edge,
+        ))
+
+        self._hist_logE_sinDec = np.copy(pdf_log10emu_sindecmu)
+        self.add_binning(log10emu_binning, name='log_energy')
+        self.add_binning(sindecmu_binning, name='sin_dec')
+
+    def assert_is_valid_for_trial_data(self, tdm):
+        """Checks if this PDF covers the entire value range of the trail
+        data events.
 
         Parameters
         ----------
-        param_grid_set : ParameterGrid instance | ParameterGridSet instance
-            The set of ParameterGrid instances, which define the grid values of
-            the model parameters, the given MultiDimGridPDF instances belong to.
-        gridparams_pdfs : sequence of (dict, MultiDimGridPDF) tuples
-            The sequence of 2-element tuples which define the mapping of grid
-            values to PDF instances.
-        """
-        super(SignalMappedMultiDimGridPDFSet, self).__init__(
-            param_grid_set=param_grid_set,
-            gridparams_pdfs=gridparams_pdfs,
-            pdf_type=SignalMultiDimGridPDF,
-            **kwargs)
-
-
-class SignalNDPhotosplinePDF(NDPhotosplinePDF, IsSignalPDF):
-    """This class provides a multi-dimensional signal PDF created from a
-    n-dimensional photospline fit. The photospline package is used to evaluate
-    the PDF fit.
-    """
+        tdm : TrialDataManager instance
+            The TrialDataManager instance holding the data events.
+            The following data fields need to exist:
 
-    def __init__(
-            self,
-            axis_binnings,
-            param_set,
-            path_to_pdf_splinefit,
-            norm_factor_func=None):
-        """Creates a new signal PDF instance for a n-dimensional photospline PDF
-        fit.
+                'sin_dec'
+
+                'log_energy'
+
+        Raises
+        ------
+        ValueError
+            If parts of the trial data is outside the value range of this
+            PDF.
+        """
+        sindecmu = tdm.get_data('sin_dec')
+        if np.min(sindecmu) < self.get_axis(0).vmin:
+            raise ValueError(
+                'The minimum sindecmu value %e of the trial data is lower '
+                'than the minimum value of the PDF %e!' % (
+                    np.min(sindecmu), self.get_axis(0).vmin))
+        if np.max(sindecmu) > self.get_axis(0).vmax:
+            raise ValueError(
+                'The maximum sindecmu value %e of the trial data is larger '
+                'than the maximum value of the PDF %e!' % (
+                    np.max(sindecmu), self.get_axis(0).vmax))
+
+        log10emu = tdm.get_data('log_energy')
+        if np.min(log10emu) < self.get_axis(1).vmin:
+            raise ValueError(
+                'The minimum log10emu value %e of the trial data is lower '
+                'than the minimum value of the PDF %e!' % (
+                    np.min(log10emu), self.get_axis(1).vmin))
+        if np.max(log10emu) > self.get_axis(1).vmax:
+            raise ValueError(
+                'The maximum log10emu value %e of the trial data is larger '
+                'than the maximum value of the PDF %e!' % (
+                    np.max(log10emu), self.get_axis(1).vmax))
+
+    def get_prob(self, tdm, params=None, tl=None):
+        """Gets the probability density for the given trial data events.
 
         Parameters
         ----------
-        axis_binnings : BinningDefinition | sequence of BinningDefinition
-            The sequence of BinningDefinition instances defining the binning of
-            the PDF axes. The name of each BinningDefinition instance defines
-            the event field name that should be used for querying the PDF.
-        param_set : Parameter | ParameterSet
-            The Parameter instance or ParameterSet instance defining the
-            parameters of this PDF. The ParameterSet holds the information
-            which parameters are fixed and which are floating (i.e. fitted).
-        path_to_pdf_splinefit : str
-            The path to the file containing the photospline fit.
-        norm_factor_func : callable | None
-            The function that calculates a possible required normalization
-            factor for the PDF value based on the event properties.
-            The call signature of this function must be
-            `__call__(pdf, tdm, params)`, where `pdf` is this PDF
-            instance, `tdm` is an instance of TrialDataManager holding the
-            event data for which to calculate the PDF values, and `params` is a
-            dictionary with the current parameter names and values.
-        """
-        super(SignalNDPhotosplinePDF, self).__init__(
-            axis_binnings=axis_binnings,
-            param_set=param_set,
-            path_to_pdf_splinefit=path_to_pdf_splinefit,
-            norm_factor_func=norm_factor_func
-        )
+        tdm : TrialDataManager instance
+            The TrialDataManager instance holding the data events.
+            The following data fields need to exist:
+
+                'sin_dec'
+
+                'log_energy'
+
+        params : dict | None
+            The dictionary containing the parameter names and values for which
+            the probability should get calculated.
+            By definition of this PDF, this is ``Ǹone``, because this PDF does
+            not depend on any parameters.
+        tl : TimeLord instance | None
+            The optional TimeLord instance that should be used to measure
+            timing information.
+
+        Returns
+        -------
+        prob : (N_events,)-shaped numpy ndarray
+            The 1D numpy ndarray with the probability density for each event.
+        """
+        get_data = tdm.get_data
+
+        log10emu = get_data('log_energy')
+        sindecmu = get_data('sin_dec')
+
+        log10emu_idxs = np.digitize(
+            log10emu, self.get_binning('log_energy').binedges) - 1
+        sindecmu_idxs = np.digitize(
+            sindecmu, self.get_binning('sin_dec').binedges) - 1
+
+        with TaskTimer(tl, 'Evaluating sindecmu-log10emu PDF.'):
+            pd = self._hist_logE_sinDec[(log10emu_idxs, sindecmu_idxs)]
+
+        return pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skyllh-23.0.0/skyllh/core/smoothing.py` & `skyllh-23.1.0/skyllh/core/smoothing.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/source_hypo_group.py` & `skyllh-23.1.0/skyllh/core/source_hypo_group.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/source_hypothesis.py` & `skyllh-23.1.0/skyllh/core/source_hypothesis.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/storage.py` & `skyllh-23.1.0/skyllh/core/storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,26 +77,28 @@
     formats = sorted(_FILE_LOADER_REG.keys())
     for fmt in formats:
         l = len(fmt)
         if(pathfilenames[0][-l:].lower() == fmt.lower()):
             cls = _FILE_LOADER_REG[fmt]
             return cls(pathfilenames, **kwargs)
 
-    raise RuntimeError('No FileLoader class is suitable to load the data file "%s"!'%(pathfilenames[0]))
+    raise RuntimeError('No FileLoader class is suitable to load the data file '
+        '"%s"!'%(pathfilenames[0]))
 
 def assert_file_exists(pathfilename):
     """Checks if the given file exists and raises a RuntimeError if it does
     not exist.
     """
     if(not os.path.isfile(pathfilename)):
         raise RuntimeError('The data file "%s" does not exist!'%(pathfilename))
 
 
 class FileLoader(object, metaclass=abc.ABCMeta):
-
+    """Abstract base class for a FileLoader class.
+    """
     def __init__(self, pathfilenames, **kwargs):
         """Initializes a new FileLoader instance.
 
         Parameters
         ----------
         pathfilenames : str | sequence of str
             The sequence of fully qualified file names of the data files that
@@ -404,14 +406,232 @@
 
         if(len(data) == 1):
             data = data[0]
 
         return data
 
 
+class TextFileLoader(FileLoader):
+    """The TextFileLoader class provides the data loading functionality for
+    data text files where values are stored in a comma, or whitespace, separated
+    format. It uses the numpy.loadtxt function to load the data. It reads the
+    first line of the text file for a table header.
+    """
+    def __init__(self, pathfilenames, header_comment='#', header_separator=None,
+            **kwargs):
+        """Creates a new file loader instance for a text data file.
+
+        Parameters
+        ----------
+        pathfilenames : str | sequence of str
+            The sequence of fully qualified file names of the data files that
+            need to be loaded.
+        header_comment : str
+            The character that defines a comment line in the text file.
+        header_separator : str | None
+            The separator of the header field names. If None, it assumes
+            whitespaces.
+        """
+        super().__init__(pathfilenames, **kwargs)
+
+        self.header_comment = header_comment
+        self.header_separator = header_separator
+
+    @property
+    def header_comment(self):
+        """The character that defines a comment line in the text file.
+        """
+        return self._header_comment
+    @header_comment.setter
+    def header_comment(self, s):
+        if(not isinstance(s, str)):
+            raise TypeError('The header_comment property must be of type str!')
+        self._header_comment = s
+
+    @property
+    def header_separator(self):
+        """The separator of the header field names. If None, it assumes
+        whitespaces.
+        """
+        return self._header_separator
+    @header_separator.setter
+    def header_separator(self, s):
+        if(s is not None):
+            if(not isinstance(s, str)):
+                raise TypeError('The header_separator property must be None or '
+                    'of type str!')
+        self._header_separator = s
+
+    def _extract_column_names(self, line):
+        """Tries to extract the column names of the data table based on the
+        given line.
+
+        Parameters
+        ----------
+        line : str
+            The text line containing the column names.
+
+        Returns
+        -------
+        names : list of str | None
+            The column names.
+            It returns None, if the column names cannot be extracted.
+        """
+        # Remove possible new-line character and leading white-spaces.
+        line = line.strip()
+        # Check if the line is a comment line.
+        if(line[0:len(self._header_comment)] != self._header_comment):
+            return None
+        # Remove the leading comment character(s).
+        line = line.strip(self._header_comment)
+        # Remove possible leading whitespace characters.
+        line = line.strip()
+        # Split the line into the column names.
+        names = line.split(self._header_separator)
+        # Remove possible whitespaces of column names.
+        names = [ n.strip() for n in names ]
+
+        if(len(names) == 0):
+            return None
+
+        return names
+
+    def _load_file(self, pathfilename, keep_fields, dtype_convertions,
+            dtype_convertion_except_fields):
+        """Loads the given file.
+
+        Parameters
+        ----------
+        pathfilename : str
+            The fully qualified file name of the data file that
+            need to be loaded.
+        keep_fields : str | sequence of str | None
+            Load the data into memory only for these data fields. If set to
+            ``None``, all in-file-present data fields are loaded into memory.
+        dtype_convertions : dict | None
+            If not None, this dictionary defines how data fields of specific
+            data types get converted into the specified data types.
+            This can be used to use less memory.
+        dtype_convertion_except_fields : str | sequence of str | None
+            The sequence of field names whose data type should not get
+            converted.
+
+        Returns
+        -------
+        data : DataFieldRecordArray instance
+            The DataFieldRecordArray instance holding the loaded data.
+        """
+        assert_file_exists(pathfilename)
+
+        with open(pathfilename, 'r') as ifile:
+            line = ifile.readline()
+            column_names = self._extract_column_names(line)
+            if(column_names is None):
+                raise ValueError('The data text file "{}" does not contain a '
+                    'readable table header as first line!'.format(pathfilename))
+            usecols = None
+            dtype = [(n,np.float64) for n in column_names]
+            if(keep_fields is not None):
+                # Select only the given columns.
+                usecols = []
+                dtype = []
+                for (idx,name) in enumerate(column_names):
+                    if(name in keep_fields):
+                        usecols.append(idx)
+                        dtype.append((name,np.float64))
+                usecols = tuple(usecols)
+            if(len(dtype) == 0):
+                raise ValueError('No data columns were selected to be loaded!')
+
+            data_ndarray = np.loadtxt(ifile,
+                dtype=dtype,
+                comments=self._header_comment,
+                usecols=usecols)
+
+        data = DataFieldRecordArray(
+            data_ndarray,
+            keep_fields=keep_fields,
+            dtype_convertions=dtype_convertions,
+            dtype_convertion_except_fields=dtype_convertion_except_fields,
+            copy=False)
+
+        return data
+
+    def load_data(self, keep_fields=None, dtype_convertions=None,
+            dtype_convertion_except_fields=None, **kwargs):
+        """Loads the data from the data files specified through their fully
+        qualified file names.
+
+        Parameters
+        ----------
+        keep_fields : str | sequence of str | None
+            Load the data into memory only for these data fields. If set to
+            ``None``, all in-file-present data fields are loaded into memory.
+        dtype_convertions : dict | None
+            If not None, this dictionary defines how data fields of specific
+            data types get converted into the specified data types.
+            This can be used to use less memory.
+        dtype_convertion_except_fields : str | sequence of str | None
+            The sequence of field names whose data type should not get
+            converted.
+
+        Returns
+        -------
+        data : DataFieldRecordArray
+            The DataFieldRecordArray holding the loaded data.
+
+        Raises
+        ------
+        RuntimeError
+            If a file does not exist.
+        ValueError
+            If the table header cannot be read.
+        """
+        if(keep_fields is not None):
+            if(isinstance(keep_fields, str)):
+                keep_fields = [ keep_fields ]
+            elif(not issequenceof(keep_fields, str)):
+                raise TypeError('The keep_fields argument must be None, an '
+                    'instance of type str, or a sequence of instances of '
+                    'type str!')
+
+        if(dtype_convertions is None):
+            dtype_convertions = dict()
+        elif(not isinstance(dtype_convertions, dict)):
+            raise TypeError('The dtype_convertions argument must be None, '
+                'or an instance of dict!')
+
+        if(dtype_convertion_except_fields is None):
+            dtype_convertion_except_fields = []
+        elif(isinstance(dtype_convertion_except_fields, str)):
+            dtype_convertion_except_fields = [ dtype_convertion_except_fields ]
+        elif(not issequenceof(dtype_convertion_except_fields, str)):
+            raise TypeError('The dtype_convertion_except_fields argument '
+                'must be a sequence of str instances.')
+
+        # Load the first data file.
+        data = self._load_file(
+            self._pathfilename_list[0],
+            keep_fields=keep_fields,
+            dtype_convertions=dtype_convertions,
+            dtype_convertion_except_fields=dtype_convertion_except_fields
+        )
+
+        # Load possible subsequent data files by appending to the first data.
+        for i in range(1, len(self._pathfilename_list)):
+            data.append(self._load_file(
+                self._pathfilename_list[i],
+                keep_fields=keep_fields,
+                dtype_convertions=dtype_convertions,
+                dtype_convertion_except_fields=dtype_convertion_except_fields
+            ))
+
+        return data
+
+
 class DataFieldRecordArray(object):
     """The DataFieldRecordArray class provides a data container similar to a numpy
     record ndarray. But the data fields are stored as individual numpy ndarray
     objects. Hence, access of single data fields is much faster compared to
     access on the record ndarray.
     """
     def __init__(self, data, keep_fields=None, dtype_convertions=None,
@@ -973,7 +1193,8 @@
         for fname in self._field_name_list:
             self._data_fields[fname] = self._data_fields[fname][sorted_idxs]
 
         return sorted_idxs
 
 register_FileLoader(['.npy'], NPYFileLoader)
 register_FileLoader(['.pkl'], PKLFileLoader)
+register_FileLoader(['.csv'], TextFileLoader)
```

### Comparing `skyllh-23.0.0/skyllh/core/test_statistic.py` & `skyllh-23.1.0/skyllh/core/test_statistic.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/times.py` & `skyllh-23.1.0/skyllh/core/times.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/timing.py` & `skyllh-23.1.0/skyllh/core/timing.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/trialdata.py` & `skyllh-23.1.0/skyllh/core/trialdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,15 @@
         tl : TimeLord | None
             The optional TimeLord instance that should be used for timing
             measurements.
         """
         # Set the events property, so that the calculation functions of the data
         # fields can access them.
         self.events = events
+        self._src_ev_idxs = None
 
         if(n_events is None):
             n_events = len(self._events)
         self.n_events = n_events
 
         # Calculate pre-event-selection data fields that are required by the
         # event selection method.
@@ -568,17 +569,20 @@
                 'events.')
             self.events = selected_events
             self._src_ev_idxs = src_ev_idxs
 
         # Sort the events by the index field, if a field was provided.
         if(self._index_field_name is not None):
             logger.debug(
-                'Sorting events in index field "{}"'.format(
-                    self._index_field_name))
-            self._events.sort_by_field(self._index_field_name)
+                f'Sorting events in index field "{self._index_field_name}"')
+            sorted_idxs = self._events.sort_by_field(self._index_field_name)
+            # If event indices are stored, we need to re-assign also those event
+            # indices according to the new order.
+            if self._src_ev_idxs is not None:
+                self._src_ev_idxs[1] = sorted_idxs[self._src_ev_idxs[1]]
 
         # Now calculate all the static data fields. This will increment the
         # trial data state ID.
         self.calculate_static_data_fields(src_hypo_group_manager)
 
     def add_source_data_field(self, name, func, dt=None):
         """Adds a new data field to the manager. The data field must depend
```

### Comparing `skyllh-23.0.0/skyllh/core/utils/multidimgridpdf.py` & `skyllh-23.1.0/skyllh/core/utils/multidimgridpdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/utils/ndphotosplinepdf.py` & `skyllh-23.1.0/skyllh/core/utils/ndphotosplinepdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/core/utils/trials.py` & `skyllh-23.1.0/skyllh/core/utils/trials.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/background_generation.py` & `skyllh-23.1.0/skyllh/i3/background_generation.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/backgroundpdf.py` & `skyllh-23.1.0/skyllh/i3/backgroundpdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/coords.py` & `skyllh-23.1.0/skyllh/i3/coords.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/dataset.py` & `skyllh-23.1.0/skyllh/i3/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import os.path
 
 from skyllh.core import display
-from skyllh.core.py import issequenceof
+from skyllh.core.py import (
+    issequenceof,
+    module_classname
+)
 from skyllh.core.dataset import (
     Dataset,
     DatasetData
 )
+from skyllh.core.debugging import get_logger
 from skyllh.core.storage import (
     DataFieldRecordArray,
     create_FileLoader
 )
 from skyllh.core.timing import TaskTimer
 
 # Load the IceCube specific config defaults.
 # This will change the skyllh.core.config.CFG dictionary.
 from skyllh.i3 import config
 
+
 class I3Dataset(Dataset):
     """The I3Dataset class is an IceCube specific Dataset class that adds
     IceCube specific properties to the Dataset class. These additional
     properties are:
 
         * good-run-list (GRL)
 
@@ -58,14 +63,16 @@
         Parameters
         ----------
         grl_pathfilenames : str | sequence of str
 
         """
         super(I3Dataset, self).__init__(*args, **kwargs)
 
+        self._logger = get_logger(module_classname(self))
+
         self.grl_pathfilename_list = grl_pathfilenames
 
         self.grl_field_name_renaming_dict = dict()
 
     @property
     def grl_pathfilename_list(self):
         """The list of file names of the good-run-list data files for this
@@ -142,16 +149,16 @@
 
         s += display.add_leading_text_line_padding(
             display.INDENTATION_WIDTH, s1)
 
         return s
 
     def load_grl(self, efficiency_mode=None, tl=None):
-        """Loads the good-run-list and returns a structured numpy ndarray with
-        the following data fields:
+        """Loads the good-run-list and returns a DataFieldRecordArray instance
+        which should contain the following data fields:
 
             run : int
                 The run number.
             start : float
                 The MJD start time of the run.
             stop : float
                 The MJD stop time of the run.
@@ -244,49 +251,30 @@
         data : instance of DatasetData
             A DatasetData instance holding the experimental and monte-carlo
             data of this data set.
         """
         # Load the good-run-list (GRL) data if it is provided for this dataset,
         # and calculate the livetime based on the GRL.
         data_grl = None
-        lt = self.livetime
         if(len(self._grl_pathfilename_list) > 0):
             data_grl = self.load_grl(
                 efficiency_mode=efficiency_mode,
                 tl=tl)
-            if('livetime' not in data_grl.field_name_list):
-                raise KeyError('The GRL file(s) "%s" has no data field named '
-                    '"livetime"!'%(','.join(self._grl_pathfilename_list)))
-            lt = np.sum(data_grl['livetime'])
-
-        # Override the livetime if there is a user defined livetime.
-        if(livetime is not None):
-            lt = livetime
 
         # Load all the defined data.
         data = I3DatasetData(
             super(I3Dataset, self).load_data(
                 keep_fields=keep_fields,
-                livetime=lt,
+                livetime=livetime,
                 dtc_dict=dtc_dict,
                 dtc_except_fields=dtc_except_fields,
                 efficiency_mode=efficiency_mode,
                 tl=tl),
             data_grl)
 
-        # Select only the experimental data which fits the good-run-list for
-        # this dataset.
-        if(data_grl is not None):
-            task = 'Selected only the experimental data that matches the GRL '\
-                'for dataset "%s".'%(self.name)
-            with TaskTimer(tl, task):
-                runs = np.unique(data_grl['run'])
-                mask = np.isin(data.exp['run'], runs)
-                data.exp = data.exp[mask]
-
         return data
 
     def prepare_data(self, data, tl=None):
         """Prepares the data for IceCube by pre-calculating the following
         experimental data fields:
 
         - sin_dec: float
@@ -305,31 +293,98 @@
             The TimeLord instance that should be used to time the data
             preparation.
         """
         # Execute all the data preparation functions for this dataset.
         super(I3Dataset, self).prepare_data(data, tl=tl)
 
         if(data.exp is not None):
+            # Append sin(dec) data field to the experimental data.
             task = 'Appending IceCube-specific data fields to exp data.'
             with TaskTimer(tl, task):
-                data.exp.append_field('sin_dec', np.sin(data.exp['dec']))
+                if 'sin_dec' not in data.exp.field_name_list:
+                    data.exp.append_field(
+                        'sin_dec', np.sin(data.exp['dec']))
+
+        if(data.mc is not None):
+            # Append sin(dec) and sin(true_dec) to the MC data.
+            task = 'Appending IceCube-specific data fields to MC data.'
+            with TaskTimer(tl, task):
+                if 'sin_dec' not in data.mc.field_name_list:
+                    data.mc.append_field(
+                        'sin_dec', np.sin(data.mc['dec']))
+                if 'sin_true_dec' not in data.mc.field_name_list:
+                    data.mc.append_field(
+                        'sin_true_dec', np.sin(data.mc['true_dec']))
+
+        # Set the livetime of the dataset from the GRL data when no livetime
+        # was specified previously.
+        if(data.livetime is None and data.grl is not None):
+            if('start' not in data.grl):
+                raise KeyError('The GRL data for dataset "{}" has no data '
+                    'field named "start"!'.format(self.name))
+            if('stop' not in data.grl):
+                raise KeyError('The GRL data for dataset "{}" has no data '
+                    'field named "stop"!'.format(self.name))
+            data.livetime = np.sum(data.grl['stop'] - data.grl['start'])
 
-        # Append sin(dec) and sin(true_dec) to the MC data.
-        task = 'Appending IceCube-specific data fields to MC data.'
-        with TaskTimer(tl, task):
-            data.mc.append_field('sin_dec', np.sin(data.mc['dec']))
-            data.mc.append_field('sin_true_dec', np.sin(data.mc['true_dec']))
+        # Select only the experimental data which fits the good-run-list for
+        # this dataset.
+        if data.grl is not None:
+            # Select based on run information.
+            if (('run' in data.grl) and
+                ('run' in data.exp)):
+                task = 'Selected only the experimental data that matches the '\
+                    'run information in the GRL for dataset "%s".'%(self.name)
+                with TaskTimer(tl, task):
+                    runs = np.unique(data.grl['run'])
+                    mask = np.isin(data.exp['run'], runs)
+                    data.exp = data.exp[mask]
+
+            # Select based on detector on-time information.
+            if (('start' in data.grl) and
+                ('stop' in data.grl) and
+                ('time' in data.exp)):
+                task = 'Selected only the experimental data that matches the '\
+                    'detector\'s on-time information in the GRL for dataset '\
+                    '"%s".'%(self.name)
+                with TaskTimer(tl, task):
+                    mask = np.zeros((len(data.exp),), dtype=np.bool_)
+                    for (start, stop) in zip(data.grl['start'],
+                                             data.grl['stop']):
+                        mask |= (
+                            (data.exp['time'] >= start) &
+                            (data.exp['time'] < stop)
+                        )
+
+                    if np.any(~mask):
+                        n_cut_evts = np.count_nonzero(~mask)
+                        self._logger.info(
+                            f'Cutting {n_cut_evts} events from dataset '
+                            f'{self.name} due to GRL on-time window '
+                            'information.')
+                        data.exp = data.exp[mask]
 
 
 class I3DatasetData(DatasetData):
     """The class provides the container for the loaded experimental and
     monto-carlo data of a data set. It's the IceCube specific class that also
     holds the good-run-list (GRL) data.
     """
     def __init__(self, data, data_grl):
+        """Constructs a new I3DatasetData instance.
+
+        Parameters
+        ----------
+        data : DatasetData instance
+            The DatasetData instance holding the experimental and monte-carlo
+            data.
+        data_grl : DataFieldRecordArray instance | None
+            The DataFieldRecordArray instance holding the good-run-list data
+            of the dataset. This can be None, if no GRL data is available.
+        """
         super(I3DatasetData, self).__init__(
             data._exp, data._mc, data._livetime)
 
         self.grl = data_grl
 
     @property
     def grl(self):
```

### Comparing `skyllh-23.0.0/skyllh/i3/detsigyield.py` & `skyllh-23.1.0/skyllh/i3/detsigyield.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,20 @@
             The array with the detector signal yield for each source.
         grads : numpy (N_sources,N_fitparams)-shaped 2D ndarray
             The array containing the gradient values for each source and fit
             parameter. Since, this implementation depends on only one fit
             parameter, i.e. gamma, the array is (N_sources,1)-shaped.
         """
         src_dec = np.atleast_1d(src['dec'])
-        src_gamma = src_flux_params['gamma']
+        if src_flux_params is None:
+            # Gamma is not a fit parameter. So we take it from the
+            # initial flux model.
+            src_gamma = np.array([self.fluxmodel.gamma], dtype=np.double)
+        else:
+            src_gamma = src_flux_params['gamma']
 
         # Create results array.
         values = np.zeros_like(src_dec, dtype=np.float64)
         grads = np.zeros_like(src_dec, dtype=np.float64)
 
         # Calculate the detector signal yield only for the sources for
         # which we actually have detector acceptance. For the other sources,
```

### Comparing `skyllh-23.0.0/skyllh/i3/livetime.py` & `skyllh-23.1.0/skyllh/i3/livetime.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/pdf.py` & `skyllh-23.1.0/skyllh/i3/pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,13 +225,16 @@
             The array with the energy probability for each event.
         """
         get_data = tdm.get_data
 
         logE_binning = self.get_binning('log_energy')
         sinDec_binning = self.get_binning('sin_dec')
 
-        logE_idx = np.digitize(get_data('log_energy'), logE_binning.binedges) - 1
-        sinDec_idx = np.digitize(get_data('sin_dec'), sinDec_binning.binedges) - 1
+        logE_idx = np.digitize(
+            get_data('log_energy'), logE_binning.binedges) - 1
+        sinDec_idx = np.digitize(
+            get_data('sin_dec'), sinDec_binning.binedges) - 1
 
         with TaskTimer(tl, 'Evaluating logE-sinDec histogram.'):
             prob = self._hist_logE_sinDec[(logE_idx,sinDec_idx)]
+
         return prob
```

### Comparing `skyllh-23.0.0/skyllh/i3/pdfratio.py` & `skyllh-23.1.0/skyllh/i3/pdfratio.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/signal_generation.py` & `skyllh-23.1.0/skyllh/i3/signal_generation.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/signalpdf.py` & `skyllh-23.1.0/skyllh/i3/signalpdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/i3/utils/sensitivity.py` & `skyllh-23.1.0/skyllh/i3/utils/sensitivity.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/physics/flux.py` & `skyllh-23.1.0/skyllh/physics/flux.py`

 * *Files 10% similar despite different names*

```diff
@@ -519,14 +519,77 @@
         flux : float | 1d ndarray of float
             Flux at energy E in unit [energy]^-1 [length]^-2 [time]^-1.
             By default in GeV^-1 cm^-2 s^-1.
         """
         flux = self.Phi0 * np.power(E / self.E0, -self.gamma)
         return flux
 
+    def get_integral(self, E_min, E_max):
+        """Returns the integral value of the flux between the given energy
+        range.
+
+        Parameters
+        ----------
+        E_min : float | 1d numpy ndarray of float
+            The lower energy bound of the integration.
+        E_max : float | 1d numpy ndarray of float
+            The upper energy bound of the integration.
+
+        Returns
+        -------
+        integral : float | 1d ndarray of float
+            The integral value(s) of the given integral range(s).
+        """
+        gamma = self.gamma
+
+        # Handle special case for gamma = 1.
+        if(gamma == 1):
+            integral = self.Phi0 * self.E0 * (
+                np.log(np.abs(E_max)) - np.log(np.abs(E_min)))
+            return integral
+
+        integral = (self.Phi0 / ((1.-gamma)*np.power(self.E0, -gamma)) *
+            (np.power(E_max, 1.-gamma) - np.power(E_min, 1.-gamma)))
+
+        return integral
+
+    def get_inv_normed_cdf(self, x, E_min, E_max):
+        """Calculates the inverse cumulative distribution function value for
+        each given value of x, which is a number between 0 and 1.
+
+        Parameters
+        ----------
+        x : float | 1d numpy ndarray of float
+            The argument value(s) of the inverse cumulative distribution
+            function. Must be between 0 and 1.
+        E_min : float
+            The lower energy edge of the flux to be considered.
+        E_max : float
+            The upper energy edge of the flux to be considered.
+
+        Returns
+        -------
+        inv_normed_cdf : float | 1d numpy ndarray
+            The energy value(s) from the inverse normed cumulative distribution
+            function.
+        """
+        gamma = self.gamma
+
+        if(gamma == 1):
+            N_0 = np.log(E_max / E_min)
+            inv_normed_cdf = E_min * np.exp(x * N_0)
+            return inv_normed_cdf
+
+        N_0 = E_max ** (1. - gamma) - E_min ** (1. - gamma)
+        inv_normed_cdf = np.power(
+            x * N_0 + E_min**(1. - gamma),
+            (1. / (1. - gamma)))
+
+        return inv_normed_cdf
+
 
 class CutoffPowerLawFlux(PowerLawFlux):
     """Cut-off power law flux of the form
 
         dN/(dEdAdt) = Phi0 * (E / E0)^(-gamma) * exp(-E/Ecut)
 
     The unit of dN/(dEdAdt) is [energy]^-1 [length]^-2 [time]^-1.
```

### Comparing `skyllh-23.0.0/skyllh/physics/flux_model.py` & `skyllh-23.1.0/skyllh/physics/flux_model.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/physics/model.py` & `skyllh-23.1.0/skyllh/physics/model.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/physics/source.py` & `skyllh-23.1.0/skyllh/physics/source.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/physics/time_profile.py` & `skyllh-23.1.0/skyllh/physics/time_profile.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/core/pdfratio.py` & `skyllh-23.1.0/skyllh/plotting/core/pdfratio.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/core/signalpdf.py` & `skyllh-23.1.0/skyllh/plotting/core/signalpdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/i3/backgroundpdf.py` & `skyllh-23.1.0/skyllh/plotting/i3/backgroundpdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/i3/pdf.py` & `skyllh-23.1.0/skyllh/plotting/i3/pdf.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/i3/pdfratio.py` & `skyllh-23.1.0/skyllh/plotting/i3/pdfratio.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/plotting/utils/trials.py` & `skyllh-23.1.0/skyllh/plotting/utils/trials.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh/utils/spline.py` & `skyllh-23.1.0/skyllh/utils/spline.py`

 * *Files identical despite different names*

### Comparing `skyllh-23.0.0/skyllh.egg-info/PKG-INFO` & `skyllh-23.1.0/skyllh.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyllh
-Version: 23.0.0
+Version: 23.1.0
 Summary: The SkyLLH framework is an open-source Python3-based package licensed under the GPLv3 license. It provides a modular framework for implementing custom likelihood functions and executing log-likelihood ratio hypothesis tests. The idea is to provide a class structure tied to the mathematical objects of the likelihood functions.
 Home-page: https://github.com/icecube/skyllh
 Author: Martin Wolf
 Author-email: martin.wolf@icecube.wisc.edu
 License: GPL-3+
 Project-URL: Bug Tracker, https://github.com/icecube/skyllh/issues
 Project-URL: Documentation, https://icecube.github.io/skyllh
@@ -29,26 +29,31 @@
 
 The SkyLLH framework is an open-source Python3-based package licensed under the GPLv3 license. It provides a modular framework for implementing custom likelihood functions and executing log-likelihood ratio hypothesis tests. The idea is to provide a class structure tied to the mathematical objects of the likelihood functions, rather than to entire abstract likelihood models.
 
 # Installation
 
 ## Using pip
 
-The `skyllh` package can be installed using pip:
+The latest `skyllh` release can be installed from [PyPI](https://pypi.org/project/skyllh/) repository:
+```bash
+pip install skyllh
+```
+
+The current development version can be installed using pip:
 ```bash
 pip install git+https://github.com/icecube/skyllh.git#egg=skyllh 
 ```
 
 Optionally, the editable package version with a specified reference can be installed by:
 ```bash
-pip install -e git+https://github.com/icecube/skyllh.git@ref#egg=skyllh 
+pip install -e git+https://github.com/icecube/skyllh.git@[ref]#egg=skyllh 
 ```
 where
 - `-e` is an editable flag
-- `ref` in `@ref` is an optional argument containing a specific commit hash, branch name or tag
+- `[ref]` is an optional argument containing a specific commit hash, branch name or tag
 
 ## Cloning from GitHub
 
 The `skyllh` (and an optional private [i3skyllh](#i3skyllh)) package can be installed by cloning the GitHub repository and adding it to the Python path:
 
 ```python
 import sys
```

### Comparing `skyllh-23.0.0/skyllh.egg-info/SOURCES.txt` & `skyllh-23.1.0/skyllh.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 skyllh/__init__.py
 skyllh/_version.py
 skyllh.egg-info/PKG-INFO
 skyllh.egg-info/SOURCES.txt
 skyllh.egg-info/dependency_links.txt
 skyllh.egg-info/requires.txt
 skyllh.egg-info/top_level.txt
+skyllh/analyses/__init__.py
+skyllh/analyses/i3/__init__.py
+skyllh/analyses/i3/publicdata_ps/__init__.py
+skyllh/analyses/i3/publicdata_ps/aeff.py
+skyllh/analyses/i3/publicdata_ps/backgroundpdf.py
+skyllh/analyses/i3/publicdata_ps/bkg_flux.py
+skyllh/analyses/i3/publicdata_ps/detsigyield.py
+skyllh/analyses/i3/publicdata_ps/mcbkg_ps.py
+skyllh/analyses/i3/publicdata_ps/pdfratio.py
+skyllh/analyses/i3/publicdata_ps/signal_generator.py
+skyllh/analyses/i3/publicdata_ps/signalpdf.py
+skyllh/analyses/i3/publicdata_ps/smearing_matrix.py
+skyllh/analyses/i3/publicdata_ps/time_dependent_ps.py
+skyllh/analyses/i3/publicdata_ps/time_integrated_ps.py
+skyllh/analyses/i3/publicdata_ps/utils.py
 skyllh/cluster/__init__.py
 skyllh/cluster/commands.py
 skyllh/cluster/compute_node.py
 skyllh/cluster/master_node.py
 skyllh/cluster/srvclt.py
 skyllh/core/__init__.py
 skyllh/core/analysis.py
@@ -25,14 +40,15 @@
 skyllh/core/binning.py
 skyllh/core/config.py
 skyllh/core/coords.py
 skyllh/core/dataset.py
 skyllh/core/debugging.py
 skyllh/core/detsigyield.py
 skyllh/core/display.py
+skyllh/core/expectation_maximization.py
 skyllh/core/interpolate.py
 skyllh/core/livetime.py
 skyllh/core/llhratio.py
 skyllh/core/math.py
 skyllh/core/minimizer.py
 skyllh/core/model.py
 skyllh/core/multiproc.py
@@ -58,14 +74,19 @@
 skyllh/core/trialdata.py
 skyllh/core/minimizers/__init__.py
 skyllh/core/minimizers/iminuit.py
 skyllh/core/utils/__init__.py
 skyllh/core/utils/multidimgridpdf.py
 skyllh/core/utils/ndphotosplinepdf.py
 skyllh/core/utils/trials.py
+skyllh/datasets/__init__.py
+skyllh/datasets/i3/PublicData_10y_ps.py
+skyllh/datasets/i3/PublicData_10y_ps_wMC.py
+skyllh/datasets/i3/PublicData_10y_ps_wMCEq.py
+skyllh/datasets/i3/__init__.py
 skyllh/i3/__init__.py
 skyllh/i3/background_generation.py
 skyllh/i3/backgroundpdf.py
 skyllh/i3/config.py
 skyllh/i3/coords.py
 skyllh/i3/dataset.py
 skyllh/i3/detsigyield.py
@@ -90,33 +111,8 @@
 skyllh/plotting/i3/__init__.py
 skyllh/plotting/i3/backgroundpdf.py
 skyllh/plotting/i3/pdf.py
 skyllh/plotting/i3/pdfratio.py
 skyllh/plotting/utils/__init__.py
 skyllh/plotting/utils/trials.py
 skyllh/utils/__init__.py
-skyllh/utils/spline.py
-tests/__init__.py
-tests/utils.py
-tests/core/__init__.py
-tests/core/test_analysis.py
-tests/core/test_dataset.py
-tests/core/test_model.py
-tests/core/test_optimize.py
-tests/core/test_parameters.py
-tests/core/test_py.py
-tests/core/test_signal_generator.py
-tests/core/test_storage.py
-tests/core/testdata/__init__.py
-tests/core/testdata/testdata_generator.py
-tests/i3/__init__.py
-tests/i3/test_background_generation.py
-tests/i3/test_coords.py
-tests/i3/test_livetime.py
-tests/i3/test_scrambling.py
-tests/i3/testdata/__init__.py
-tests/i3/testdata/testdata_generator.py
-tests/physics/__init__.py
-tests/physics/test_flux.py
-tests/physics/test_flux_model.py
-tests/physics/test_source.py
-tests/physics/test_time_profile.py
+skyllh/utils/spline.py
```

### Comparing `skyllh-23.0.0/versioneer.py` & `skyllh-23.1.0/versioneer.py`

 * *Files identical despite different names*

