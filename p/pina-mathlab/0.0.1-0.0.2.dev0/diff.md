# Comparing `tmp/pina-mathlab-0.0.1.tar.gz` & `tmp/pina-mathlab-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pina-mathlab-0.0.1.tar", last modified: Thu Mar 17 15:52:55 2022, max compression
+gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-idoflel_/pina-mathlab-0.0.2.dev0.tar", last modified: Wed Apr 19 08:09:22 2023, max compression
```

## Comparing `pina-mathlab-0.0.1.tar` & `pina-mathlab-0.0.2.dev0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/
--rw-r--r--   0 ndemo     (6157) ma         (700)     2036 2021-11-29 14:28:07.000000 pina-mathlab-0.0.1/.gitignore
--rw-r--r--   0 ndemo     (6157) ma         (700)     1089 2021-11-29 16:04:30.000000 pina-mathlab-0.0.1/LICENSE.rst
--rw-r--r--   0 ndemo     (6157) ma         (700)      776 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/PKG-INFO
--rw-r--r--   0 ndemo     (6157) ma         (700)    10407 2022-02-17 11:20:29.000000 pina-mathlab-0.0.1/README.md
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/examples/
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/examples/problems/
--rw-r--r--   0 ndemo     (6157) ma         (700)     1247 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/problems/burgers.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1982 2021-11-29 16:18:22.000000 pina-mathlab-0.0.1/examples/problems/elliptic_optimal_control.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     2251 2021-11-29 16:18:22.000000 pina-mathlab-0.0.1/examples/problems/parametric_elliptic_optimal_control.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     2250 2021-11-29 16:18:22.000000 pina-mathlab-0.0.1/examples/problems/parametric_elliptic_optimal_control_alpha_variable.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1411 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/problems/parametric_poisson.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1136 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/problems/poisson.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1702 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/run_burgers.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     7341 2021-07-15 08:34:25.000000 pina-mathlab-0.0.1/examples/run_parametric_elliptic_optimal_control_alpha.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1575 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/run_parametric_poisson.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1982 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/examples/run_poisson.py
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina/
--rw-r--r--   0 ndemo     (6157) ma         (700)      292 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/__init__.py
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina/adaptive_functions/
--rw-r--r--   0 ndemo     (6157) ma         (700)      205 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/__init__.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1656 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_cos.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1581 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_exp.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1277 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_linear.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1300 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_relu.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1584 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_sin.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1189 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_softplus.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1294 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_square.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1768 2021-11-29 14:22:17.000000 pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_tanh.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      234 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/chebyshev.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1053 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/condition.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1407 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/label_tensor.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      147 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/location.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      494 2022-03-17 15:50:25.000000 pina-mathlab-0.0.1/pina/meta.py
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina/model/
--rw-r--r--   0 ndemo     (6157) ma         (700)      144 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/model/__init__.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     2120 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/model/feed_forward.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      375 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/model/multi_feed_forward.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     1094 2022-01-27 10:51:47.000000 pina-mathlab-0.0.1/pina/operators.py
--rw-r--r--   0 ndemo     (6157) ma         (700)    18166 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/pinn.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     4539 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/plotter.py
--rw-r--r--   0 ndemo     (6157) ma         (700)    14373 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/ppinn.py
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina/problem/
--rw-r--r--   0 ndemo     (6157) ma         (700)      303 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/problem/__init__.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      803 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/problem/abstract_problem.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      196 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/problem/parametric_problem.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      186 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/problem/spatial_problem.py
--rw-r--r--   0 ndemo     (6157) ma         (700)      206 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/problem/timedep_problem.py
--rw-r--r--   0 ndemo     (6157) ma         (700)     2199 2022-02-17 09:00:13.000000 pina-mathlab-0.0.1/pina/span.py
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/
--rw-r--r--   0 ndemo     (6157) ma         (700)      776 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/PKG-INFO
--rw-r--r--   0 ndemo     (6157) ma         (700)     1507 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/SOURCES.txt
--rw-r--r--   0 ndemo     (6157) ma         (700)        1 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/dependency_links.txt
--rw-r--r--   0 ndemo     (6157) ma         (700)        1 2022-03-17 15:52:24.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/not-zip-safe
--rw-r--r--   0 ndemo     (6157) ma         (700)       88 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/requires.txt
--rw-r--r--   0 ndemo     (6157) ma         (700)        5 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/pina_mathlab.egg-info/top_level.txt
-drwxr-xr-x   0 ndemo     (6157) ma         (700)        0 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/readme/
--rw-r--r--   0 ndemo     (6157) ma         (700)    44885 2022-02-17 11:17:49.000000 pina-mathlab-0.0.1/readme/poisson_plot.png
--rw-r--r--   0 ndemo     (6157) ma         (700)    26673 2022-02-17 11:16:38.000000 pina-mathlab-0.0.1/readme/poisson_problem.png
--rw-r--r--   0 ndemo     (6157) ma         (700)       38 2022-03-17 15:52:55.000000 pina-mathlab-0.0.1/setup.cfg
--rw-r--r--   0 ndemo     (6157) ma         (700)     1389 2022-03-17 15:52:21.000000 pina-mathlab-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/feed_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/convolution_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/stride.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/layers/utils_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/multi_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/model/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/parametric_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/spatial_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/problem/timedep_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/pina/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/pina_mathlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:09:22.000000 pina-mathlab-0.0.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_fnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 08:09:04.000000 pina-mathlab-0.0.2.dev0/tests/test_utils.py
```

### Comparing `pina-mathlab-0.0.1/LICENSE.rst` & `pina-mathlab-0.0.2.dev0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/README.md` & `pina-mathlab-0.0.2.dev0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,44 @@
-<!-- <p align="center"> -->
-<!--   <a href="http://mathlab.github.io/PyDMD/" target="_blank" > -->
-<!--     <img alt="Python Dynamic Mode Decomposition" src="readme/logo_PyDMD.png" width="200" /> -->
-<!--   </a> -->
-<!-- </p> -->
-<!-- <p align="center"> -->
-<!--     <a href="https://doi.org/10.21105/joss.00530" target="_blank"> -->
-<!--         <img alt="JOSS DOI" src="http://joss.theoj.org/papers/10.21105/joss.00530/status.svg"> -->
-<!--     </a> -->
-<!--     <a href="https://github.com/mathLab/PyDMD/blob/master/LICENSE" target="_blank"> -->
-<!--         <img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square"> -->
-<!--     </a> -->
-<!--     <a href="https://badge.fury.io/py/pydmd"  target="_blank"> -->
-<!--         <img alt="PyPI version" src="https://badge.fury.io/py/pydmd.svg"> -->
-<!--     </a> -->
-<!--     <a href="https://travis-ci.org/mathLab/PyDMD" target="_blank"> -->
-<!--         <img alt="Build Status" src="https://travis-ci.org/mathLab/PyDMD.svg"> -->
-<!--     </a> -->
-<!--     <a href="https://www.codacy.com/gh/mathLab/PyDMD/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PyDMD&amp;utm_campaign=Badge_Coverage"> -->
-<!--       <img src="https://app.codacy.com/project/badge/Coverage/c36adbea2e4a44eb8c0e4505b75e8245"/> -->
-<!--     </a> -->
-<!--     <a href="https://www.codacy.com/gh/mathLab/PyDMD/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PyDMD&amp;utm_campaign=Badge_Grade"> -->
-<!--       <img src="https://app.codacy.com/project/badge/Grade/c36adbea2e4a44eb8c0e4505b75e8245"/> -->
-<!--     </a> -->
-<!-- </p> -->
+<p align="center">
+    <a href="http://mathlab.github.io/PINA/" target="_blank" >
+    <img alt="Physics-Informed Neural networks for Advanced modeling" src="readme/pina_logo.png" width="200" />
+    </a>
+</p>
+<p align="center">
+    <a href="https://github.com/mathLab/PINA/blob/master/LICENSE" target="_blank">
+        <img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square">
+    </a>
+    <a href="https://badge.fury.io/py/pina-mathlab">
+	<img src="https://badge.fury.io/py/pina-mathlab.svg" alt="PyPI version" height="18">
+    </a>
+    <a href="https://github.com/mathLab/PINA/actions/workflows/ci.yml" target="_blank">
+        <img alt="Build Status" src="https://github.com/mathLab/PINA/actions/workflows/ci.yml/badge.svg">
+    </a>
+    <a href="https://www.codacy.com/gh/mathLab/PINA/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PINA&amp;utm_campaign=Badge_Grade">
+	<img src="https://app.codacy.com/project/badge/Grade/1ed0b0279cbe44cc8207575fe6e55f91"/>
+    </a>
+    <a href="https://www.codacy.com/gh/mathLab/PINA/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PINA&amp;utm_campaign=Badge_Coverage">
+	<img src="https://app.codacy.com/project/badge/Coverage/1ed0b0279cbe44cc8207575fe6e55f91"/>
+    </a>
+</p>
 
 
-**PINA**: Physics-Informed Neural networks for Advance modeling
+**PINA**: Physics-Informed Neural networks for Advanced modeling
 
 ## Table of contents
 * [Description](#description)
      * [Problem definition](#problem-definition)
      * [Problem solution](#problem-solution)
 * [Dependencies and installation](#dependencies-and-installation)
 	* [Installing via PIP](#installing-via-pip)
 	* [Installing from source](#installing-from-source)
 <!-- * [Documentation](#documentation) -->
 <!-- * [Testing](#testing) -->
 * [Examples and Tutorials](#examples-and-tutorials)
-<!-- * [Awards](#awards) -->
-* [How to cite](#how-to-cite)
-	* [References](#references)
+* [References](#references)
 	<!-- * [Recent works with PyDMD](#recent-works-with-pydmd) -->
 * [Authors and contributors](#authors-and-contributors)
 * [How to contribute](#how-to-contribute)
 	* [Submitting a patch](#submitting-a-patch)
 * [License](#license)
 
 ## Description
@@ -51,44 +46,46 @@
 
 #### Physics-informed neural network
 PINN is a novel approach that involves neural networks to solve supervised learning tasks while respecting any given law of physics described by general nonlinear differential equations. Proposed in *"Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations"*, such framework aims to solve problems in a continuous and nonlinear settings.
 
 #### Problem definition
 First step is formalization of the problem in the PINA framework. We take as example here a simple Poisson problem, but PINA is already able to deal with **multi-dimensional**, **parametric**, **time-dependent** problems.
 Consider:
-<p align="center">
-  <img alt="Poisson approximation" src="readme/poisson_problem.png" width="80%" />
-</p>
-where *D* is a square domain, *Gamma*s are the boundaries and *u* the unknown field. The translation in PINA code becomes a new class containing all the information about the domain, about the `conditions` and nothing more:
+
+$$\begin{cases} \Delta u = \sin(\pi x)\sin(\pi y)\quad& \text{in} \\ D \\\\ u = 0& \text{on} \\ \partial D \end{cases}$$
+
+where $D = [0, 1]^2$ is a square domain, $u$ the unknown field, and $\partial D  = \Gamma_1 \cup \Gamma_2 \cup \Gamma_3 \cup \Gamma_4$, where $\Gamma_i$ are the boundaries of the square for $i=1,\cdots,4$. The translation in PINA code becomes a new class containing all the information about the domain, about the `conditions` and nothing more:
+
 ```python
 class Poisson(SpatialProblem):
-	spatial_variables = ['x', 'y']
-	output_variables = ['u']
-	domain = Span({'x': [0, 1], 'y': [0, 1]})
-
-	def laplace_equation(input_, output_):
-		force_term = (torch.sin(input_['x']*torch.pi) *
-		              torch.sin(input_['y']*torch.pi))
-		return nabla(output_['u'], input_).flatten() - force_term
-
-	def nil_dirichlet(input_, output_):
-		value = 0.0
-		return output_['u'] - value
-
-	conditions = {
-		'gamma1': Condition(Span({'x': [-1, 1], 'y':  1}), nil_dirichlet),
-		'gamma2': Condition(Span({'x': [-1, 1], 'y': -1}), nil_dirichlet),
-		'gamma3': Condition(Span({'x':  1, 'y': [-1, 1]}), nil_dirichlet),
-		'gamma4': Condition(Span({'x': -1, 'y': [-1, 1]}), nil_dirichlet),
-		'D': Condition(Span({'x': [-1, 1], 'y': [-1, 1]}), laplace_equation),
-	}
+    output_variables = ['u']
+    spatial_domain = Span({'x': [0, 1], 'y': [0, 1]})
+
+    def laplace_equation(input_, output_):
+        force_term = (torch.sin(input_.extract(['x'])*torch.pi) *
+                      torch.sin(input_.extract(['y'])*torch.pi))
+        nabla_u = nabla(output_.extract(['u']), input_)
+        return nabla_u - force_term
+
+    def nil_dirichlet(input_, output_):
+      	value = 0.0
+      	return output_.extract(['u']) - value
+
+    conditions = {
+        'gamma1': Condition(Span({'x': [-1, 1], 'y':  1}), nil_dirichlet),
+        'gamma2': Condition(Span({'x': [-1, 1], 'y': -1}), nil_dirichlet),
+        'gamma3': Condition(Span({'x':  1, 'y': [-1, 1]}), nil_dirichlet),
+        'gamma4': Condition(Span({'x': -1, 'y': [-1, 1]}), nil_dirichlet),
+        'D': Condition(Span({'x': [-1, 1], 'y': [-1, 1]}), laplace_equation),
+    }
 ```
 
 #### Problem solution
 After defining it, we want of course to solve such a problem. The only things we need is a `model`, in this case a feed forward network, and some samples of the domain and boundaries, here using a Cartesian grid. In these points we are going to evaluate the residuals, which is nothing but the loss of the network.
+
 ```python
 poisson_problem = Poisson()
 
 model = FeedForward(layers=[10, 10],
                     output_variables=poisson_problem.output_variables,
                     input_variables=poisson_problem.input_variables)
 
@@ -96,22 +93,22 @@
 pinn.span_pts(20, 'grid', ['D'])
 pinn.span_pts(20, 'grid', ['gamma1', 'gamma2', 'gamma3', 'gamma4'])
 pinn.train(1000, 100)
 
 plotter = Plotter()
 plotter.plot(pinn)
 ```
-After the training we can infer our model, save it or just plot the PINN approximation.
+After the training we can infer our model, save it or just plot the PINN approximation. Below the graphical representation of the PINN approximation, the analytical solution of the problem and the absolute error, from left to right.
 <p align="center">
-  <img alt="Poisson approximation" src="readme/poisson_plot.png" width="80%" />
+  <img alt="Poisson approximation" src="readme/poisson_plot.png" width="100%" />
 </p>
 
 
 ## Dependencies and installation
-**PINA** requires requires `numpy`, `scipy`, `matplotlib`, `future`, `torch`, `sphinx` (for the documentation) and `pytest` (for local test). The code is tested for Python 3, while compatibility of Python 2 is not guaranteed anymore. It can be installed using `pip` or directly from the source code.
+**PINA** requires `numpy`, `scipy`, `matplotlib`, `future`, `torch`, `sphinx` (for the documentation) and `pytest` (for local test). The code is tested for Python 3, while compatibility of Python 2 is not guaranteed anymore. It can be installed using `pip` or directly from the source code.
 
 ### Installing via PIP
 Mac and Linux users can install pre-built binary packages using pip.
 To install the package just type:
 ```bash
 > pip install git+https://github.com/mathLab/PINA.git
 ```
@@ -168,15 +165,15 @@
 **PINA** is currently developed and mantained at [SISSA mathLab](http://mathlab.sissa.it/) by
 * [Nicola Demo](mailto:demo.nicola@gmail.com)
 * [Maria Strazzullo](mailto:mstrazzu@gmail.com)
 
 
 under the supervision of [Prof. Gianluigi Rozza](mailto:gianluigi.rozza@sissa.it).
 
-Contact us by email for further information or questions about **PyDMD**, or suggest pull requests. Contributions improving either the code or the documentation are welcome!
+Contact us by email for further information or questions about **PINA**, or suggest pull requests. Contributions improving either the code or the documentation are welcome!
 
 
 ## How to contribute
 We'd love to accept your patches and contributions to this project. There are just a few small guidelines you need to follow.
 
 ### Submitting a patch
```

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_cos.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_cos.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_exp.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_exp.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_linear.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_linear.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_relu.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_relu.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_sin.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_sin.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_softplus.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_softplus.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_square.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_square.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/pina/adaptive_functions/adaptive_tanh.py` & `pina-mathlab-0.0.2.dev0/pina/adaptive_functions/adaptive_tanh.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.1/setup.py` & `pina-mathlab-0.0.2.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 EXTRAS = {
     'docs': ['sphinx', 'sphinx_rtd_theme'],
     'test': ['pytest', 'pytest-cov'],
 }
 
 LDESCRIPTION = (
-    ""
+    "PINA is a Python package providing an easy interface to deal with "
+    "physics-informed neural networks (PINN) for the approximation of "
+    "(differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a "
+    "simple and intuitive way to formalize a specific problem and solve it "
+    "using PINN."
 )
 
 setup(
     name=PIPNAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LDESCRIPTION,
```

