# Comparing `tmp/kafe2-2.7.0rc1.tar.gz` & `tmp/kafe2-2.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafe2-2.7.0rc1.tar", last modified: Fri Sep 23 16:16:50 2022, max compression
+gzip compressed data, was "kafe2-2.8.0rc1.tar", last modified: Wed Apr 19 15:27:43 2023, max compression
```

## Comparing `kafe2-2.7.0rc1.tar` & `kafe2-2.8.0rc1.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.039296 kafe2-2.7.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-09-23 16:16:50.039296 kafe2-2.7.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/_version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/config/
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19041 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/config/kafe2.matplotlibrc.conf
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/config/kafe2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/config/plot_style_color.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/core/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/confidence.py
--rw-r--r--   0 runner    (1001) docker     (121)    12135 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/constraint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/contour.py
--rw-r--r--   0 runner    (1001) docker     (121)    24145 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/core/fitters/
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/fitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    50344 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/fitters/nexus.py
--rw-r--r--   0 runner    (1001) docker     (121)     8547 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/fitters/nexus_fitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3884 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/fitters/simple_fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/core/minimizers/
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/minimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15158 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/minimizers/iminuit_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    21416 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/minimizers/minimizer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16436 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    27007 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2/fit/
--rw-r--r--   0 runner    (1001) docker     (121)     7745 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5730 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/_base/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14482 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/container.py
--rw-r--r--   0 runner    (1001) docker     (121)    33791 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)    56832 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)    31622 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/format.py
--rw-r--r--   0 runner    (1001) docker     (121)    14245 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    66959 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/_base/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/custom/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/custom/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/histogram/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11000 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)     5744 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/histogram/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/indexed/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4746 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     4587 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/indexed/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/io/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/io/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     9018 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/io/handle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/multi/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/multi/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)    41242 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/multi/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/_yaml_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/constraint/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/constraint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/constraint/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/container/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/container/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/container/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/error/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11402 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/error/common_error_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/fit/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/fit/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/fit/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.031296 kafe2-2.7.0rc1/kafe2/fit/representation/format/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/format/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7523 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/format/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/fit/representation/model/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    19395 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/representation/model/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/fit/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40114 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/contours_profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)    31872 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/fit_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       88 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/kafe2go
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/tools/kafe2go.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/fit/unbinned/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/unbinned/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/fit/util/
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/util/function_library.py
--rw-r--r--   0 runner    (1001) docker     (121)     9449 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/util/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/fit/xy/
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13243 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     7513 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)    29429 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)    29088 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9451 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/fit/xy/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/test/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.035296 kafe2-2.7.0rc1/kafe2/test/core/minimizers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/minimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21360 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/minimizers/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_iminuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_confidence.py
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_cov_mat.py
--rw-r--r--   0 runner    (1001) docker     (121)    22558 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_gaussian_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    29537 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_nexus.py
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_nexus_fitter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12606 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/core/test_parameter_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.039296 kafe2-2.7.0rc1/kafe2/test/fit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15833 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_containers_histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     7568 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_containers_indexed.py
--rw-r--r--   0 runner    (1001) docker     (121)    12267 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_containers_xy.py
--rw-r--r--   0 runner    (1001) docker     (121)    15572 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_cost_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8322 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_ensemble_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5522 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_custom.py
--rw-r--r--   0 runner    (1001) docker     (121)    15941 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_hist.py
--rw-r--r--   0 runner    (1001) docker     (121)    23697 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_indexed.py
--rw-r--r--   0 runner    (1001) docker     (121)    31993 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     9381 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_unbinned.py
--rw-r--r--   0 runner    (1001) docker     (121)    39098 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fit_xy.py
--rw-r--r--   0 runner    (1001) docker     (121)    15958 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     5294 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_model_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10363 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    23602 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_container_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    43986 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_fit_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    12812 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_format_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    18868 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    24649 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/test/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7362 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/kafe2/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:16:50.027296 kafe2-2.7.0rc1/kafe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-09-23 16:16:49.000000 kafe2-2.7.0rc1/kafe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-09-23 16:16:49.000000 kafe2-2.7.0rc1/kafe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 16:16:49.000000 kafe2-2.7.0rc1/kafe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-23 16:16:49.000000 kafe2-2.7.0rc1/kafe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-23 16:16:49.000000 kafe2-2.7.0rc1/kafe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 16:16:50.039296 kafe2-2.7.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-09-23 16:16:39.000000 kafe2-2.7.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.950596 kafe2-2.8.0rc1/kafe2/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/_version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/kafe2.matplotlibrc.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/kafe2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/plot_style_color.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24145 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/fitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50344 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/nexus_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/simple_fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/minimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/iminuit_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30571 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/minimizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56936 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31671 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68406 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/custom/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/indexed/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/multi/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41242 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/_yaml_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/container/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/error/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/error/common_error_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45151 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/contours_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31872 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/fit_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/unbinned/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/function_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/xy/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/core/minimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28560 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_cov_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_gaussian_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29537 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_nexus_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_parameter_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/kafe2/test/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_cost_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_ensemble_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31993 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_unbinned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40080 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_model_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_container_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43978 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_fit_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_format_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.950596 kafe2-2.8.0rc1/kafe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/setup.py
```

### Comparing `kafe2-2.7.0rc1/LICENSE` & `kafe2-2.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/PKG-INFO` & `kafe2-2.8.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kafe2
-Version: 2.7.0rc1
+Version: 2.8.0rc1
 Summary: Karlsruhe Fit Environment 2: a package for fitting and elementary data analysis
-Home-page: http://github.com/dsavoiu/kafe2
+Home-page: https://github.com/PhiLFitters/kafe2
 Author: Daniel Savoiu
 Author-email: daniel.savoiu@cern.ch
 License: GPL3
 Keywords: kafe2 kit karlsruhe data analysis lab laboratory practical courses education university students physics fitting minimization minimisation regression parametric parameter estimation optimization optimisation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -31,43 +31,39 @@
 .. image:: https://badge.fury.io/py/kafe2.svg
     :target: https://badge.fury.io/py/kafe2
 
 .. image:: https://readthedocs.org/projects/kafe2/badge/?version=latest
     :target: https://kafe2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://travis-ci.org/dsavoiu/kafe2.svg?branch=master
-    :target: https://travis-ci.org/dsavoiu/kafe2
 
-
-*kafe2* is an open-source Python package designed to provide a flexible
-Python interface for the estimation of model parameters from measured
-data. It is the spiritual successor to the original *kafe* package.
-
-*kafe2* offers support for several types of data formats (including series
-of indexed measurements, xy value pairs, and histograms) and data
-uncertainty models, as well as arbitrarily complex parametric
-models. The numeric aspects are handled using the scientific Python
-stack (NumPy, SciPy, ...). Visualization of the data and the estimated
-model are provided by matplotlib.
+*kafe2* is an open-source Python package for the likelihood-based estimation of model parameters
+from measured data.
+As the spiritual successor to the original *kafe* package it aims to provide
+state-of-the-art statistical methods in a way that is still easy to use.
+More information `here <https://philfitters.github.io/kafe2/>`__.
 
 If you have installed pip just run
 
 .. code-block:: bash
 
     pip install kafe2
 
-to install the latest stable version and you're ready to go.
+to install the latest stable version and you're (mostly) ready to go.
+The Python package *iminuit* which *kafe2* uses internally for numerical optimization
+`may fail to be installed automatically if no C++ compiler is available on your system
+<https://iminuit.readthedocs.io/en/stable/install.html>`__ .
+While *iminuit* is strictly speaking not required its use is heavily recommended.
+**Make sure to read the pip installation log.**
 As of *kafe2* v2.4.0 only Python 3 is supported.
 
-The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`_
+The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`__
 has more detailed installation instructions.
-It also explains basic *kafe2* features as well as the mathematical foundations
-upon which *kafe2* is built.
+It also explains *kafe2* usage as well as the mathematical foundations upon which *kafe2* is built.
 
 If you prefer a more practical approach you can instead look at the various
-`examples <https://github.com/dsavoiu/kafe2/tree/master/examples>`_.
+`examples <https://github.com/PhiLFitters/kafe2/tree/master/examples>`__.
 In addition to the regular Python/kafe2go files there are also Jupyter notebook
 tutorials (in English and in German) that mostly cover the same topics.
 
 If you encounter any bugs or have an improvement proposal, please let us
-know by opening an issue `here <https://github.com/dsavoiu/kafe2/issues>`_.
+know by opening an issue `here <https://github.com/PhiLFitters/kafe2/issues>`__.
```

### Comparing `kafe2-2.7.0rc1/README.rst` & `kafe2-2.8.0rc1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,43 +6,39 @@
 .. image:: https://badge.fury.io/py/kafe2.svg
     :target: https://badge.fury.io/py/kafe2
 
 .. image:: https://readthedocs.org/projects/kafe2/badge/?version=latest
     :target: https://kafe2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://travis-ci.org/dsavoiu/kafe2.svg?branch=master
-    :target: https://travis-ci.org/dsavoiu/kafe2
 
-
-*kafe2* is an open-source Python package designed to provide a flexible
-Python interface for the estimation of model parameters from measured
-data. It is the spiritual successor to the original *kafe* package.
-
-*kafe2* offers support for several types of data formats (including series
-of indexed measurements, xy value pairs, and histograms) and data
-uncertainty models, as well as arbitrarily complex parametric
-models. The numeric aspects are handled using the scientific Python
-stack (NumPy, SciPy, ...). Visualization of the data and the estimated
-model are provided by matplotlib.
+*kafe2* is an open-source Python package for the likelihood-based estimation of model parameters
+from measured data.
+As the spiritual successor to the original *kafe* package it aims to provide
+state-of-the-art statistical methods in a way that is still easy to use.
+More information `here <https://philfitters.github.io/kafe2/>`__.
 
 If you have installed pip just run
 
 .. code-block:: bash
 
     pip install kafe2
 
-to install the latest stable version and you're ready to go.
+to install the latest stable version and you're (mostly) ready to go.
+The Python package *iminuit* which *kafe2* uses internally for numerical optimization
+`may fail to be installed automatically if no C++ compiler is available on your system
+<https://iminuit.readthedocs.io/en/stable/install.html>`__ .
+While *iminuit* is strictly speaking not required its use is heavily recommended.
+**Make sure to read the pip installation log.**
 As of *kafe2* v2.4.0 only Python 3 is supported.
 
-The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`_
+The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`__
 has more detailed installation instructions.
-It also explains basic *kafe2* features as well as the mathematical foundations
-upon which *kafe2* is built.
+It also explains *kafe2* usage as well as the mathematical foundations upon which *kafe2* is built.
 
 If you prefer a more practical approach you can instead look at the various
-`examples <https://github.com/dsavoiu/kafe2/tree/master/examples>`_.
+`examples <https://github.com/PhiLFitters/kafe2/tree/master/examples>`__.
 In addition to the regular Python/kafe2go files there are also Jupyter notebook
 tutorials (in English and in German) that mostly cover the same topics.
 
 If you encounter any bugs or have an improvement proposal, please let us
