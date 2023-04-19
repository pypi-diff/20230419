# Comparing `tmp/gEconpy-1.2.0.tar.gz` & `tmp/gEconpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gEconpy-1.2.0.tar", last modified: Tue Apr 18 22:38:24 2023, max compression
+gzip compressed data, was "gEconpy-1.2.1.tar", last modified: Wed Apr 19 00:46:03 2023, max compression
```

## Comparing `gEconpy-1.2.0.tar` & `gEconpy-1.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.634982 gEconpy-1.2.0/
--rw-rw-rw-   0        0        0    35823 2023-02-22 12:40:07.000000 gEconpy-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    14070 2023-04-18 22:38:24.634982 gEconpy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    13759 2023-02-22 12:40:07.000000 gEconpy-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.560983 gEconpy-1.2.0/gEconpy/
--rw-rw-rw-   0        0        0      498 2023-04-18 22:37:10.000000 gEconpy-1.2.0/gEconpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.586982 gEconpy-1.2.0/gEconpy/classes/
--rw-rw-rw-   0        0        0       74 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/classes/__init__.py
--rw-rw-rw-   0        0        0    28710 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/classes/block.py
--rw-rw-rw-   0        0        0     6144 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/classes/containers.py
--rw-rw-rw-   0        0        0    66226 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/classes/model.py
--rw-rw-rw-   0        0        0     3472 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/classes/progress_bar.py
--rw-rw-rw-   0        0        0     2523 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/classes/time_aware_symbol.py
--rw-rw-rw-   0        0        0     1856 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/classes/transformers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.591982 gEconpy-1.2.0/gEconpy/estimation/
--rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/estimation/__init__.py
--rw-rw-rw-   0        0        0     9085 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/estimation/estimate.py
--rw-rw-rw-   0        0        0    11831 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/estimation/estimation_utilities.py
--rw-rw-rw-   0        0        0     8557 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/estimation/kalman_filter.py
--rw-rw-rw-   0        0        0     1386 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/estimation/kalman_smoother.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.593982 gEconpy-1.2.0/gEconpy/exceptions/
--rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/exceptions/__init__.py
--rw-rw-rw-   0        0        0    11729 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.597983 gEconpy-1.2.0/gEconpy/numba_tools/
--rw-rw-rw-   0        0        0     8396 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/numba_tools/LAPACK.py
--rw-rw-rw-   0        0        0        0 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/numba_tools/__init__.py
--rw-rw-rw-   0        0        0     1836 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/numba_tools/intrinsics.py
--rw-rw-rw-   0        0        0    24886 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/numba_tools/overloads.py
--rw-rw-rw-   0        0        0     9132 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/numba_tools/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.603982 gEconpy-1.2.0/gEconpy/parser/
--rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/__init__.py
--rw-rw-rw-   0        0        0     1617 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/constants.py
--rw-rw-rw-   0        0        0      370 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/file_loaders.py
--rw-rw-rw-   0        0        0    11985 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/gEcon_parser.py
--rw-rw-rw-   0        0        0    55526 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/parse_distributions.py
--rw-rw-rw-   0        0        0    13526 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/parser/parse_equations.py
--rw-rw-rw-   0        0        0     8288 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/parse_plaintext.py
--rw-rw-rw-   0        0        0     4264 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/parser/validation.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.605982 gEconpy-1.2.0/gEconpy/plotting/
--rw-rw-rw-   0        0        0      492 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/plotting/__init__.py
--rw-rw-rw-   0        0        0    31786 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/plotting/plotting.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.607982 gEconpy-1.2.0/gEconpy/sampling/
--rw-rw-rw-   0        0        0      490 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/sampling/__init__.py
--rw-rw-rw-   0        0        0     6643 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/sampling/posterior_utilities.py
--rw-rw-rw-   0        0        0     9249 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/sampling/prior_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.611982 gEconpy-1.2.0/gEconpy/shared/
--rw-rw-rw-   0        0        0      127 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/shared/__init__.py
--rw-rw-rw-   0        0        0    11458 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/shared/dynare_convert.py
--rw-rw-rw-   0        0        0    30597 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/shared/statsmodel_convert.py
--rw-rw-rw-   0        0        0      168 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/shared/typing.py
--rw-rw-rw-   0        0        0    10340 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/shared/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.614982 gEconpy-1.2.0/gEconpy/solvers/
--rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/solvers/__init__.py
--rw-rw-rw-   0        0        0     5114 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/solvers/cycle_reduction.py
--rw-rw-rw-   0        0        0    13757 2023-02-22 12:40:07.000000 gEconpy-1.2.0/gEconpy/solvers/gensys.py
--rw-rw-rw-   0        0        0    11313 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/solvers/perturbation.py
--rw-rw-rw-   0        0        0    60257 2023-04-18 22:20:22.000000 gEconpy-1.2.0/gEconpy/solvers/steady_state.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.579981 gEconpy-1.2.0/gEconpy.egg-info/
--rw-rw-rw-   0        0        0    14070 2023-04-18 22:38:24.000000 gEconpy-1.2.0/gEconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2023-04-18 22:38:24.000000 gEconpy-1.2.0/gEconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:38:24.000000 gEconpy-1.2.0/gEconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-18 22:38:24.000000 gEconpy-1.2.0/gEconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 22:38:24.000000 gEconpy-1.2.0/gEconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      579 2023-04-18 22:37:10.000000 gEconpy-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      549 2023-04-18 22:38:24.636982 gEconpy-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-22 12:40:07.000000 gEconpy-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:38:24.633981 gEconpy-1.2.0/tests/
--rw-rw-rw-   0        0        0    10623 2023-04-18 22:20:22.000000 gEconpy-1.2.0/tests/test_block.py
--rw-rw-rw-   0        0        0     3639 2023-04-18 22:20:22.000000 gEconpy-1.2.0/tests/test_containers.py
--rw-rw-rw-   0        0        0     8818 2023-02-22 12:40:07.000000 gEconpy-1.2.0/tests/test_distribution_parser.py
--rw-rw-rw-   0        0        0     1800 2023-02-22 12:40:07.000000 gEconpy-1.2.0/tests/test_estimation.py
--rw-rw-rw-   0        0        0    19212 2023-02-22 12:40:07.000000 gEconpy-1.2.0/tests/test_gensys.py
--rw-rw-rw-   0        0        0     6594 2023-04-18 22:20:22.000000 gEconpy-1.2.0/tests/test_kalman_filter.py
--rw-rw-rw-   0        0        0    26905 2023-04-18 22:20:22.000000 gEconpy-1.2.0/tests/test_model.py
--rw-rw-rw-   0        0        0    21844 2023-04-18 22:20:22.000000 gEconpy-1.2.0/tests/test_parser.py
--rw-rw-rw-   0        0        0    14712 2023-02-22 12:40:07.000000 gEconpy-1.2.0/tests/test_steady_state.py
--rw-rw-rw-   0        0        0     2379 2023-02-22 12:40:07.000000 gEconpy-1.2.0/tests/test_time_aware_symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.995937 gEconpy-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-02-22 12:40:07.000000 gEconpy-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    14070 2023-04-19 00:46:02.995937 gEconpy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13759 2023-02-22 12:40:07.000000 gEconpy-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.931932 gEconpy-1.2.1/gEconpy/
+-rw-rw-rw-   0        0        0      498 2023-04-19 00:45:11.000000 gEconpy-1.2.1/gEconpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.956932 gEconpy-1.2.1/gEconpy/classes/
+-rw-rw-rw-   0        0        0       74 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/classes/__init__.py
+-rw-rw-rw-   0        0        0    28804 2023-04-18 23:52:37.000000 gEconpy-1.2.1/gEconpy/classes/block.py
+-rw-rw-rw-   0        0        0     6144 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/classes/containers.py
+-rw-rw-rw-   0        0        0    66334 2023-04-18 23:37:58.000000 gEconpy-1.2.1/gEconpy/classes/model.py
+-rw-rw-rw-   0        0        0     3472 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/classes/progress_bar.py
+-rw-rw-rw-   0        0        0     2523 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/classes/time_aware_symbol.py
+-rw-rw-rw-   0        0        0     1856 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/classes/transformers.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.960933 gEconpy-1.2.1/gEconpy/estimation/
+-rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/estimation/__init__.py
+-rw-rw-rw-   0        0        0     9085 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/estimation/estimate.py
+-rw-rw-rw-   0        0        0    11831 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/estimation/estimation_utilities.py
+-rw-rw-rw-   0        0        0     8557 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/estimation/kalman_filter.py
+-rw-rw-rw-   0        0        0     1386 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/estimation/kalman_smoother.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.962933 gEconpy-1.2.1/gEconpy/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/exceptions/__init__.py
+-rw-rw-rw-   0        0        0    11729 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.966932 gEconpy-1.2.1/gEconpy/numba_tools/
+-rw-rw-rw-   0        0        0     8396 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/numba_tools/LAPACK.py
+-rw-rw-rw-   0        0        0        0 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/numba_tools/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/numba_tools/intrinsics.py
+-rw-rw-rw-   0        0        0    24886 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/numba_tools/overloads.py
+-rw-rw-rw-   0        0        0     9132 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/numba_tools/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.973932 gEconpy-1.2.1/gEconpy/parser/
+-rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/__init__.py
+-rw-rw-rw-   0        0        0     1617 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/constants.py
+-rw-rw-rw-   0        0        0      370 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/file_loaders.py
+-rw-rw-rw-   0        0        0    11985 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/gEcon_parser.py
+-rw-rw-rw-   0        0        0    55526 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/parse_distributions.py
+-rw-rw-rw-   0        0        0    13526 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/parser/parse_equations.py
+-rw-rw-rw-   0        0        0     8288 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/parse_plaintext.py
+-rw-rw-rw-   0        0        0     4264 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/parser/validation.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.974932 gEconpy-1.2.1/gEconpy/plotting/
+-rw-rw-rw-   0        0        0      492 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/plotting/__init__.py
+-rw-rw-rw-   0        0        0    31887 2023-04-19 00:00:58.000000 gEconpy-1.2.1/gEconpy/plotting/plotting.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.977932 gEconpy-1.2.1/gEconpy/sampling/
+-rw-rw-rw-   0        0        0      490 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/sampling/__init__.py
+-rw-rw-rw-   0        0        0     6643 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/sampling/posterior_utilities.py
+-rw-rw-rw-   0        0        0     9314 2023-04-19 00:04:02.000000 gEconpy-1.2.1/gEconpy/sampling/prior_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.981938 gEconpy-1.2.1/gEconpy/shared/
+-rw-rw-rw-   0        0        0      127 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/shared/__init__.py
+-rw-rw-rw-   0        0        0    11445 2023-04-18 23:59:41.000000 gEconpy-1.2.1/gEconpy/shared/dynare_convert.py
+-rw-rw-rw-   0        0        0    30597 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/shared/statsmodel_convert.py
+-rw-rw-rw-   0        0        0      168 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/shared/typing.py
+-rw-rw-rw-   0        0        0    10340 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/shared/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.985932 gEconpy-1.2.1/gEconpy/solvers/
+-rw-rw-rw-   0        0        0        0 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/solvers/__init__.py
+-rw-rw-rw-   0        0        0     5114 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/solvers/cycle_reduction.py
+-rw-rw-rw-   0        0        0    13757 2023-02-22 12:40:07.000000 gEconpy-1.2.1/gEconpy/solvers/gensys.py
+-rw-rw-rw-   0        0        0    11313 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/solvers/perturbation.py
+-rw-rw-rw-   0        0        0    60257 2023-04-18 22:20:22.000000 gEconpy-1.2.1/gEconpy/solvers/steady_state.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.950931 gEconpy-1.2.1/gEconpy.egg-info/
+-rw-rw-rw-   0        0        0    14070 2023-04-19 00:46:02.000000 gEconpy-1.2.1/gEconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2023-04-19 00:46:02.000000 gEconpy-1.2.1/gEconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 00:46:02.000000 gEconpy-1.2.1/gEconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-19 00:46:02.000000 gEconpy-1.2.1/gEconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 00:46:02.000000 gEconpy-1.2.1/gEconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      579 2023-04-19 00:45:11.000000 gEconpy-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      549 2023-04-19 00:46:03.000933 gEconpy-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-22 12:40:07.000000 gEconpy-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 00:46:02.994933 gEconpy-1.2.1/tests/
+-rw-rw-rw-   0        0        0    10623 2023-04-18 22:20:22.000000 gEconpy-1.2.1/tests/test_block.py
+-rw-rw-rw-   0        0        0     3639 2023-04-18 22:20:22.000000 gEconpy-1.2.1/tests/test_containers.py
+-rw-rw-rw-   0        0        0     8818 2023-02-22 12:40:07.000000 gEconpy-1.2.1/tests/test_distribution_parser.py
+-rw-rw-rw-   0        0        0     1800 2023-02-22 12:40:07.000000 gEconpy-1.2.1/tests/test_estimation.py
+-rw-rw-rw-   0        0        0    19212 2023-02-22 12:40:07.000000 gEconpy-1.2.1/tests/test_gensys.py
+-rw-rw-rw-   0        0        0     6594 2023-04-18 22:20:22.000000 gEconpy-1.2.1/tests/test_kalman_filter.py
+-rw-rw-rw-   0        0        0    26905 2023-04-18 22:20:22.000000 gEconpy-1.2.1/tests/test_model.py
+-rw-rw-rw-   0        0        0    21844 2023-04-18 22:20:22.000000 gEconpy-1.2.1/tests/test_parser.py
+-rw-rw-rw-   0        0        0    14712 2023-02-22 12:40:07.000000 gEconpy-1.2.1/tests/test_steady_state.py
+-rw-rw-rw-   0        0        0     2379 2023-02-22 12:40:07.000000 gEconpy-1.2.1/tests/test_time_aware_symbols.py
```

### Comparing `gEconpy-1.2.0/LICENSE` & `gEconpy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/PKG-INFO` & `gEconpy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gEconpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for solving, estimating, and analyzing DSGE models
 Home-page: https://github.com/jessegrabowski/gEcon.py
 Author: Jesse Grabowski
 Author-email: jessegrabowski@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gEconpy-1.2.0/README.md` & `gEconpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/classes/block.py` & `gEconpy-1.2.1/gEconpy/classes/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,18 @@
         if not self._validate_key(block_dict, key):
             return
 
         equations = block_dict[key]
         equations, lagrange_multipliers = self._extract_lagrange_multipliers(equations, assumptions)
 
         parser_output = parse_equations.build_sympy_equations(equations, assumptions)