-know by opening an issue `here <https://github.com/dsavoiu/kafe2/issues>`_.
+know by opening an issue `here <https://github.com/PhiLFitters/kafe2/issues>`__.
```

### Comparing `kafe2-2.7.0rc1/kafe2/config/__init__.py` & `kafe2-2.8.0rc1/kafe2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/config/kafe2.matplotlibrc.conf` & `kafe2-2.8.0rc1/kafe2/config/kafe2.matplotlibrc.conf`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/config/kafe2.yaml` & `kafe2-2.8.0rc1/kafe2/config/kafe2.yaml`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/config/plot_style_color.yaml` & `kafe2-2.8.0rc1/kafe2/config/plot_style_color.yaml`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/confidence.py` & `kafe2-2.8.0rc1/kafe2/core/confidence.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,61 +6,80 @@
 __all__ = ['ConfidenceLevel']
 
 
 class ConfidenceLevel(object):
     """
     Helper class for handling the conversion from confidence levels to sigma values and vice versa.
     """
-    def __init__(self, n_dimensions, cl=None, sigma=None):
+    def __init__(self, n_dimensions=1, cl=None, sigma=None, delta_nll=None):
         self.ndim = n_dimensions
-        if (cl is None and sigma is None) or (cl is not None and sigma is not None):
-            raise ValueError("Exactly one out of cl and sigma must be defined!")
+        _num_spec_not_none = 0
+        if cl is not None:
+            _num_spec_not_none += 1
+        if sigma is not None:
+            _num_spec_not_none += 1
+        if delta_nll is not None:
+            _num_spec_not_none += 1
+        if _num_spec_not_none != 1:
+            raise ValueError("Exactly one out of cl, sigma, and delta_nll must be defined!")
         if cl is not None:
             self.cl = cl
         if sigma is not None:
             self.sigma = sigma
+        if delta_nll is not None:
+            self.sigma = np.sqrt(delta_nll)
 
     def __str__(self):
         return "<ConfidenceLevel (d=%d): %.4g%% (%.3g-sigma)>" % (
             self.ndim, self.cl*100., self.sigma)
 
     def _calc_sigma_from_cl(self):
         self._sigma = np.sqrt(2 * gammainccinv(self.ndim/2.0, 1.0 - self.cl))
 
     def _calc_cl_from_sigma(self):
         self._cl = 1. - gammaincc(self.ndim/2.0, self.sigma**2/2.0)
 
     @property
-    def cl(self):
+    def cl(self) -> float:
         if self._cl is None:
             self._calc_cl_from_sigma()
         return self._cl
 
     @cl.setter
-    def cl(self, new_cl):
+    def cl(self, new_cl: float):
         if new_cl <= 0 or new_cl >= 1:
             raise ValueError(
                 "Confidence level must be greater than 0 and less than 1. Got: %g" % (new_cl,))
         self._cl = float(new_cl)
         self._sigma = None
 
     @property
-    def sigma(self):
+    def sigma(self) -> float:
         if self._sigma is None:
             self._calc_sigma_from_cl()
         return self._sigma
 
     @sigma.setter
-    def sigma(self, new_sigma):
+    def sigma(self, new_sigma: float):
         if new_sigma <= 0:
             raise ValueError("Sigma value must be greater than 0! Got: %g" % (new_sigma,))
         self._sigma = float(new_sigma)
         self._cl = None
 
     @property
+    def delta_nll(self) -> float:
+        return self.sigma ** 2
+
+    @delta_nll.setter
+    def delta_nll(self, new_delta_nll: float):
+        if new_delta_nll <= 0:
+            raise ValueError("delta_nll value must be greater than 0! Got: %g" % (new_delta_nll,))
+        self.sigma = np.sqrt(new_delta_nll)
+
+    @property
     def ndim(self):
         return self._ndim
 
     @ndim.setter
     def ndim(self, new_ndim):
         if not isinstance(new_ndim, int):
             raise ValueError(
```

### Comparing `kafe2-2.7.0rc1/kafe2/core/constraint.py` & `kafe2-2.8.0rc1/kafe2/core/constraint.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/contour.py` & `kafe2-2.8.0rc1/kafe2/core/contour.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/error.py` & `kafe2-2.8.0rc1/kafe2/core/error.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/fitters/__init__.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/fitters/nexus.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/nexus.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/fitters/nexus_fitter.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/nexus_fitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,21 +195,22 @@
         if not self.__state_is_from_minimizer:
             raise RuntimeError(
                 "To calculate a contour the do_fit method has to be called first."
             )
 
         return self._minimizer.contour(parameter_name_1, parameter_name_2, sigma=sigma, **kwargs)
 
-    def profile(self, parameter_name, bins=20, bound=2, args=None, subtract_min=False):
+    def profile(self, parameter_name, low=None, high=None, sigma=None, cl=None, size=20,
+                subtract_min=False, arrows=False):
         if not self.__state_is_from_minimizer:
             raise RuntimeError(
                 "To calculate a profile the do_fit method has to be called first."
             )
-
-        return self._minimizer.profile(parameter_name, bins=bins, bound=bound, subtract_min=subtract_min)
+        return self._minimizer.profile(
+            parameter_name, low, high, sigma, cl, size, subtract_min, arrows)
 
     def get_fit_parameter_values(self, parameter_names=None):
         if parameter_names is None:
             parameter_names = self._fit_par_names
         return OrderedDict([
             (_pn, self._nx.get(_pn).value)
             for _pn in parameter_names
```

### Comparing `kafe2-2.7.0rc1/kafe2/core/fitters/simple_fitter.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/simple_fitter.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/minimizers/__init__.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/minimizers/iminuit_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/iminuit_minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import numpy as np
+from scipy.stats import norm
 from copy import deepcopy
 
 from .minimizer_base import MinimizerBase
 from ..contour import ContourFactory
 
 try:
     import iminuit
@@ -293,26 +294,33 @@
             _contour_line = self._get_iminuit().mncontour(
                 parameter_name_1, parameter_name_2, size=_numpoints, cl=_cl)
         self.minimize()  # return to minimum
         if len(_contour_line) == 0:
             return None  # failed to find any point on contour
         return ContourFactory.create_xy_contour(np.array(_contour_line), sigma)
 
-    def profile(self, parameter_name, bins=20, bound=2, subtract_min=False):
+    def profile(self, parameter_name, low=None, high=None, sigma=None, cl=None, size=20,
+                subtract_min=False, arrows=False):
         if not self.did_fit:
             raise RuntimeError("Need to perform a fit before calling profile()!")
-        _kwargs = dict(bound=bound, subtract_min=subtract_min)
+        _bound_low, _bound_high, _arrow_specs = self._get_profile_bound(
+            parameter_name, low, high, sigma, cl, subtract_min, arrows)
+        self.minimize()  # return to minimum
+        _kwargs = dict(
+            bound=(_bound_low, _bound_high),
+            subtract_min=subtract_min
+        )
         if _IMINUIT_1:
-            _kwargs["bins"] = bins
+            _kwargs["bins"] = size
         else:
-            _kwargs["size"] = bins
+            _kwargs["size"] = size
         _bins, _vals, _statuses = self.__iminuit.mnprofile(parameter_name, **_kwargs)
         # TODO: check statuses (?)
         self.minimize()  # return to minimum
-        return np.array([_bins, _vals])
+        return np.array([_bins, _vals]), _arrow_specs
 
     def set(self, parameter_name, parameter_value):
         if parameter_name not in self._minimizer_param_dict:
             raise ValueError("No parameter named '%s'!" % (parameter_name,))
         self._minimizer_param_dict[parameter_name] = parameter_value
         self.reset()
```

### Comparing `kafe2-2.7.0rc1/kafe2/core/minimizers/minimizer_base.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/minimizer_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from copy import copy
 import six
 from abc import ABCMeta, abstractmethod
 import numpy as np
 import numdifftools as nd
-from scipy.optimize import brentq
+from scipy.optimize import root_scalar
+from typing import Sequence, Union
 
 from ..error import CovMat
+from kafe2.core.confidence import ConfidenceLevel
 
 
 @six.add_metaclass(ABCMeta)
 class MinimizerBase(object):
 
     ERRORDEF_CHI2 = 1.0
     ERRORDEF_NLL = 0.5
@@ -150,24 +152,53 @@
                 _target_chi_2 = self.function_value + 1.0
                 _min_parameters = self.parameter_values
 
                 _par_min = self.parameter_values[_par_index]
                 _par_err = self.parameter_errors[_par_index]
 
                 _cut_dn = self._find_cost_cut(
-                    _par_name, _par_min - 2 * _par_err, _par_min, _target_chi_2, _min_parameters)
+                    _par_name, _par_min - _par_err, _target_chi_2, _min_parameters)
                 _asymm_par_errs[_par_index, 0] = _cut_dn - _par_min
 
                 _cut_up = self._find_cost_cut(
-                    _par_name, _par_min, _par_min + 2 * _par_err, _target_chi_2, _min_parameters)
+                    _par_name, _par_min + _par_err, _target_chi_2, _min_parameters)
                 _asymm_par_errs[_par_index, 1] = _cut_up - _par_min
                 self._load_state()
         return _asymm_par_errs
 
-    def _find_cost_cut(self, parameter_name, low, high, target_cost, min_parameters):
+    def _get_cost_value(self, parameter_name, parameter_value, min_parameters):
+        """
+        Utility function that finds the parameter value for a single parameter at which the cost
+        function reaches a given value. The other parameters are **not** fixed. Instead the profile
+        likelihood method is used.
+        :param parameter_name: the name of the parameter to vary.
+        :param low: lower bound of the parameter.
+        :param high: upper bound of the parameter.
+        :param target_cost: cost function value to find the cut for.
+        :param min_parameters: parameter values at the cost function minimum.
+        :return: the parameter value where the cost function value has the given value.
+        :rtype: float
+        """
+        _all_pars_would_be_fixed = True
+        for _par_name in self._par_names:
+            if _par_name != parameter_name and not self.is_fixed(_par_name):
+                _all_pars_would_be_fixed = False
+                break
+
+        self.set_several(self.parameter_names, min_parameters)
+        self.set(parameter_name, parameter_value)
+        self._fval = None  # Clear fval cache
+        if not _all_pars_would_be_fixed:
+            self.fix(parameter_name)
+            self.minimize()
+            self.release(parameter_name)
+        return self.function_value
+
+
+    def _find_cost_cut(self, parameter_name, guess, target_cost, min_parameters):
         """
         Utility function that finds the parameter value for a single parameter at which the cost
         function reaches a given value. The other parameters are **not** fixed. Instead the profile
         likelihood method is used.
         :param parameter_name: the name of the parameter to vary.
         :param low: lower bound of the parameter.
         :param high: upper bound of the parameter.
@@ -188,15 +219,167 @@
             self._fval = None  # Clear fval cache
             if not _all_pars_would_be_fixed:
                 self.fix(parameter_name)
                 self.minimize()
                 self.release(parameter_name)
             return self.function_value - target_cost
 
-        return brentq(f=_profile, a=low, b=high, xtol=self.tolerance)
+        return root_scalar(
+            f=_profile, x0=guess, x1=min_parameters[self.parameter_names.index(parameter_name)],
+            xtol=self.tolerance, method="secant").root
+
+    def _get_profile_bound(
+            self, parameter_name, low=None, high=None, sigma=None, cl=None, subtract_min=False, arrows=False):
+        if low is not None and high is not None and cl is not None:
+            raise ValueError("At most two out of low, high, and cl can be defined.")
+        _parameter_index = self._par_names.index(parameter_name)
+        _parameter_error = self.parameter_errors[_parameter_index]
+        _min_cost = self.function_value
+        _min_par_vals = self.parameter_values
+        _min_par_val = _min_par_vals[_parameter_index]
+
+        if low is not None and np.max(low) > _min_par_val:
+            raise ValueError(f"low={low} must be smaller than <{parameter_name}>={_min_par_val}")
+        if high is not None and np.min(high) < _min_par_val:
+            raise ValueError(f"high={high} must be larger than <{parameter_name}>={_min_par_val}")
+
+        _arrow_specs = self._get_arrow_specs(
+            parameter_name, low, high, cl, subtract_min, arrows, _min_cost, _min_par_val,
+            _parameter_error, _min_par_vals)
+        low = np.min(low)
+        high = np.max(high)
+        cl = np.max(cl)
+        if sigma is not None:
+            _low_sigma = _min_par_val - sigma * _parameter_error
+            low = _low_sigma if low is None else min(low, _low_sigma)
+            _high_sigma = _min_par_val + sigma * _parameter_error
+            high = _high_sigma if high is None else max(high, _high_sigma)
+        elif cl is None:
+            sigma = 2
+            if low is None:
+                low = _min_par_val - sigma * _parameter_error
+            if high is None:
+                high = _min_par_val + sigma * _parameter_error
+        if _arrow_specs is not None:
+            for _arrow_spec in _arrow_specs:
+                low = _arrow_spec["x"] if low is None else min(low, _arrow_spec["x"])
+                high = _arrow_spec["x"] if high is None else max(high, _arrow_spec["x"])
+            _original_low = low
+            _original_high = high
+            _margin = 0.13 if arrows else 0
+            for _arrow_spec in _arrow_specs:
+                low = min(low, _arrow_spec["x"] + _margin * (_arrow_spec["x"] - _original_high))
+                high = max(high, _arrow_spec["x"] + _margin * (_arrow_spec["x"] - _original_low))
+
+        return low, high, _arrow_specs
+
+    def _get_arrow_specs(
+            self, parameter_name: str, low: Union[None, float, Sequence[float]],
+            high: Union[None, float, Sequence[float]], cl: Union[None, float, Sequence[float]],
+            subtract_min: bool, arrows: bool, min_cost: float, min_par_val: float,
+            par_err: float, min_par_vals: Sequence[float]):
+        if low is None and high is None and cl is None:
+            return None
+        _arrow_specs = []
+
+        _num_defined = 0
+        if low is not None:
+            _num_defined += 1
+        if high is not None:
+            _num_defined += 1
+        if cl is not None:
+            _num_defined += 1
+        if _num_defined > 2:
+            raise ValueError("At most 2 out of low, high, and cl can be defined but received "
+                             f"low={low}, high={high}, cl={cl}")
+
+        if low is not None:
+            try:
+                iter(low)
+            except TypeError:
+                low = [low]
+        if high is not None:
+            try:
+                iter(high)
+            except TypeError:
+                high = [high]
+        if cl is None:
+            if arrows:
+                cl = [0.90, 0.95, 0.99]
+        else:
+            try:
+                iter(cl)
+            except TypeError:
+                cl = [cl]
+
+        _y_offset = min_cost if subtract_min else 0
+
+        if low is None:
+            if cl is not None:
+                for _cl_i in cl:
+                    if high is None:
+                        _cl_i_outside = (1 - _cl_i) / 2
+                    else:
+                        _cl_i_outside = 1 - _cl_i
+                        _cl_i = 2 * _cl_i - 1
+                    _sigma_i = ConfidenceLevel(cl=_cl_i).sigma
+                    _arrow_specs.append({
+                        "side": "left",
+                        "x": self._find_cost_cut(
+                            parameter_name=parameter_name,
+                            guess=min_par_val-_sigma_i*par_err,
+                            target_cost=min_cost+_sigma_i**2,
+                            min_parameters=min_par_vals
+                        ),
+                        "y": min_cost-_y_offset+_sigma_i**2,
+                        "cl": _cl_i_outside
+                    })
+        else:
+            for _low_i in low:
+                _cost_low = self._get_cost_value(parameter_name, _low_i, min_par_vals)
+                _cl_low = (1 - ConfidenceLevel(delta_nll=_cost_low-min_cost).cl) / 2
+                _arrow_specs.append({
+                    "side": "left",
+                    "x": _low_i,
+                    "y": _cost_low-_y_offset,
+                    "cl": _cl_low
+                })
+
+        if high is None:
+            if cl is not None:
+                for _cl_i in cl:
+                    if low is None:
+                        _cl_i_outside = (1 - _cl_i) / 2
+                    else:
+                        _cl_i_outside = 1 - _cl_i
+                        _cl_i = 2 * _cl_i - 1
+                    _sigma_i = ConfidenceLevel(cl=_cl_i).sigma
+                    _arrow_specs.append({
+                        "side": "right",
+                        "x": self._find_cost_cut(
+                            parameter_name=parameter_name,
+                            guess=min_par_val+_sigma_i*par_err,
+                            target_cost=min_cost+_sigma_i**2,
+                            min_parameters=min_par_vals
+                        ),
+                        "y": min_cost-_y_offset+_sigma_i**2,
+                        "cl": _cl_i_outside
+                    })
+        else:
+            for _high_i in high:
+                _cost_high = self._get_cost_value(parameter_name, _high_i, min_par_vals)
+                _cl_high = (1 - ConfidenceLevel(delta_nll=_cost_high-min_cost).cl) / 2
+                _arrow_specs.append({
+                    "side": "right",
+                    "x": _high_i,
+                    "y": _cost_high-_y_offset,
+                    "cl": _cl_high
+                })
+
+        return _arrow_specs
 
     def _remove_zeroes_for_fixed(self, matrix):
         """
         Takes a full error matrix and removes the rows and
         columns that corresponding to fixed parameters.
         """
         assert (matrix.shape == (self.num_pars, self.num_pars))
@@ -522,27 +705,45 @@
         :type sigma: float
         :param minimizer_contour_kwargs: backend-specific kwargs.
         :return: the calculated contour
         :rtype: kafe2.core.contour.Contour
         """
 
     @abstractmethod
-    def profile(self, parameter_name, bins=20, bound=2, subtract_min=False):
+    def profile(self, parameter_name, low=None, high=None, sigma=None, cl=None, size=20,
+                subtract_min=False, arrows=False):
         """
         Calculate a 1D profile using the profile likelihood method: a single parameter is fixed
         while the rest are varied to minimize the cost function. The mapping of parameter value to
         cost function value around the minimum is the profile.
         The interval [par_min - par_err * bound, par_min + par_err * bound] is profiled by this
         method.
-        :param parameter_name: the name of the parameter to fix.
+        :param parameter_name: the name of the parameter to profile.
         :type parameter_name: str
-        :param bins: the number of points to evaluate the cost function at.
-        :type bins: int
+        :param low: Lower bound of the profiled interval. If multiple values are provided the
+            minimum value is used.
+        :param high: Upper bound of the profiled interval. If multiple values are provided the
+            maximum value is used.
+        :type high: float or Sequence[float] or None
+        :param sigma: Number of std deviations to deviate at least from the optimal value in either
+            direction if low or high aren't defined.
+        :type sigma: float
+        :param cl: Confidence level of the profiled interval. If low or high is defined then cl is
+            interpreted as the confidence level of a one-sided confidence interval. If both low
+            and high are undefined then cl is interpreted as the confidence level of a central
+            confidence interval. Cannot be defined if both high and low are defined. If multiple
+            values are provided then the maximum value is used.
+        :type cl: float or Sequence[float] or None
+        :param size: the number of points to evaluate the cost function at.
+        :type size: int
         :param bound: parameter determining the size of the interval to profile (see above).
         :type bound: float
         :param subtract_min: if True, subtract the cost function value of the minimum from the cost
         function values of the profile.
         :type subtract_min: bool
+        :param arrows: if True, calculate arrow specifications for annotating plots of the profile.
+            This can extend the profile range if necessary.
+        :type arrows: bool
         :return: the parameter values of the fixed parameter and the corresponding cost function
-        values.
-        :rtype: numpy.ndarray of shape (2, bins)
+        values and the arrow specifications.
+        :rtype: tuple of numpy.ndarray of shape (2, bins) and list
         """
```

### Comparing `kafe2-2.7.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -538,35 +538,34 @@
                                constraints=_local_constraints,
                                tol=self.tolerance,
                                callback=None,
                                options=dict(maxiter=6000, disp=False))
         self._x0 = _result.x
         return _result.fun
 
-    def profile(self, parameter_name, bins=21, bound=2, subtract_min=False):
+    def profile(self, parameter_name, low=None, high=None, sigma=None, cl=None, size=20,
+                subtract_min=False, arrows=False):
         if not self.did_fit:
             raise RuntimeError("Need to perform a fit before calling profile()!")
+        self._save_state()
         _par_id = self._par_names.index(parameter_name)
-        _par_err = self.parameter_errors[_par_id]
-        _par_min = self._par_val[_par_id]
-        _par = np.linspace(
-            start=_par_min - bound * _par_err,
-            stop=_par_min + bound * _par_err,
-            num=bins, endpoint=True
-        )
         _y_offset = self.function_value if subtract_min else 0
+        _bound_low, _bound_high, _arrow_specs = self._get_profile_bound(
+            parameter_name, low, high, sigma, cl, arrows)
+        self._load_state()
+        _par = np.linspace(start=_bound_low, stop=_bound_high, num=size, endpoint=True)
 
-        _y = np.empty(bins)
+        _y = np.zeros(size)
         self._x0 = self._par_val
-        for i in range(bins):
+        for i in range(size):
             _y[i] = self._calc_fun_with_constraints(
                 [{"type": "eq", "fun": lambda x: x[_par_id] - _par[i]}], continuous_x0=True
             )
-        self._func_wrapper_unpack_args(self._par_val)
-        return np.asarray([_par, _y - _y_offset])
+        self._load_state()
+        return np.asarray([_par, _y - _y_offset]), _arrow_specs
 
     def _func_wrapper(self, *parameter_values):
         '''call FCN, but ensure fixed parameters are passed with their fixed value'''
         # Note: this is needed in order to ensure that derivatives of `_func_wrapper`
         #       take parameter fixing into account
         assert (len(self.parameter_values) == len(self._par_fixed) == len(parameter_values))
         # replace parameter values
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,151 @@
-r"""The :py:mod:`kafe2.fit` module provides an essential toolkit for estimating model
+r"""The :py:mod:`kafe2.fit` module provides an object-oriented toolkit for estimating model
 parameters from data ("fitting").
 
 It distinguishes between a number of different data types:
 
+*  *xy* data (dedicated submodule: :py:mod:`~kafe2.fit.xy`),
 *  series of indexed measurements (dedicated submodule: :py:mod:`~kafe2.fit.indexed`),
-*  *xy* data (dedicated submodule: :py:mod:`~kafe2.fit.xy`), and
-*  histograms (dedicated submodule: :py:mod:`~kafe2.fit.histogram`)
+*  histograms (dedicated submodule: :py:mod:`~kafe2.fit.histogram`),
+*  raw 1D data using the method of maximum likelihood ("unbinned fit",
+   dedicated submodule: :py:mod:`~kafe2.fit.histogram`), and
+*  direct minimization of a cost function (dedicated submodule: :py:mod:`~kafe2.fit.custom`).
 
 Each of the above data types has its own particularities when it comes to fitting.
 The main difference is due to the way uncertainties can be defined and
-interpreted for each type of data.
+interpreted for each type of data and how the fit results are presented.
 
 
-Indexed data
-------------
+XY Data
+-------
 
-For **indexed** data, one data set consists of a list of :math:`N` distinct measurements
-:math:`d_i`, with the (discrete) index :math:`i` ranging from :math:`0` to :math:`N-1`.
+For *xy* data, one data set consists of a list of :math:`N` distinct :math:`y` measurements
+:math:`d_i` with the (discrete) index :math:`i` ranging from :math:`0` to :math:`N-1`.
+The measurements were taken at :math:`x` values :math:`x_i`.
 For each measurement in the series, one or more uncertainty sources can be defined,
-each being a numerical estimate of how much the respective measurement fluctuates.
+each being a numerical estimate of how much the respective measurement has fluctuated from the
+"true values".
 Correlations between uncertainties on separate measurements :math:`d_i` and :math:`d_j` can also
 be taken into account by using *covariance/correlation matrices*.
 
-Fits to *indexed* data take these uncertainties and correlations into account when estimating
-the model parameters and their uncertainties. When plotting indexed data, measurements are
-represented as data points with error bars at :math:`(x=i, y=d_i)`, whereas the model
-is indicated by a horizontal line near the corresponding data point.
-
-The following objects are provided for handling *indexed* data, as described above:
-
-*  :py:obj:`~kafe2.fit.indexed.IndexedContainer`: data container for storing *indexed* data
-*  :py:obj:`~kafe2.fit.indexed.IndexedParametricModel`: corresponding model:
-
-   - uses a model function (:py:obj:`~kafe2.fit.indexed.model.IndexedModelFunction`) to calculate the model
-     predictions and stores the result in an :py:obj:`~kafe2.fit.IndexedContainer`
-
-*  :py:obj:`~kafe2.fit.indexed.IndexedFit`: a fit of a parametric model to *indexed* data:
-
-   - finds the minimum of the *cost function* to find the
-     parameter values for which the model best fits the data
-
-
-XY data
--------
-
-For **xy** data, the same principle as for *indexed* data applies, except each measurement and model prediction
-now depends on a continuous real independent variable :math:`x` instead of a discrete index :math:`i`.
-In effect, the data now consist of :math:`N` ordered pairs :math:`(x=x_i, y=d_i)`.
-
-In contrast to *indexed* data, where only uncertainties on the measurement could be defined,
-for *xy* data there is the additional possibility of defining additional uncertainites on :math:`x`.
-These can be handled in a number of different ways when fitting an *xy* model to data.
+Additional uncertainites on :math:`x_i` can also be defined.
+When fitting an *xy* model to data they are converted to :math:`y` uncertainties via multiplication
+with the derivative of the model function by :math:`x`.
 When plotting the result of *xy* fits, the model function is displayed as a continuous