-        equations, flags = list(zip(*parser_output))
+        if len(parser_output) > 0:
+            equations, flags = list(zip(*parser_output))
+        else:
+            equations, flags = [], {}
         equation_numbers = self._get_and_record_equation_numbers(equations)
 
         equations = dict(zip(equation_numbers, equations))
         flags = dict(zip(equation_numbers, flags))
 
         lagrange_multipliers = dict(zip(equation_numbers, lagrange_multipliers))
         self.multipliers.update(lagrange_multipliers)
```

### Comparing `gEconpy-1.2.0/gEconpy/classes/containers.py` & `gEconpy-1.2.1/gEconpy/classes/containers.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/classes/model.py` & `gEconpy-1.2.1/gEconpy/classes/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,26 +658,28 @@
         -------
 
         """
         if self.build_perturbation_matrices is None:
             raise PerturbationSolutionNotFoundException()
 
         if free_param_dict is not None:
-            ss_dict, calib_dict = self.f_ss(free_param_dict)
-        else:
-            free_param_dict = self.free_param_dict
-            ss_dict = self.steady_state_dict
-            calib_dict = self.calib_param_dict
+            results = self.f_ss(self.free_param_dict)
+            self.steady_state_dict = results["ss_dict"]
+            self.calib_param_dict = results["calib_dict"]
+
+        param_dict = self.free_param_dict | self.calib_param_dict
+        steady_state_dict = self.steady_state_dict
 
         if system_matrices is not None:
             A, B, C, D = system_matrices
         else:
             A, B, C, D = self.build_perturbation_matrices(
-                **ss_dict, **free_param_dict, **calib_dict
+                np.array(list(param_dict.values())), np.array(list(steady_state_dict.values()))
             )
+
         n_forward = (C.sum(axis=0) > 0).sum().astype(int)
         n_eq, n_vars = A.shape
 
         # TODO: Compute system eigenvalues -- avoids calling the whole Gensys routine, but there is code duplication
         #   building Gamma_0 and Gamma_1
         lead_var_idx = np.where(np.sum(np.abs(C), axis=0) > tol)[0]
```

### Comparing `gEconpy-1.2.0/gEconpy/classes/progress_bar.py` & `gEconpy-1.2.1/gEconpy/classes/progress_bar.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/classes/time_aware_symbol.py` & `gEconpy-1.2.1/gEconpy/classes/time_aware_symbol.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/classes/transformers.py` & `gEconpy-1.2.1/gEconpy/classes/transformers.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/estimation/estimate.py` & `gEconpy-1.2.1/gEconpy/estimation/estimate.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/estimation/estimation_utilities.py` & `gEconpy-1.2.1/gEconpy/estimation/estimation_utilities.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/estimation/kalman_filter.py` & `gEconpy-1.2.1/gEconpy/estimation/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/estimation/kalman_smoother.py` & `gEconpy-1.2.1/gEconpy/estimation/kalman_smoother.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/exceptions/exceptions.py` & `gEconpy-1.2.1/gEconpy/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/numba_tools/LAPACK.py` & `gEconpy-1.2.1/gEconpy/numba_tools/LAPACK.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/numba_tools/intrinsics.py` & `gEconpy-1.2.1/gEconpy/numba_tools/intrinsics.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/numba_tools/overloads.py` & `gEconpy-1.2.1/gEconpy/numba_tools/overloads.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/numba_tools/utilities.py` & `gEconpy-1.2.1/gEconpy/numba_tools/utilities.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/constants.py` & `gEconpy-1.2.1/gEconpy/parser/constants.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/gEcon_parser.py` & `gEconpy-1.2.1/gEconpy/parser/gEcon_parser.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/parse_distributions.py` & `gEconpy-1.2.1/gEconpy/parser/parse_distributions.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/parse_equations.py` & `gEconpy-1.2.1/gEconpy/parser/parse_equations.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/parse_plaintext.py` & `gEconpy-1.2.1/gEconpy/parser/parse_plaintext.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/parser/validation.py` & `gEconpy-1.2.1/gEconpy/parser/validation.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/plotting/plotting.py` & `gEconpy-1.2.1/gEconpy/plotting/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,17 @@
 
     n_plots = len(vars_to_plot)
     n_cols = min(4, n_plots) if n_cols is None else n_cols
 
     gs, plot_locs = prepare_gridspec_figure(n_cols, n_plots)
     fig = plt.figure(figsize=figsize, dpi=dpi)
 
+    if shocks_to_plot is None:
+        shocks_to_plot = irf.columns.get_level_values(1).unique()
+
     for idx, variable in enumerate(vars_to_plot):
         axis = fig.add_subplot(gs[plot_locs[idx]])
 
         _plot_single_variable(
             irf.loc[variable, pd.IndexSlice[:, shocks_to_plot]].unstack(1),
             ax=axis,
             cmap=cmap,
```

### Comparing `gEconpy-1.2.0/gEconpy/sampling/posterior_utilities.py` & `gEconpy-1.2.1/gEconpy/sampling/posterior_utilities.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/sampling/prior_utilities.py` & `gEconpy-1.2.1/gEconpy/sampling/prior_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,28 +123,29 @@
 ):
     simulations = []
     model_var_names = [x.base_name for x in model.variables]
     shock_names = [x.name for x in model.shocks]
 
     param_dicts = pd.DataFrame(model.sample_param_dict_from_prior(n_samples)).T.to_dict()
     i = 0
-
+    print(param_dicts)
     progress_bar = ProgressBar(n_samples, "Sampling")
     for param_dict in param_dicts.values():
-        # free_param_dict, shock_dict, obs_dict = split_random_variables(param_dict, shock_names, model_var_names)
-        model.free_param_dict.update(param_dict)
+        free_param_dict, shock_dict, obs_dict = split_random_variables(param_dict, shock_names, model_var_names)
+        model.free_param_dict.update(free_param_dict)
         progress_bar.start()
 
         try:
             model.steady_state(verbose=False)
             model.solve_model(verbose=False, on_failure="ignore")
 
             data = model.simulate(
                 simulation_length=simulation_length,
                 n_simulations=n_simulations,
+                shock_dict=shock_dict,
                 show_progress_bar=False,
             )
             simulaton_ids = np.arange(n_simulations).astype(int)
 
             data = data.rename(
                 axis=1,
                 level=1,
```

### Comparing `gEconpy-1.2.0/gEconpy/shared/dynare_convert.py` & `gEconpy-1.2.1/gEconpy/shared/dynare_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,20 +224,19 @@
         A string representation of a Dynare model file.
 
     References
     ----------
     ..[1] Adjemian, Stéphane, et al. "Dynare: Reference manual, version 4." (2011).
     """
 