-function of :math:`x`, and an **error band** can be computed to reflect the model uncertainty,
-as determined by propagating the data uncertainties.
-
-.. TODO: complete section on x errors
+function of :math:`x`, and an *error band* can be computed to reflect the model uncertainty,
+as determined by propagating the parameter uncertainties onto the *y* axis.
 
 The following objects are provided for handling *xy* data:
 
 *  :py:obj:`~kafe2.fit.xy.XYContainer`: data container for storing *xy* data
-*  :py:obj:`~kafe2.fit.xy.XYParametricModel`: corresponding model:
-
-   - uses a model function (:py:obj:`~kafe2.fit.xy.model.XYModelFunction`) to calculate the model predictions and
-     stores the result in an :py:obj:`~kafe2.fit.XYContainer`
+*  :py:obj:`~kafe2.fit.xy.XYParametricModel`: corresponding model
+*  :py:obj:`~kafe2.fit.xy.XYFit`: a fit of a parametric model to *xy* data
 
-*  :py:obj:`~kafe2.fit.xy.XYFit`: a fit of a parametric model to *xy* data:
-
-   - finds the minimum of the *cost function* to find the parameter values for which the model best fits the data
+Indexed data
+------------
 
+Compared to *xy* data indexed data no longer has an explicit *x* axis.
+The data simply appears as an indexed list of data points.
+As a consequence the model function does not expect an indendent variable.
+
+The following objects are provided for handling indexed data, as described above:
+
+*  :py:obj:`~kafe2.fit.indexed.IndexedContainer`: data container for storing indexed data
+*  :py:obj:`~kafe2.fit.indexed.IndexedParametricModel`: corresponding model
+*  :py:obj:`~kafe2.fit.indexed.IndexedFit`: a fit of a parametric model to *indexed* data
 
 Histograms
 ----------
 
-Finally, *kafe2* is also able to handle **histograms**. Histograms organize measurements whose
+*kafe2* is also able to handle *histograms*. Histograms organize measurements whose
 values can fall anywhere across a continuum of values into a number of discrete regions
-or "bins". Typically, the continuous "measurement space" (a closed real interval :math:`[x_{\rm min}, x_{\rm max}]`)
+or "bins". Typically, the continuous "measurement space" (a closed real interval
+:math:`[x_{\rm min}, x_{\rm max}]`)
 is subdivided into a sequence of successive intervals at the "bin edges"
-:math:`x_{\rm min} < x_1 < x_2 < \ldots < x_{\rm max}`. Whenever a measurement falls into one of the bins, the
-value of that histogram bin is incremented by one.
-So a histogram is completely defined by its bin edges and the bin values.
+:math:`x_{\rm min} < x_1 < x_2 < \ldots < x_{\rm max}`. Whenever a measurement falls into one of
+the bins, the value of that histogram bin is incremented by one.
+A histogram is completely defined by its bin edges and the bin values.
 
 .. note::
     The bin numbering starts at :math:`1` for the first bin and ends at :math:`N`, where :math:`N`
-    is defined as the *size* of the histogram. The bin numbers :math:`0` and :math:`N+1` refer to the
-    underflow (below :math:`x_{\rm min}`) and overflow bin (above :math:`x_{\rm max}`), respectively.
-
+    is defined as the *size* of the histogram. The bin numbers :math:`0` and :math:`N+1` refer to
+    the underflow (below :math:`x_{\rm min}`) and overflow bin (above :math:`x_{\rm max}`),
+    respectively.
 
-Defining a parametric model for histograms is not as straightforward as for *xy* and *indexed* data.
-Seeing as they keep track of the number of entries in different intervals of the continuum, the bin values
-can be interpreted using probability theory.
 
-As the number of entries approaches infinity, the number of entries :math:`n` in the bin covering an interval
-:math:`[a, b)`, divided by the total number of entries :math:`N_{\rm E}`, will approach the probablity of an
-event landing in that bin:
+Defining a parametric model for histograms is not as straightforward as for *xy* and indexed data.
+Seeing as they keep track of the number of entries in different intervals of the continuum, the bin
+values can be interpreted using probability theory.
+
+As the number of entries approaches infinity, the number of entries :math:`n` in the bin covering an
+interval :math:`[a, b)`, divided by the total number of entries :math:`N_{\rm E}`, will approach the
+probablity of an event landing in that bin:
 
 .. math::
     \lim_{N_{\rm E}\rightarrow\infty} \frac{n}{N_{\rm E}} = \int_a^b f(x)\,{\rm d}x = F(b) - F(a)
 
-In the above formula, :math:`f(x)` is the **probability distribution function** (or **probability density**),
+In the above formula, :math:`f(x)` is the *probability density function*,
 and :math:`F(x)` is an antiderivative of :math:`f`
-(for example the **cumulative probability distribution function**).
+(for example the *cumulative distribution function*).
 
-Using the above relation, the model prediction :math:`m` for the bin :math:`[a, b)` can be defined as:
+Using the above relation, the model prediction :math:`m` for the bin :math:`[a, b)` can be defined
+as:
 
 .. math::
     m = N_{\rm E} \int_a^b f(x)\,{\rm d}x = N_{\rm E} \left(F(b) - F(a)\right)
 
-This means that, for histograms, the *model density* :math:`f(x)` needs to be specified.
+This means that, for histograms, the model density :math:`f(x)` needs to be specified as the model
+function.
 The model is then calculated by numerically integrating this function over each bin.
-When fitting, however, the model needs to be calculated for many different points in parameter space,
-which makes this approach very slow (many numerical integrations until the fit converges).
 
 An alternative would be to specify the model density *antiderviative* :math:`F` alongside
-the model, so that the model can be calculated as a simple difference, rather than a complicated integral.
+the model, so that the model can be calculated as a simple difference, rather than as an integral.
 
 The following objects are provided for handling histograms:
 
 *  :py:obj:`~kafe2.fit.histogram.HistContainer`: data container for storing histograms
-*  :py:obj:`~kafe2.fit.histogram.HistParametricModel`: corresponding model:
+*  :py:obj:`~kafe2.fit.histogram.HistParametricModel`: corresponding model
+*  :py:obj:`~kafe2.fit.histogram.HistFit`: a fit of a parametric model to histograms
+
+Unbinned
+--------
+
+If data is treated as *unbinned* the model function :math:`f(x)` is interpreted as a
+*model density function*.
+The cost function value :math:`C` is then directly calculated as the negative log-likelihood of the
+data given said PDF:
+
+.. math::
+    C = - 2 \sum_{i=0}^{N-1} \ln f(x_i) .
+
+An unbinned fit is the edge case of a histogram fit for as the individual bins become
+infinitessimally thin.
+
+The following objects are provided for handling unbinned data:
+
+*  :py:obj:`~kafe2.fit.unbinned.UnbinnedContainer`: data container for storing unbinned data
+*  :py:obj:`~kafe2.fit.unbinned.UnbinnedParametricModel`: corresponding model
+*  :py:obj:`~kafe2.fit.unbinned.UnbinnedFit`: a fit of a parametric model to unbinned data
+
+Custom
+------
+
+Lets the user directly define a cost function.
+Since this fit type does not have explicit data the fit results cannot be plotted automatically.
 
-   - uses a model function (:py:obj:`~kafe2.fit.xy.model.HistModelFunction`) to calculate the model predictions
-     and stores the result in an :py:obj:`~kafe2.fit.HistContainer`
+The following objects are provided for custom fits:
 
-*  :py:obj:`~kafe2.fit.histogram.HistFit`: a fit of a parametric model to histograms:
+*  :py:obj:`~kafe2.fit.custom.CustomFit`: a fit for minimizing a cost function
 
-   - finds the minimum of the *cost function* to find the parameter values for which the model best fits the data
+Plots
+-----
 
-For creating graphical representations of fits, the :py:obj:`~kafe2.fit.Plot` is provided. It can be instantiated
-with any fit object (or list of fit objects) as an argument and will produce one or more plots accordingly
-using `matplotlib`.
+For creating graphical representations of fits, the :py:obj:`~kafe2.fit.Plot` is provided.
+It can be instantiated with any fit object (or list of fit objects) as an argument and will produce
+one or more plots accordingly using `matplotlib`.
 
 :synopsis: This module contains specialized objects for storing measurement data,
            defining and fitting parametric models to these data and producing
            graphical representations ("plots") of the result.
            It relies on the :py:mod:`kafe2.core` module for basic functionality.
 
 .. moduleauthor:: Daniel Savoiu <daniel.savoiu@cern.ch>
@@ -150,8 +162,9 @@
 from .tools import *
 from .xy import *
 from .unbinned import *
 
 from ._base.plot import Plot
 from .tools.fit_wrapper import Fit  # import after every fit to avoid import conflicts with other tools
 
-from .util import function_library, xy_fit, plot, plot_xy_data, k2Fit
+from .util import function_library, custom_fit, hist_fit, indexed_fit, unbinned_fit, xy_fit, plot, \
+    k2Fit
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_aux.py` & `kafe2-2.8.0rc1/kafe2/fit/_aux.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/container.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,16 @@
                 _invalid_args = self.RESERVED_NODE_NAMES.intersection(
                     set(self._model_function.signature.parameters))
                 raise ValueError(
                     "The following names are reserved and cannot be used as model function arguments: %r"
                     % (_invalid_args,))
 
         # set and validate the cost function
-        self._implicit_no_errors = cost_function == "chi2" and isinstance(data, DataContainerBase) \
-            and not data.has_errors
+        _data_has_errors = isinstance(data, DataContainerBase) and data.has_errors
+        self._implicit_no_errors = cost_function == "chi2" and not _data_has_errors
         if self._implicit_no_errors:
             cost_function = "chi2_no_errors"
         if isinstance(cost_function, CostFunction):
             self._cost_function = cost_function
         elif isinstance(cost_function, str):
             try:
                 _cost_function_class, _kwargs = self._STRING_TO_COST_FUNCTION[cost_function]
@@ -393,14 +393,15 @@
         for _error_name in self._BASIC_ERROR_NAMES:
             self._nexus.get(_error_name).mark_for_update()
         if self._implicit_no_errors:
             _cost_function_class, _kwargs = self._STRING_TO_COST_FUNCTION["chi2_covariance"]
             self._cost_function = _cost_function_class(**_kwargs)
             self._cost_function_pointwise = self._cost_function.pointwise_version
             self._init_cost_function(existing_behavior='replace')
+            self._fitter.parameter_to_minimize = self._cost_function.name
             self._implicit_no_errors = False
 
 
     def _set_data_as_model_ref(self):
         for _err in self._param_model.get_matching_errors({"relative": True}).values():
             _old_ref = _err.reference
             _err.reference = self._data_container.data
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/format.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         """
         return self._fixed
 
     @fixed.setter
     def fixed(self, fixed):
         self._fixed = fixed
 
-    def get_formatted(self, with_name=False, with_value=True, with_errors=True,
+    def get_formatted(self, value=None, with_name=False, with_value=True, with_errors=True,
                       n_significant_digits=2, round_value_to_error=True, asymmetric_error=False,
                       format_as_latex=False):
         """Get a formatted string representing this model parameter.
 
         :param bool with_name: If :py:obj:`True`, the output will include the parameter name.
         :param bool with_value: If :py:obj:`True`, the output will include the parameter value.
         :param bool with_errors: If :py:obj:`True`, the output will include the parameter error(s).
@@ -274,14 +274,16 @@
         :param bool asymmetric_error: If :py:obj:`True`, the asymmetric parameter uncertainties are
             used.
         :param bool format_as_latex: If :py:obj:`True`, the returned string will be formatted using
             LaTeX syntax.
         :return: The string representation of the parameter.
         :rtype: str
         """
+        if value is None:
+            value = self.value
         _display_string = ""
         if with_name:
             if format_as_latex:
                 _display_string += "$%s$" % (self.latex_name,)
             else:
                 _display_string += "%s" % (self.name,)
 
@@ -294,41 +296,41 @@
                     _display_string += r"$%g$ (fixed)" % self._value
                 else:
                     _display_string += "%g (fixed)" % self._value
             elif not with_errors or (not asymmetric_error and self.error in (None, 0)) or \
                     (asymmetric_error and (
                             self.asymmetric_error is None or np.all(self.asymmetric_error == 0))):
                 if format_as_latex:
-                    _display_string += f"$%.{n_significant_digits}g$" % self.value
+                    _display_string += f"$%.{n_significant_digits}g$" % value
                 else:
-                    _display_string += f"%.{n_significant_digits}g" % self.value
+                    _display_string += f"%.{n_significant_digits}g" % value
             else:
                 if asymmetric_error:
                     _min_err = min(abs(self.error_up), abs(self.error_down))
                 else:
                     _min_err = self.error
                 # fallback to rounding to 10^(-1) if error is zero
                 if not _min_err or np.isnan(_min_err):
                     _min_err = 1e-1
 
                 # calculate decimal precision if rounding:
                 if round_value_to_error:
                     val_formatter = ScalarFormatter(_min_err, n_significant_digits=n_significant_digits)
-                    _val = val_formatter(self.value)
+                    _val = val_formatter(value)
                     _err = "%#.{n}g".format(n=n_significant_digits) % self.error
                     if asymmetric_error:  # needed for different powers of 10 in asymmetric errs
                         if abs(self.error_down) <= abs(self.error_up):
                             _err_u = val_formatter(abs(self.error_up))
                             _err_d = "%#.{n}g".format(n=n_significant_digits) % abs(self.error_down)
                         else:
                             _err_d = val_formatter(abs(self.error_down))
                             _err_u = "%#.{n}g".format(n=n_significant_digits) % abs(self.error_up)
                 # default cases if no rounding
                 else:
-                    _val = f"%.{n_significant_digits}g" % self.value
+                    _val = f"%.{n_significant_digits}g" % value
                     _err = f"%.{n_significant_digits}g" % self.error
                     if asymmetric_error:
                         _err_u = f"%.{n_significant_digits}g" % self.error_up
                         _err_d = f"%.{n_significant_digits}g" % self.error_down
 
                 if asymmetric_error:
                     if format_as_latex:
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/model.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
                 self._model_function_handle = sp.lambdify(_symbols, _symbolic_function)
                 _latex_string = sp.latex(_symbolic_function)
                 _latex_string = _latex_string.replace(r"{", r"{{")
                 _latex_string = _latex_string.replace(r"}", r"}}")
                 for _symbol in _symbols:
                     _latex_string = _latex_string.replace(r"{{%s}}" % _symbol, r"{%s}" % _symbol)
 
-                print(_latex_string)
                 self._model_function_handle.latex_name = _latex_name
                 self._model_function_handle.latex_expression_format_string = _latex_string
             if not self._model_function_handle:
                 raise ValueError('Unknown model function: %s' % model_function)
             self._callable = self._model_function_handle
 
         # special handling of numpy vectorized functions
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/_base/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 import matplotlib as mpl
 import os
 from collections.abc import Iterable
 
 from .container import DataContainerBase
 from .format import ParameterFormatter
 from ..multi.fit import MultiFit
+from ..util.wrapper import _fit_history
 from ...config import kc, ConfigError, kafe2_rc
 
 from collections import OrderedDict
 from matplotlib import pyplot as plt
 from matplotlib import gridspec as gs
 from matplotlib.legend_handler import HandlerBase
 from matplotlib import rc_context
 
+try:
+    import typing  # help IDEs with type-hinting inside docstrings
+except ImportError:
+    pass
+
 __all__ = ["PlotAdapterBase", "Plot", "kc_plot_style"]
 
 
 def kc_plot_style(data_type, subplot_key, property_key):
     try:
         # try to find plot style-related configuration entry
         return kc('fit', 'plot', 'style', data_type, subplot_key, property_key)
@@ -690,22 +696,38 @@
         {model_function}
         {parameters}
             $\\hookrightarrow${cost}
             $\\hookrightarrow${fit_quality}
     """)
 
     def __init__(self, fit_objects, separate_figures=False):
+        """
+        :param fit_objects: which kafe2 fits to use for the plot. A positive integer is interpreted
+            as the fit with the given index that has been performed (with wrappers) since the
+            program started. A negative integer *-n* is interpreted as the last *n* fits. kafe2 fit
+            objects are used directly. If a sequence of fit objects is passed they can be displayed
+            as part of the same plot.
+        :type fit_objects: int or :py:class:`~kafe2.fit._base.FitBase`
+            or Sequence[:py:class:`~kafe2.fit._base.FitBase`]
+        :param separate_figures: whether the fits should be displayed in separate figures.
+        :type separate_figures: bool
+        """
         from kafe2.fit.tools.fit_wrapper import Fit
 
         # set the managed fit objects
         if isinstance(fit_objects, MultiFit):
             self._multifit = fit_objects
             fit_objects = fit_objects.fits
         else:
             self._multifit = None
+        if isinstance(fit_objects, int):
+            if fit_objects >= 0:
+                fit_objects = [_fit_history[fit_objects]["fit"]]
+            else:
+                fit_objects = [_f["fit"] for _f in _fit_history[fit_objects:]]
         try:
             iter(fit_objects)
         except TypeError:
             fit_objects = (fit_objects,)
         self._from_container = tuple(isinstance(_fo, DataContainerBase) for _fo in fit_objects)
         self._fits = tuple(
             Fit(_fo) if _fc else _fo for _fc, _fo in zip(self._from_container, fit_objects))
@@ -1079,17 +1101,21 @@
             _y_ticks = _adapter.y_ticks
 
             if len(_x_ticks) > 0:
                 if isinstance(_x_ticks[0], str):
                     _ax.set_xticks(np.arange(len(_x_ticks)), labels=_x_ticks)
                 else:
                     _ax.set_xticks(_x_ticks)
+                # Use default formatter for custom ticks, log formatter doesn't seem to work:
+                _ax.get_xaxis().set_major_formatter(mpl.ticker.ScalarFormatter())
 
             if len(_y_ticks) > 0:
                 _ax.set_yticks(_y_ticks)
+                # Use default formatter for custom ticks, log formatter doesn't seem to work:
+                _ax.get_yaxis().set_major_formatter(mpl.ticker.ScalarFormatter())
 
         # hide x tick labels in all but the lowest axes
         for _key in axes_keys[:-1]:
             self._current_axes[_key].set_xlabel(None)
             for _label in self._current_axes[_key].get_xticklabels():
                 _label.set_visible(False)
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/custom/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/custom/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/container.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         """fill any entries marked as unprocessed into the histogram"""
         if self._manual_heights:
             raise RuntimeError("The bin heights have been set manually. Filling entries is not "
                                "available anymore. Please construct a new HistContainer!")
         if not self._unprocessed_entries:
             return
         _entries_sorted = np.sort(self._unprocessed_entries)
+        if np.all(self._unprocessed_entries == np.floor(self._unprocessed_entries)):
+            warnings.warn("Histogram data is int. Make sure to consider this for your bin edges!")
 
         _current_entry_index = 0
         _current_entry_value = _entries_sorted[0]
         _current_bin_index = 0  # start with underflow bin
         _current_bin_upper_edge = self.low
         _current_bin_lower_edge = -np.inf
 
@@ -120,16 +122,14 @@
             self._data[-1] += len(_overflow_entries)
             # print "Bin %d (of): add %d entries" % (_current_bin_index+1, len(_overflow_entries))
             # for i in _overflow_entries:
             #     print '\t', i
             self._processed_entries += list(_overflow_entries)
 
         self._unprocessed_entries = []
-        if np.all(self._data == np.floor(self._data)):
-            warnings.warn("Historam data is int. Make sure to consider this for your bin edges!")
 
     def _get_error_reference(self):
         return self._data[1:-1]
 
     # -- public properties
 
     @property
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,16 +35,17 @@
         Construct a fit of a model to a histogram. If bin_evaluation is a Python function or
         of a numpy.vectorize object it is interpreted as the antiderivative of
         model_density_function. If bin_evaluation is equal to "rectangle", "midpoint", "trapezoid",
         or "simpson" the bin heights are evaluated according to the corresponding quadrature
         formula. If bin_evaluation is equal to "numerical" the bin heights are evaluated by
         numerically integrating model_density_function.
 
-        :param data: a :py:class:`~kafe2.fit.hist.HistContainer` representing histogrammed data
-        :type data: :py:class:`~kafe2.fit.hist.HistContainer`
+        :param data: an encapsulated representation of the histogrammed data.
+        :type data: :py:class:`~kafe2.fit.hist.HistContainer` or two-dimensional iterable of bin
+            heights and bin edges as returned by `np.histogram`.
         :param model_function: the model (density) function
         :type model__function: :py:class:`~kafe2.fit.hist.HistModelFunction` or unwrapped
             native Python function
         :param cost_function: the cost function
         :type cost_function: :py:class:`~kafe2.fit._base.CostFunctionBase`-derived or unwrapped
             native Python function
         :param bin_evaluation: how the model evaluates bin heights.
@@ -72,21 +73,35 @@
             'model',
             depends_on=(
                 'parameter_values'
             )
         )
 
     def _set_new_data(self, new_data):
-        if isinstance(new_data, self.CONTAINER_TYPE):
+        try:
+            _new_data_is_numpy_histogram = len(new_data) == 2 \
+                and len(new_data[0]) + 1 == len(new_data[1])
+        except TypeError:
+            _new_data_is_numpy_histogram = False
+        if _new_data_is_numpy_histogram:
+            self._data_container = self.CONTAINER_TYPE(
+                n_bins=len(new_data[0]), bin_range=(new_data[1][0], new_data[1][-1]),
+                bin_edges=new_data[1]
+            )
+            self._data_container.set_bins(new_data[0])
+        elif isinstance(new_data, self.CONTAINER_TYPE):
             self._data_container = deepcopy(new_data)
         elif isinstance(new_data, DataContainerBase):
             raise TypeError("Incompatible container type '{}' (expected '{}')"
                             .format(type(new_data), self.CONTAINER_TYPE))
         else:
-            raise TypeError("Fitting a histogram requires a HistContainer!")
+            raise TypeError(
+                "Fitting a histogram requires a kafe2 HistContainer or a NumPy histogram as data "
+                f"but received {new_data}"
+            )
         self._data_container._on_error_change_callback = self._on_error_change
 
         self._nexus.get('data').mark_for_update()
 
     def _set_new_parametric_model(self):
         # create the child ParametricModel object
         self._param_model = HistParametricModel(
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/model.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/histogram/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/container.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/format.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/format.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/model.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/indexed/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/io/file.py` & `kafe2-2.8.0rc1/kafe2/fit/io/file.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/io/handle.py` & `kafe2-2.8.0rc1/kafe2/fit/io/handle.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/multi/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/multi/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/multi/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/multi/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/_yaml_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/_yaml_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/constraint/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/constraint/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/container/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/container/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/container/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/container/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/error/common_error_tools.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/error/common_error_tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/fit/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/fit/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/fit/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/fit/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/format/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/format/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/format/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/format/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/model/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/model/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/representation/model/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/model/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/tools/contours_profiler.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/contours_profiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -124,14 +124,20 @@
     functions of two variables and can be visualized in the plane by drawing the 3D *contours*
     along which this function remains constant.
 
     This object offers a means of calculating both profiles and contours
     """
 
     _DEFAULT_PLOT_PROFILE_KWARGS = dict(marker='', linewidth=2)
+    _DEFAULT_PLOT_PROFILE_ARROW_KWARGS = dict(
+        color="black", linewidth=1, shrinkA=0, shrinkB=0, horizontal_arrow_length=0.05,
+        arrowstyle=mpl.patches.ArrowStyle("fancy", head_length=6, head_width=6, tail_width=0.01),
+        vertical_x_text=0.005, vertical_y_text=0.005, horizontal_x_text=0.015,
+        horizontal_y_text=-0.03
+    )
     _DEFAULT_PLOT_PARABOLA_KWARGS = dict(marker='', linewidth=2, linestyle='--')
     _DEFAULT_PLOT_ERROR_SPAN_ON_PROFILE_KWARGS = dict(color='gray', alpha=0.5)
     _DEFAULT_PLOT_MINIMUM_KWARGS = dict(markersize=12, marker='*', linewidth=1.5, linestyle='',
                                         capsize=4, color='green', ecolor='green', elinewidth=1.5)
     _DEFAULT_PLOT_MINIMUM_HVLINES_KWARGS = dict(linewidth=1.0, linestyle='--', color='green', marker='')
     _DEFAULT_PLOT_FILL_CONTOUR_KWARGS = dict(alpha=0.3, linewidth=2)
 
@@ -175,14 +181,26 @@
         self._cost_function_formatted_name = "${}$".format(self._fit._cost_function.formatter.latex_name)
         # FIXME MultiFit does not have an internal _model_function field
         self._parameters_formatted_names = ["${}$".format(pf.latex_name)
                                             for pf in self._fit._get_model_function_parameter_formatters()]
 
         self._figures = []
 
+    def _get_profile(self, parameter, low=None, high=None, sigma=None, cl=None, points=None,
+                     subtract_min=None, arrows=False):
+        if low is None and high is None and sigma is None and cl is None:
+            sigma = 2
+        if points is None:
+            points = self._profile_kwargs['points']
+        if subtract_min is None:
+            subtract_min = self._profile_kwargs['subtract_min']
+        self._fit._check_dynamic_error_compatibility()
+        return self._fit._fitter.profile(
+            parameter, low, high, sigma, cl, points, subtract_min, arrows)
+
     def _make_figure_gs(self, nrows=1, ncols=1):
         _fig = plt.figure(figsize=(8, 8))  # defaults from matplotlibrc
 
         if mpl.__version__.startswith('1'):
             # old API does not support passing 'figure'
             _gs = gs.GridSpec(nrows=nrows, ncols=ncols)
         else:
@@ -194,14 +212,50 @@
 
     @staticmethod
     def _plot_profile_xy(target_axes, x, y, label):
         _kwargs = ContoursProfiler._DEFAULT_PLOT_PROFILE_KWARGS.copy()
         return target_axes.plot(x, y, label=label, **_kwargs)
 
     @staticmethod
+    def _plot_profile_arrow(target_axes, x_span, y_span, par_formatter, side, x, y, cl):
+        _kwargs_vertical = ContoursProfiler._DEFAULT_PLOT_PROFILE_ARROW_KWARGS.copy()
+        del _kwargs_vertical["horizontal_arrow_length"]
+        del _kwargs_vertical["horizontal_x_text"]
+        del _kwargs_vertical["horizontal_y_text"]
+        if side == "left":
+            _x_text = x + _kwargs_vertical.pop("vertical_x_text") * x_span
+            _y_text = y + _kwargs_vertical.pop("vertical_y_text") * y_span
+        elif side == "right":
+            _x_text = x - _kwargs_vertical.pop("vertical_x_text") * x_span
+            _y_text = y + _kwargs_vertical.pop("vertical_y_text") * y_span
+        target_axes.add_patch(mpl.patches.FancyArrowPatch((x, y), (x, 0), **_kwargs_vertical))
+        _par_text = par_formatter.get_formatted(
+            value=x, with_name=True, with_errors=False, format_as_latex=True)
+        target_axes.text(_x_text, _y_text, _par_text, horizontalalignment=side)
+
+        _kwargs_horizontal = ContoursProfiler._DEFAULT_PLOT_PROFILE_ARROW_KWARGS.copy()
+        del _kwargs_horizontal["vertical_x_text"]
+        del _kwargs_horizontal["vertical_y_text"]
+        if side == "left":
+            _x_target = x - _kwargs_horizontal.pop("horizontal_arrow_length") * x_span
+            _x_text = x - _kwargs_horizontal.pop("horizontal_x_text") * x_span
+            _y_text = y + _kwargs_horizontal.pop("horizontal_y_text") * y_span
+            _alignment = "right"
+        elif side == "right":
+            _x_target = x + _kwargs_horizontal.pop("horizontal_arrow_length") * x_span
+            _x_text = x + _kwargs_horizontal.pop("horizontal_x_text") * x_span
+            _y_text = y + _kwargs_horizontal.pop("horizontal_y_text") * y_span
+            _alignment = "left"
+        else:
+            raise ValueError(f"Unknown side: {side}")
+        target_axes.add_patch(mpl.patches.FancyArrowPatch(
+            (x, y), (_x_target, y), **_kwargs_horizontal))
+        target_axes.text(_x_text, _y_text, f"${100*cl:.2f}\%$", horizontalalignment=_alignment)
+
+    @staticmethod
     def _plot_parabolic_cost(target_axes, x, quad_coeff, x_offset, y_offset, label):
         _kwargs = ContoursProfiler._DEFAULT_PLOT_PARABOLA_KWARGS.copy()
         _y = quad_coeff * (x - x_offset) ** 2 + y_offset
         return target_axes.plot(x, _y, label=label, **_kwargs)
 
     @staticmethod
     def _plot_error_span_on_profile(target_axes, xmin, xmax, label):
@@ -252,41 +306,47 @@
 
     @staticmethod
     def show(*args, **kwargs):
         """Convenience wrapper for matplotlib.pyplot.show()"""
         plt.show(*args, **kwargs)
 
 
-    def get_profile(self, parameter, points=None, bound=None, subtract_min=None):
+    def get_profile(self, parameter, low=None, high=None, sigma=None, cl=None, points=None,
+                    subtract_min=None):
         """
         Calculate and return a profile of the cost function in a parameter.
 
         :param parameter: name of the parameter to profile (referred to as *x* here).
         :type parameter: str
+        :param low: Lower bound for the profile.
+        :type low: float or None
+        :param high: Upper bound for the profile.
+        :type high: float or None
+        :param sigma: Number of std deviations to deviate at least from the optimal value in either
+            direction if low or high aren't defined.
+        :type sigma: float
+        :param cl: Confidence level of the profiled region. If low or high is defined then cl is
+            interpreted as the confidence level of a one-sided confidence interval. If both low
+            and high are undefined then cl is interpreted as the confidence level of the central
+            confidence interval. Cannot be defined if both high and low are defined.
+        :type cl: float or None
         :param points: number of equidistant points to use as *x* values
         :type points: int
         :param bound: parameter region for the profile. A single value is interpreted as a sigma
             value for an interval symmetric around the cost function minimum. A tuple of two values
             is interpreted as the bounds of an arbitrary *x* interval to be profiled.
         :type bound: int or tuple of int
         :subtract_min: if the minimal cost function value should be subtracted from the profile
             *y* values.
         :type subtract_min: bool
         :return: two-dimensional array of *x* (parameter) values and *y* (cost function) values
         :rtype: two-dimensional array of float
         """
-        if bound is None:
-            bound = 2
-        if points is None:
-            points = self._profile_kwargs['points']
-        if subtract_min is None:
-            subtract_min = self._profile_kwargs['subtract_min']
-        _kwargs = dict(bins=points, bound=bound, args=None, subtract_min=subtract_min)
-        self._fit._check_dynamic_error_compatibility()
-        return self._fit._fitter.profile(parameter, **_kwargs)  # TODO fix for single fit inside multifit
+        return self._get_profile(parameter, low, high, sigma, cl, points, subtract_min,
+                                 arrows=False)[0]
 
     def get_contours(self, parameter_1, parameter_2, smoothing_sigma=None):
         """
         Calculate and return a list of contours (one for each requested sigma value).
 
         :param parameter_1: name of the first contour parameter
         :type parameter_1: str
@@ -316,68 +376,98 @@
 
             _contours.append((_cl_obj, _cont))
         self._fit._check_dynamic_error_compatibility()
         return _contours
 
     # - plot profiles/contours
 
-    def plot_profile(self, parameter, target_axes=None,
+    def plot_profile(self,
+                     parameter,
+                     low=None,
+                     high=None,
+                     sigma=None,
+                     cl=None,
+                     target_axes=None,
                      show_parabolic=True,
                      show_grid=True,
                      show_legend=True,
                      show_fit_minimum=True,
                      show_error_span=True,
                      show_ticks=True,
                      label_ticks_in_sigma=True,
                      label_fit_minimum=True):
         """
         Plot the profile cost function for a parameter.
 
         :param parameter: name of the parameter to profile in
         :type parameter: str
+        :param low: Lower bound(s) at which to display confidence levels.
+        :type low: float or Sequence[float] or None
+        :param high: Upper bound(s) at which to display confidence levels.
+        :type high: float or Sequence[float] or None
+        :param sigma: Number of std deviations to deviate at least from the optimal value in either
+            direction if low or high aren't defined.
+        :type sigma: float
+        :param cl: Confidence level(s) to mark in the plot. If low or high is defined then cl is
+            interpreted as the confidence level(s) of one-sided confidence intervals. If both low
+            and high are undefined then cl is interpreted as the confidence level(s) of central
+            confidence intervals. Cannot be defined if both high and low are defined.
+        :type cl: float or Sequence[float] or None
         :param target_axes: ``Axes`` object (if ``None``, a new figure is created)
         :type target_axes: ``matplotlib`` ``Axes`` or ``None``
         :param show_parabolic: if ``True``, a parabolic approximation of the profile near the minimum is also drawn
         :type show_parabolic: bool`
         :param show_grid: if ``True``, a grid is drawn
         :type show_grid: bool
         :param show_legend: if ``True``, the legend is displayed
+        :type show_legend: bool
         :param show_fit_minimum: if ``True``, the fit minumum is shown as a marker with error bars
         :type show_fit_minimum: bool
-        :type show_legend: bool
         :param show_error_span: if ``True``, the parameter error region is shaded
         :type show_error_span: bool
         :param show_ticks: if ``True``, *x* and *y* ticks are displayed
         :type show_ticks: bool
         :param label_ticks_in_sigma: if ``True``, label ticks are in units of 1 sigma
         :type label_ticks_in_sigma: bool
         :param label_fit_minimum: if ``True``, the parameter value and the 1 sigma error
             will be shown as an annotation
         :type label_fit_minimum: bool
 
         :return: figure containing the plot result
         :rtype: `matplotlib.figure.Figure`
         """
+
         with rc_context(kafe2_rc):
             if target_axes is None:
                 _fig, _gs = self._make_figure_gs(1, 1)
                 _axes = plt.subplot(_gs[0, 0])
             else:
                 _axes = target_axes
 
             _par_val = self._fit.parameter_name_value_dict[parameter]
             _par_id = list(self._fit.parameter_name_value_dict.keys()).index(parameter)
             _par_err = self._fit.parameter_errors[_par_id]
             _cost_function_min = self._fit.cost_function_value
             _par_formatted_name = self._parameters_formatted_names[_par_id]
 
-            _x, _y = self.get_profile(parameter)
-
-            _profile_artist = self._plot_profile_xy(_axes, _x, _y,
-                                                    label="profile %s" % (self._cost_function_formatted_name,))
+            (_x, _y), _arrow_specs = self._get_profile(
+                parameter, low, high, sigma, cl,
+                arrows=True)
+
+            _profile_artist = self._plot_profile_xy(
+                _axes, _x, _y, label="profile %s" % (self._cost_function_formatted_name,))
+
+            _x_span = np.max(_x) - np.min(_x)
+            _y_span = max(np.max(_y) - np.min(_y), np.max(((_x - _par_val) / _par_err) ** 2))
+            if _arrow_specs is not None:
+                for _arrow_spec in _arrow_specs:
+                    self._plot_profile_arrow(
+                        _axes, _x_span, _y_span,
+                        self._fit._get_model_function_parameter_formatters()[_par_id],
+                        **_arrow_spec)
 
             _y_offset = _cost_function_min if not self._profile_kwargs['subtract_min'] else 0.0
 
             _parabola_artist = None
             if show_parabolic:
                 _parabola_artist = self._plot_parabolic_cost(_axes,
                                                              _x,
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/tools/ensemble.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/ensemble.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/tools/fit_wrapper.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/fit_wrapper.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/tools/kafe2go.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from kafe2.fit.xy.plot import XYPlotAdapter
 
 
 def kafe2go():
     _parser = argparse.ArgumentParser(
         description="Perform a fit with the kafe2 package driven by an input file.\n"
                     "Example files can be found at "
-                    "https://github.com/dsavoiu/kafe2/tree/master/examples.\n"
+                    "https://github.com/PhiLFitters/kafe2/tree/master/examples.\n"
                     "Further information on how to create input files is given at "
                     "https://kafe2.readthedocs.io/en/latest/parts/user_guide.html#kafe2go."
         )
 
     _parser.add_argument('filename', type=str, nargs='+',
                          help="Name(s) of fit input file(s).")
     _parser.add_argument('-if', '--inputformat',
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/container.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/model.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/unbinned/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/util/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
     """
     Perform Cholesky decomposition of a matrix. Covariance matrices != 0 are always symmetric and
     positive-definite.
     """
     try:
         return np.linalg.cholesky(mat)
     except np.linalg.LinAlgError:
-        warnings.warn(
-            "Singular covariance matrix. Are the errors for some data points equal to zero?")
+        if np.all(np.isfinite(mat)):
+            warnings.warn(
+                "Singular covariance matrix. Are the errors for some data points equal to zero?")
         return None
 
 
 def log_determinant(cholesky_mat):
     """
     Calculate the logarithm of the determinant of a matrix from its Cholesky decomposition.
     """
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/util/function_library.py` & `kafe2-2.8.0rc1/kafe2/fit/util/function_library.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/container.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/ensemble.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/ensemble.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,16 @@
                  dynamic_error_algorithm="nonlinear"):
         """Construct a fit of a model to *xy* data.
 
         :param xy_data: A :py:obj:`~.XYContainer` or a raw 2D array of shape ``(2, N)``
          containing the measurement data.
         :type xy_data: XYContainer or typing.Sequence
         :param model_function: The model function as a native Python function where the first
-            argument denotes the independent *x* variable or an already defined
-            :py:class:`~kafe2.fit.xy.XYModelFunction` object.
+            argument denotes the independent *x* variable. Alternatively an already defined
+            :py:class:`~kafe2.fit.xy.XYModelFunction` object. Defaults to a straight line.
         :type model_function: typing.Callable
         :param cost_function: The cost function this fit uses to find the best parameters.
         :type cost_function: str or typing.Callable
         :param minimizer: The minimizer to use for fitting. Either :py:obj:`None`, ``"iminuit"``,
             ``"tminuit"``, or ``"scipy"``.
         :type minimizer: str or None
         :param minimizer_kwargs: Dictionary with kwargs for the minimizer.
```

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/model.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/fit/xy/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/minimizers/_base.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 import numpy as np
+from scipy.stats import norm
 from scipy.optimize import minimize
 import unittest
 
 
 def fcn_1(x):
     return 42.*(x - 42.)**2 + 42.
 
@@ -480,37 +481,170 @@
         for _minimizer in [self.m1, self.m3]:
             with self.assertRaises(ValueError):
                 _minimizer.set("DEADBEEF", 1)
 
     def test_profile_m3_x(self):
         self.m3.minimize()
         self.assertTrue(np.allclose(
-            self.m3.profile('x', bins=5, subtract_min=True),
+            self.m3.profile('x', size=5, subtract_min=True)[0],
             self._ref_profile_m3_x_5, atol=1e-7
         ))
 
     def test_profile_m3_x_no_subtract_min(self):
         self.m3.minimize()
         self.assertTrue(np.allclose(
-            self.m3.profile('x', bins=5, subtract_min=False),
+            self.m3.profile('x', size=5, subtract_min=False)[0],
             self._ref_profile_m3_x_5_no_subtract_min, atol=1e-7
         ))
 
     def test_profile_m3_x_fix_y(self):
         self.m3.fix("y")
         self.m3.minimize()
         self.assertTrue(np.allclose(
-            self.m3.profile('x', bins=5, subtract_min=True),
+            self.m3.profile('x', size=5, subtract_min=True)[0],
             self._ref_profile_m3_x_5, atol=1e-7
         ))
 
+    def test_profile_m3_x_low(self):
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', low=self._ref_profile_m3_x_5[0, 0], size=5, subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_high(self):
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', high=self._ref_profile_m3_x_5[0, -1], size=5,
+                            subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_low_high(self):
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', low=self._ref_profile_m3_x_5[0, 0],
+                            high=self._ref_profile_m3_x_5[0, -1], size=5, subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_cl(self):
+        _cl = norm.cdf(2) - norm.cdf(-2)
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', cl=_cl, size=5, subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_cl_low(self):
+        _cl = (1 + norm.cdf(2) - norm.cdf(-2)) / 2
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', low=self._ref_profile_m3_x_5[0, 0],
+                            cl=_cl, size=5, subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_cl_high(self):
+        _cl = (1 + norm.cdf(2) - norm.cdf(-2)) / 2
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', low=self._ref_profile_m3_x_5[0, 0],
+                            cl=_cl, size=5, subtract_min=True)[0],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_cl_sigma(self):
+        self.m3.minimize()
+        self.assertTrue(np.allclose(
+            self.m3.profile('x', sigma=3, size=7, subtract_min=True)[0][:, 1:-1],
+            self._ref_profile_m3_x_5, atol=1e-7
+        ))
+
+    def test_profile_m3_x_arrows_cl(self):
+        _cl = [norm.cdf(1) - norm.cdf(-1), norm.cdf(2) - norm.cdf(-2)]
+        self.m3.minimize()
+        _arrow_specs = self.m3.profile('x', cl=_cl, size=5, subtract_min=True, arrows=True)[1]
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 1], _arrow_specs[0]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 1], _arrow_specs[0]['y'])
+        self.assertAlmostEqual((1-_cl[0])/2, _arrow_specs[0]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 0], _arrow_specs[1]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 0], _arrow_specs[1]['y'])
+        self.assertAlmostEqual((1-_cl[1])/2, _arrow_specs[1]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 3], _arrow_specs[2]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 3], _arrow_specs[2]['y'])
+        self.assertAlmostEqual((1-_cl[0])/2, _arrow_specs[2]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 4], _arrow_specs[3]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 4], _arrow_specs[3]['y'])
+        self.assertAlmostEqual((1-_cl[1])/2, _arrow_specs[3]['cl'])
+
+    def test_profile_m3_x_arrows_low_high(self):
+        _cl = [norm.cdf(-1), norm.cdf(-2)]
+        self.m3.minimize()
+        _arrow_specs = self.m3.profile(
+            'x', low=self._ref_profile_m3_x_5[0, :2], high=self._ref_profile_m3_x_5[0, -2:],
+            size=5, subtract_min=True, arrows=True)[1]
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 0], _arrow_specs[0]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 0], _arrow_specs[0]['y'])
+        self.assertAlmostEqual(_cl[1], _arrow_specs[0]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 1], _arrow_specs[1]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 1], _arrow_specs[1]['y'])
+        self.assertAlmostEqual(_cl[0], _arrow_specs[1]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 3], _arrow_specs[2]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 3], _arrow_specs[2]['y'])
+        self.assertAlmostEqual(_cl[0], _arrow_specs[2]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 4], _arrow_specs[3]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 4], _arrow_specs[3]['y'])
+        self.assertAlmostEqual(_cl[1], _arrow_specs[3]['cl'])
+
+    def test_profile_m3_x_arrows_low_cl(self):
+        _cl = [norm.cdf(1), norm.cdf(2)]
+        self.m3.minimize()
+        _arrow_specs = self.m3.profile('x', low=self._ref_profile_m3_x_5[0, :2], cl=_cl, size=5,
+                                       subtract_min=True, arrows=True)[1]
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 0], _arrow_specs[0]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 0], _arrow_specs[0]['y'])
+        self.assertAlmostEqual(1-_cl[1], _arrow_specs[0]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 1], _arrow_specs[1]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 1], _arrow_specs[1]['y'])
+        self.assertAlmostEqual(1-_cl[0], _arrow_specs[1]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 3], _arrow_specs[2]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 3], _arrow_specs[2]['y'])
+        self.assertAlmostEqual(1-_cl[0], _arrow_specs[2]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 4], _arrow_specs[3]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 4], _arrow_specs[3]['y'])
+        self.assertAlmostEqual(1-_cl[1], _arrow_specs[3]['cl'])
+
+    def test_profile_m3_x_arrows_high_cl(self):
+        _cl = [norm.cdf(1), norm.cdf(2)]
+        self.m3.minimize()
+        _arrow_specs = self.m3.profile('x', high=self._ref_profile_m3_x_5[0, -2:], cl=_cl, size=5,
+                                       subtract_min=True, arrows=True)[1]
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 1], _arrow_specs[0]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 1], _arrow_specs[0]['y'])
+        self.assertAlmostEqual(1-_cl[0], _arrow_specs[0]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 0], _arrow_specs[1]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 0], _arrow_specs[1]['y'])
+        self.assertAlmostEqual(1-_cl[1], _arrow_specs[1]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 3], _arrow_specs[2]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 3], _arrow_specs[2]['y'])
+        self.assertAlmostEqual(1-_cl[0], _arrow_specs[2]['cl'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[0, 4], _arrow_specs[3]['x'])
+        self.assertAlmostEqual(self._ref_profile_m3_x_5[1, 4], _arrow_specs[3]['y'])
+        self.assertAlmostEqual(1-_cl[1], _arrow_specs[3]['cl'])
+
     def test_profile_raise_no_fit(self):
         with self.assertRaises(RuntimeError):
             self.m3.profile("x")
 
+    def test_profile_raise_low_high_and_cl(self):
+        self.m3.minimize()
+        with self.assertRaises(ValueError):
+            self.m3.profile("x", low=0, high=4, cl=0.95)
+
     @unittest.skip("Testing contours not yet implemented!")
     def test_contour_m3_x_y(self):
         self.m3.minimize()
         _cont = self.m3.contour('x', 'y', numpoints=5, sigma=1.0)
         self.assertTrue(
             np.allclose(_cont, self._ref_contour_m3_x_y_5, atol=1e-3)
         )
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_iminuit.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_iminuit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_confidence.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_confidence.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_cov_mat.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_cov_mat.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_gaussian_error.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_gaussian_error.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_nexus.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_nexus.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_nexus_fitter.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_nexus_fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
     def test_profile_without_do_fit(self):
         with self.assertRaises(RuntimeError):
             self.fitter.profile('x')
 
     def test_profile(self):
         self.fitter.do_fit()
-        p = self.fitter.profile('x', bins=20, bound=2)
+        p = self.fitter.profile('x', size=20, sigma=2)[0]
         self.assertEqual(
             p.shape,
             (2, 20)
         )
         self.assertAlmostEqual(
             p[0][-1] - p[0][0],
             4 * self.fitter.fit_parameter_errors[0]
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/core/test_parameter_constraints.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_containers_histogram.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_histogram.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_containers_indexed.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_indexed.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_containers_xy.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_xy.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_cost_functions.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_cost_functions.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_ensemble_tools.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_ensemble_tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_custom.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_custom.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_hist.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                                       11.59865691,  13.41486068,  14.25999508,  10.70887047,
                                        4.08280244,  13.1043861 ,  14.62321312,  14.85894591,
                                       14.89235398,  10.60967181,  15.22310211,  10.77853626,
                                       14.56823312,  14.46093346,  13.34031129,  14.14203599])
 
         self._ref_hist_cont = HistContainer(
             self._ref_n_bins, self._ref_n_bin_range, bin_edges=None, fill_data=self._ref_entries)
+        self._ref_hist_numpy = np.histogram(
+            self._ref_entries, bins=self._ref_n_bins, range=self._ref_n_bin_range)
 
 
         # reference initial values
         self._ref_initial_pars = np.array([14., 3.])
         self._ref_initial_model = (
             hist_model_density_antideriv(self._ref_bin_edges[1:], *self._ref_initial_pars) -
             hist_model_density_antideriv(self._ref_bin_edges[:-1], *self._ref_initial_pars)) * len(self._ref_entries)
@@ -107,43 +109,44 @@
             parameter_values=self._ref_initial_pars,
             parameter_names=('mu', 'sigma'),
 
             data=self._ref_data,
             model=self._ref_initial_model,
         )
 
-    def _get_fit(self, model_density_function=None, bin_evaluation="numerical", cost_function=None):
+    def _get_fit(self, model_density_function=None, bin_evaluation="numerical", cost_function=None,
+                 numpy_histogram=False):
         '''convenience'''
 
         model_density_function = model_density_function or hist_model_density
 
         # TODO: fix default
         cost_function = cost_function or HistCostFunction_NegLogLikelihood(
             data_point_distribution='poisson')
 
         _fit = HistFit(
-            data=self._ref_hist_cont,
+            data=self._ref_hist_numpy if numpy_histogram else self._ref_hist_cont,
             model_function=model_density_function,
             bin_evaluation=bin_evaluation,
             cost_function=cost_function,
             minimizer=self.MINIMIZER
         )
         _fit.add_error(1.0)  # only considered for chi2
 
         return _fit
 
     def _get_test_fits(self):
         return {
             # numeric integration takes too long for testing
             #'default': \
             #    self._get_fit(),
-            'explicit_chi2': \
-                self._get_fit(cost_function=simple_chi2, bin_evaluation=hist_model_density_antideriv),
-            'model_with_antiderivative': \
-                self._get_fit(bin_evaluation=hist_model_density_antideriv),
+            'explicit_chi2': self._get_fit(
+                cost_function=simple_chi2, bin_evaluation=hist_model_density_antideriv),
+            'model_with_antiderivative': self._get_fit(bin_evaluation=hist_model_density_antideriv),
+            'numpy_histogram': self._get_fit(numpy_histogram=True)
         }
 
     def test_initial_state(self):
         self.run_test_for_all_fits(
             dict(
                 self._ref_prop_dict,
                 cost_function_value=np.float64(self._ref_initial_cost_nll),  # TODO: fix type
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_indexed.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_indexed.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_multi.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_multi.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_unbinned.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_unbinned.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fit_xy.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_xy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import numpy as np
 import six
 
 from kafe2.core.minimizers import AVAILABLE_MINIMIZERS
 
 from kafe2.config import kc
 
-from kafe2.fit import XYFit
+from kafe2.fit.xy.container import XYContainer
+from kafe2.fit.xy.fit import XYFit
 from kafe2.fit.xy.cost import XYCostFunction_Chi2
 
 from kafe2.test.fit.test_fit import AbstractTestFit
 
 
 def simple_chi2(y_data, y_model):
     return np.sum((y_data - y_model)**2)
@@ -605,14 +606,38 @@
 
     def test_get_matching_error_reference_model(self):
         _fit = self._get_test_fits()['named_errors']
         _errs = _fit.get_matching_errors(matching_criteria=dict(reference='model'))
         self.assertEqual(len(_errs), 1)
         self.assertIs(_fit._param_model._error_dicts['MyYModelError']['err'], _errs['MyYModelError'])
 
+    def test_fit_with_no_errors(self):
+        _fit_with_unity_errors = XYFit(
+            xy_data=self._ref_xy_data,
+            model_function=simple_xy_model,
+            minimizer=self.MINIMIZER
+        )
+        _fit_with_unity_errors.add_error("y", 1.0)
+        _fit_with_no_errors_1 = XYFit(
+            xy_data=self._ref_xy_data,
+            model_function=simple_xy_model,
+            minimizer=self.MINIMIZER
+        )
+        _fit_with_no_errors_2 = XYFit(
+            xy_data=XYContainer(self._ref_xy_data[0], self._ref_xy_data[1]),
+            model_function=simple_xy_model,
+            minimizer=self.MINIMIZER
+        )
+
+        _fit_with_unity_errors.do_fit()
+        _fit_with_no_errors_1.do_fit()
+        _fit_with_no_errors_2.do_fit()
+        self._assert_fit_results_equal(_fit_with_unity_errors, _fit_with_no_errors_1)
+        self._assert_fit_results_equal(_fit_with_unity_errors, _fit_with_no_errors_2)
+
 
 class TestXYFitWithMatrixErrors(AbstractTestFit, unittest.TestCase):
 
     MINIMIZER = 'scipy'
 
     def setUp(self):
         six.get_unbound_function(TestXYFitBasicInterface.setUp)(self)
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_model_functions.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_model_functions.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_plot.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 import sys
 import numpy as np
 import os
+import matplotlib.pyplot as plt
 from kafe2 import XYFit, Plot
 
 
 class TestXYPlot(unittest.TestCase):
     def setUp(self):
         self._ref_data = [[1, 2, 3], [0.9, 2.1, 3.0]]
         self._ref_dataset_label = 'My Dataset'
@@ -20,21 +21,26 @@
 
         self.fit.data_container.label = self._ref_dataset_label
         self.fit.data_container.axis_labels = (self._ref_x_label, self._ref_y_label)
         self.fit.model_label = self._ref_model_label
 
         self.plot = Plot(self.fit)
 
+    def tearDown(self):
+        plt.close("all")
+
     def test_warning_no_fit_performed(self):
         _fit = XYFit(xy_data=self._ref_data)
-        _fit.add_error('y', 0.1)
+        _fit.add_error("y", 0.1)
         _plot = Plot(fit_objects=_fit)
-        with self.assertWarns(Warning) as w:
-            _plot.plot()
-        self.assertIn("Did you forget to run fit.do_fit()?", str(w.warning))
+        self.assertWarnsRegex(
+            UserWarning,
+            "Did you forget to run fit.do_fit()?",
+            _plot.plot,
+        )
 
     def test_plot_with_asymmetric_errors(self):
         self.plot.plot(asymmetric_parameter_errors=True)
 
     def test_labels_after_plotting(self):
         self.plot.plot()
         self.assertEqual(self.plot.axes[0]['main'].get_xlabel(), self._ref_x_label)
@@ -162,14 +168,17 @@
         self.fit1.do_fit()
         self.fit2.add_error('y', 0.1)
         self.fit2.do_fit()
 
         self.plot = Plot([self.fit1, self.fit2])
         self.plot_sep = Plot([self.fit1, self.fit2], separate_figures=True)
 
+    def tearDown(self):
+        plt.close("all")
+
     def test_label_setter_str(self):
         x_label, y_label = "123x", "Y_test"
         for _p in (self.plot, self.plot_sep):
             _p.x_label = x_label
             _p.y_label = y_label
             _p.plot()
         self.assertEqual(self.plot.axes[0]['main'].get_xlabel(), x_label)
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_container_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_container_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_fit_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_fit_yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,15 +1075,15 @@
                            0.9477286127925121, 0.08899785814182719]
         self._test_parameters = np.array([0.1, -1.0])
         self._test_parameters_default = np.array([0.1, 1.0])
         self._test_parameters_default_simple = np.array([1.0, 1.0])
         self._test_parameters_do_fit = np.array([0.1, 1.09727982])
         self._test_parameters_do_fit_simple = np.array([-0.07060323, 1.02375445])
 
-        self._fit = UnbinnedFit(data=self._test_data, model_density_function='normal_distribution_pdf')
+        self._fit = UnbinnedFit(data=self._test_data, model_function='normal_distribution_pdf')
         self._fit.fix_parameter('mu', 0.1)
 
         self.setup_streams()
 
     def test_read_from_testfile_stream(self):
         _read_fit = self._testfile_streamreader.read()
         self.assertTrue(isinstance(_read_fit, self.FIT_CLASS))
```

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_format_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_format_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/test/tools.py` & `kafe2-2.8.0rc1/kafe2/test/tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2/tools.py` & `kafe2-2.8.0rc1/kafe2/tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.7.0rc1/kafe2.egg-info/PKG-INFO` & `kafe2-2.8.0rc1/kafe2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kafe2
-Version: 2.7.0rc1
+Version: 2.8.0rc1
 Summary: Karlsruhe Fit Environment 2: a package for fitting and elementary data analysis
-Home-page: http://github.com/dsavoiu/kafe2
+Home-page: https://github.com/PhiLFitters/kafe2
 Author: Daniel Savoiu
 Author-email: daniel.savoiu@cern.ch
 License: GPL3
 Keywords: kafe2 kit karlsruhe data analysis lab laboratory practical courses education university students physics fitting minimization minimisation regression parametric parameter estimation optimization optimisation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -31,43 +31,39 @@
 .. image:: https://badge.fury.io/py/kafe2.svg
     :target: https://badge.fury.io/py/kafe2
 
 .. image:: https://readthedocs.org/projects/kafe2/badge/?version=latest
     :target: https://kafe2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://travis-ci.org/dsavoiu/kafe2.svg?branch=master
-    :target: https://travis-ci.org/dsavoiu/kafe2
 
-
-*kafe2* is an open-source Python package designed to provide a flexible
-Python interface for the estimation of model parameters from measured
-data. It is the spiritual successor to the original *kafe* package.
-
-*kafe2* offers support for several types of data formats (including series
-of indexed measurements, xy value pairs, and histograms) and data
-uncertainty models, as well as arbitrarily complex parametric
-models. The numeric aspects are handled using the scientific Python
-stack (NumPy, SciPy, ...). Visualization of the data and the estimated
-model are provided by matplotlib.
+*kafe2* is an open-source Python package for the likelihood-based estimation of model parameters
+from measured data.
+As the spiritual successor to the original *kafe* package it aims to provide
+state-of-the-art statistical methods in a way that is still easy to use.
+More information `here <https://philfitters.github.io/kafe2/>`__.
 
 If you have installed pip just run
 
 .. code-block:: bash
 
     pip install kafe2
 
-to install the latest stable version and you're ready to go.
+to install the latest stable version and you're (mostly) ready to go.
+The Python package *iminuit* which *kafe2* uses internally for numerical optimization
+`may fail to be installed automatically if no C++ compiler is available on your system
+<https://iminuit.readthedocs.io/en/stable/install.html>`__ .
+While *iminuit* is strictly speaking not required its use is heavily recommended.
+**Make sure to read the pip installation log.**
 As of *kafe2* v2.4.0 only Python 3 is supported.
 
-The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`_
+The documentation under `kafe2.readthedocs.io <https://kafe2.readthedocs.io/>`__
 has more detailed installation instructions.
-It also explains basic *kafe2* features as well as the mathematical foundations
-upon which *kafe2* is built.
+It also explains *kafe2* usage as well as the mathematical foundations upon which *kafe2* is built.
 
 If you prefer a more practical approach you can instead look at the various
-`examples <https://github.com/dsavoiu/kafe2/tree/master/examples>`_.
+`examples <https://github.com/PhiLFitters/kafe2/tree/master/examples>`__.
 In addition to the regular Python/kafe2go files there are also Jupyter notebook
 tutorials (in English and in German) that mostly cover the same topics.
 
 If you encounter any bugs or have an improvement proposal, please let us
-know by opening an issue `here <https://github.com/dsavoiu/kafe2/issues>`_.
+know by opening an issue `here <https://github.com/PhiLFitters/kafe2/issues>`__.
```

### Comparing `kafe2-2.7.0rc1/kafe2.egg-info/SOURCES.txt` & `kafe2-2.8.0rc1/kafe2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -131,8 +131,9 @@
 kafe2/test/fit/test_model_functions.py
 kafe2/test/fit/test_plot.py
 kafe2/test/fit/test_representers_constraint_yaml.py
 kafe2/test/fit/test_representers_container_yaml.py
 kafe2/test/fit/test_representers_fit_yaml.py
 kafe2/test/fit/test_representers_format_yaml.py
 kafe2/test/fit/test_representers_model_function_yaml.py
-kafe2/test/fit/test_representers_parametric_model_yaml.py
+kafe2/test/fit/test_representers_parametric_model_yaml.py
+kafe2/test/fit/test_wrappers.py
```

### Comparing `kafe2-2.7.0rc1/setup.py` & `kafe2-2.8.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name='kafe2',
     version=get_version(),
     description='Karlsruhe Fit Environment 2: a package for fitting and elementary data analysis',
     long_description=read_local('README.rst'),
     long_description_content_type="text/x-rst",
     author='Daniel Savoiu',
     author_email='daniel.savoiu@cern.ch',
-    url='http://github.com/dsavoiu/kafe2',
+    url='https://github.com/PhiLFitters/kafe2',
     packages=find_packages(),
     package_data={'kafe2': ['config/*.conf', 'config/*.yaml', 'config/*.yml', 'fit/tools/kafe2go']},
     scripts=['kafe2/fit/tools/kafe2go.py', 'kafe2/fit/tools/kafe2go'],
     test_suite='setup.discover_kafe_tests',
     keywords=("kafe2 kit karlsruhe data analysis lab laboratory practical courses "
               "education university students physics fitting minimization minimisation "
               "regression parametric parameter estimation optimization optimisation"),
```