-    var_list = model.variables
-    param_dict = model.free_param_dict
-    param_dict.update(model.calib_param_dict)
+    var_list = model.variables.copy()
+    param_dict = model.free_param_dict | model.calib_param_dict
 
     shocks = model.shocks
-    ss_value_dict = model.steady_state_dict
+    ss_value_dict = model.steady_state_dict.copy()
 
     var_to_matlab = make_var_to_matlab_sub_dict(
         make_all_var_time_combos(var_list), clash_prefix="var_"
     )
     par_to_matlab = make_var_to_matlab_sub_dict(param_dict.keys(), clash_prefix="param_")
     shock_to_matlab = make_var_to_matlab_sub_dict(shocks, clash_prefix="exog_")
 
@@ -253,15 +252,15 @@
     )
     file = write_lines_from_list(
         [re.sub(UNDER_T_PATTERN, "", x) for x in shock_to_matlab.values()],
         file,
         line_start="varexo",
     )
     file += "\n"
-    file = write_lines_from_list(par_to_matlab.values(), file, line_start="parameters")
+    file = write_lines_from_list(list(par_to_matlab.values()), file, line_start="parameters")
     file += "\n"
 
     for model_param in sorted(param_dict.keys()):
         matlab_param = par_to_matlab[model_param]
         value = param_dict[model_param]
         file += f"{matlab_param} = {value};\n"
 
@@ -329,15 +328,15 @@
         matlab_eq = re.sub(UNDER_T_PATTERN, "", matlab_eq)
 
         file += matlab_eq + "\n"
 
     file += "end;\n\n"
 
     file += "initval;\n"
-    for var, val in string_keys_to_sympy(ss_value_dict).items():
+    for var, val in ss_value_dict.to_sympy().items():
         matlab_var = var_to_matlab[var].replace("_ss", "")
         file += f"{matlab_var} = {val:0.4f};\n"
 
     file += "end;\n\n"
     file += "steady;\n"
     file += "check(qz_zero_threshold=1e-20);\n\n"
```

### Comparing `gEconpy-1.2.0/gEconpy/shared/statsmodel_convert.py` & `gEconpy-1.2.1/gEconpy/shared/statsmodel_convert.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/shared/utilities.py` & `gEconpy-1.2.1/gEconpy/shared/utilities.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/solvers/cycle_reduction.py` & `gEconpy-1.2.1/gEconpy/solvers/cycle_reduction.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/solvers/gensys.py` & `gEconpy-1.2.1/gEconpy/solvers/gensys.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/solvers/perturbation.py` & `gEconpy-1.2.1/gEconpy/solvers/perturbation.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy/solvers/steady_state.py` & `gEconpy-1.2.1/gEconpy/solvers/steady_state.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/gEconpy.egg-info/PKG-INFO` & `gEconpy-1.2.1/gEconpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gEconpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for solving, estimating, and analyzing DSGE models
 Home-page: https://github.com/jessegrabowski/gEcon.py
 Author: Jesse Grabowski
 Author-email: jessegrabowski@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gEconpy-1.2.0/gEconpy.egg-info/SOURCES.txt` & `gEconpy-1.2.1/gEconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/pyproject.toml` & `gEconpy-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.nbqa.mutate]
 isort = 1
 black = 1
 pyupgrade = 1
 
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gEconpy-1.2.0/setup.cfg` & `gEconpy-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 4563 6f6e 7079 0d0a 7665 7273   = gEconpy..vers
-00000020: 696f 6e20 3d20 312e 322e 300d 0a64 6573  ion = 1.2.0..des
+00000020: 696f 6e20 3d20 312e 322e 310d 0a64 6573  ion = 1.2.1..des
 00000030: 6372 6970 7469 6f6e 203d 2041 2070 6163  cription = A pac
 00000040: 6b61 6765 2066 6f72 2073 6f6c 7669 6e67  kage for solving
 00000050: 2c20 6573 7469 6d61 7469 6e67 2c20 616e  , estimating, an
 00000060: 6420 616e 616c 797a 696e 6720 4453 4745  d analyzing DSGE
 00000070: 206d 6f64 656c 730d 0a6c 6f6e 675f 6465   models..long_de
 00000080: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000090: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
```

### Comparing `gEconpy-1.2.0/tests/test_block.py` & `gEconpy-1.2.1/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_containers.py` & `gEconpy-1.2.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_distribution_parser.py` & `gEconpy-1.2.1/tests/test_distribution_parser.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_estimation.py` & `gEconpy-1.2.1/tests/test_estimation.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_gensys.py` & `gEconpy-1.2.1/tests/test_gensys.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_kalman_filter.py` & `gEconpy-1.2.1/tests/test_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_model.py` & `gEconpy-1.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_parser.py` & `gEconpy-1.2.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_steady_state.py` & `gEconpy-1.2.1/tests/test_steady_state.py`

 * *Files identical despite different names*

### Comparing `gEconpy-1.2.0/tests/test_time_aware_symbols.py` & `gEconpy-1.2.1/tests/test_time_aware_symbols.py`

 * *Files identical despite different names*

